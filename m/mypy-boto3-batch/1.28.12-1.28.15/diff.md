# Comparing `tmp/mypy-boto3-batch-1.28.12.tar.gz` & `tmp/mypy-boto3-batch-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-batch-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-batch-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
```

## Comparing `mypy-boto3-batch-1.28.12.tar` & `mypy-boto3-batch-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.140569 mypy-boto3-batch-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-27 05:34:22.132569 mypy-boto3-batch-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17885 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.132569 mypy-boto3-batch-1.28.12/mypy_boto3_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20489 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59854 2023-07-27 05:17:59.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59771 2023-07-27 05:17:58.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.132569 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:22.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:21.000000 mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.140569 mypy-boto3-batch-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:17:57.000000 mypy-boto3-batch-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.232736 mypy-boto3-batch-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-28 20:42:22.224736 mypy-boto3-batch-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.212736 mypy-boto3-batch-1.28.15/mypy_boto3_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20489 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51341 2023-07-28 20:20:12.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51272 2023-07-28 20:20:11.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.224736 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:42:22.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:42:21.000000 mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.232736 mypy-boto3-batch-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:20:10.000000 mypy-boto3-batch-1.28.15/setup.py
```

### Comparing `mypy-boto3-batch-1.28.12/LICENSE` & `mypy-boto3-batch-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/PKG-INFO` & `mypy-boto3-batch-1.28.15/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.12
-Summary: Type annotations for boto3.Batch 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,126 +365,98 @@
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
     CancelJobRequestRequestTypeDef,
-    EksConfigurationOutputTypeDef,
-    UpdatePolicyOutputTypeDef,
-    ComputeEnvironmentOrderOutputTypeDef,
+    EksConfigurationTypeDef,
+    UpdatePolicyTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    Ec2ConfigurationOutputTypeDef,
-    LaunchTemplateSpecificationOutputTypeDef,
     Ec2ConfigurationTypeDef,
     LaunchTemplateSpecificationTypeDef,
-    EphemeralStorageOutputTypeDef,
-    FargatePlatformConfigurationOutputTypeDef,
-    KeyValuePairOutputTypeDef,
-    MountPointOutputTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    ResourceRequirementOutputTypeDef,
-    RuntimePlatformOutputTypeDef,
-    SecretOutputTypeDef,
-    UlimitOutputTypeDef,
-    KeyValuePairTypeDef,
-    ResourceRequirementTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
+    KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
+    ResourceRequirementTypeDef,
     RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    EksConfigurationTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
     DeviceOutputTypeDef,
     DeviceTypeDef,
-    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
-    EksContainerEnvironmentVariableOutputTypeDef,
-    EksContainerResourceRequirementsOutputTypeDef,
-    EksContainerSecurityContextOutputTypeDef,
-    EksContainerVolumeMountOutputTypeDef,
     EksContainerEnvironmentVariableTypeDef,
-    EksContainerResourceRequirementsTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
-    EksEmptyDirOutputTypeDef,
+    EksContainerResourceRequirementsTypeDef,
     EksEmptyDirTypeDef,
-    EksHostPathOutputTypeDef,
     EksHostPathTypeDef,
     EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
-    EksSecretOutputTypeDef,
     EksSecretTypeDef,
-    EvaluateOnExitOutputTypeDef,
     EvaluateOnExitTypeDef,
-    ShareAttributesOutputTypeDef,
     ShareAttributesTypeDef,
-    HostOutputTypeDef,
     HostTypeDef,
-    JobTimeoutOutputTypeDef,
-    JobDependencyOutputTypeDef,
+    JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
-    JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePolicyTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
-    JobQueueDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
+    JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
     ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
-    LogConfigurationOutputTypeDef,
     ContainerOverridesTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
-    EFSVolumeConfigurationOutputTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    SubmitJobResponseTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
     EksContainerDetailTypeDef,
     EksContainerOutputTypeDef,
     EksContainerOverrideTypeDef,
     EksContainerTypeDef,
-    EksVolumeOutputTypeDef,
     EksVolumeTypeDef,
     RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
     FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
@@ -494,15 +466,14 @@
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
-    VolumeOutputTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
     EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
     SchedulingPolicyDetailTypeDef,
     CreateSchedulingPolicyRequestRequestTypeDef,
```

### Comparing `mypy-boto3-batch-1.28.12/README.md` & `mypy-boto3-batch-1.28.15/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,126 +333,98 @@
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
     CancelJobRequestRequestTypeDef,
-    EksConfigurationOutputTypeDef,
-    UpdatePolicyOutputTypeDef,
-    ComputeEnvironmentOrderOutputTypeDef,
+    EksConfigurationTypeDef,
+    UpdatePolicyTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    Ec2ConfigurationOutputTypeDef,
-    LaunchTemplateSpecificationOutputTypeDef,
     Ec2ConfigurationTypeDef,
     LaunchTemplateSpecificationTypeDef,
-    EphemeralStorageOutputTypeDef,
-    FargatePlatformConfigurationOutputTypeDef,
-    KeyValuePairOutputTypeDef,
-    MountPointOutputTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    ResourceRequirementOutputTypeDef,
-    RuntimePlatformOutputTypeDef,
-    SecretOutputTypeDef,
-    UlimitOutputTypeDef,
-    KeyValuePairTypeDef,
-    ResourceRequirementTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
+    KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
+    ResourceRequirementTypeDef,
     RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    EksConfigurationTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
     DeviceOutputTypeDef,
     DeviceTypeDef,
-    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
-    EksContainerEnvironmentVariableOutputTypeDef,
-    EksContainerResourceRequirementsOutputTypeDef,
-    EksContainerSecurityContextOutputTypeDef,
-    EksContainerVolumeMountOutputTypeDef,
     EksContainerEnvironmentVariableTypeDef,
-    EksContainerResourceRequirementsTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
-    EksEmptyDirOutputTypeDef,
+    EksContainerResourceRequirementsTypeDef,
     EksEmptyDirTypeDef,
-    EksHostPathOutputTypeDef,
     EksHostPathTypeDef,
     EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
-    EksSecretOutputTypeDef,
     EksSecretTypeDef,
-    EvaluateOnExitOutputTypeDef,
     EvaluateOnExitTypeDef,
-    ShareAttributesOutputTypeDef,
     ShareAttributesTypeDef,
-    HostOutputTypeDef,
     HostTypeDef,
-    JobTimeoutOutputTypeDef,
-    JobDependencyOutputTypeDef,
+    JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
-    JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePolicyTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
-    JobQueueDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
+    JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
     ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
-    LogConfigurationOutputTypeDef,
     ContainerOverridesTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
-    EFSVolumeConfigurationOutputTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    SubmitJobResponseTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
     EksContainerDetailTypeDef,
     EksContainerOutputTypeDef,
     EksContainerOverrideTypeDef,
     EksContainerTypeDef,
-    EksVolumeOutputTypeDef,
     EksVolumeTypeDef,
     RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
     FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
@@ -462,15 +434,14 @@
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
-    VolumeOutputTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
     EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
     SchedulingPolicyDetailTypeDef,
     CreateSchedulingPolicyRequestRequestTypeDef,
```

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.py` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/__init__.pyi` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/__main__.py` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Batch 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Batch 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.py` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/client.pyi` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.py` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/literals.pyi` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.py` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeComputeEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
 
@@ -87,30 +87,30 @@
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobdefinitionspaginator)
         """
 
 
 class DescribeJobQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
     """
 
     def paginate(
-        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
         """
 
 
@@ -124,28 +124,28 @@
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listjobspaginator)
         """
 
 
 class ListSchedulingPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchedulingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
         """
```

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/paginator.pyi` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeComputeEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
 class DescribeJobDefinitionsPaginator(Paginator):
@@ -83,29 +83,29 @@
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobdefinitionspaginator)
         """
 
 class DescribeJobQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
     """
 
     def paginate(
-        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -118,27 +118,27 @@
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listjobspaginator)
         """
 
 class ListSchedulingPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchedulingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
         """
```

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/type_defs.py` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,126 +45,98 @@
 
 __all__ = (
     "ArrayPropertiesDetailTypeDef",
     "ArrayPropertiesSummaryTypeDef",
     "ArrayPropertiesTypeDef",
     "NetworkInterfaceTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "EksConfigurationOutputTypeDef",
-    "UpdatePolicyOutputTypeDef",
-    "ComputeEnvironmentOrderOutputTypeDef",
+    "EksConfigurationTypeDef",
+    "UpdatePolicyTypeDef",
     "ComputeEnvironmentOrderTypeDef",
-    "Ec2ConfigurationOutputTypeDef",
-    "LaunchTemplateSpecificationOutputTypeDef",
     "Ec2ConfigurationTypeDef",
     "LaunchTemplateSpecificationTypeDef",
-    "EphemeralStorageOutputTypeDef",
-    "FargatePlatformConfigurationOutputTypeDef",
-    "KeyValuePairOutputTypeDef",
-    "MountPointOutputTypeDef",
-    "NetworkConfigurationOutputTypeDef",
-    "ResourceRequirementOutputTypeDef",
-    "RuntimePlatformOutputTypeDef",
-    "SecretOutputTypeDef",
-    "UlimitOutputTypeDef",
-    "KeyValuePairTypeDef",
-    "ResourceRequirementTypeDef",
     "EphemeralStorageTypeDef",
     "FargatePlatformConfigurationTypeDef",
+    "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
+    "ResourceRequirementTypeDef",
     "RuntimePlatformTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
-    "EksConfigurationTypeDef",
-    "CreateComputeEnvironmentResponseTypeDef",
-    "CreateJobQueueResponseTypeDef",
-    "CreateSchedulingPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
     "DeregisterJobDefinitionRequestRequestTypeDef",
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     "DeviceOutputTypeDef",
     "DeviceTypeDef",
-    "EFSAuthorizationConfigOutputTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
-    "EksContainerEnvironmentVariableOutputTypeDef",
-    "EksContainerResourceRequirementsOutputTypeDef",
-    "EksContainerSecurityContextOutputTypeDef",
-    "EksContainerVolumeMountOutputTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
-    "EksContainerResourceRequirementsTypeDef",
+    "EksContainerResourceRequirementsOutputTypeDef",
     "EksContainerSecurityContextTypeDef",
     "EksContainerVolumeMountTypeDef",
-    "EksEmptyDirOutputTypeDef",
+    "EksContainerResourceRequirementsTypeDef",
     "EksEmptyDirTypeDef",
-    "EksHostPathOutputTypeDef",
     "EksHostPathTypeDef",
     "EksMetadataOutputTypeDef",
     "EksMetadataTypeDef",
-    "EksSecretOutputTypeDef",
     "EksSecretTypeDef",
-    "EvaluateOnExitOutputTypeDef",
     "EvaluateOnExitTypeDef",
-    "ShareAttributesOutputTypeDef",
     "ShareAttributesTypeDef",
-    "HostOutputTypeDef",
     "HostTypeDef",
-    "JobTimeoutOutputTypeDef",
-    "JobDependencyOutputTypeDef",
+    "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
-    "JobTimeoutTypeDef",
     "KeyValuesPairTypeDef",
     "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterJobDefinitionResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubmitJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdatePolicyTypeDef",
-    "UpdateComputeEnvironmentResponseTypeDef",
-    "UpdateJobQueueResponseTypeDef",
     "AttemptContainerDetailTypeDef",
-    "JobQueueDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
+    "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
     "ComputeResourceOutputTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
-    "LogConfigurationOutputTypeDef",
     "ContainerOverridesTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
-    "EFSVolumeConfigurationOutputTypeDef",
+    "CreateComputeEnvironmentResponseTypeDef",
+    "CreateJobQueueResponseTypeDef",
+    "CreateSchedulingPolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterJobDefinitionResponseTypeDef",
+    "SubmitJobResponseTypeDef",
+    "UpdateComputeEnvironmentResponseTypeDef",
+    "UpdateJobQueueResponseTypeDef",
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
     "EksContainerDetailTypeDef",
     "EksContainerOutputTypeDef",
     "EksContainerOverrideTypeDef",
     "EksContainerTypeDef",
-    "EksVolumeOutputTypeDef",
     "EksVolumeTypeDef",
     "RetryStrategyOutputTypeDef",
     "RetryStrategyTypeDef",
     "FairsharePolicyOutputTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
@@ -174,15 +146,14 @@
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
-    "VolumeOutputTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
     "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
     "SchedulingPolicyDetailTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
@@ -251,79 +222,39 @@
     "CancelJobRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
 
-EksConfigurationOutputTypeDef = TypedDict(
-    "EksConfigurationOutputTypeDef",
+EksConfigurationTypeDef = TypedDict(
+    "EksConfigurationTypeDef",
     {
         "eksClusterArn": str,
         "kubernetesNamespace": str,
     },
 )
 
-UpdatePolicyOutputTypeDef = TypedDict(
-    "UpdatePolicyOutputTypeDef",
+UpdatePolicyTypeDef = TypedDict(
+    "UpdatePolicyTypeDef",
     {
         "terminateJobsOnUpdate": bool,
         "jobExecutionTimeoutMinutes": int,
     },
     total=False,
 )
 
-ComputeEnvironmentOrderOutputTypeDef = TypedDict(
-    "ComputeEnvironmentOrderOutputTypeDef",
-    {
-        "order": int,
-        "computeEnvironment": str,
-    },
-)
-
 ComputeEnvironmentOrderTypeDef = TypedDict(
     "ComputeEnvironmentOrderTypeDef",
     {
         "order": int,
         "computeEnvironment": str,
     },
 )
 
-_RequiredEc2ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEc2ConfigurationOutputTypeDef",
-    {
-        "imageType": str,
-    },
-)
-_OptionalEc2ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEc2ConfigurationOutputTypeDef",
-    {
-        "imageIdOverride": str,
-        "imageKubernetesVersion": str,
-    },
-    total=False,
-)
-
-
-class Ec2ConfigurationOutputTypeDef(
-    _RequiredEc2ConfigurationOutputTypeDef, _OptionalEc2ConfigurationOutputTypeDef
-):
-    pass
-
-
-LaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "LaunchTemplateSpecificationOutputTypeDef",
-    {
-        "launchTemplateId": str,
-        "launchTemplateName": str,
-        "version": str,
-    },
-    total=False,
-)
-
 _RequiredEc2ConfigurationTypeDef = TypedDict(
     "_RequiredEc2ConfigurationTypeDef",
     {
         "imageType": str,
     },
 )
 _OptionalEc2ConfigurationTypeDef = TypedDict(
@@ -346,140 +277,64 @@
         "launchTemplateId": str,
         "launchTemplateName": str,
         "version": str,
     },
     total=False,
 )
 
-EphemeralStorageOutputTypeDef = TypedDict(
-    "EphemeralStorageOutputTypeDef",
+EphemeralStorageTypeDef = TypedDict(
+    "EphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
-FargatePlatformConfigurationOutputTypeDef = TypedDict(
-    "FargatePlatformConfigurationOutputTypeDef",
+FargatePlatformConfigurationTypeDef = TypedDict(
+    "FargatePlatformConfigurationTypeDef",
     {
         "platformVersion": str,
     },
     total=False,
 )
 
-KeyValuePairOutputTypeDef = TypedDict(
-    "KeyValuePairOutputTypeDef",
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
     {
         "name": str,
         "value": str,
     },
     total=False,
 )
 
-MountPointOutputTypeDef = TypedDict(
-    "MountPointOutputTypeDef",
+MountPointTypeDef = TypedDict(
+    "MountPointTypeDef",
     {
         "containerPath": str,
         "readOnly": bool,
         "sourceVolume": str,
     },
     total=False,
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
-ResourceRequirementOutputTypeDef = TypedDict(
-    "ResourceRequirementOutputTypeDef",
-    {
-        "value": str,
-        "type": ResourceTypeType,
-    },
-)
-
-RuntimePlatformOutputTypeDef = TypedDict(
-    "RuntimePlatformOutputTypeDef",
-    {
-        "operatingSystemFamily": str,
-        "cpuArchitecture": str,
-    },
-    total=False,
-)
-
-SecretOutputTypeDef = TypedDict(
-    "SecretOutputTypeDef",
-    {
-        "name": str,
-        "valueFrom": str,
-    },
-)
-
-UlimitOutputTypeDef = TypedDict(
-    "UlimitOutputTypeDef",
-    {
-        "hardLimit": int,
-        "name": str,
-        "softLimit": int,
-    },
-)
-
-KeyValuePairTypeDef = TypedDict(
-    "KeyValuePairTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-    total=False,
-)
-
 ResourceRequirementTypeDef = TypedDict(
     "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
-EphemeralStorageTypeDef = TypedDict(
-    "EphemeralStorageTypeDef",
-    {
-        "sizeInGiB": int,
-    },
-)
-
-FargatePlatformConfigurationTypeDef = TypedDict(
-    "FargatePlatformConfigurationTypeDef",
-    {
-        "platformVersion": str,
-    },
-    total=False,
-)
-
-MountPointTypeDef = TypedDict(
-    "MountPointTypeDef",
-    {
-        "containerPath": str,
-        "readOnly": bool,
-        "sourceVolume": str,
-    },
-    total=False,
-)
-
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
-    {
-        "assignPublicIp": AssignPublicIpType,
-    },
-    total=False,
-)
-
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "operatingSystemFamily": str,
         "cpuArchitecture": str,
     },
     total=False,
@@ -507,46 +362,22 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-EksConfigurationTypeDef = TypedDict(
-    "EksConfigurationTypeDef",
-    {
-        "eksClusterArn": str,
-        "kubernetesNamespace": str,
-    },
-)
-
-CreateComputeEnvironmentResponseTypeDef = TypedDict(
-    "CreateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateJobQueueResponseTypeDef = TypedDict(
-    "CreateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSchedulingPolicyResponseTypeDef = TypedDict(
-    "CreateSchedulingPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironment": str,
@@ -570,65 +401,46 @@
 DeregisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinition": str,
     },
 )
 
-DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "computeEnvironments": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeComputeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     {
         "computeEnvironments": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    {
-        "jobDefinitions": Sequence[str],
-        "jobDefinitionName": str,
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeJobDefinitionsRequestRequestTypeDef",
     {
         "jobDefinitions": Sequence[str],
         "maxResults": int,
         "jobDefinitionName": str,
         "status": str,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    {
-        "jobQueues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobQueuesRequestRequestTypeDef = TypedDict(
     "DescribeJobQueuesRequestRequestTypeDef",
     {
         "jobQueues": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -685,23 +497,14 @@
 )
 
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
 
-EFSAuthorizationConfigOutputTypeDef = TypedDict(
-    "EFSAuthorizationConfigOutputTypeDef",
-    {
-        "accessPointId": str,
-        "iam": EFSAuthorizationConfigIAMType,
-    },
-    total=False,
-)
-
 EFSAuthorizationConfigTypeDef = TypedDict(
     "EFSAuthorizationConfigTypeDef",
     {
         "accessPointId": str,
         "iam": EFSAuthorizationConfigIAMType,
     },
     total=False,
@@ -712,67 +515,14 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-_RequiredEksContainerEnvironmentVariableOutputTypeDef = TypedDict(
-    "_RequiredEksContainerEnvironmentVariableOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalEksContainerEnvironmentVariableOutputTypeDef = TypedDict(
-    "_OptionalEksContainerEnvironmentVariableOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class EksContainerEnvironmentVariableOutputTypeDef(
-    _RequiredEksContainerEnvironmentVariableOutputTypeDef,
-    _OptionalEksContainerEnvironmentVariableOutputTypeDef,
-):
-    pass
-
-
-EksContainerResourceRequirementsOutputTypeDef = TypedDict(
-    "EksContainerResourceRequirementsOutputTypeDef",
-    {
-        "limits": Dict[str, str],
-        "requests": Dict[str, str],
-    },
-    total=False,
-)
-
-EksContainerSecurityContextOutputTypeDef = TypedDict(
-    "EksContainerSecurityContextOutputTypeDef",
-    {
-        "runAsUser": int,
-        "runAsGroup": int,
-        "privileged": bool,
-        "readOnlyRootFilesystem": bool,
-        "runAsNonRoot": bool,
-    },
-    total=False,
-)
-
-EksContainerVolumeMountOutputTypeDef = TypedDict(
-    "EksContainerVolumeMountOutputTypeDef",
-    {
-        "name": str,
-        "mountPath": str,
-        "readOnly": bool,
-    },
-    total=False,
-)
-
 _RequiredEksContainerEnvironmentVariableTypeDef = TypedDict(
     "_RequiredEksContainerEnvironmentVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalEksContainerEnvironmentVariableTypeDef = TypedDict(
@@ -786,19 +536,19 @@
 
 class EksContainerEnvironmentVariableTypeDef(
     _RequiredEksContainerEnvironmentVariableTypeDef, _OptionalEksContainerEnvironmentVariableTypeDef
 ):
     pass
 
 
-EksContainerResourceRequirementsTypeDef = TypedDict(
-    "EksContainerResourceRequirementsTypeDef",
+EksContainerResourceRequirementsOutputTypeDef = TypedDict(
+    "EksContainerResourceRequirementsOutputTypeDef",
     {
-        "limits": Mapping[str, str],
-        "requests": Mapping[str, str],
+        "limits": Dict[str, str],
+        "requests": Dict[str, str],
     },
     total=False,
 )
 
 EksContainerSecurityContextTypeDef = TypedDict(
     "EksContainerSecurityContextTypeDef",
     {
@@ -817,40 +567,32 @@
         "name": str,
         "mountPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-EksEmptyDirOutputTypeDef = TypedDict(
-    "EksEmptyDirOutputTypeDef",
+EksContainerResourceRequirementsTypeDef = TypedDict(
+    "EksContainerResourceRequirementsTypeDef",
     {
-        "medium": str,
-        "sizeLimit": str,
+        "limits": Mapping[str, str],
+        "requests": Mapping[str, str],
     },
     total=False,
 )
 
 EksEmptyDirTypeDef = TypedDict(
     "EksEmptyDirTypeDef",
     {
         "medium": str,
         "sizeLimit": str,
     },
     total=False,
 )
 
-EksHostPathOutputTypeDef = TypedDict(
-    "EksHostPathOutputTypeDef",
-    {
-        "path": str,
-    },
-    total=False,
-)
-
 EksHostPathTypeDef = TypedDict(
     "EksHostPathTypeDef",
     {
         "path": str,
     },
     total=False,
 )
@@ -867,33 +609,14 @@
     "EksMetadataTypeDef",
     {
         "labels": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredEksSecretOutputTypeDef = TypedDict(
-    "_RequiredEksSecretOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-_OptionalEksSecretOutputTypeDef = TypedDict(
-    "_OptionalEksSecretOutputTypeDef",
-    {
-        "optional": bool,
-    },
-    total=False,
-)
-
-
-class EksSecretOutputTypeDef(_RequiredEksSecretOutputTypeDef, _OptionalEksSecretOutputTypeDef):
-    pass
-
-
 _RequiredEksSecretTypeDef = TypedDict(
     "_RequiredEksSecretTypeDef",
     {
         "secretName": str,
     },
 )
 _OptionalEksSecretTypeDef = TypedDict(
@@ -905,37 +628,14 @@
 )
 
 
 class EksSecretTypeDef(_RequiredEksSecretTypeDef, _OptionalEksSecretTypeDef):
     pass
 
 
-_RequiredEvaluateOnExitOutputTypeDef = TypedDict(
-    "_RequiredEvaluateOnExitOutputTypeDef",
-    {
-        "action": RetryActionType,
-    },
-)
-_OptionalEvaluateOnExitOutputTypeDef = TypedDict(
-    "_OptionalEvaluateOnExitOutputTypeDef",
-    {
-        "onStatusReason": str,
-        "onReason": str,
-        "onExitCode": str,
-    },
-    total=False,
-)
-
-
-class EvaluateOnExitOutputTypeDef(
-    _RequiredEvaluateOnExitOutputTypeDef, _OptionalEvaluateOnExitOutputTypeDef
-):
-    pass
-
-
 _RequiredEvaluateOnExitTypeDef = TypedDict(
     "_RequiredEvaluateOnExitTypeDef",
     {
         "action": RetryActionType,
     },
 )
 _OptionalEvaluateOnExitTypeDef = TypedDict(
@@ -949,35 +649,14 @@
 )
 
 
 class EvaluateOnExitTypeDef(_RequiredEvaluateOnExitTypeDef, _OptionalEvaluateOnExitTypeDef):
     pass
 
 
-_RequiredShareAttributesOutputTypeDef = TypedDict(
-    "_RequiredShareAttributesOutputTypeDef",
-    {
-        "shareIdentifier": str,
-    },
-)
-_OptionalShareAttributesOutputTypeDef = TypedDict(
-    "_OptionalShareAttributesOutputTypeDef",
-    {
-        "weightFactor": float,
-    },
-    total=False,
-)
-
-
-class ShareAttributesOutputTypeDef(
-    _RequiredShareAttributesOutputTypeDef, _OptionalShareAttributesOutputTypeDef
-):
-    pass
-
-
 _RequiredShareAttributesTypeDef = TypedDict(
     "_RequiredShareAttributesTypeDef",
     {
         "shareIdentifier": str,
     },
 )
 _OptionalShareAttributesTypeDef = TypedDict(
@@ -989,47 +668,30 @@
 )
 
 
 class ShareAttributesTypeDef(_RequiredShareAttributesTypeDef, _OptionalShareAttributesTypeDef):
     pass
 
 
-HostOutputTypeDef = TypedDict(
-    "HostOutputTypeDef",
-    {
-        "sourcePath": str,
-    },
-    total=False,
-)
-
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "sourcePath": str,
     },
     total=False,
 )
 
-JobTimeoutOutputTypeDef = TypedDict(
-    "JobTimeoutOutputTypeDef",
+JobTimeoutTypeDef = TypedDict(
+    "JobTimeoutTypeDef",
     {
         "attemptDurationSeconds": int,
     },
     total=False,
 )
 
-JobDependencyOutputTypeDef = TypedDict(
-    "JobDependencyOutputTypeDef",
-    {
-        "jobId": str,
-        "type": ArrayJobDependencyType,
-    },
-    total=False,
-)
-
 JobDependencyTypeDef = TypedDict(
     "JobDependencyTypeDef",
     {
         "jobId": str,
         "type": ArrayJobDependencyType,
     },
     total=False,
@@ -1050,22 +712,14 @@
         "isMainNode": bool,
         "numNodes": int,
         "nodeIndex": int,
     },
     total=False,
 )
 
-JobTimeoutTypeDef = TypedDict(
-    "JobTimeoutTypeDef",
-    {
-        "attemptDurationSeconds": int,
-    },
-    total=False,
-)
-
 KeyValuesPairTypeDef = TypedDict(
     "KeyValuesPairTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
@@ -1107,22 +761,14 @@
 )
 
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
 
-ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "ListSchedulingPoliciesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1138,63 +784,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
-RegisterJobDefinitionResponseTypeDef = TypedDict(
-    "RegisterJobDefinitionResponseTypeDef",
-    {
-        "jobDefinitionName": str,
-        "jobDefinitionArn": str,
-        "revision": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
-SubmitJobResponseTypeDef = TypedDict(
-    "SubmitJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobName": str,
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1211,102 +808,75 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdatePolicyTypeDef = TypedDict(
-    "UpdatePolicyTypeDef",
-    {
-        "terminateJobsOnUpdate": bool,
-        "jobExecutionTimeoutMinutes": int,
-    },
-    total=False,
-)
-
-UpdateComputeEnvironmentResponseTypeDef = TypedDict(
-    "UpdateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateJobQueueResponseTypeDef = TypedDict(
-    "UpdateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttemptContainerDetailTypeDef = TypedDict(
     "AttemptContainerDetailTypeDef",
     {
         "containerInstanceArn": str,
         "taskArn": str,
         "exitCode": int,
         "reason": str,
         "logStreamName": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
-_RequiredJobQueueDetailTypeDef = TypedDict(
-    "_RequiredJobQueueDetailTypeDef",
+_RequiredCreateJobQueueRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobQueueRequestRequestTypeDef",
     {
         "jobQueueName": str,
-        "jobQueueArn": str,
-        "state": JQStateType,
         "priority": int,
-        "computeEnvironmentOrder": List[ComputeEnvironmentOrderOutputTypeDef],
+        "computeEnvironmentOrder": Sequence[ComputeEnvironmentOrderTypeDef],
     },
 )
-_OptionalJobQueueDetailTypeDef = TypedDict(
-    "_OptionalJobQueueDetailTypeDef",
+_OptionalCreateJobQueueRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobQueueRequestRequestTypeDef",
     {
+        "state": JQStateType,
         "schedulingPolicyArn": str,
-        "status": JQStatusType,
-        "statusReason": str,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class JobQueueDetailTypeDef(_RequiredJobQueueDetailTypeDef, _OptionalJobQueueDetailTypeDef):
+class CreateJobQueueRequestRequestTypeDef(
+    _RequiredCreateJobQueueRequestRequestTypeDef, _OptionalCreateJobQueueRequestRequestTypeDef
+):
     pass
 
 
-_RequiredCreateJobQueueRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobQueueRequestRequestTypeDef",
+_RequiredJobQueueDetailTypeDef = TypedDict(
+    "_RequiredJobQueueDetailTypeDef",
     {
         "jobQueueName": str,
+        "jobQueueArn": str,
+        "state": JQStateType,
         "priority": int,
-        "computeEnvironmentOrder": Sequence[ComputeEnvironmentOrderTypeDef],
+        "computeEnvironmentOrder": List[ComputeEnvironmentOrderTypeDef],
     },
 )
-_OptionalCreateJobQueueRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobQueueRequestRequestTypeDef",
+_OptionalJobQueueDetailTypeDef = TypedDict(
+    "_OptionalJobQueueDetailTypeDef",
     {
-        "state": JQStateType,
         "schedulingPolicyArn": str,
-        "tags": Mapping[str, str],
+        "status": JQStatusType,
+        "statusReason": str,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateJobQueueRequestRequestTypeDef(
-    _RequiredCreateJobQueueRequestRequestTypeDef, _OptionalCreateJobQueueRequestRequestTypeDef
-):
+class JobQueueDetailTypeDef(_RequiredJobQueueDetailTypeDef, _OptionalJobQueueDetailTypeDef):
     pass
 
 
 _RequiredUpdateJobQueueRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobQueueRequestRequestTypeDef",
     {
         "jobQueue": str,
@@ -1349,16 +919,16 @@
         "securityGroupIds": List[str],
         "ec2KeyPair": str,
         "instanceRole": str,
         "tags": Dict[str, str],
         "placementGroup": str,
         "bidPercentage": int,
         "spotIamFleetRole": str,
-        "launchTemplate": LaunchTemplateSpecificationOutputTypeDef,
-        "ec2Configuration": List[Ec2ConfigurationOutputTypeDef],
+        "launchTemplate": LaunchTemplateSpecificationTypeDef,
+        "ec2Configuration": List[Ec2ConfigurationTypeDef],
     },
     total=False,
 )
 
 
 class ComputeResourceOutputTypeDef(
     _RequiredComputeResourceOutputTypeDef, _OptionalComputeResourceOutputTypeDef
@@ -1420,49 +990,49 @@
         "updateToLatestImageVersion": bool,
         "type": CRTypeType,
         "imageId": str,
     },
     total=False,
 )
 
+ContainerOverridesTypeDef = TypedDict(
+    "ContainerOverridesTypeDef",
+    {
+        "vcpus": int,
+        "memory": int,
+        "command": Sequence[str],
+        "instanceType": str,
+        "environment": Sequence[KeyValuePairTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
+    },
+    total=False,
+)
+
 _RequiredLogConfigurationOutputTypeDef = TypedDict(
     "_RequiredLogConfigurationOutputTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationOutputTypeDef = TypedDict(
     "_OptionalLogConfigurationOutputTypeDef",
     {
         "options": Dict[str, str],
-        "secretOptions": List[SecretOutputTypeDef],
+        "secretOptions": List[SecretTypeDef],
     },
     total=False,
 )
 
 
 class LogConfigurationOutputTypeDef(
     _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
 ):
     pass
 
 
-ContainerOverridesTypeDef = TypedDict(
-    "ContainerOverridesTypeDef",
-    {
-        "vcpus": int,
-        "memory": int,
-        "command": Sequence[str],
-        "instanceType": str,
-        "environment": Sequence[KeyValuePairTypeDef],
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
-    },
-    total=False,
-)
-
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -1475,37 +1045,123 @@
 )
 
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
 
-_RequiredEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEFSVolumeConfigurationOutputTypeDef",
+CreateComputeEnvironmentResponseTypeDef = TypedDict(
+    "CreateComputeEnvironmentResponseTypeDef",
     {
-        "fileSystemId": str,
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEFSVolumeConfigurationOutputTypeDef",
+
+CreateJobQueueResponseTypeDef = TypedDict(
+    "CreateJobQueueResponseTypeDef",
     {
-        "rootDirectory": str,
-        "transitEncryption": EFSTransitEncryptionType,
-        "transitEncryptionPort": int,
-        "authorizationConfig": EFSAuthorizationConfigOutputTypeDef,
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchedulingPolicyResponseTypeDef = TypedDict(
+    "CreateSchedulingPolicyResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterJobDefinitionResponseTypeDef = TypedDict(
+    "RegisterJobDefinitionResponseTypeDef",
+    {
+        "jobDefinitionName": str,
+        "jobDefinitionArn": str,
+        "revision": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitJobResponseTypeDef = TypedDict(
+    "SubmitJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobName": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComputeEnvironmentResponseTypeDef = TypedDict(
+    "UpdateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobQueueResponseTypeDef = TypedDict(
+    "UpdateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    {
+        "computeEnvironments": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    {
+        "jobDefinitions": Sequence[str],
+        "jobDefinitionName": str,
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class EFSVolumeConfigurationOutputTypeDef(
-    _RequiredEFSVolumeConfigurationOutputTypeDef, _OptionalEFSVolumeConfigurationOutputTypeDef
-):
-    pass
+DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    {
+        "jobQueues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
+ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
@@ -1544,20 +1200,20 @@
     "EksContainerDetailTypeDef",
     {
         "name": str,
         "image": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
-        "env": List[EksContainerEnvironmentVariableOutputTypeDef],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsOutputTypeDef,
         "exitCode": int,
         "reason": str,
-        "volumeMounts": List[EksContainerVolumeMountOutputTypeDef],
-        "securityContext": EksContainerSecurityContextOutputTypeDef,
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 _RequiredEksContainerOutputTypeDef = TypedDict(
     "_RequiredEksContainerOutputTypeDef",
     {
@@ -1567,18 +1223,18 @@
 _OptionalEksContainerOutputTypeDef = TypedDict(
     "_OptionalEksContainerOutputTypeDef",
     {
         "name": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
-        "env": List[EksContainerEnvironmentVariableOutputTypeDef],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsOutputTypeDef,
-        "volumeMounts": List[EksContainerVolumeMountOutputTypeDef],
-        "securityContext": EksContainerSecurityContextOutputTypeDef,
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 
 class EksContainerOutputTypeDef(
     _RequiredEksContainerOutputTypeDef, _OptionalEksContainerOutputTypeDef
@@ -1620,35 +1276,14 @@
 )
 
 
 class EksContainerTypeDef(_RequiredEksContainerTypeDef, _OptionalEksContainerTypeDef):
     pass
 
 
-_RequiredEksVolumeOutputTypeDef = TypedDict(
-    "_RequiredEksVolumeOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalEksVolumeOutputTypeDef = TypedDict(
-    "_OptionalEksVolumeOutputTypeDef",
-    {
-        "hostPath": EksHostPathOutputTypeDef,
-        "emptyDir": EksEmptyDirOutputTypeDef,
-        "secret": EksSecretOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EksVolumeOutputTypeDef(_RequiredEksVolumeOutputTypeDef, _OptionalEksVolumeOutputTypeDef):
-    pass
-
-
 _RequiredEksVolumeTypeDef = TypedDict(
     "_RequiredEksVolumeTypeDef",
     {
         "name": str,
     },
 )
 _OptionalEksVolumeTypeDef = TypedDict(
@@ -1666,15 +1301,15 @@
     pass
 
 
 RetryStrategyOutputTypeDef = TypedDict(
     "RetryStrategyOutputTypeDef",
     {
         "attempts": int,
-        "evaluateOnExit": List[EvaluateOnExitOutputTypeDef],
+        "evaluateOnExit": List[EvaluateOnExitTypeDef],
     },
     total=False,
 )
 
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
@@ -1685,15 +1320,15 @@
 )
 
 FairsharePolicyOutputTypeDef = TypedDict(
     "FairsharePolicyOutputTypeDef",
     {
         "shareDecaySeconds": int,
         "computeReservation": int,
-        "shareDistribution": List[ShareAttributesOutputTypeDef],
+        "shareDistribution": List[ShareAttributesTypeDef],
     },
     total=False,
 )
 
 FairsharePolicyTypeDef = TypedDict(
     "FairsharePolicyTypeDef",
     {
@@ -1737,15 +1372,15 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "jobQueue": str,
         "arrayJobId": str,
         "multiNodeJobId": str,
         "jobStatus": JobStatusType,
         "filters": Sequence[KeyValuesPairTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
@@ -1787,15 +1422,15 @@
 )
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttemptDetailTypeDef = TypedDict(
     "AttemptDetailTypeDef",
     {
         "container": AttemptContainerDetailTypeDef,
@@ -1807,15 +1442,15 @@
 )
 
 DescribeJobQueuesResponseTypeDef = TypedDict(
     "DescribeJobQueuesResponseTypeDef",
     {
         "jobQueues": List[JobQueueDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComputeEnvironmentDetailTypeDef = TypedDict(
     "_RequiredComputeEnvironmentDetailTypeDef",
     {
         "computeEnvironmentName": str,
@@ -1830,16 +1465,16 @@
         "tags": Dict[str, str],
         "type": CETypeType,
         "state": CEStateType,
         "status": CEStatusType,
         "statusReason": str,
         "computeResources": ComputeResourceOutputTypeDef,
         "serviceRole": str,
-        "updatePolicy": UpdatePolicyOutputTypeDef,
-        "eksConfiguration": EksConfigurationOutputTypeDef,
+        "updatePolicy": UpdatePolicyTypeDef,
+        "eksConfiguration": EksConfigurationTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
         "uuid": str,
     },
     total=False,
 )
 
 
@@ -1920,24 +1555,14 @@
 
 class NodePropertyOverrideTypeDef(
     _RequiredNodePropertyOverrideTypeDef, _OptionalNodePropertyOverrideTypeDef
 ):
     pass
 
 
-VolumeOutputTypeDef = TypedDict(
-    "VolumeOutputTypeDef",
-    {
-        "host": HostOutputTypeDef,
-        "name": str,
-        "efsVolumeConfiguration": EFSVolumeConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "host": HostTypeDef,
         "name": str,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
     },
@@ -1956,30 +1581,30 @@
 EksPodPropertiesDetailTypeDef = TypedDict(
     "EksPodPropertiesDetailTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
-        "volumes": List[EksVolumeOutputTypeDef],
+        "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
         "metadata": EksMetadataOutputTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesOutputTypeDef = TypedDict(
     "EksPodPropertiesOutputTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerOutputTypeDef],
-        "volumes": List[EksVolumeOutputTypeDef],
+        "volumes": List[EksVolumeTypeDef],
         "metadata": EksMetadataOutputTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
@@ -2063,24 +1688,24 @@
 
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobSummaryList": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComputeEnvironmentsResponseTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponseTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeOverridesTypeDef = TypedDict(
     "NodeOverridesTypeDef",
     {
         "numNodes": int,
@@ -2094,65 +1719,65 @@
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
-        "volumes": List[VolumeOutputTypeDef],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "mountPoints": List[MountPointOutputTypeDef],
+        "volumes": List[VolumeTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
-        "ulimits": List[UlimitOutputTypeDef],
+        "ulimits": List[UlimitTypeDef],
         "privileged": bool,
         "user": str,
         "exitCode": int,
         "reason": str,
         "containerInstanceArn": str,
         "taskArn": str,
         "logStreamName": str,
         "instanceType": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersOutputTypeDef,
         "logConfiguration": LogConfigurationOutputTypeDef,
-        "secrets": List[SecretOutputTypeDef],
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "fargatePlatformConfiguration": FargatePlatformConfigurationOutputTypeDef,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
-        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "secrets": List[SecretTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesOutputTypeDef = TypedDict(
     "ContainerPropertiesOutputTypeDef",
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
-        "volumes": List[VolumeOutputTypeDef],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "mountPoints": List[MountPointOutputTypeDef],
+        "volumes": List[VolumeTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
         "privileged": bool,
-        "ulimits": List[UlimitOutputTypeDef],
+        "ulimits": List[UlimitTypeDef],
         "user": str,
         "instanceType": str,
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersOutputTypeDef,
         "logConfiguration": LogConfigurationOutputTypeDef,
-        "secrets": List[SecretOutputTypeDef],
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "fargatePlatformConfiguration": FargatePlatformConfigurationOutputTypeDef,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
-        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "secrets": List[SecretTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesTypeDef = TypedDict(
     "ContainerPropertiesTypeDef",
     {
@@ -2214,15 +1839,15 @@
     total=False,
 )
 
 DescribeSchedulingPoliciesResponseTypeDef = TypedDict(
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNodeRangePropertyOutputTypeDef = TypedDict(
     "_RequiredNodeRangePropertyOutputTypeDef",
     {
         "targetNodes": str,
@@ -2329,15 +1954,15 @@
     "_OptionalJobDefinitionTypeDef",
     {
         "status": str,
         "schedulingPriority": int,
         "parameters": Dict[str, str],
         "retryStrategy": RetryStrategyOutputTypeDef,
         "containerProperties": ContainerPropertiesOutputTypeDef,
-        "timeout": JobTimeoutOutputTypeDef,
+        "timeout": JobTimeoutTypeDef,
         "nodeProperties": NodePropertiesOutputTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesOutputTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
     },
@@ -2367,21 +1992,21 @@
         "shareIdentifier": str,
         "schedulingPriority": int,
         "attempts": List[AttemptDetailTypeDef],
         "statusReason": str,
         "createdAt": int,
         "retryStrategy": RetryStrategyOutputTypeDef,
         "stoppedAt": int,
-        "dependsOn": List[JobDependencyOutputTypeDef],
+        "dependsOn": List[JobDependencyTypeDef],
         "parameters": Dict[str, str],
         "container": ContainerDetailTypeDef,
         "nodeDetails": NodeDetailsTypeDef,
         "nodeProperties": NodePropertiesOutputTypeDef,
         "arrayProperties": ArrayPropertiesDetailTypeDef,
-        "timeout": JobTimeoutOutputTypeDef,
+        "timeout": JobTimeoutTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesDetailTypeDef,
         "eksAttempts": List[EksAttemptDetailTypeDef],
         "isCancelled": bool,
         "isTerminated": bool,
@@ -2427,18 +2052,18 @@
 
 
 DescribeJobDefinitionsResponseTypeDef = TypedDict(
     "DescribeJobDefinitionsResponseTypeDef",
     {
         "jobDefinitions": List[JobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "jobs": List[JobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch/type_defs.pyi` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -44,126 +44,98 @@
 
 __all__ = (
     "ArrayPropertiesDetailTypeDef",
     "ArrayPropertiesSummaryTypeDef",
     "ArrayPropertiesTypeDef",
     "NetworkInterfaceTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "EksConfigurationOutputTypeDef",
-    "UpdatePolicyOutputTypeDef",
-    "ComputeEnvironmentOrderOutputTypeDef",
+    "EksConfigurationTypeDef",
+    "UpdatePolicyTypeDef",
     "ComputeEnvironmentOrderTypeDef",
-    "Ec2ConfigurationOutputTypeDef",
-    "LaunchTemplateSpecificationOutputTypeDef",
     "Ec2ConfigurationTypeDef",
     "LaunchTemplateSpecificationTypeDef",
-    "EphemeralStorageOutputTypeDef",
-    "FargatePlatformConfigurationOutputTypeDef",
-    "KeyValuePairOutputTypeDef",
-    "MountPointOutputTypeDef",
-    "NetworkConfigurationOutputTypeDef",
-    "ResourceRequirementOutputTypeDef",
-    "RuntimePlatformOutputTypeDef",
-    "SecretOutputTypeDef",
-    "UlimitOutputTypeDef",
-    "KeyValuePairTypeDef",
-    "ResourceRequirementTypeDef",
     "EphemeralStorageTypeDef",
     "FargatePlatformConfigurationTypeDef",
+    "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
+    "ResourceRequirementTypeDef",
     "RuntimePlatformTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
-    "EksConfigurationTypeDef",
-    "CreateComputeEnvironmentResponseTypeDef",
-    "CreateJobQueueResponseTypeDef",
-    "CreateSchedulingPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
     "DeregisterJobDefinitionRequestRequestTypeDef",
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     "DeviceOutputTypeDef",
     "DeviceTypeDef",
-    "EFSAuthorizationConfigOutputTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
-    "EksContainerEnvironmentVariableOutputTypeDef",
-    "EksContainerResourceRequirementsOutputTypeDef",
-    "EksContainerSecurityContextOutputTypeDef",
-    "EksContainerVolumeMountOutputTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
-    "EksContainerResourceRequirementsTypeDef",
+    "EksContainerResourceRequirementsOutputTypeDef",
     "EksContainerSecurityContextTypeDef",
     "EksContainerVolumeMountTypeDef",
-    "EksEmptyDirOutputTypeDef",
+    "EksContainerResourceRequirementsTypeDef",
     "EksEmptyDirTypeDef",
-    "EksHostPathOutputTypeDef",
     "EksHostPathTypeDef",
     "EksMetadataOutputTypeDef",
     "EksMetadataTypeDef",
-    "EksSecretOutputTypeDef",
     "EksSecretTypeDef",
-    "EvaluateOnExitOutputTypeDef",
     "EvaluateOnExitTypeDef",
-    "ShareAttributesOutputTypeDef",
     "ShareAttributesTypeDef",
-    "HostOutputTypeDef",
     "HostTypeDef",
-    "JobTimeoutOutputTypeDef",
-    "JobDependencyOutputTypeDef",
+    "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
-    "JobTimeoutTypeDef",
     "KeyValuesPairTypeDef",
     "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterJobDefinitionResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubmitJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdatePolicyTypeDef",
-    "UpdateComputeEnvironmentResponseTypeDef",
-    "UpdateJobQueueResponseTypeDef",
     "AttemptContainerDetailTypeDef",
-    "JobQueueDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
+    "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
     "ComputeResourceOutputTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
-    "LogConfigurationOutputTypeDef",
     "ContainerOverridesTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
-    "EFSVolumeConfigurationOutputTypeDef",
+    "CreateComputeEnvironmentResponseTypeDef",
+    "CreateJobQueueResponseTypeDef",
+    "CreateSchedulingPolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterJobDefinitionResponseTypeDef",
+    "SubmitJobResponseTypeDef",
+    "UpdateComputeEnvironmentResponseTypeDef",
+    "UpdateJobQueueResponseTypeDef",
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
     "EksContainerDetailTypeDef",
     "EksContainerOutputTypeDef",
     "EksContainerOverrideTypeDef",
     "EksContainerTypeDef",
-    "EksVolumeOutputTypeDef",
     "EksVolumeTypeDef",
     "RetryStrategyOutputTypeDef",
     "RetryStrategyTypeDef",
     "FairsharePolicyOutputTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
@@ -173,15 +145,14 @@
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
-    "VolumeOutputTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
     "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
     "SchedulingPolicyDetailTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
@@ -250,77 +221,39 @@
     "CancelJobRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
 
-EksConfigurationOutputTypeDef = TypedDict(
-    "EksConfigurationOutputTypeDef",
+EksConfigurationTypeDef = TypedDict(
+    "EksConfigurationTypeDef",
     {
         "eksClusterArn": str,
         "kubernetesNamespace": str,
     },
 )
 
-UpdatePolicyOutputTypeDef = TypedDict(
-    "UpdatePolicyOutputTypeDef",
+UpdatePolicyTypeDef = TypedDict(
+    "UpdatePolicyTypeDef",
     {
         "terminateJobsOnUpdate": bool,
         "jobExecutionTimeoutMinutes": int,
     },
     total=False,
 )
 
-ComputeEnvironmentOrderOutputTypeDef = TypedDict(
-    "ComputeEnvironmentOrderOutputTypeDef",
-    {
-        "order": int,
-        "computeEnvironment": str,
-    },
-)
-
 ComputeEnvironmentOrderTypeDef = TypedDict(
     "ComputeEnvironmentOrderTypeDef",
     {
         "order": int,
         "computeEnvironment": str,
     },
 )
 
-_RequiredEc2ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEc2ConfigurationOutputTypeDef",
-    {
-        "imageType": str,
-    },
-)
-_OptionalEc2ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEc2ConfigurationOutputTypeDef",
-    {
-        "imageIdOverride": str,
-        "imageKubernetesVersion": str,
-    },
-    total=False,
-)
-
-class Ec2ConfigurationOutputTypeDef(
-    _RequiredEc2ConfigurationOutputTypeDef, _OptionalEc2ConfigurationOutputTypeDef
-):
-    pass
-
-LaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "LaunchTemplateSpecificationOutputTypeDef",
-    {
-        "launchTemplateId": str,
-        "launchTemplateName": str,
-        "version": str,
-    },
-    total=False,
-)
-
 _RequiredEc2ConfigurationTypeDef = TypedDict(
     "_RequiredEc2ConfigurationTypeDef",
     {
         "imageType": str,
     },
 )
 _OptionalEc2ConfigurationTypeDef = TypedDict(
@@ -341,140 +274,64 @@
         "launchTemplateId": str,
         "launchTemplateName": str,
         "version": str,
     },
     total=False,
 )
 
-EphemeralStorageOutputTypeDef = TypedDict(
-    "EphemeralStorageOutputTypeDef",
+EphemeralStorageTypeDef = TypedDict(
+    "EphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
-FargatePlatformConfigurationOutputTypeDef = TypedDict(
-    "FargatePlatformConfigurationOutputTypeDef",
+FargatePlatformConfigurationTypeDef = TypedDict(
+    "FargatePlatformConfigurationTypeDef",
     {
         "platformVersion": str,
     },
     total=False,
 )
 
-KeyValuePairOutputTypeDef = TypedDict(
-    "KeyValuePairOutputTypeDef",
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
     {
         "name": str,
         "value": str,
     },
     total=False,
 )
 
-MountPointOutputTypeDef = TypedDict(
-    "MountPointOutputTypeDef",
+MountPointTypeDef = TypedDict(
+    "MountPointTypeDef",
     {
         "containerPath": str,
         "readOnly": bool,
         "sourceVolume": str,
     },
     total=False,
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
-ResourceRequirementOutputTypeDef = TypedDict(
-    "ResourceRequirementOutputTypeDef",
-    {
-        "value": str,
-        "type": ResourceTypeType,
-    },
-)
-
-RuntimePlatformOutputTypeDef = TypedDict(
-    "RuntimePlatformOutputTypeDef",
-    {
-        "operatingSystemFamily": str,
-        "cpuArchitecture": str,
-    },
-    total=False,
-)
-
-SecretOutputTypeDef = TypedDict(
-    "SecretOutputTypeDef",
-    {
-        "name": str,
-        "valueFrom": str,
-    },
-)
-
-UlimitOutputTypeDef = TypedDict(
-    "UlimitOutputTypeDef",
-    {
-        "hardLimit": int,
-        "name": str,
-        "softLimit": int,
-    },
-)
-
-KeyValuePairTypeDef = TypedDict(
-    "KeyValuePairTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-    total=False,
-)
-
 ResourceRequirementTypeDef = TypedDict(
     "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
-EphemeralStorageTypeDef = TypedDict(
-    "EphemeralStorageTypeDef",
-    {
-        "sizeInGiB": int,
-    },
-)
-
-FargatePlatformConfigurationTypeDef = TypedDict(
-    "FargatePlatformConfigurationTypeDef",
-    {
-        "platformVersion": str,
-    },
-    total=False,
-)
-
-MountPointTypeDef = TypedDict(
-    "MountPointTypeDef",
-    {
-        "containerPath": str,
-        "readOnly": bool,
-        "sourceVolume": str,
-    },
-    total=False,
-)
-
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
-    {
-        "assignPublicIp": AssignPublicIpType,
-    },
-    total=False,
-)
-
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "operatingSystemFamily": str,
         "cpuArchitecture": str,
     },
     total=False,
@@ -502,46 +359,22 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-EksConfigurationTypeDef = TypedDict(
-    "EksConfigurationTypeDef",
-    {
-        "eksClusterArn": str,
-        "kubernetesNamespace": str,
-    },
-)
-
-CreateComputeEnvironmentResponseTypeDef = TypedDict(
-    "CreateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateJobQueueResponseTypeDef = TypedDict(
-    "CreateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSchedulingPolicyResponseTypeDef = TypedDict(
-    "CreateSchedulingPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironment": str,
@@ -565,65 +398,46 @@
 DeregisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinition": str,
     },
 )
 
-DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "computeEnvironments": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeComputeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     {
         "computeEnvironments": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    {
-        "jobDefinitions": Sequence[str],
-        "jobDefinitionName": str,
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeJobDefinitionsRequestRequestTypeDef",
     {
         "jobDefinitions": Sequence[str],
         "maxResults": int,
         "jobDefinitionName": str,
         "status": str,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    {
-        "jobQueues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobQueuesRequestRequestTypeDef = TypedDict(
     "DescribeJobQueuesRequestRequestTypeDef",
     {
         "jobQueues": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -676,23 +490,14 @@
     },
     total=False,
 )
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
-EFSAuthorizationConfigOutputTypeDef = TypedDict(
-    "EFSAuthorizationConfigOutputTypeDef",
-    {
-        "accessPointId": str,
-        "iam": EFSAuthorizationConfigIAMType,
-    },
-    total=False,
-)
-
 EFSAuthorizationConfigTypeDef = TypedDict(
     "EFSAuthorizationConfigTypeDef",
     {
         "accessPointId": str,
         "iam": EFSAuthorizationConfigIAMType,
     },
     total=False,
@@ -703,65 +508,14 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-_RequiredEksContainerEnvironmentVariableOutputTypeDef = TypedDict(
-    "_RequiredEksContainerEnvironmentVariableOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalEksContainerEnvironmentVariableOutputTypeDef = TypedDict(
-    "_OptionalEksContainerEnvironmentVariableOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class EksContainerEnvironmentVariableOutputTypeDef(
-    _RequiredEksContainerEnvironmentVariableOutputTypeDef,
-    _OptionalEksContainerEnvironmentVariableOutputTypeDef,
-):
-    pass
-
-EksContainerResourceRequirementsOutputTypeDef = TypedDict(
-    "EksContainerResourceRequirementsOutputTypeDef",
-    {
-        "limits": Dict[str, str],
-        "requests": Dict[str, str],
-    },
-    total=False,
-)
-
-EksContainerSecurityContextOutputTypeDef = TypedDict(
-    "EksContainerSecurityContextOutputTypeDef",
-    {
-        "runAsUser": int,
-        "runAsGroup": int,
-        "privileged": bool,
-        "readOnlyRootFilesystem": bool,
-        "runAsNonRoot": bool,
-    },
-    total=False,
-)
-
-EksContainerVolumeMountOutputTypeDef = TypedDict(
-    "EksContainerVolumeMountOutputTypeDef",
-    {
-        "name": str,
-        "mountPath": str,
-        "readOnly": bool,
-    },
-    total=False,
-)
-
 _RequiredEksContainerEnvironmentVariableTypeDef = TypedDict(
     "_RequiredEksContainerEnvironmentVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalEksContainerEnvironmentVariableTypeDef = TypedDict(
@@ -773,19 +527,19 @@
 )
 
 class EksContainerEnvironmentVariableTypeDef(
     _RequiredEksContainerEnvironmentVariableTypeDef, _OptionalEksContainerEnvironmentVariableTypeDef
 ):
     pass
 
-EksContainerResourceRequirementsTypeDef = TypedDict(
-    "EksContainerResourceRequirementsTypeDef",
+EksContainerResourceRequirementsOutputTypeDef = TypedDict(
+    "EksContainerResourceRequirementsOutputTypeDef",
     {
-        "limits": Mapping[str, str],
-        "requests": Mapping[str, str],
+        "limits": Dict[str, str],
+        "requests": Dict[str, str],
     },
     total=False,
 )
 
 EksContainerSecurityContextTypeDef = TypedDict(
     "EksContainerSecurityContextTypeDef",
     {
@@ -804,40 +558,32 @@
         "name": str,
         "mountPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-EksEmptyDirOutputTypeDef = TypedDict(
-    "EksEmptyDirOutputTypeDef",
+EksContainerResourceRequirementsTypeDef = TypedDict(
+    "EksContainerResourceRequirementsTypeDef",
     {
-        "medium": str,
-        "sizeLimit": str,
+        "limits": Mapping[str, str],
+        "requests": Mapping[str, str],
     },
     total=False,
 )
 
 EksEmptyDirTypeDef = TypedDict(
     "EksEmptyDirTypeDef",
     {
         "medium": str,
         "sizeLimit": str,
     },
     total=False,
 )
 
-EksHostPathOutputTypeDef = TypedDict(
-    "EksHostPathOutputTypeDef",
-    {
-        "path": str,
-    },
-    total=False,
-)
-
 EksHostPathTypeDef = TypedDict(
     "EksHostPathTypeDef",
     {
         "path": str,
     },
     total=False,
 )
@@ -854,31 +600,14 @@
     "EksMetadataTypeDef",
     {
         "labels": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredEksSecretOutputTypeDef = TypedDict(
-    "_RequiredEksSecretOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-_OptionalEksSecretOutputTypeDef = TypedDict(
-    "_OptionalEksSecretOutputTypeDef",
-    {
-        "optional": bool,
-    },
-    total=False,
-)
-
-class EksSecretOutputTypeDef(_RequiredEksSecretOutputTypeDef, _OptionalEksSecretOutputTypeDef):
-    pass
-
 _RequiredEksSecretTypeDef = TypedDict(
     "_RequiredEksSecretTypeDef",
     {
         "secretName": str,
     },
 )
 _OptionalEksSecretTypeDef = TypedDict(
@@ -888,35 +617,14 @@
     },
     total=False,
 )
 
 class EksSecretTypeDef(_RequiredEksSecretTypeDef, _OptionalEksSecretTypeDef):
     pass
 
-_RequiredEvaluateOnExitOutputTypeDef = TypedDict(
-    "_RequiredEvaluateOnExitOutputTypeDef",
-    {
-        "action": RetryActionType,
-    },
-)
-_OptionalEvaluateOnExitOutputTypeDef = TypedDict(
-    "_OptionalEvaluateOnExitOutputTypeDef",
-    {
-        "onStatusReason": str,
-        "onReason": str,
-        "onExitCode": str,
-    },
-    total=False,
-)
-
-class EvaluateOnExitOutputTypeDef(
-    _RequiredEvaluateOnExitOutputTypeDef, _OptionalEvaluateOnExitOutputTypeDef
-):
-    pass
-
 _RequiredEvaluateOnExitTypeDef = TypedDict(
     "_RequiredEvaluateOnExitTypeDef",
     {
         "action": RetryActionType,
     },
 )
 _OptionalEvaluateOnExitTypeDef = TypedDict(
@@ -928,33 +636,14 @@
     },
     total=False,
 )
 
 class EvaluateOnExitTypeDef(_RequiredEvaluateOnExitTypeDef, _OptionalEvaluateOnExitTypeDef):
     pass
 
-_RequiredShareAttributesOutputTypeDef = TypedDict(
-    "_RequiredShareAttributesOutputTypeDef",
-    {
-        "shareIdentifier": str,
-    },
-)
-_OptionalShareAttributesOutputTypeDef = TypedDict(
-    "_OptionalShareAttributesOutputTypeDef",
-    {
-        "weightFactor": float,
-    },
-    total=False,
-)
-
-class ShareAttributesOutputTypeDef(
-    _RequiredShareAttributesOutputTypeDef, _OptionalShareAttributesOutputTypeDef
-):
-    pass
-
 _RequiredShareAttributesTypeDef = TypedDict(
     "_RequiredShareAttributesTypeDef",
     {
         "shareIdentifier": str,
     },
 )
 _OptionalShareAttributesTypeDef = TypedDict(
@@ -964,47 +653,30 @@
     },
     total=False,
 )
 
 class ShareAttributesTypeDef(_RequiredShareAttributesTypeDef, _OptionalShareAttributesTypeDef):
     pass
 
-HostOutputTypeDef = TypedDict(
-    "HostOutputTypeDef",
-    {
-        "sourcePath": str,
-    },
-    total=False,
-)
-
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "sourcePath": str,
     },
     total=False,
 )
 
-JobTimeoutOutputTypeDef = TypedDict(
-    "JobTimeoutOutputTypeDef",
+JobTimeoutTypeDef = TypedDict(
+    "JobTimeoutTypeDef",
     {
         "attemptDurationSeconds": int,
     },
     total=False,
 )
 
-JobDependencyOutputTypeDef = TypedDict(
-    "JobDependencyOutputTypeDef",
-    {
-        "jobId": str,
-        "type": ArrayJobDependencyType,
-    },
-    total=False,
-)
-
 JobDependencyTypeDef = TypedDict(
     "JobDependencyTypeDef",
     {
         "jobId": str,
         "type": ArrayJobDependencyType,
     },
     total=False,
@@ -1025,22 +697,14 @@
         "isMainNode": bool,
         "numNodes": int,
         "nodeIndex": int,
     },
     total=False,
 )
 
-JobTimeoutTypeDef = TypedDict(
-    "JobTimeoutTypeDef",
-    {
-        "attemptDurationSeconds": int,
-    },
-    total=False,
-)
-
 KeyValuesPairTypeDef = TypedDict(
     "KeyValuesPairTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
@@ -1078,22 +742,14 @@
     },
     total=False,
 )
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
-ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "ListSchedulingPoliciesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1109,63 +765,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
-RegisterJobDefinitionResponseTypeDef = TypedDict(
-    "RegisterJobDefinitionResponseTypeDef",
-    {
-        "jobDefinitionName": str,
-        "jobDefinitionArn": str,
-        "revision": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
-SubmitJobResponseTypeDef = TypedDict(
-    "SubmitJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobName": str,
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1182,99 +789,72 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdatePolicyTypeDef = TypedDict(
-    "UpdatePolicyTypeDef",
-    {
-        "terminateJobsOnUpdate": bool,
-        "jobExecutionTimeoutMinutes": int,
-    },
-    total=False,
-)
-
-UpdateComputeEnvironmentResponseTypeDef = TypedDict(
-    "UpdateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateJobQueueResponseTypeDef = TypedDict(
-    "UpdateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttemptContainerDetailTypeDef = TypedDict(
     "AttemptContainerDetailTypeDef",
     {
         "containerInstanceArn": str,
         "taskArn": str,
         "exitCode": int,
         "reason": str,
         "logStreamName": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
-_RequiredJobQueueDetailTypeDef = TypedDict(
-    "_RequiredJobQueueDetailTypeDef",
+_RequiredCreateJobQueueRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobQueueRequestRequestTypeDef",
     {
         "jobQueueName": str,
-        "jobQueueArn": str,
-        "state": JQStateType,
         "priority": int,
-        "computeEnvironmentOrder": List[ComputeEnvironmentOrderOutputTypeDef],
+        "computeEnvironmentOrder": Sequence[ComputeEnvironmentOrderTypeDef],
     },
 )
-_OptionalJobQueueDetailTypeDef = TypedDict(
-    "_OptionalJobQueueDetailTypeDef",
+_OptionalCreateJobQueueRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobQueueRequestRequestTypeDef",
     {
+        "state": JQStateType,
         "schedulingPolicyArn": str,
-        "status": JQStatusType,
-        "statusReason": str,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class JobQueueDetailTypeDef(_RequiredJobQueueDetailTypeDef, _OptionalJobQueueDetailTypeDef):
+class CreateJobQueueRequestRequestTypeDef(
+    _RequiredCreateJobQueueRequestRequestTypeDef, _OptionalCreateJobQueueRequestRequestTypeDef
+):
     pass
 
-_RequiredCreateJobQueueRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobQueueRequestRequestTypeDef",
+_RequiredJobQueueDetailTypeDef = TypedDict(
+    "_RequiredJobQueueDetailTypeDef",
     {
         "jobQueueName": str,
+        "jobQueueArn": str,
+        "state": JQStateType,
         "priority": int,
-        "computeEnvironmentOrder": Sequence[ComputeEnvironmentOrderTypeDef],
+        "computeEnvironmentOrder": List[ComputeEnvironmentOrderTypeDef],
     },
 )
-_OptionalCreateJobQueueRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobQueueRequestRequestTypeDef",
+_OptionalJobQueueDetailTypeDef = TypedDict(
+    "_OptionalJobQueueDetailTypeDef",
     {
-        "state": JQStateType,
         "schedulingPolicyArn": str,
-        "tags": Mapping[str, str],
+        "status": JQStatusType,
+        "statusReason": str,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateJobQueueRequestRequestTypeDef(
-    _RequiredCreateJobQueueRequestRequestTypeDef, _OptionalCreateJobQueueRequestRequestTypeDef
-):
+class JobQueueDetailTypeDef(_RequiredJobQueueDetailTypeDef, _OptionalJobQueueDetailTypeDef):
     pass
 
 _RequiredUpdateJobQueueRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobQueueRequestRequestTypeDef",
     {
         "jobQueue": str,
     },
@@ -1314,16 +894,16 @@
         "securityGroupIds": List[str],
         "ec2KeyPair": str,
         "instanceRole": str,
         "tags": Dict[str, str],
         "placementGroup": str,
         "bidPercentage": int,
         "spotIamFleetRole": str,
-        "launchTemplate": LaunchTemplateSpecificationOutputTypeDef,
-        "ec2Configuration": List[Ec2ConfigurationOutputTypeDef],
+        "launchTemplate": LaunchTemplateSpecificationTypeDef,
+        "ec2Configuration": List[Ec2ConfigurationTypeDef],
     },
     total=False,
 )
 
 class ComputeResourceOutputTypeDef(
     _RequiredComputeResourceOutputTypeDef, _OptionalComputeResourceOutputTypeDef
 ):
@@ -1381,47 +961,47 @@
         "updateToLatestImageVersion": bool,
         "type": CRTypeType,
         "imageId": str,
     },
     total=False,
 )
 
+ContainerOverridesTypeDef = TypedDict(
+    "ContainerOverridesTypeDef",
+    {
+        "vcpus": int,
+        "memory": int,
+        "command": Sequence[str],
+        "instanceType": str,
+        "environment": Sequence[KeyValuePairTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
+    },
+    total=False,
+)
+
 _RequiredLogConfigurationOutputTypeDef = TypedDict(
     "_RequiredLogConfigurationOutputTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationOutputTypeDef = TypedDict(
     "_OptionalLogConfigurationOutputTypeDef",
     {
         "options": Dict[str, str],
-        "secretOptions": List[SecretOutputTypeDef],
+        "secretOptions": List[SecretTypeDef],
     },
     total=False,
 )
 
 class LogConfigurationOutputTypeDef(
     _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
 ):
     pass
 
-ContainerOverridesTypeDef = TypedDict(
-    "ContainerOverridesTypeDef",
-    {
-        "vcpus": int,
-        "memory": int,
-        "command": Sequence[str],
-        "instanceType": str,
-        "environment": Sequence[KeyValuePairTypeDef],
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
-    },
-    total=False,
-)
-
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -1432,35 +1012,123 @@
     },
     total=False,
 )
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
-_RequiredEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEFSVolumeConfigurationOutputTypeDef",
+CreateComputeEnvironmentResponseTypeDef = TypedDict(
+    "CreateComputeEnvironmentResponseTypeDef",
     {
-        "fileSystemId": str,
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEFSVolumeConfigurationOutputTypeDef",
+
+CreateJobQueueResponseTypeDef = TypedDict(
+    "CreateJobQueueResponseTypeDef",
     {
-        "rootDirectory": str,
-        "transitEncryption": EFSTransitEncryptionType,
-        "transitEncryptionPort": int,
-        "authorizationConfig": EFSAuthorizationConfigOutputTypeDef,
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchedulingPolicyResponseTypeDef = TypedDict(
+    "CreateSchedulingPolicyResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterJobDefinitionResponseTypeDef = TypedDict(
+    "RegisterJobDefinitionResponseTypeDef",
+    {
+        "jobDefinitionName": str,
+        "jobDefinitionArn": str,
+        "revision": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitJobResponseTypeDef = TypedDict(
+    "SubmitJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobName": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComputeEnvironmentResponseTypeDef = TypedDict(
+    "UpdateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobQueueResponseTypeDef = TypedDict(
+    "UpdateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    {
+        "computeEnvironments": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class EFSVolumeConfigurationOutputTypeDef(
-    _RequiredEFSVolumeConfigurationOutputTypeDef, _OptionalEFSVolumeConfigurationOutputTypeDef
-):
-    pass
+DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    {
+        "jobDefinitions": Sequence[str],
+        "jobDefinitionName": str,
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    {
+        "jobQueues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
@@ -1497,20 +1165,20 @@
     "EksContainerDetailTypeDef",
     {
         "name": str,
         "image": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
-        "env": List[EksContainerEnvironmentVariableOutputTypeDef],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsOutputTypeDef,
         "exitCode": int,
         "reason": str,
-        "volumeMounts": List[EksContainerVolumeMountOutputTypeDef],
-        "securityContext": EksContainerSecurityContextOutputTypeDef,
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 _RequiredEksContainerOutputTypeDef = TypedDict(
     "_RequiredEksContainerOutputTypeDef",
     {
@@ -1520,18 +1188,18 @@
 _OptionalEksContainerOutputTypeDef = TypedDict(
     "_OptionalEksContainerOutputTypeDef",
     {
         "name": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
-        "env": List[EksContainerEnvironmentVariableOutputTypeDef],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsOutputTypeDef,
-        "volumeMounts": List[EksContainerVolumeMountOutputTypeDef],
-        "securityContext": EksContainerSecurityContextOutputTypeDef,
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 class EksContainerOutputTypeDef(
     _RequiredEksContainerOutputTypeDef, _OptionalEksContainerOutputTypeDef
 ):
@@ -1569,33 +1237,14 @@
     },
     total=False,
 )
 
 class EksContainerTypeDef(_RequiredEksContainerTypeDef, _OptionalEksContainerTypeDef):
     pass
 
-_RequiredEksVolumeOutputTypeDef = TypedDict(
-    "_RequiredEksVolumeOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalEksVolumeOutputTypeDef = TypedDict(
-    "_OptionalEksVolumeOutputTypeDef",
-    {
-        "hostPath": EksHostPathOutputTypeDef,
-        "emptyDir": EksEmptyDirOutputTypeDef,
-        "secret": EksSecretOutputTypeDef,
-    },
-    total=False,
-)
-
-class EksVolumeOutputTypeDef(_RequiredEksVolumeOutputTypeDef, _OptionalEksVolumeOutputTypeDef):
-    pass
-
 _RequiredEksVolumeTypeDef = TypedDict(
     "_RequiredEksVolumeTypeDef",
     {
         "name": str,
     },
 )
 _OptionalEksVolumeTypeDef = TypedDict(
@@ -1611,15 +1260,15 @@
 class EksVolumeTypeDef(_RequiredEksVolumeTypeDef, _OptionalEksVolumeTypeDef):
     pass
 
 RetryStrategyOutputTypeDef = TypedDict(
     "RetryStrategyOutputTypeDef",
     {
         "attempts": int,
-        "evaluateOnExit": List[EvaluateOnExitOutputTypeDef],
+        "evaluateOnExit": List[EvaluateOnExitTypeDef],
     },
     total=False,
 )
 
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
@@ -1630,15 +1279,15 @@
 )
 
 FairsharePolicyOutputTypeDef = TypedDict(
     "FairsharePolicyOutputTypeDef",
     {
         "shareDecaySeconds": int,
         "computeReservation": int,
-        "shareDistribution": List[ShareAttributesOutputTypeDef],
+        "shareDistribution": List[ShareAttributesTypeDef],
     },
     total=False,
 )
 
 FairsharePolicyTypeDef = TypedDict(
     "FairsharePolicyTypeDef",
     {
@@ -1680,15 +1329,15 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "jobQueue": str,
         "arrayJobId": str,
         "multiNodeJobId": str,
         "jobStatus": JobStatusType,
         "filters": Sequence[KeyValuesPairTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
@@ -1730,15 +1379,15 @@
 )
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttemptDetailTypeDef = TypedDict(
     "AttemptDetailTypeDef",
     {
         "container": AttemptContainerDetailTypeDef,
@@ -1750,15 +1399,15 @@
 )
 
 DescribeJobQueuesResponseTypeDef = TypedDict(
     "DescribeJobQueuesResponseTypeDef",
     {
         "jobQueues": List[JobQueueDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComputeEnvironmentDetailTypeDef = TypedDict(
     "_RequiredComputeEnvironmentDetailTypeDef",
     {
         "computeEnvironmentName": str,
@@ -1773,16 +1422,16 @@
         "tags": Dict[str, str],
         "type": CETypeType,
         "state": CEStateType,
         "status": CEStatusType,
         "statusReason": str,
         "computeResources": ComputeResourceOutputTypeDef,
         "serviceRole": str,
-        "updatePolicy": UpdatePolicyOutputTypeDef,
-        "eksConfiguration": EksConfigurationOutputTypeDef,
+        "updatePolicy": UpdatePolicyTypeDef,
+        "eksConfiguration": EksConfigurationTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
         "uuid": str,
     },
     total=False,
 )
 
 class ComputeEnvironmentDetailTypeDef(
@@ -1855,24 +1504,14 @@
 )
 
 class NodePropertyOverrideTypeDef(
     _RequiredNodePropertyOverrideTypeDef, _OptionalNodePropertyOverrideTypeDef
 ):
     pass
 
-VolumeOutputTypeDef = TypedDict(
-    "VolumeOutputTypeDef",
-    {
-        "host": HostOutputTypeDef,
-        "name": str,
-        "efsVolumeConfiguration": EFSVolumeConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "host": HostTypeDef,
         "name": str,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
     },
@@ -1891,30 +1530,30 @@
 EksPodPropertiesDetailTypeDef = TypedDict(
     "EksPodPropertiesDetailTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
-        "volumes": List[EksVolumeOutputTypeDef],
+        "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
         "metadata": EksMetadataOutputTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesOutputTypeDef = TypedDict(
     "EksPodPropertiesOutputTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerOutputTypeDef],
-        "volumes": List[EksVolumeOutputTypeDef],
+        "volumes": List[EksVolumeTypeDef],
         "metadata": EksMetadataOutputTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
@@ -1992,24 +1631,24 @@
     pass
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobSummaryList": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComputeEnvironmentsResponseTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponseTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeOverridesTypeDef = TypedDict(
     "NodeOverridesTypeDef",
     {
         "numNodes": int,
@@ -2023,65 +1662,65 @@
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
-        "volumes": List[VolumeOutputTypeDef],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "mountPoints": List[MountPointOutputTypeDef],
+        "volumes": List[VolumeTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
-        "ulimits": List[UlimitOutputTypeDef],
+        "ulimits": List[UlimitTypeDef],
         "privileged": bool,
         "user": str,
         "exitCode": int,
         "reason": str,
         "containerInstanceArn": str,
         "taskArn": str,
         "logStreamName": str,
         "instanceType": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersOutputTypeDef,
         "logConfiguration": LogConfigurationOutputTypeDef,
-        "secrets": List[SecretOutputTypeDef],
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "fargatePlatformConfiguration": FargatePlatformConfigurationOutputTypeDef,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
-        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "secrets": List[SecretTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesOutputTypeDef = TypedDict(
     "ContainerPropertiesOutputTypeDef",
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
-        "volumes": List[VolumeOutputTypeDef],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "mountPoints": List[MountPointOutputTypeDef],
+        "volumes": List[VolumeTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
         "privileged": bool,
-        "ulimits": List[UlimitOutputTypeDef],
+        "ulimits": List[UlimitTypeDef],
         "user": str,
         "instanceType": str,
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersOutputTypeDef,
         "logConfiguration": LogConfigurationOutputTypeDef,
-        "secrets": List[SecretOutputTypeDef],
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "fargatePlatformConfiguration": FargatePlatformConfigurationOutputTypeDef,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
-        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "secrets": List[SecretTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesTypeDef = TypedDict(
     "ContainerPropertiesTypeDef",
     {
@@ -2143,15 +1782,15 @@
     total=False,
 )
 
 DescribeSchedulingPoliciesResponseTypeDef = TypedDict(
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNodeRangePropertyOutputTypeDef = TypedDict(
     "_RequiredNodeRangePropertyOutputTypeDef",
     {
         "targetNodes": str,
@@ -2252,15 +1891,15 @@
     "_OptionalJobDefinitionTypeDef",
     {
         "status": str,
         "schedulingPriority": int,
         "parameters": Dict[str, str],
         "retryStrategy": RetryStrategyOutputTypeDef,
         "containerProperties": ContainerPropertiesOutputTypeDef,
-        "timeout": JobTimeoutOutputTypeDef,
+        "timeout": JobTimeoutTypeDef,
         "nodeProperties": NodePropertiesOutputTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesOutputTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
     },
@@ -2288,21 +1927,21 @@
         "shareIdentifier": str,
         "schedulingPriority": int,
         "attempts": List[AttemptDetailTypeDef],
         "statusReason": str,
         "createdAt": int,
         "retryStrategy": RetryStrategyOutputTypeDef,
         "stoppedAt": int,
-        "dependsOn": List[JobDependencyOutputTypeDef],
+        "dependsOn": List[JobDependencyTypeDef],
         "parameters": Dict[str, str],
         "container": ContainerDetailTypeDef,
         "nodeDetails": NodeDetailsTypeDef,
         "nodeProperties": NodePropertiesOutputTypeDef,
         "arrayProperties": ArrayPropertiesDetailTypeDef,
-        "timeout": JobTimeoutOutputTypeDef,
+        "timeout": JobTimeoutTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesDetailTypeDef,
         "eksAttempts": List[EksAttemptDetailTypeDef],
         "isCancelled": bool,
         "isTerminated": bool,
@@ -2344,18 +1983,18 @@
     pass
 
 DescribeJobDefinitionsResponseTypeDef = TypedDict(
     "DescribeJobDefinitionsResponseTypeDef",
     {
         "jobDefinitions": List[JobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "jobs": List[JobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/PKG-INFO` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.12
-Summary: Type annotations for boto3.Batch 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,126 +365,98 @@
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
     CancelJobRequestRequestTypeDef,
-    EksConfigurationOutputTypeDef,
-    UpdatePolicyOutputTypeDef,
-    ComputeEnvironmentOrderOutputTypeDef,
+    EksConfigurationTypeDef,
+    UpdatePolicyTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    Ec2ConfigurationOutputTypeDef,
-    LaunchTemplateSpecificationOutputTypeDef,
     Ec2ConfigurationTypeDef,
     LaunchTemplateSpecificationTypeDef,
-    EphemeralStorageOutputTypeDef,
-    FargatePlatformConfigurationOutputTypeDef,
-    KeyValuePairOutputTypeDef,
-    MountPointOutputTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    ResourceRequirementOutputTypeDef,
-    RuntimePlatformOutputTypeDef,
-    SecretOutputTypeDef,
-    UlimitOutputTypeDef,
-    KeyValuePairTypeDef,
-    ResourceRequirementTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
+    KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
+    ResourceRequirementTypeDef,
     RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    EksConfigurationTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
     DeviceOutputTypeDef,
     DeviceTypeDef,
-    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
-    EksContainerEnvironmentVariableOutputTypeDef,
-    EksContainerResourceRequirementsOutputTypeDef,
-    EksContainerSecurityContextOutputTypeDef,
-    EksContainerVolumeMountOutputTypeDef,
     EksContainerEnvironmentVariableTypeDef,
-    EksContainerResourceRequirementsTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
-    EksEmptyDirOutputTypeDef,
+    EksContainerResourceRequirementsTypeDef,
     EksEmptyDirTypeDef,
-    EksHostPathOutputTypeDef,
     EksHostPathTypeDef,
     EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
-    EksSecretOutputTypeDef,
     EksSecretTypeDef,
-    EvaluateOnExitOutputTypeDef,
     EvaluateOnExitTypeDef,
-    ShareAttributesOutputTypeDef,
     ShareAttributesTypeDef,
-    HostOutputTypeDef,
     HostTypeDef,
-    JobTimeoutOutputTypeDef,
-    JobDependencyOutputTypeDef,
+    JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
-    JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePolicyTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
-    JobQueueDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
+    JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
     ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
-    LogConfigurationOutputTypeDef,
     ContainerOverridesTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
-    EFSVolumeConfigurationOutputTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    SubmitJobResponseTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
     EksContainerDetailTypeDef,
     EksContainerOutputTypeDef,
     EksContainerOverrideTypeDef,
     EksContainerTypeDef,
-    EksVolumeOutputTypeDef,
     EksVolumeTypeDef,
     RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
     FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
@@ -494,15 +466,14 @@
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
-    VolumeOutputTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
     EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
     SchedulingPolicyDetailTypeDef,
     CreateSchedulingPolicyRequestRequestTypeDef,
```

### Comparing `mypy-boto3-batch-1.28.12/mypy_boto3_batch.egg-info/SOURCES.txt` & `mypy-boto3-batch-1.28.15/mypy_boto3_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.12/setup.py` & `mypy-boto3-batch-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-batch",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Batch 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

