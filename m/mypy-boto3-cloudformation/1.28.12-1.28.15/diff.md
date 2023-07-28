# Comparing `tmp/mypy-boto3-cloudformation-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudformation-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudformation-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
```

## Comparing `mypy-boto3-cloudformation-1.28.12.tar` & `mypy-boto3-cloudformation-1.28.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.012562 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66147 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66048 2023-07-27 05:18:31.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17308 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    95531 2023-07-27 05:18:35.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    95414 2023-07-27 05:18:33.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-27 05:18:32.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:24.000000 mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.016563 mypy-boto3-cloudformation-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:18:30.000000 mypy-boto3-cloudformation-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66347 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66248 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22911 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    93669 2023-07-28 19:46:53.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93552 2023-07-28 19:46:53.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:46:50.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-07-28 19:46:51.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 19:47:31.000000 mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.692180 mypy-boto3-cloudformation-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 19:46:49.000000 mypy-boto3-cloudformation-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudformation-1.28.12/LICENSE` & `mypy-boto3-cloudformation-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/PKG-INFO` & `mypy-boto3-cloudformation-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudFormation 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudFormation 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -580,175 +580,169 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
-    AutoDeploymentOutputTypeDef,
+    ResponseMetadataTypeDef,
     AutoDeploymentTypeDef,
-    TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
     DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
-    ParameterOutputTypeDef,
-    TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
-    LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
     TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
     WarningsTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
     ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ManagedExecutionOutputTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
     StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
+    StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
@@ -761,21 +755,19 @@
     ListStackInstancesInputRequestTypeDef,
     ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     ListStackSetOperationResultsInputRequestTypeDef,
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
-    StackSetSummaryTypeDef,
     ParameterDeclarationTypeDef,
     StackInstanceResourceDriftsSummaryTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
     RollbackConfigurationOutputTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
     StackResourceSummaryTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.12/README.md` & `mypy-boto3-cloudformation-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -548,175 +548,169 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
-    AutoDeploymentOutputTypeDef,
+    ResponseMetadataTypeDef,
     AutoDeploymentTypeDef,
-    TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
     DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
-    ParameterOutputTypeDef,
-    TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
-    LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
     TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
     WarningsTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
     ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ManagedExecutionOutputTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
     StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
+    StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
@@ -729,21 +723,19 @@
     ListStackInstancesInputRequestTypeDef,
     ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     ListStackSetOperationResultsInputRequestTypeDef,
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
-    StackSetSummaryTypeDef,
     ParameterDeclarationTypeDef,
     StackInstanceResourceDriftsSummaryTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
     RollbackConfigurationOutputTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
     StackResourceSummaryTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__init__.pyi` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/__main__.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFormation 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudFormation 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
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

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> CreateStackOutputTypeDef:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#create_stack)
         """
@@ -716,15 +717,16 @@
 
     def execute_change_set(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         ClientRequestToken: str = ...,
-        DisableRollback: bool = ...
+        DisableRollback: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates a stack using the input information that was provided when the specified
         change set was created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.execute_change_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#execute_change_set)
@@ -1047,15 +1049,20 @@
         Registers an extension with the CloudFormation service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.register_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#register_type)
         """
 
     def rollback_stack(
-        self, *, StackName: str, RoleARN: str = ..., ClientRequestToken: str = ...
+        self,
+        *,
+        StackName: str,
+        RoleARN: str = ...,
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> RollbackStackOutputTypeDef:
         """
         When specifying `RollbackStack`, you preserve the state of previously
         provisioned resources when an operation fails.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.rollback_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#rollback_stack)
@@ -1161,15 +1168,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#update_stack)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/client.pyi` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> CreateStackOutputTypeDef:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#create_stack)
         """
@@ -673,15 +674,16 @@
         """
     def execute_change_set(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         ClientRequestToken: str = ...,
-        DisableRollback: bool = ...
+        DisableRollback: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates a stack using the input information that was provided when the specified
         change set was created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.execute_change_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#execute_change_set)
@@ -981,15 +983,20 @@
         """
         Registers an extension with the CloudFormation service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.register_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#register_type)
         """
     def rollback_stack(
-        self, *, StackName: str, RoleARN: str = ..., ClientRequestToken: str = ...
+        self,
+        *,
+        StackName: str,
+        RoleARN: str = ...,
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> RollbackStackOutputTypeDef:
         """
         When specifying `RollbackStack`, you preserve the state of previously
         provisioned resources when an operation fails.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.rollback_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#rollback_stack)
@@ -1088,15 +1095,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#update_stack)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/literals.pyi` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,261 +92,245 @@
     "ListStackSetOperationResultsPaginator",
     "ListStackSetOperationsPaginator",
     "ListStackSetsPaginator",
     "ListStacksPaginator",
     "ListTypesPaginator",
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
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
-
 class DescribeChangeSetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
-
 class DescribeStackEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
         """
 
-
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
-
 class ListChangeSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
         """
 
-
 class ListExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
         """
 
-
 class ListImportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
         """
 
-
 class ListStackInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
         """
 
-
 class ListStackResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
         """
 
-
 class ListStackSetOperationResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
-
 class ListStackSetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
-
 class ListStackSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
         """
 
-
 class ListStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
         """
 
-
 class ListTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/paginator.pyi` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,245 +92,261 @@
     "ListStackSetOperationResultsPaginator",
     "ListStackSetOperationsPaginator",
     "ListStackSetsPaginator",
     "ListStacksPaginator",
     "ListTypesPaginator",
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
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
+
 class DescribeChangeSetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
+
 class DescribeStackEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackeventspaginator)
         """
 
+
 class DescribeStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
+
 class ListChangeSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listchangesetspaginator)
         """
 
+
 class ListExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listexportspaginator)
         """
 
+
 class ListImportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listimportspaginator)
         """
 
+
 class ListStackInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackinstancespaginator)
         """
 
+
 class ListStackResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackresourcespaginator)
         """
 
+
 class ListStackSetOperationResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
+
 class ListStackSetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
+
 class ListStackSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetspaginator)
         """
 
+
 class ListStacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststackspaginator)
         """
 
+
 class ListTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,24 +33,21 @@
     HookFailureModeType,
     HookStatusType,
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
-    ModuleInfoResponseMetadataTypeDef,
+    ModuleInfoResponseTypeDef,
     OutputTypeDef,
-    ParameterOutputTypeDef,
     ParameterTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
-    TagOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -234,32 +231,33 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#stack)
     """
 
     stack_id: str
     stack_name: str
     change_set_id: str
     description: str
-    parameters: List[ParameterOutputTypeDef]
+    parameters: List[ParameterTypeDef]
     creation_time: datetime
     deletion_time: datetime
     last_updated_time: datetime
-    rollback_configuration: RollbackConfigurationResponseMetadataTypeDef
+    rollback_configuration: RollbackConfigurationTypeDef
     stack_status: StackStatusType
     stack_status_reason: str
     disable_rollback: bool
     notification_arns: List[str]
     timeout_in_minutes: int
     capabilities: List[CapabilityType]
     outputs: List[OutputTypeDef]
     role_arn: str
-    tags: List[TagOutputTypeDef]
+    tags: List[TagTypeDef]
     enable_termination_protection: bool
     parent_id: str
     root_id: str
-    drift_information: StackDriftInformationResponseMetadataTypeDef
+    drift_information: StackDriftInformationResponseTypeDef
+    retain_except_on_create: bool
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
 
     def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
@@ -330,15 +328,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#stackupdate-method)
         """
@@ -358,16 +357,16 @@
     physical_resource_id: str
     resource_type: str
     last_updated_timestamp: datetime
     resource_status: ResourceStatusType
     resource_status_reason: str
     description: str
     metadata: str
-    drift_information: StackResourceDriftInformationResponseMetadataTypeDef
-    module_info: ModuleInfoResponseMetadataTypeDef
+    drift_information: StackResourceDriftInformationResponseTypeDef
+    module_info: ModuleInfoResponseTypeDef
     stack_name: str
     logical_id: str
 
     def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -413,16 +412,16 @@
 
     logical_resource_id: str
     physical_resource_id: str
     resource_type: str
     last_updated_timestamp: datetime
     resource_status: ResourceStatusType
     resource_status_reason: str
-    drift_information: StackResourceDriftInformationSummaryResponseMetadataTypeDef
-    module_info: ModuleInfoResponseMetadataTypeDef
+    drift_information: StackResourceDriftInformationSummaryResponseTypeDef
+    module_info: ModuleInfoResponseTypeDef
     stack_name: str
     logical_id: str
 
     def Resource(self) -> _StackResource:
         """
         Creates a StackResource resource.
 
@@ -502,15 +501,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> _Stack:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#cloudformationserviceresourcecreate_stack-method)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/service_resource.pyi` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,21 @@
     HookFailureModeType,
     HookStatusType,
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
-    ModuleInfoResponseMetadataTypeDef,
+    ModuleInfoResponseTypeDef,
     OutputTypeDef,
-    ParameterOutputTypeDef,
     ParameterTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
-    TagOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -212,32 +209,33 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#stack)
     """
 
     stack_id: str
     stack_name: str
     change_set_id: str
     description: str
-    parameters: List[ParameterOutputTypeDef]
+    parameters: List[ParameterTypeDef]
     creation_time: datetime
     deletion_time: datetime
     last_updated_time: datetime
-    rollback_configuration: RollbackConfigurationResponseMetadataTypeDef
+    rollback_configuration: RollbackConfigurationTypeDef
     stack_status: StackStatusType
     stack_status_reason: str
     disable_rollback: bool
     notification_arns: List[str]
     timeout_in_minutes: int
     capabilities: List[CapabilityType]
     outputs: List[OutputTypeDef]
     role_arn: str
-    tags: List[TagOutputTypeDef]
+    tags: List[TagTypeDef]
     enable_termination_protection: bool
     parent_id: str
     root_id: str
-    drift_information: StackDriftInformationResponseMetadataTypeDef
+    drift_information: StackDriftInformationResponseTypeDef
+    retain_except_on_create: bool
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
 
     def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
@@ -302,15 +300,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#stackupdate-method)
         """
@@ -328,16 +327,16 @@
     physical_resource_id: str
     resource_type: str
     last_updated_timestamp: datetime
     resource_status: ResourceStatusType
     resource_status_reason: str
     description: str
     metadata: str
-    drift_information: StackResourceDriftInformationResponseMetadataTypeDef
-    module_info: ModuleInfoResponseMetadataTypeDef
+    drift_information: StackResourceDriftInformationResponseTypeDef
+    module_info: ModuleInfoResponseTypeDef
     stack_name: str
     logical_id: str
 
     def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -378,16 +377,16 @@
 
     logical_resource_id: str
     physical_resource_id: str
     resource_type: str
     last_updated_timestamp: datetime
     resource_status: ResourceStatusType
     resource_status_reason: str
-    drift_information: StackResourceDriftInformationSummaryResponseMetadataTypeDef
-    module_info: ModuleInfoResponseMetadataTypeDef
+    drift_information: StackResourceDriftInformationSummaryResponseTypeDef
+    module_info: ModuleInfoResponseTypeDef
     stack_name: str
     logical_id: str
 
     def Resource(self) -> _StackResource:
         """
         Creates a StackResource resource.
 
@@ -459,15 +458,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> _Stack:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/service_resource/#cloudformationserviceresourcecreate_stack-method)
         """
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cloudformation.type_defs import AccountGateResultTypeDef
 
     data: AccountGateResultTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -79,175 +79,169 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ActivateTypeOutputTypeDef",
-    "AutoDeploymentOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AutoDeploymentTypeDef",
-    "TypeConfigurationIdentifierOutputTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
-    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
-    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
     "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
-    "ParameterOutputTypeDef",
-    "TagOutputTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
-    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
-    "LoggingConfigOutputTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
-    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
-    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateOutputTypeDef",
     "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
     "WarningsTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListChangeSetsInputRequestTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListImportsOutputTypeDef",
     "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ManagedExecutionOutputTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
-    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
-    "RollbackTriggerOutputTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
-    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
     "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "TestTypeOutputTypeDef",
-    "UpdateStackInstancesOutputTypeDef",
-    "UpdateStackOutputTypeDef",
-    "UpdateStackSetOutputTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
-    "UpdateTerminationProtectionOutputTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
     "ActivateTypeInputRequestTypeDef",
     "RegisterTypeInputRequestTypeDef",
+    "ActivateTypeOutputTypeDef",
+    "CreateChangeSetOutputTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
+    "CreateStackSetOutputTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
+    "DescribePublisherOutputTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
+    "DetectStackDriftOutputTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
+    "GetStackPolicyOutputTypeDef",
+    "GetTemplateOutputTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListImportsOutputTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
+    "ModuleInfoResponseTypeDef",
+    "PublishTypeOutputTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
+    "RollbackStackOutputTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
+    "StackDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    "TestTypeOutputTypeDef",
+    "UpdateStackInstancesOutputTypeDef",
+    "UpdateStackOutputTypeDef",
+    "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionOutputTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
+    "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
@@ -260,21 +254,19 @@
     "ListStackInstancesInputRequestTypeDef",
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
-    "StackSetSummaryTypeDef",
     "ParameterDeclarationTypeDef",
     "StackInstanceResourceDriftsSummaryTypeDef",
     "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
     "RollbackConfigurationOutputTypeDef",
-    "RollbackConfigurationResponseMetadataTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
     "StackResourceDetailTypeDef",
     "StackResourceTypeDef",
     "StackResourceSummaryTypeDef",
@@ -334,52 +326,34 @@
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AutoDeploymentOutputTypeDef = TypedDict(
-    "AutoDeploymentOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Enabled": bool,
-        "RetainStacksOnAccountRemoval": bool,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
     },
     total=False,
 )
 
-TypeConfigurationIdentifierOutputTypeDef = TypedDict(
-    "TypeConfigurationIdentifierOutputTypeDef",
-    {
-        "TypeArn": str,
-        "TypeConfigurationAlias": str,
-        "TypeConfigurationArn": str,
-        "Type": ThirdPartyTypeType,
-        "TypeName": str,
-    },
-    total=False,
-)
-
 TypeConfigurationIdentifierTypeDef = TypedDict(
     "TypeConfigurationIdentifierTypeDef",
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
         "TypeConfigurationArn": str,
         "Type": ThirdPartyTypeType,
@@ -508,23 +482,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -541,46 +506,22 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -637,22 +578,14 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
@@ -688,18 +621,20 @@
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -737,37 +672,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -782,98 +694,37 @@
 
 class DescribeChangeSetInputRequestTypeDef(
     _RequiredDescribeChangeSetInputRequestTypeDef, _OptionalDescribeChangeSetInputRequestTypeDef
 ):
     pass
 
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
-    {
-        "ParameterKey": str,
-        "ParameterValue": str,
-        "UsePreviousValue": bool,
-        "ResolvedValue": str,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
     "DescribeOrganizationsAccessInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
-    {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePublisherInputRequestTypeDef = TypedDict(
     "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
     },
     total=False,
 )
 
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -1018,23 +869,14 @@
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
 
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -1049,22 +891,14 @@
         "VersionId": str,
         "PublisherId": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-LoggingConfigOutputTypeDef = TypedDict(
-    "LoggingConfigOutputTypeDef",
-    {
-        "LogRoleArn": str,
-        "LogGroupName": str,
-    },
-)
-
 RequiredActivatedTypeTypeDef = TypedDict(
     "RequiredActivatedTypeTypeDef",
     {
         "TypeNameAlias": str,
         "OriginalTypeName": str,
         "PublisherId": str,
         "SupportedMajorVersions": List[int],
@@ -1075,25 +909,14 @@
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
@@ -1107,65 +930,35 @@
 
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
 
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_OptionalExecuteChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ClientRequestToken": str,
         "DisableRollback": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class ExecuteChangeSetInputRequestTypeDef(
     _RequiredExecuteChangeSetInputRequestTypeDef, _OptionalExecuteChangeSetInputRequestTypeDef
@@ -1186,41 +979,24 @@
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
-    {
-        "TemplateBody": str,
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TemplateSummaryConfigTypeDef = TypedDict(
     "TemplateSummaryConfigTypeDef",
     {
         "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
@@ -1239,44 +1015,14 @@
     "WarningsTypeDef",
     {
         "UnrecognizedResourceTypes": List[str],
     },
     total=False,
 )
 
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
@@ -1290,52 +1036,22 @@
 
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
 
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
-    {
-        "ExportName": str,
-    },
-)
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListImportsInputRequestTypeDef = TypedDict(
     "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
 _OptionalListImportsInputRequestTypeDef = TypedDict(
@@ -1349,23 +1065,14 @@
 
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
-    {
-        "Imports": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
     "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "OperationId": str,
@@ -1395,36 +1102,14 @@
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
@@ -1447,37 +1132,14 @@
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1494,44 +1156,25 @@
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
 
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1546,23 +1189,14 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1614,31 +1248,14 @@
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
     total=False,
 )
 
-ManagedExecutionOutputTypeDef = TypedDict(
-    "ManagedExecutionOutputTypeDef",
-    {
-        "Active": bool,
-    },
-    total=False,
-)
-
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
     total=False,
@@ -1651,24 +1268,14 @@
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
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
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
     total=False,
 )
@@ -1698,22 +1305,14 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1742,59 +1341,24 @@
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
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
-RollbackTriggerOutputTypeDef = TypedDict(
-    "RollbackTriggerOutputTypeDef",
-    {
-        "Arn": str,
-        "Type": str,
-    },
-)
-
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -1806,33 +1370,26 @@
     },
 )
 _OptionalRollbackStackInputRequestTypeDef = TypedDict(
     "_OptionalRollbackStackInputRequestTypeDef",
     {
         "RoleARN": str,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
 
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalSetStackPolicyInputRequestTypeDef = TypedDict(
@@ -1872,22 +1429,14 @@
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
 
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1901,23 +1450,14 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStackDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackDriftInformationSummaryTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
     },
 )
 _OptionalStackDriftInformationSummaryTypeDef = TypedDict(
@@ -1981,32 +1521,14 @@
 
 class StackResourceDriftInformationTypeDef(
     _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
 ):
     pass
 
 
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackResourceDriftInformationSummaryTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
     },
 )
 _OptionalStackResourceDriftInformationSummaryTypeDef = TypedDict(
@@ -2103,62 +1625,22 @@
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -2173,23 +1655,14 @@
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
         "PublisherId": str,
         "TypeName": str,
@@ -2224,20 +1697,312 @@
 
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
 
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
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
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": Dict[str, Any],
+        "StagesAvailable": List[TemplateStageType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModuleInfoResponseTypeDef = TypedDict(
+    "ModuleInfoResponseTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackDriftInformationResponseTypeDef = TypedDict(
+    "StackDriftInformationResponseTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationSummaryResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "TypeConfigurationIdentifier": TypeConfigurationIdentifierOutputTypeDef,
+        "TypeConfigurationIdentifier": TypeConfigurationIdentifierTypeDef,
     },
     total=False,
 )
 
 BatchDescribeTypeConfigurationsInputRequestTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     {
@@ -2255,15 +2020,15 @@
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2437,14 +2202,30 @@
 
 class CreateStackSetInputRequestTypeDef(
     _RequiredCreateStackSetInputRequestTypeDef, _OptionalCreateStackSetInputRequestTypeDef
 ):
     pass
 
 
+StackSetSummaryTypeDef = TypedDict(
+    "StackSetSummaryTypeDef",
+    {
+        "StackSetName": str,
+        "StackSetId": str,
+        "Description": str,
+        "Status": StackSetStatusType,
+        "AutoDeployment": AutoDeploymentTypeDef,
+        "PermissionModel": PermissionModelsType,
+        "DriftStatus": StackDriftStatusType,
+        "LastDriftCheckTimestamp": datetime,
+        "ManagedExecution": ManagedExecutionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateStackSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalUpdateStackSetInputRequestTypeDef = TypedDict(
@@ -2475,14 +2256,179 @@
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
+
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
+
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
@@ -2586,15 +2532,15 @@
 
 
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2604,15 +2550,15 @@
         "IsDefaultVersion": bool,
         "TypeTestsStatus": TypeTestsStatusType,
         "TypeTestsStatusDescription": str,
         "Description": str,
         "Schema": str,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
-        "LoggingConfig": LoggingConfigOutputTypeDef,
+        "LoggingConfig": LoggingConfigTypeDef,
         "RequiredActivatedTypes": List[RequiredActivatedTypeTypeDef],
         "ExecutionRoleArn": str,
         "Visibility": VisibilityType,
         "SourceUrl": str,
         "DocumentationUrl": str,
         "LastUpdated": datetime,
         "TimeCreated": datetime,
@@ -2620,24 +2566,24 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryInputRequestTypeDef = TypedDict(
     "GetTemplateSummaryInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2659,15 +2605,15 @@
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
@@ -2710,15 +2656,15 @@
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
@@ -2754,27 +2700,27 @@
 
 
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2790,34 +2736,18 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StackSetSummaryTypeDef = TypedDict(
-    "StackSetSummaryTypeDef",
-    {
-        "StackSetName": str,
-        "StackSetId": str,
-        "Description": str,
-        "Status": StackSetStatusType,
-        "AutoDeployment": AutoDeploymentOutputTypeDef,
-        "PermissionModel": PermissionModelsType,
-        "DriftStatus": StackDriftStatusType,
-        "LastDriftCheckTimestamp": datetime,
-        "ManagedExecution": ManagedExecutionOutputTypeDef,
-    },
-    total=False,
-)
-
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "ParameterType": str,
         "NoEcho": bool,
@@ -2895,29 +2825,20 @@
     },
     total=False,
 )
 
 RollbackConfigurationOutputTypeDef = TypedDict(
     "RollbackConfigurationOutputTypeDef",
     {
-        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
-RollbackConfigurationResponseMetadataTypeDef = TypedDict(
-    "RollbackConfigurationResponseMetadataTypeDef",
-    {
-        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
-        "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
@@ -2972,15 +2893,15 @@
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
-        "ParameterOverrides": List[ParameterOutputTypeDef],
+        "ParameterOverrides": List[ParameterTypeDef],
         "Status": StackInstanceStatusType,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "StatusReason": str,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
@@ -3078,25 +2999,25 @@
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
         "TemplateBody": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "StackSetARN": str,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
-        "AutoDeployment": AutoDeploymentOutputTypeDef,
+        "AutoDeployment": AutoDeploymentTypeDef,
         "PermissionModel": PermissionModelsType,
         "OrganizationalUnitIds": List[str],
-        "ManagedExecution": ManagedExecutionOutputTypeDef,
+        "ManagedExecution": ManagedExecutionTypeDef,
         "Regions": List[str],
     },
     total=False,
 )
 
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
@@ -3138,34 +3059,34 @@
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
-        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierOutputTypeDef],
+        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
@@ -3179,15 +3100,15 @@
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -3196,41 +3117,41 @@
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
         "Warnings": WarningsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
     "ListStackInstanceResourceDriftsOutputTypeDef",
     {
         "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3256,30 +3177,31 @@
 )
 _OptionalStackTypeDef = TypedDict(
     "_OptionalStackTypeDef",
     {
         "StackId": str,
         "ChangeSetId": str,
         "Description": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "DeletionTime": datetime,
         "LastUpdatedTime": datetime,
         "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "StackStatusReason": str,
         "DisableRollback": bool,
         "NotificationARNs": List[str],
         "TimeoutInMinutes": int,
         "Capabilities": List[CapabilityType],
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
@@ -3343,14 +3265,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class CreateStackInputRequestTypeDef(
     _RequiredCreateStackInputRequestTypeDef, _OptionalCreateStackInputRequestTypeDef
@@ -3379,14 +3302,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
@@ -3416,14 +3340,15 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class UpdateStackInputRequestTypeDef(
     _RequiredUpdateStackInputRequestTypeDef, _OptionalUpdateStackInputRequestTypeDef
@@ -3446,105 +3371,106 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
@@ -3555,37 +3481,37 @@
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
         "ChangeSetId": str,
         "StackId": str,
         "StackName": str,
         "Description": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
         "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/type_defs.pyi` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cloudformation.type_defs import AccountGateResultTypeDef
 
     data: AccountGateResultTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -78,175 +78,169 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ActivateTypeOutputTypeDef",
-    "AutoDeploymentOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AutoDeploymentTypeDef",
-    "TypeConfigurationIdentifierOutputTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
-    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
-    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
     "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
-    "ParameterOutputTypeDef",
-    "TagOutputTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
-    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
-    "LoggingConfigOutputTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
-    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
-    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateOutputTypeDef",
     "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
     "WarningsTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListChangeSetsInputRequestTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListImportsOutputTypeDef",
     "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ManagedExecutionOutputTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
-    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
-    "RollbackTriggerOutputTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
-    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
     "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "TestTypeOutputTypeDef",
-    "UpdateStackInstancesOutputTypeDef",
-    "UpdateStackOutputTypeDef",
-    "UpdateStackSetOutputTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
-    "UpdateTerminationProtectionOutputTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
     "ActivateTypeInputRequestTypeDef",
     "RegisterTypeInputRequestTypeDef",
+    "ActivateTypeOutputTypeDef",
+    "CreateChangeSetOutputTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
+    "CreateStackSetOutputTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
+    "DescribePublisherOutputTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
+    "DetectStackDriftOutputTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
+    "GetStackPolicyOutputTypeDef",
+    "GetTemplateOutputTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListImportsOutputTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
+    "ModuleInfoResponseTypeDef",
+    "PublishTypeOutputTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
+    "RollbackStackOutputTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
+    "StackDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    "TestTypeOutputTypeDef",
+    "UpdateStackInstancesOutputTypeDef",
+    "UpdateStackOutputTypeDef",
+    "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionOutputTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
+    "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
@@ -259,21 +253,19 @@
     "ListStackInstancesInputRequestTypeDef",
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
-    "StackSetSummaryTypeDef",
     "ParameterDeclarationTypeDef",
     "StackInstanceResourceDriftsSummaryTypeDef",
     "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
     "RollbackConfigurationOutputTypeDef",
-    "RollbackConfigurationResponseMetadataTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
     "StackResourceDetailTypeDef",
     "StackResourceTypeDef",
     "StackResourceSummaryTypeDef",
@@ -333,52 +325,34 @@
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AutoDeploymentOutputTypeDef = TypedDict(
-    "AutoDeploymentOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Enabled": bool,
-        "RetainStacksOnAccountRemoval": bool,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
         "RetainStacksOnAccountRemoval": bool,
     },
     total=False,
 )
 
-TypeConfigurationIdentifierOutputTypeDef = TypedDict(
-    "TypeConfigurationIdentifierOutputTypeDef",
-    {
-        "TypeArn": str,
-        "TypeConfigurationAlias": str,
-        "TypeConfigurationArn": str,
-        "Type": ThirdPartyTypeType,
-        "TypeName": str,
-    },
-    total=False,
-)
-
 TypeConfigurationIdentifierTypeDef = TypedDict(
     "TypeConfigurationIdentifierTypeDef",
     {
         "TypeArn": str,
         "TypeConfigurationAlias": str,
         "TypeConfigurationArn": str,
         "Type": ThirdPartyTypeType,
@@ -503,23 +477,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -536,46 +501,22 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -628,22 +569,14 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
@@ -677,18 +610,20 @@
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -724,35 +659,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -765,98 +679,37 @@
 )
 
 class DescribeChangeSetInputRequestTypeDef(
     _RequiredDescribeChangeSetInputRequestTypeDef, _OptionalDescribeChangeSetInputRequestTypeDef
 ):
     pass
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
-    {
-        "ParameterKey": str,
-        "ParameterValue": str,
-        "UsePreviousValue": bool,
-        "ResolvedValue": str,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
     "DescribeOrganizationsAccessInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
-    {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePublisherInputRequestTypeDef = TypedDict(
     "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
     },
     total=False,
 )
 
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -991,23 +844,14 @@
 
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -1022,22 +866,14 @@
         "VersionId": str,
         "PublisherId": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-LoggingConfigOutputTypeDef = TypedDict(
-    "LoggingConfigOutputTypeDef",
-    {
-        "LogRoleArn": str,
-        "LogGroupName": str,
-    },
-)
-
 RequiredActivatedTypeTypeDef = TypedDict(
     "RequiredActivatedTypeTypeDef",
     {
         "TypeNameAlias": str,
         "OriginalTypeName": str,
         "PublisherId": str,
         "SupportedMajorVersions": List[int],
@@ -1048,25 +884,14 @@
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
@@ -1078,65 +903,35 @@
 )
 
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_OptionalExecuteChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ClientRequestToken": str,
         "DisableRollback": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class ExecuteChangeSetInputRequestTypeDef(
     _RequiredExecuteChangeSetInputRequestTypeDef, _OptionalExecuteChangeSetInputRequestTypeDef
 ):
@@ -1155,41 +950,24 @@
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
-    {
-        "TemplateBody": str,
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TemplateSummaryConfigTypeDef = TypedDict(
     "TemplateSummaryConfigTypeDef",
     {
         "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
@@ -1208,42 +986,14 @@
     "WarningsTypeDef",
     {
         "UnrecognizedResourceTypes": List[str],
     },
     total=False,
 )
 
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
@@ -1255,50 +1005,22 @@
 )
 
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
-    {
-        "ExportName": str,
-    },
-)
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
-):
-    pass
-
 _RequiredListImportsInputRequestTypeDef = TypedDict(
     "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
 _OptionalListImportsInputRequestTypeDef = TypedDict(
@@ -1310,23 +1032,14 @@
 )
 
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
-    {
-        "Imports": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
     "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "OperationId": str,
@@ -1354,34 +1067,14 @@
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
@@ -1402,35 +1095,14 @@
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1445,44 +1117,25 @@
 
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1497,23 +1150,14 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1565,31 +1209,14 @@
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
     total=False,
 )
 
-ManagedExecutionOutputTypeDef = TypedDict(
-    "ManagedExecutionOutputTypeDef",
-    {
-        "Active": bool,
-    },
-    total=False,
-)
-
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
     total=False,
@@ -1602,24 +1229,14 @@
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
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
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
     total=False,
 )
@@ -1649,22 +1266,14 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1691,59 +1300,24 @@
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
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
-RollbackTriggerOutputTypeDef = TypedDict(
-    "RollbackTriggerOutputTypeDef",
-    {
-        "Arn": str,
-        "Type": str,
-    },
-)
-
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -1755,31 +1329,24 @@
     },
 )
 _OptionalRollbackStackInputRequestTypeDef = TypedDict(
     "_OptionalRollbackStackInputRequestTypeDef",
     {
         "RoleARN": str,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalSetStackPolicyInputRequestTypeDef = TypedDict(
@@ -1815,22 +1382,14 @@
 
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1844,23 +1403,14 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStackDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackDriftInformationSummaryTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
     },
 )
 _OptionalStackDriftInformationSummaryTypeDef = TypedDict(
@@ -1918,32 +1468,14 @@
 )
 
 class StackResourceDriftInformationTypeDef(
     _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
 ):
     pass
 
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackResourceDriftInformationSummaryTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
     },
 )
 _OptionalStackResourceDriftInformationSummaryTypeDef = TypedDict(
@@ -2036,62 +1568,22 @@
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -2106,23 +1598,14 @@
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
         "PublisherId": str,
         "TypeName": str,
@@ -2155,20 +1638,312 @@
 )
 
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
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
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": Dict[str, Any],
+        "StagesAvailable": List[TemplateStageType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModuleInfoResponseTypeDef = TypedDict(
+    "ModuleInfoResponseTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackDriftInformationResponseTypeDef = TypedDict(
+    "StackDriftInformationResponseTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationSummaryResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "TypeConfigurationIdentifier": TypeConfigurationIdentifierOutputTypeDef,
+        "TypeConfigurationIdentifier": TypeConfigurationIdentifierTypeDef,
     },
     total=False,
 )
 
 BatchDescribeTypeConfigurationsInputRequestTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     {
@@ -2186,15 +1961,15 @@
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2356,14 +2131,30 @@
 )
 
 class CreateStackSetInputRequestTypeDef(
     _RequiredCreateStackSetInputRequestTypeDef, _OptionalCreateStackSetInputRequestTypeDef
 ):
     pass
 
+StackSetSummaryTypeDef = TypedDict(
+    "StackSetSummaryTypeDef",
+    {
+        "StackSetName": str,
+        "StackSetId": str,
+        "Description": str,
+        "Status": StackSetStatusType,
+        "AutoDeployment": AutoDeploymentTypeDef,
+        "PermissionModel": PermissionModelsType,
+        "DriftStatus": StackDriftStatusType,
+        "LastDriftCheckTimestamp": datetime,
+        "ManagedExecution": ManagedExecutionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateStackSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalUpdateStackSetInputRequestTypeDef = TypedDict(
@@ -2392,14 +2183,169 @@
 )
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
@@ -2499,15 +2445,15 @@
     pass
 
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2517,15 +2463,15 @@
         "IsDefaultVersion": bool,
         "TypeTestsStatus": TypeTestsStatusType,
         "TypeTestsStatusDescription": str,
         "Description": str,
         "Schema": str,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
-        "LoggingConfig": LoggingConfigOutputTypeDef,
+        "LoggingConfig": LoggingConfigTypeDef,
         "RequiredActivatedTypes": List[RequiredActivatedTypeTypeDef],
         "ExecutionRoleArn": str,
         "Visibility": VisibilityType,
         "SourceUrl": str,
         "DocumentationUrl": str,
         "LastUpdated": datetime,
         "TimeCreated": datetime,
@@ -2533,24 +2479,24 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryInputRequestTypeDef = TypedDict(
     "GetTemplateSummaryInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2572,15 +2518,15 @@
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
     _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef,
@@ -2619,15 +2565,15 @@
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
@@ -2659,27 +2605,27 @@
     pass
 
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2695,32 +2641,16 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackSetSummaryTypeDef = TypedDict(
-    "StackSetSummaryTypeDef",
-    {
-        "StackSetName": str,
-        "StackSetId": str,
-        "Description": str,
-        "Status": StackSetStatusType,
-        "AutoDeployment": AutoDeploymentOutputTypeDef,
-        "PermissionModel": PermissionModelsType,
-        "DriftStatus": StackDriftStatusType,
-        "LastDriftCheckTimestamp": datetime,
-        "ManagedExecution": ManagedExecutionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
@@ -2796,29 +2726,20 @@
     },
     total=False,
 )
 
 RollbackConfigurationOutputTypeDef = TypedDict(
     "RollbackConfigurationOutputTypeDef",
     {
-        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
-RollbackConfigurationResponseMetadataTypeDef = TypedDict(
-    "RollbackConfigurationResponseMetadataTypeDef",
-    {
-        "RollbackTriggers": List[RollbackTriggerOutputTypeDef],
-        "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
@@ -2871,15 +2792,15 @@
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
-        "ParameterOverrides": List[ParameterOutputTypeDef],
+        "ParameterOverrides": List[ParameterTypeDef],
         "Status": StackInstanceStatusType,
         "StackInstanceStatus": StackInstanceComprehensiveStatusTypeDef,
         "StatusReason": str,
         "OrganizationalUnitId": str,
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
@@ -2971,25 +2892,25 @@
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
         "TemplateBody": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "StackSetARN": str,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
-        "AutoDeployment": AutoDeploymentOutputTypeDef,
+        "AutoDeployment": AutoDeploymentTypeDef,
         "PermissionModel": PermissionModelsType,
         "OrganizationalUnitIds": List[str],
-        "ManagedExecution": ManagedExecutionOutputTypeDef,
+        "ManagedExecution": ManagedExecutionTypeDef,
         "Regions": List[str],
     },
     total=False,
 )
 
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
@@ -3031,34 +2952,34 @@
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
-        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierOutputTypeDef],
+        "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
@@ -3072,15 +2993,15 @@
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -3089,41 +3010,41 @@
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
         "Warnings": WarningsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
     "ListStackInstanceResourceDriftsOutputTypeDef",
     {
         "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3149,30 +3070,31 @@
 )
 _OptionalStackTypeDef = TypedDict(
     "_OptionalStackTypeDef",
     {
         "StackId": str,
         "ChangeSetId": str,
         "Description": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "DeletionTime": datetime,
         "LastUpdatedTime": datetime,
         "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "StackStatusReason": str,
         "DisableRollback": bool,
         "NotificationARNs": List[str],
         "TimeoutInMinutes": int,
         "Capabilities": List[CapabilityType],
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
@@ -3232,14 +3154,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class CreateStackInputRequestTypeDef(
     _RequiredCreateStackInputRequestTypeDef, _OptionalCreateStackInputRequestTypeDef
 ):
@@ -3266,14 +3189,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
@@ -3301,14 +3225,15 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class UpdateStackInputRequestTypeDef(
     _RequiredUpdateStackInputRequestTypeDef, _OptionalUpdateStackInputRequestTypeDef
 ):
@@ -3329,105 +3254,106 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
@@ -3438,37 +3364,37 @@
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
         "ChangeSetId": str,
         "StackId": str,
         "StackName": str,
         "Description": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
         "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "Capabilities": List[CapabilityType],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.py` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation/waiter.pyi` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/PKG-INFO` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudFormation 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudFormation 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [mypy-boto3-cloudformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -580,175 +580,169 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
-    AutoDeploymentOutputTypeDef,
+    ResponseMetadataTypeDef,
     AutoDeploymentTypeDef,
-    TypeConfigurationIdentifierOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
     DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
-    ParameterOutputTypeDef,
-    TagOutputTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
-    LoggingConfigOutputTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
     TemplateSummaryConfigTypeDef,
     ResourceIdentifierSummaryTypeDef,
     WarningsTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
     ListStackInstanceResourceDriftsInputRequestTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ManagedExecutionOutputTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackTriggerOutputTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
     StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
+    StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
@@ -761,21 +755,19 @@
     ListStackInstancesInputRequestTypeDef,
     ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     ListStackSetOperationResultsInputRequestTypeDef,
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
-    StackSetSummaryTypeDef,
     ParameterDeclarationTypeDef,
     StackInstanceResourceDriftsSummaryTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
     RollbackConfigurationOutputTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
     StackResourceSummaryTypeDef,
```

### Comparing `mypy-boto3-cloudformation-1.28.12/mypy_boto3_cloudformation.egg-info/SOURCES.txt` & `mypy-boto3-cloudformation-1.28.15/mypy_boto3_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.12/setup.py` & `mypy-boto3-cloudformation-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudformation",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFormation 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CloudFormation 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

