# Comparing `tmp/mypy-boto3-ecs-1.28.12.tar.gz` & `tmp/mypy-boto3-ecs-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
```

## Comparing `mypy-boto3-ecs-1.28.12.tar` & `mypy-boto3-ecs-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26619 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25148 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.072522 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   107340 2023-07-27 05:21:36.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   107211 2023-07-27 05:21:35.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-27 05:21:34.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26619 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.076522 mypy-boto3-ecs-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:33.000000 mypy-boto3-ecs-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.709040 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:24:51.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-28 20:24:53.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-07-28 20:24:53.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:51.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    95601 2023-07-28 20:24:56.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95482 2023-07-28 20:24:54.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-28 20:24:52.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:43.000000 mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.717040 mypy-boto3-ecs-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:24:50.000000 mypy-boto3-ecs-1.28.15/setup.py
```

### Comparing `mypy-boto3-ecs-1.28.12/LICENSE` & `mypy-boto3-ecs-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/PKG-INFO` & `mypy-boto3-ecs-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.12
-Summary: Type annotations for boto3.ECS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -445,63 +445,46 @@
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
-    KeyValuePairOutputTypeDef,
-    AttributeOutputTypeDef,
+    KeyValuePairTypeDef,
     AttributeTypeDef,
-    ManagedScalingOutputTypeDef,
     ManagedScalingTypeDef,
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
-    ClusterSettingOutputTypeDef,
     ClusterSettingTypeDef,
-    ContainerDependencyOutputTypeDef,
-    EnvironmentFileOutputTypeDef,
-    FirelensConfigurationOutputTypeDef,
-    HealthCheckOutputTypeDef,
-    HostEntryOutputTypeDef,
-    MountPointOutputTypeDef,
-    PortMappingOutputTypeDef,
-    RepositoryCredentialsOutputTypeDef,
-    ResourceRequirementOutputTypeDef,
-    SecretOutputTypeDef,
-    SystemControlOutputTypeDef,
-    UlimitOutputTypeDef,
-    VolumeFromOutputTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
-    FirelensConfigurationTypeDef,
-    HealthCheckTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
     HostEntryTypeDef,
-    KeyValuePairTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
+    FirelensConfigurationTypeDef,
+    HealthCheckTypeDef,
     InstanceHealthCheckResultTypeDef,
     ResourceOutputTypeDef,
-    VersionInfoOutputTypeDef,
+    VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
-    NetworkBindingOutputTypeDef,
     NetworkInterfaceTypeDef,
-    TagTypeDef,
+    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
@@ -510,172 +493,148 @@
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
     DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
-    DeploymentCircuitBreakerOutputTypeDef,
     DeploymentCircuitBreakerTypeDef,
-    DeploymentControllerOutputTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
     DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
     DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
-    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
-    EphemeralStorageOutputTypeDef,
     EphemeralStorageTypeDef,
-    ExecuteCommandLogConfigurationOutputTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
-    FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
-    HostVolumePropertiesOutputTypeDef,
     HostVolumePropertiesTypeDef,
-    InferenceAcceleratorOutputTypeDef,
-    InferenceAcceleratorOverrideOutputTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
     KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
     TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
-    LoadBalancerOutputTypeDef,
     ManagedAgentStateChangeTypeDef,
-    PaginatorConfigTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     ResourceTypeDef,
-    VersionInfoTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    ResponseMetadataTypeDef,
-    RuntimePlatformOutputTypeDef,
-    ScaleOutputTypeDef,
-    ServiceConnectClientAliasOutputTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
-    ServiceRegistryOutputTypeDef,
     StopTaskRequestRequestTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
-    TaskDefinitionPlacementConstraintOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
     ProxyConfigurationOutputTypeDef,
-    DeleteAttributesResponseTypeDef,
-    ListAttributesResponseTypeDef,
-    PutAttributesResponseTypeDef,
+    ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
     PutAttributesRequestRequestTypeDef,
-    AutoScalingGroupProviderOutputTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
     ContainerOverrideOutputTypeDef,
-    LogConfigurationOutputTypeDef,
-    ProxyConfigurationTypeDef,
     ContainerOverrideTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DeleteAttributesResponseTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
+    ListAttributesResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksResponseTypeDef,
+    PutAttributesResponseTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
-    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
-    ExecuteCommandConfigurationOutputTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
-    FSxWindowsFileServerVolumeConfigurationOutputTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     TaskSetTypeDef,
     CreateTaskSetRequestRequestTypeDef,
     TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
-    ClusterConfigurationOutputTypeDef,
     ClusterConfigurationTypeDef,
     VolumeOutputTypeDef,
     VolumeTypeDef,
     ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
     ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
```

### Comparing `mypy-boto3-ecs-1.28.12/README.md` & `mypy-boto3-ecs-1.28.15/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -413,63 +413,46 @@
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
-    KeyValuePairOutputTypeDef,
-    AttributeOutputTypeDef,
+    KeyValuePairTypeDef,
     AttributeTypeDef,
-    ManagedScalingOutputTypeDef,
     ManagedScalingTypeDef,
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
-    ClusterSettingOutputTypeDef,
     ClusterSettingTypeDef,
-    ContainerDependencyOutputTypeDef,
-    EnvironmentFileOutputTypeDef,
-    FirelensConfigurationOutputTypeDef,
-    HealthCheckOutputTypeDef,
-    HostEntryOutputTypeDef,
-    MountPointOutputTypeDef,
-    PortMappingOutputTypeDef,
-    RepositoryCredentialsOutputTypeDef,
-    ResourceRequirementOutputTypeDef,
-    SecretOutputTypeDef,
-    SystemControlOutputTypeDef,
-    UlimitOutputTypeDef,
-    VolumeFromOutputTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
-    FirelensConfigurationTypeDef,
-    HealthCheckTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
     HostEntryTypeDef,
-    KeyValuePairTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
+    FirelensConfigurationTypeDef,
+    HealthCheckTypeDef,
     InstanceHealthCheckResultTypeDef,
     ResourceOutputTypeDef,
-    VersionInfoOutputTypeDef,
+    VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
-    NetworkBindingOutputTypeDef,
     NetworkInterfaceTypeDef,
-    TagTypeDef,
+    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
@@ -478,172 +461,148 @@
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
     DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
-    DeploymentCircuitBreakerOutputTypeDef,
     DeploymentCircuitBreakerTypeDef,
-    DeploymentControllerOutputTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
     DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
     DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
-    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
-    EphemeralStorageOutputTypeDef,
     EphemeralStorageTypeDef,
-    ExecuteCommandLogConfigurationOutputTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
-    FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
-    HostVolumePropertiesOutputTypeDef,
     HostVolumePropertiesTypeDef,
-    InferenceAcceleratorOutputTypeDef,
-    InferenceAcceleratorOverrideOutputTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
     KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
     TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
-    LoadBalancerOutputTypeDef,
     ManagedAgentStateChangeTypeDef,
-    PaginatorConfigTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     ResourceTypeDef,
-    VersionInfoTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    ResponseMetadataTypeDef,
-    RuntimePlatformOutputTypeDef,
-    ScaleOutputTypeDef,
-    ServiceConnectClientAliasOutputTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
-    ServiceRegistryOutputTypeDef,
     StopTaskRequestRequestTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
-    TaskDefinitionPlacementConstraintOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
     ProxyConfigurationOutputTypeDef,
-    DeleteAttributesResponseTypeDef,
-    ListAttributesResponseTypeDef,
-    PutAttributesResponseTypeDef,
+    ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
     PutAttributesRequestRequestTypeDef,
-    AutoScalingGroupProviderOutputTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
     ContainerOverrideOutputTypeDef,
-    LogConfigurationOutputTypeDef,
-    ProxyConfigurationTypeDef,
     ContainerOverrideTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DeleteAttributesResponseTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
+    ListAttributesResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksResponseTypeDef,
+    PutAttributesResponseTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
-    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
-    ExecuteCommandConfigurationOutputTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
-    FSxWindowsFileServerVolumeConfigurationOutputTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     TaskSetTypeDef,
     CreateTaskSetRequestRequestTypeDef,
     TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
-    ClusterConfigurationOutputTypeDef,
     ClusterConfigurationTypeDef,
     VolumeOutputTypeDef,
     VolumeTypeDef,
     ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
     ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
```

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ECS 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
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

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,189 +64,177 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
     "ListServicesPaginator",
     "ListServicesByNamespacePaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
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
 class ListAccountSettingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
     """
 
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
         """
 
-
 class ListAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
     """
 
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
         """
 
-
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
         """
 
-
 class ListContainerInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
         """
 
-
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
         """
 
-
 class ListServicesByNamespacePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
     """
 
     def paginate(
-        self, *, namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesByNamespaceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
         """
 
-
 class ListTaskDefinitionFamiliesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
-
 class ListTaskDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
-
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
     """
 
     def paginate(
@@ -255,13 +243,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,177 +64,189 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
     "ListServicesPaginator",
     "ListServicesByNamespacePaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
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
 class ListAccountSettingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
     """
 
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
         """
 
+
 class ListAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
     """
 
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
         """
 
+
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
         """
 
+
 class ListContainerInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
         """
 
+
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
         """
 
+
 class ListServicesByNamespacePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
     """
 
     def paginate(
-        self, *, namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesByNamespaceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
         """
 
+
 class ListTaskDefinitionFamiliesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
+
 class ListTaskDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
+
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
     """
 
     def paginate(
@@ -243,13 +255,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,63 +70,46 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttachmentStateChangeTypeDef",
-    "KeyValuePairOutputTypeDef",
-    "AttributeOutputTypeDef",
+    "KeyValuePairTypeDef",
     "AttributeTypeDef",
-    "ManagedScalingOutputTypeDef",
     "ManagedScalingTypeDef",
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
-    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
-    "ClusterSettingOutputTypeDef",
     "ClusterSettingTypeDef",
-    "ContainerDependencyOutputTypeDef",
-    "EnvironmentFileOutputTypeDef",
-    "FirelensConfigurationOutputTypeDef",
-    "HealthCheckOutputTypeDef",
-    "HostEntryOutputTypeDef",
-    "MountPointOutputTypeDef",
-    "PortMappingOutputTypeDef",
-    "RepositoryCredentialsOutputTypeDef",
-    "ResourceRequirementOutputTypeDef",
-    "SecretOutputTypeDef",
-    "SystemControlOutputTypeDef",
-    "UlimitOutputTypeDef",
-    "VolumeFromOutputTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
-    "FirelensConfigurationTypeDef",
-    "HealthCheckTypeDef",
+    "FirelensConfigurationOutputTypeDef",
+    "HealthCheckOutputTypeDef",
     "HostEntryTypeDef",
-    "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
+    "FirelensConfigurationTypeDef",
+    "HealthCheckTypeDef",
     "InstanceHealthCheckResultTypeDef",
     "ResourceOutputTypeDef",
-    "VersionInfoOutputTypeDef",
+    "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
-    "NetworkBindingOutputTypeDef",
     "NetworkInterfaceTypeDef",
-    "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
@@ -135,172 +118,148 @@
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
     "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
-    "DeploymentCircuitBreakerOutputTypeDef",
     "DeploymentCircuitBreakerTypeDef",
-    "DeploymentControllerOutputTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
     "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
-    "DiscoverPollEndpointResponseTypeDef",
     "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
-    "EFSAuthorizationConfigOutputTypeDef",
     "EFSAuthorizationConfigTypeDef",
-    "EphemeralStorageOutputTypeDef",
     "EphemeralStorageTypeDef",
-    "ExecuteCommandLogConfigurationOutputTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
-    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
-    "HostVolumePropertiesOutputTypeDef",
     "HostVolumePropertiesTypeDef",
-    "InferenceAcceleratorOutputTypeDef",
-    "InferenceAcceleratorOverrideOutputTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
     "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
     "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
-    "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
-    "ListContainerInstancesResponseTypeDef",
-    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
-    "ListServicesByNamespaceResponseTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
-    "ListServicesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
-    "ListTaskDefinitionsResponseTypeDef",
-    "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseTypeDef",
-    "LoadBalancerOutputTypeDef",
     "ManagedAgentStateChangeTypeDef",
-    "PaginatorConfigTypeDef",
-    "PlacementConstraintOutputTypeDef",
-    "PlacementStrategyOutputTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "ResourceTypeDef",
-    "VersionInfoTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
-    "ResponseMetadataTypeDef",
-    "RuntimePlatformOutputTypeDef",
-    "ScaleOutputTypeDef",
-    "ServiceConnectClientAliasOutputTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
-    "ServiceRegistryOutputTypeDef",
     "StopTaskRequestRequestTypeDef",
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    "SubmitContainerStateChangeResponseTypeDef",
-    "SubmitTaskStateChangeResponseTypeDef",
-    "TaskDefinitionPlacementConstraintOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
     "ProxyConfigurationOutputTypeDef",
-    "DeleteAttributesResponseTypeDef",
-    "ListAttributesResponseTypeDef",
-    "PutAttributesResponseTypeDef",
+    "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
     "PutAttributesRequestRequestTypeDef",
-    "AutoScalingGroupProviderOutputTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
     "ContainerOverrideOutputTypeDef",
-    "LogConfigurationOutputTypeDef",
-    "ProxyConfigurationTypeDef",
     "ContainerOverrideTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "DeleteAttributesResponseTypeDef",
+    "DiscoverPollEndpointResponseTypeDef",
+    "ListAttributesResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
+    "ListServicesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    "ListTaskDefinitionsResponseTypeDef",
+    "ListTasksResponseTypeDef",
+    "PutAttributesResponseTypeDef",
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    "SubmitContainerStateChangeResponseTypeDef",
+    "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
     "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
-    "EFSVolumeConfigurationOutputTypeDef",
     "EFSVolumeConfigurationTypeDef",
-    "ExecuteCommandConfigurationOutputTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
-    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
     "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "ListAttributesRequestListAttributesPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    "ListTasksRequestListTasksPaginateTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "TaskSetTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
     "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
-    "ClusterConfigurationOutputTypeDef",
     "ClusterConfigurationTypeDef",
     "VolumeOutputTypeDef",
     "VolumeTypeDef",
     "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
     "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
@@ -354,44 +313,23 @@
     "AttachmentStateChangeTypeDef",
     {
         "attachmentArn": str,
         "status": str,
     },
 )
 
-KeyValuePairOutputTypeDef = TypedDict(
-    "KeyValuePairOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-    total=False,
-)
-
-_RequiredAttributeOutputTypeDef = TypedDict(
-    "_RequiredAttributeOutputTypeDef",
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAttributeOutputTypeDef = TypedDict(
-    "_OptionalAttributeOutputTypeDef",
-    {
         "value": str,
-        "targetType": Literal["container-instance"],
-        "targetId": str,
     },
     total=False,
 )
 
-
-class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
-    pass
-
-
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "name": str,
     },
 )
 _OptionalAttributeTypeDef = TypedDict(
@@ -405,26 +343,14 @@
 )
 
 
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
 
-ManagedScalingOutputTypeDef = TypedDict(
-    "ManagedScalingOutputTypeDef",
-    {
-        "status": ManagedScalingStatusType,
-        "targetCapacity": int,
-        "minimumScalingStepSize": int,
-        "maximumScalingStepSize": int,
-        "instanceWarmupPeriod": int,
-    },
-    total=False,
-)
-
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
@@ -473,37 +399,14 @@
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
 
-_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "capacityProvider": str,
-    },
-)
-_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "weight": int,
-        "base": int,
-    },
-    total=False,
-)
-
-
-class CapacityProviderStrategyItemOutputTypeDef(
-    _RequiredCapacityProviderStrategyItemOutputTypeDef,
-    _OptionalCapacityProviderStrategyItemOutputTypeDef,
-):
-    pass
-
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -518,16 +421,16 @@
 
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
 
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
 
@@ -542,42 +445,33 @@
     "ClusterServiceConnectDefaultsTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
-ClusterSettingOutputTypeDef = TypedDict(
-    "ClusterSettingOutputTypeDef",
-    {
-        "name": Literal["containerInsights"],
-        "value": str,
-    },
-    total=False,
-)
-
 ClusterSettingTypeDef = TypedDict(
     "ClusterSettingTypeDef",
     {
         "name": Literal["containerInsights"],
         "value": str,
     },
     total=False,
 )
 
-ContainerDependencyOutputTypeDef = TypedDict(
-    "ContainerDependencyOutputTypeDef",
+ContainerDependencyTypeDef = TypedDict(
+    "ContainerDependencyTypeDef",
     {
         "containerName": str,
         "condition": ContainerConditionType,
     },
 )
 
-EnvironmentFileOutputTypeDef = TypedDict(
-    "EnvironmentFileOutputTypeDef",
+EnvironmentFileTypeDef = TypedDict(
+    "EnvironmentFileTypeDef",
     {
         "value": str,
         "type": Literal["s3"],
     },
 )
 
 _RequiredFirelensConfigurationOutputTypeDef = TypedDict(
@@ -621,111 +515,95 @@
 
 class HealthCheckOutputTypeDef(
     _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
 ):
     pass
 
 
-HostEntryOutputTypeDef = TypedDict(
-    "HostEntryOutputTypeDef",
+HostEntryTypeDef = TypedDict(
+    "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
 
-MountPointOutputTypeDef = TypedDict(
-    "MountPointOutputTypeDef",
+MountPointTypeDef = TypedDict(
+    "MountPointTypeDef",
     {
         "sourceVolume": str,
         "containerPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-PortMappingOutputTypeDef = TypedDict(
-    "PortMappingOutputTypeDef",
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
     {
         "containerPort": int,
         "hostPort": int,
         "protocol": TransportProtocolType,
         "name": str,
         "appProtocol": ApplicationProtocolType,
         "containerPortRange": str,
     },
     total=False,
 )
 
-RepositoryCredentialsOutputTypeDef = TypedDict(
-    "RepositoryCredentialsOutputTypeDef",
+RepositoryCredentialsTypeDef = TypedDict(
+    "RepositoryCredentialsTypeDef",
     {
         "credentialsParameter": str,
     },
 )
 
-ResourceRequirementOutputTypeDef = TypedDict(
-    "ResourceRequirementOutputTypeDef",
+ResourceRequirementTypeDef = TypedDict(
+    "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
-SecretOutputTypeDef = TypedDict(
-    "SecretOutputTypeDef",
+SecretTypeDef = TypedDict(
+    "SecretTypeDef",
     {
         "name": str,
         "valueFrom": str,
     },
 )
 
-SystemControlOutputTypeDef = TypedDict(
-    "SystemControlOutputTypeDef",
+SystemControlTypeDef = TypedDict(
+    "SystemControlTypeDef",
     {
         "namespace": str,
         "value": str,
     },
     total=False,
 )
 
-UlimitOutputTypeDef = TypedDict(
-    "UlimitOutputTypeDef",
+UlimitTypeDef = TypedDict(
+    "UlimitTypeDef",
     {
         "name": UlimitNameType,
         "softLimit": int,
         "hardLimit": int,
     },
 )
 
-VolumeFromOutputTypeDef = TypedDict(
-    "VolumeFromOutputTypeDef",
+VolumeFromTypeDef = TypedDict(
+    "VolumeFromTypeDef",
     {
         "sourceContainer": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-ContainerDependencyTypeDef = TypedDict(
-    "ContainerDependencyTypeDef",
-    {
-        "containerName": str,
-        "condition": ContainerConditionType,
-    },
-)
-
-EnvironmentFileTypeDef = TypedDict(
-    "EnvironmentFileTypeDef",
-    {
-        "value": str,
-        "type": Literal["s3"],
-    },
-)
-
 _RequiredFirelensConfigurationTypeDef = TypedDict(
     "_RequiredFirelensConfigurationTypeDef",
     {
         "type": FirelensConfigurationTypeType,
     },
 )
 _OptionalFirelensConfigurationTypeDef = TypedDict(
@@ -761,104 +639,14 @@
 )
 
 
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
 
-HostEntryTypeDef = TypedDict(
-    "HostEntryTypeDef",
-    {
-        "hostname": str,
-        "ipAddress": str,
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
-MountPointTypeDef = TypedDict(
-    "MountPointTypeDef",
-    {
-        "sourceVolume": str,
-        "containerPath": str,
-        "readOnly": bool,
-    },
-    total=False,
-)
-
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "containerPort": int,
-        "hostPort": int,
-        "protocol": TransportProtocolType,
-        "name": str,
-        "appProtocol": ApplicationProtocolType,
-        "containerPortRange": str,
-    },
-    total=False,
-)
-
-RepositoryCredentialsTypeDef = TypedDict(
-    "RepositoryCredentialsTypeDef",
-    {
-        "credentialsParameter": str,
-    },
-)
-
-ResourceRequirementTypeDef = TypedDict(
-    "ResourceRequirementTypeDef",
-    {
-        "value": str,
-        "type": ResourceTypeType,
-    },
-)
-
-SecretTypeDef = TypedDict(
-    "SecretTypeDef",
-    {
-        "name": str,
-        "valueFrom": str,
-    },
-)
-
-SystemControlTypeDef = TypedDict(
-    "SystemControlTypeDef",
-    {
-        "namespace": str,
-        "value": str,
-    },
-    total=False,
-)
-
-UlimitTypeDef = TypedDict(
-    "UlimitTypeDef",
-    {
-        "name": UlimitNameType,
-        "softLimit": int,
-        "hardLimit": int,
-    },
-)
-
-VolumeFromTypeDef = TypedDict(
-    "VolumeFromTypeDef",
-    {
-        "sourceContainer": str,
-        "readOnly": bool,
-    },
-    total=False,
-)
-
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
@@ -875,16 +663,16 @@
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
     },
     total=False,
 )
 
-VersionInfoOutputTypeDef = TypedDict(
-    "VersionInfoOutputTypeDef",
+VersionInfoTypeDef = TypedDict(
+    "VersionInfoTypeDef",
     {
         "agentVersion": str,
         "agentHash": str,
         "dockerVersion": str,
     },
     total=False,
 )
@@ -909,44 +697,33 @@
         "name": Literal["ExecuteCommandAgent"],
         "reason": str,
         "lastStatus": str,
     },
     total=False,
 )
 
-NetworkBindingOutputTypeDef = TypedDict(
-    "NetworkBindingOutputTypeDef",
-    {
-        "bindIP": str,
-        "containerPort": int,
-        "hostPort": int,
-        "protocol": TransportProtocolType,
-        "containerPortRange": str,
-        "hostPortRange": str,
-    },
-    total=False,
-)
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "key": str,
-        "value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
@@ -1123,37 +900,22 @@
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
     },
 )
 
-DeploymentCircuitBreakerOutputTypeDef = TypedDict(
-    "DeploymentCircuitBreakerOutputTypeDef",
-    {
-        "enable": bool,
-        "rollback": bool,
-    },
-)
-
 DeploymentCircuitBreakerTypeDef = TypedDict(
     "DeploymentCircuitBreakerTypeDef",
     {
         "enable": bool,
         "rollback": bool,
     },
 )
 
-DeploymentControllerOutputTypeDef = TypedDict(
-    "DeploymentControllerOutputTypeDef",
-    {
-        "type": DeploymentControllerTypeType,
-    },
-)
-
 ServiceConnectServiceResourceTypeDef = TypedDict(
     "ServiceConnectServiceResourceTypeDef",
     {
         "discoveryName": str,
         "discoveryArn": str,
     },
     total=False,
@@ -1375,24 +1137,14 @@
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
-DiscoverPollEndpointResponseTypeDef = TypedDict(
-    "DiscoverPollEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "telemetryEndpoint": str,
-        "serviceConnectEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DockerVolumeConfigurationOutputTypeDef = TypedDict(
     "DockerVolumeConfigurationOutputTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
         "driverOpts": Dict[str, str],
@@ -1409,58 +1161,30 @@
         "driver": str,
         "driverOpts": Mapping[str, str],
         "labels": Mapping[str, str],
     },
     total=False,
 )
 
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
 )
 
-EphemeralStorageOutputTypeDef = TypedDict(
-    "EphemeralStorageOutputTypeDef",
-    {
-        "sizeInGiB": int,
-    },
-)
-
 EphemeralStorageTypeDef = TypedDict(
     "EphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
-ExecuteCommandLogConfigurationOutputTypeDef = TypedDict(
-    "ExecuteCommandLogConfigurationOutputTypeDef",
-    {
-        "cloudWatchLogGroupName": str,
-        "cloudWatchEncryptionEnabled": bool,
-        "s3BucketName": str,
-        "s3EncryptionEnabled": bool,
-        "s3KeyPrefix": str,
-    },
-    total=False,
-)
-
 ExecuteCommandLogConfigurationTypeDef = TypedDict(
     "ExecuteCommandLogConfigurationTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "cloudWatchEncryptionEnabled": bool,
         "s3BucketName": str,
         "s3EncryptionEnabled": bool,
@@ -1499,22 +1223,14 @@
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
     total=False,
 )
 
-FSxWindowsFileServerAuthorizationConfigOutputTypeDef = TypedDict(
-    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
-    {
-        "credentialsParameter": str,
-        "domain": str,
-    },
-)
-
 FSxWindowsFileServerAuthorizationConfigTypeDef = TypedDict(
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     {
         "credentialsParameter": str,
         "domain": str,
     },
 )
@@ -1546,47 +1262,22 @@
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
     total=False,
 )
 
-HostVolumePropertiesOutputTypeDef = TypedDict(
-    "HostVolumePropertiesOutputTypeDef",
-    {
-        "sourcePath": str,
-    },
-    total=False,
-)
-
 HostVolumePropertiesTypeDef = TypedDict(
     "HostVolumePropertiesTypeDef",
     {
         "sourcePath": str,
     },
     total=False,
 )
 
-InferenceAcceleratorOutputTypeDef = TypedDict(
-    "InferenceAcceleratorOutputTypeDef",
-    {
-        "deviceName": str,
-        "deviceType": str,
-    },
-)
-
-InferenceAcceleratorOverrideOutputTypeDef = TypedDict(
-    "InferenceAcceleratorOverrideOutputTypeDef",
-    {
-        "deviceName": str,
-        "deviceType": str,
-    },
-    total=False,
-)
-
 InferenceAcceleratorOverrideTypeDef = TypedDict(
     "InferenceAcceleratorOverrideTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
     total=False,
@@ -1654,22 +1345,20 @@
 )
 
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
 
-ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "name": SettingNameType,
-        "value": str,
-        "principalArn": str,
-        "effectiveSettings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountSettingsRequestRequestTypeDef = TypedDict(
     "ListAccountSettingsRequestRequestTypeDef",
     {
@@ -1679,39 +1368,14 @@
         "effectiveSettings": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "targetType": Literal["container-instance"],
-    },
-)
-_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "cluster": str,
-        "attributeName": str,
-        "attributeValue": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttributesRequestListAttributesPaginateTypeDef(
-    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
-    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributesRequestRequestTypeDef",
     {
         "targetType": Literal["container-instance"],
     },
 )
 _OptionalListAttributesRequestRequestTypeDef = TypedDict(
@@ -1729,94 +1393,35 @@
 
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
 
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusterArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    {
-        "cluster": str,
-        "filter": str,
-        "status": ContainerInstanceStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContainerInstancesRequestRequestTypeDef = TypedDict(
     "ListContainerInstancesRequestRequestTypeDef",
     {
         "cluster": str,
         "filter": str,
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
-ListContainerInstancesResponseTypeDef = TypedDict(
-    "ListContainerInstancesResponseTypeDef",
-    {
-        "containerInstanceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "namespace": str,
-    },
-)
-_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
-    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesByNamespaceRequestRequestTypeDef",
     {
         "namespace": str,
     },
 )
 _OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
@@ -1832,139 +1437,56 @@
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
 
-ListServicesByNamespaceResponseTypeDef = TypedDict(
-    "ListServicesByNamespaceResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "cluster": str,
-        "launchType": LaunchTypeType,
-        "schedulingStrategy": SchedulingStrategyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
     },
     total=False,
 )
 
-ListServicesResponseTypeDef = TypedDict(
-    "ListServicesResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionFamilyStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionFamiliesRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionFamilyStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    {
-        "families": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionStatusType,
-        "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionsRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionStatusType,
         "sort": SortOrderType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListTaskDefinitionsResponseTypeDef",
-    {
-        "taskDefinitionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTasksRequestListTasksPaginateTypeDef = TypedDict(
-    "ListTasksRequestListTasksPaginateTypeDef",
-    {
-        "cluster": str,
-        "containerInstance": str,
-        "family": str,
-        "startedBy": str,
-        "serviceName": str,
-        "desiredStatus": DesiredStatusType,
-        "launchType": LaunchTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTasksRequestRequestTypeDef = TypedDict(
     "ListTasksRequestRequestTypeDef",
     {
         "cluster": str,
         "containerInstance": str,
         "family": str,
         "nextToken": str,
@@ -1973,34 +1495,14 @@
         "serviceName": str,
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
     },
     total=False,
 )
 
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
-    {
-        "taskArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LoadBalancerOutputTypeDef = TypedDict(
-    "LoadBalancerOutputTypeDef",
-    {
-        "targetGroupArn": str,
-        "loadBalancerName": str,
-        "containerName": str,
-        "containerPort": int,
-    },
-    total=False,
-)
-
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -2016,42 +1518,14 @@
 
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
 
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
-PlacementConstraintOutputTypeDef = TypedDict(
-    "PlacementConstraintOutputTypeDef",
-    {
-        "type": PlacementConstraintTypeType,
-        "expression": str,
-    },
-    total=False,
-)
-
-PlacementStrategyOutputTypeDef = TypedDict(
-    "PlacementStrategyOutputTypeDef",
-    {
-        "type": PlacementStrategyTypeType,
-        "field": str,
-    },
-    total=False,
-)
-
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -2095,24 +1569,14 @@
         "longValue": int,
         "integerValue": int,
         "stringSetValue": Sequence[str],
     },
     total=False,
 )
 
-VersionInfoTypeDef = TypedDict(
-    "VersionInfoTypeDef",
-    {
-        "agentVersion": str,
-        "agentHash": str,
-        "dockerVersion": str,
-    },
-    total=False,
-)
-
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -2123,64 +1587,14 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
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
-RuntimePlatformOutputTypeDef = TypedDict(
-    "RuntimePlatformOutputTypeDef",
-    {
-        "cpuArchitecture": CPUArchitectureType,
-        "operatingSystemFamily": OSFamilyType,
-    },
-    total=False,
-)
-
-ScaleOutputTypeDef = TypedDict(
-    "ScaleOutputTypeDef",
-    {
-        "value": float,
-        "unit": Literal["PERCENT"],
-    },
-    total=False,
-)
-
-_RequiredServiceConnectClientAliasOutputTypeDef = TypedDict(
-    "_RequiredServiceConnectClientAliasOutputTypeDef",
-    {
-        "port": int,
-    },
-)
-_OptionalServiceConnectClientAliasOutputTypeDef = TypedDict(
-    "_OptionalServiceConnectClientAliasOutputTypeDef",
-    {
-        "dnsName": str,
-    },
-    total=False,
-)
-
-
-class ServiceConnectClientAliasOutputTypeDef(
-    _RequiredServiceConnectClientAliasOutputTypeDef, _OptionalServiceConnectClientAliasOutputTypeDef
-):
-    pass
-
-
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -2204,25 +1618,14 @@
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
     total=False,
 )
 
-ServiceRegistryOutputTypeDef = TypedDict(
-    "ServiceRegistryOutputTypeDef",
-    {
-        "registryArn": str,
-        "port": int,
-        "containerName": str,
-        "containerPort": int,
-    },
-    total=False,
-)
-
 _RequiredStopTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStopTaskRequestRequestTypeDef",
     {
         "task": str,
     },
 )
 _OptionalStopTaskRequestRequestTypeDef = TypedDict(
@@ -2237,47 +1640,14 @@
 
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
 
-SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitContainerStateChangeResponseTypeDef = TypedDict(
-    "SubmitContainerStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitTaskStateChangeResponseTypeDef = TypedDict(
-    "SubmitTaskStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TaskDefinitionPlacementConstraintOutputTypeDef = TypedDict(
-    "TaskDefinitionPlacementConstraintOutputTypeDef",
-    {
-        "type": Literal["memberOf"],
-        "expression": str,
-    },
-    total=False,
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -2384,65 +1754,62 @@
 
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
-        "details": List[KeyValuePairOutputTypeDef],
+        "details": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
 _RequiredProxyConfigurationOutputTypeDef = TypedDict(
     "_RequiredProxyConfigurationOutputTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationOutputTypeDef = TypedDict(
     "_OptionalProxyConfigurationOutputTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairOutputTypeDef],
+        "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
 
 class ProxyConfigurationOutputTypeDef(
     _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
 ):
     pass
 
 
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
+_RequiredProxyConfigurationTypeDef = TypedDict(
+    "_RequiredProxyConfigurationTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "containerName": str,
     },
 )
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
+_OptionalProxyConfigurationTypeDef = TypedDict(
+    "_OptionalProxyConfigurationTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "type": Literal["APPMESH"],
+        "properties": Sequence[KeyValuePairTypeDef],
     },
+    total=False,
 )
 
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+
+class ProxyConfigurationTypeDef(
+    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
+):
+    pass
+
 
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
@@ -2478,36 +1845,14 @@
 
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAutoScalingGroupProviderOutputTypeDef = TypedDict(
-    "_RequiredAutoScalingGroupProviderOutputTypeDef",
-    {
-        "autoScalingGroupArn": str,
-    },
-)
-_OptionalAutoScalingGroupProviderOutputTypeDef = TypedDict(
-    "_OptionalAutoScalingGroupProviderOutputTypeDef",
-    {
-        "managedScaling": ManagedScalingOutputTypeDef,
-        "managedTerminationProtection": ManagedTerminationProtectionType,
-    },
-    total=False,
-)
-
-
-class AutoScalingGroupProviderOutputTypeDef(
-    _RequiredAutoScalingGroupProviderOutputTypeDef, _OptionalAutoScalingGroupProviderOutputTypeDef
-):
-    pass
-
-
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -2556,19 +1901,19 @@
     {
         "cluster": str,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 UpdateClusterSettingsRequestRequestTypeDef = TypedDict(
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
@@ -2577,83 +1922,61 @@
 )
 
 ContainerOverrideOutputTypeDef = TypedDict(
     "ContainerOverrideOutputTypeDef",
     {
         "name": str,
         "command": List[str],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "environmentFiles": List[EnvironmentFileOutputTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "environmentFiles": List[EnvironmentFileTypeDef],
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "resourceRequirements": List[ResourceRequirementTypeDef],
+    },
+    total=False,
+)
+
+ContainerOverrideTypeDef = TypedDict(
+    "ContainerOverrideTypeDef",
+    {
+        "name": str,
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
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
 
 
-_RequiredProxyConfigurationTypeDef = TypedDict(
-    "_RequiredProxyConfigurationTypeDef",
-    {
-        "containerName": str,
-    },
-)
-_OptionalProxyConfigurationTypeDef = TypedDict(
-    "_OptionalProxyConfigurationTypeDef",
-    {
-        "type": Literal["APPMESH"],
-        "properties": Sequence[KeyValuePairTypeDef],
-    },
-    total=False,
-)
-
-
-class ProxyConfigurationTypeDef(
-    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
-):
-    pass
-
-
-ContainerOverrideTypeDef = TypedDict(
-    "ContainerOverrideTypeDef",
-    {
-        "name": str,
-        "command": Sequence[str],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "environmentFiles": Sequence[EnvironmentFileTypeDef],
-        "cpu": int,
-        "memory": int,
-        "memoryReservation": int,
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
@@ -2716,31 +2039,153 @@
         "name": str,
         "image": str,
         "imageDigest": str,
         "runtimeId": str,
         "lastStatus": str,
         "exitCode": int,
         "reason": str,
-        "networkBindings": List[NetworkBindingOutputTypeDef],
+        "networkBindings": List[NetworkBindingTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "healthStatus": HealthStatusType,
         "managedAgents": List[ManagedAgentTypeDef],
         "cpu": str,
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DiscoverPollEndpointResponseTypeDef = TypedDict(
+    "DiscoverPollEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusterArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainerInstancesResponseTypeDef = TypedDict(
+    "ListContainerInstancesResponseTypeDef",
+    {
+        "containerInstanceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesResponseTypeDef = TypedDict(
+    "ListServicesResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    {
+        "families": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
+    {
+        "taskArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitContainerStateChangeResponseTypeDef = TypedDict(
+    "SubmitContainerStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitTaskStateChangeResponseTypeDef = TypedDict(
+    "SubmitTaskStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
@@ -2750,47 +2195,47 @@
     },
 )
 
 DeleteAccountSettingResponseTypeDef = TypedDict(
     "DeleteAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountSettingsResponseTypeDef = TypedDict(
     "ListAccountSettingsResponseTypeDef",
     {
         "settings": List[SettingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingDefaultResponseTypeDef = TypedDict(
     "PutAccountSettingDefaultResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingResponseTypeDef = TypedDict(
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentConfigurationOutputTypeDef = TypedDict(
     "DeploymentConfigurationOutputTypeDef",
     {
-        "deploymentCircuitBreaker": DeploymentCircuitBreakerOutputTypeDef,
+        "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsOutputTypeDef,
     },
     total=False,
 )
 
@@ -2897,38 +2342,14 @@
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
 
-_RequiredEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEFSVolumeConfigurationOutputTypeDef",
-    {
-        "fileSystemId": str,
-    },
-)
-_OptionalEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEFSVolumeConfigurationOutputTypeDef",
-    {
-        "rootDirectory": str,
-        "transitEncryption": EFSTransitEncryptionType,
-        "transitEncryptionPort": int,
-        "authorizationConfig": EFSAuthorizationConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EFSVolumeConfigurationOutputTypeDef(
-    _RequiredEFSVolumeConfigurationOutputTypeDef, _OptionalEFSVolumeConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -2945,24 +2366,14 @@
 
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
 
-ExecuteCommandConfigurationOutputTypeDef = TypedDict(
-    "ExecuteCommandConfigurationOutputTypeDef",
-    {
-        "kmsKeyId": str,
-        "logging": ExecuteCommandLoggingType,
-        "logConfiguration": ExecuteCommandLogConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2974,24 +2385,15 @@
     {
         "clusterArn": str,
         "containerArn": str,
         "containerName": str,
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-FSxWindowsFileServerVolumeConfigurationOutputTypeDef = TypedDict(
-    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
-    {
-        "fileSystemId": str,
-        "rootDirectory": str,
-        "authorizationConfig": FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
@@ -3001,24 +2403,24 @@
 )
 
 GetTaskProtectionResponseTypeDef = TypedDict(
     "GetTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskProtectionResponseTypeDef = TypedDict(
     "UpdateTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LinuxParametersOutputTypeDef = TypedDict(
     "LinuxParametersOutputTypeDef",
     {
         "capabilities": KernelCapabilitiesOutputTypeDef,
@@ -3042,14 +2444,139 @@
         "tmpfs": Sequence[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
+ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    {
+        "name": SettingNameType,
+        "value": str,
+        "principalArn": str,
+        "effectiveSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "targetType": Literal["container-instance"],
+    },
+)
+_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "cluster": str,
+        "attributeName": str,
+        "attributeValue": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttributesRequestListAttributesPaginateTypeDef(
+    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
+    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
+):
+    pass
+
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    {
+        "cluster": str,
+        "filter": str,
+        "status": ContainerInstanceStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "cluster": str,
+        "launchType": LaunchTypeType,
+        "schedulingStrategy": SchedulingStrategyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionFamilyStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionStatusType,
+        "sort": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTasksRequestListTasksPaginateTypeDef = TypedDict(
+    "ListTasksRequestListTasksPaginateTypeDef",
+    {
+        "cluster": str,
+        "containerInstance": str,
+        "family": str,
+        "startedBy": str,
+        "serviceName": str,
+        "desiredStatus": DesiredStatusType,
+        "launchType": LaunchTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "RegisterContainerInstanceRequestRequestTypeDef",
     {
         "cluster": str,
         "instanceIdentityDocument": str,
         "instanceIdentityDocumentSignature": str,
         "totalResources": Sequence[ResourceTypeDef],
@@ -3068,15 +2595,15 @@
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceOutputTypeDef = TypedDict(
     "_OptionalServiceConnectServiceOutputTypeDef",
     {
         "discoveryName": str,
-        "clientAliases": List[ServiceConnectClientAliasOutputTypeDef],
+        "clientAliases": List[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
 
 class ServiceConnectServiceOutputTypeDef(
@@ -3110,18 +2637,18 @@
 
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
-        "autoScalingGroupProvider": AutoScalingGroupProviderOutputTypeDef,
+        "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
         "updateStatus": CapacityProviderUpdateStatusType,
         "updateStatusReason": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateCapacityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCapacityProviderRequestRequestTypeDef",
     {
@@ -3166,24 +2693,24 @@
         "taskDefinition": str,
         "computedDesiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "createdAt": datetime,
         "updatedAt": datetime,
         "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "loadBalancers": List[LoadBalancerOutputTypeDef],
-        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
-        "scale": ScaleOutputTypeDef,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "scale": ScaleTypeDef,
         "stabilityStatus": StabilityStatusType,
         "stabilityStatusAt": datetime,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
@@ -3217,19 +2744,19 @@
 
 
 TaskOverrideOutputTypeDef = TypedDict(
     "TaskOverrideOutputTypeDef",
     {
         "containerOverrides": List[ContainerOverrideOutputTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideOutputTypeDef],
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
@@ -3247,27 +2774,27 @@
 ContainerInstanceTypeDef = TypedDict(
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
-        "versionInfo": VersionInfoOutputTypeDef,
+        "versionInfo": VersionInfoTypeDef,
         "remainingResources": List[ResourceOutputTypeDef],
         "registeredResources": List[ResourceOutputTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
         "registeredAt": datetime,
         "attachments": List[AttachmentTypeDef],
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "healthStatus": ContainerInstanceHealthStatusTypeDef,
     },
     total=False,
 )
 
 SubmitTaskStateChangeRequestRequestTypeDef = TypedDict(
     "SubmitTaskStateChangeRequestRequestTypeDef",
@@ -3282,40 +2809,30 @@
         "pullStartedAt": Union[datetime, str],
         "pullStoppedAt": Union[datetime, str],
         "executionStoppedAt": Union[datetime, str],
     },
     total=False,
 )
 
-ClusterConfigurationOutputTypeDef = TypedDict(
-    "ClusterConfigurationOutputTypeDef",
-    {
-        "executeCommandConfiguration": ExecuteCommandConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
 VolumeOutputTypeDef = TypedDict(
     "VolumeOutputTypeDef",
     {
         "name": str,
-        "host": HostVolumePropertiesOutputTypeDef,
+        "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
-        "efsVolumeConfiguration": EFSVolumeConfigurationOutputTypeDef,
-        "fsxWindowsFileServerVolumeConfiguration": (
-            FSxWindowsFileServerVolumeConfigurationOutputTypeDef
-        ),
+        "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
+        "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
@@ -3329,50 +2846,50 @@
 )
 
 ContainerDefinitionOutputTypeDef = TypedDict(
     "ContainerDefinitionOutputTypeDef",
     {
         "name": str,
         "image": str,
-        "repositoryCredentials": RepositoryCredentialsOutputTypeDef,
+        "repositoryCredentials": RepositoryCredentialsTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "links": List[str],
-        "portMappings": List[PortMappingOutputTypeDef],
+        "portMappings": List[PortMappingTypeDef],
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "environmentFiles": List[EnvironmentFileOutputTypeDef],
-        "mountPoints": List[MountPointOutputTypeDef],
-        "volumesFrom": List[VolumeFromOutputTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "environmentFiles": List[EnvironmentFileTypeDef],
+        "mountPoints": List[MountPointTypeDef],
+        "volumesFrom": List[VolumeFromTypeDef],
         "linuxParameters": LinuxParametersOutputTypeDef,
-        "secrets": List[SecretOutputTypeDef],
-        "dependsOn": List[ContainerDependencyOutputTypeDef],
+        "secrets": List[SecretTypeDef],
+        "dependsOn": List[ContainerDependencyTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
         "disableNetworking": bool,
         "privileged": bool,
         "readonlyRootFilesystem": bool,
         "dnsServers": List[str],
         "dnsSearchDomains": List[str],
-        "extraHosts": List[HostEntryOutputTypeDef],
+        "extraHosts": List[HostEntryTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
-        "ulimits": List[UlimitOutputTypeDef],
+        "ulimits": List[UlimitTypeDef],
         "logConfiguration": LogConfigurationOutputTypeDef,
         "healthCheck": HealthCheckOutputTypeDef,
-        "systemControls": List[SystemControlOutputTypeDef],
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "systemControls": List[SystemControlTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationOutputTypeDef,
         "credentialSpecs": List[str],
     },
     total=False,
 )
 
 ContainerDefinitionTypeDef = TypedDict(
@@ -3469,124 +2986,124 @@
     pass
 
 
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCapacityProviderResponseTypeDef = TypedDict(
     "DeleteCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCapacityProvidersResponseTypeDef = TypedDict(
     "DescribeCapacityProvidersResponseTypeDef",
     {
         "capacityProviders": List[CapacityProviderTypeDef],
         "failures": List[FailureTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCapacityProviderResponseTypeDef = TypedDict(
     "UpdateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTaskSetResponseTypeDef = TypedDict(
     "CreateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskSetResponseTypeDef = TypedDict(
     "DeleteTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskSetsResponseTypeDef = TypedDict(
     "DescribeTaskSetsResponseTypeDef",
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskSetResponseTypeDef = TypedDict(
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaskTypeDef = TypedDict(
     "TaskTypeDef",
     {
         "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
         "availabilityZone": str,
         "capacityProviderName": str,
         "clusterArn": str,
         "connectivity": ConnectivityType,
         "connectivityAt": datetime,
         "containerInstanceArn": str,
         "containers": List[ContainerTypeDef],
         "cpu": str,
         "createdAt": datetime,
         "desiredStatus": str,
         "enableExecuteCommand": bool,
         "executionStoppedAt": datetime,
         "group": str,
         "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "lastStatus": str,
         "launchType": LaunchTypeType,
         "memory": str,
         "overrides": TaskOverrideOutputTypeDef,
         "platformVersion": str,
         "platformFamily": str,
         "pullStartedAt": datetime,
         "pullStoppedAt": datetime,
         "startedAt": datetime,
         "startedBy": str,
         "stopCode": TaskStopCodeType,
         "stoppedAt": datetime,
         "stoppedReason": str,
         "stoppingAt": datetime,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "taskArn": str,
         "taskDefinitionArn": str,
         "version": int,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
@@ -3654,68 +3171,68 @@
     pass
 
 
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContainerInstancesResponseTypeDef = TypedDict(
     "DescribeContainerInstancesResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterContainerInstanceResponseTypeDef = TypedDict(
     "RegisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerAgentResponseTypeDef = TypedDict(
     "UpdateContainerAgentResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerInstancesStateResponseTypeDef = TypedDict(
     "UpdateContainerInstancesStateResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
-        "configuration": ClusterConfigurationOutputTypeDef,
+        "configuration": ClusterConfigurationTypeDef,
         "status": str,
         "registeredContainerInstancesCount": int,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "activeServicesCount": int,
-        "statistics": List[KeyValuePairOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "settings": List[ClusterSettingOutputTypeDef],
+        "statistics": List[KeyValuePairTypeDef],
+        "tags": List[TagTypeDef],
+        "settings": List[ClusterSettingTypeDef],
         "capacityProviders": List[str],
-        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "attachments": List[AttachmentTypeDef],
         "attachmentsStatus": str,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsTypeDef,
     },
     total=False,
 )
 
@@ -3764,29 +3281,29 @@
         "family": str,
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
         "revision": int,
         "volumes": List[VolumeOutputTypeDef],
         "status": TaskDefinitionStatusType,
-        "requiresAttributes": List[AttributeOutputTypeDef],
-        "placementConstraints": List[TaskDefinitionPlacementConstraintOutputTypeDef],
+        "requiresAttributes": List[AttributeTypeDef],
+        "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
         "compatibilities": List[CompatibilityType],
-        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
         "requiresCompatibilities": List[CompatibilityType],
         "cpu": str,
         "memory": str,
-        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
         "proxyConfiguration": ProxyConfigurationOutputTypeDef,
         "registeredAt": datetime,
         "deregisteredAt": datetime,
         "registeredBy": str,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
@@ -3832,15 +3349,15 @@
         "taskDefinition": str,
         "desiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "failedTasks": int,
         "createdAt": datetime,
         "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "launchType": LaunchTypeType,
         "platformVersion": str,
         "platformFamily": str,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "rolloutState": DeploymentRolloutStateType,
         "rolloutStateReason": str,
         "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
@@ -3929,191 +3446,191 @@
 
 
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RunTaskResponseTypeDef = TypedDict(
     "RunTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTaskResponseTypeDef = TypedDict(
     "StartTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopTaskResponseTypeDef = TypedDict(
     "StopTaskResponseTypeDef",
     {
         "task": TaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "clusters": List[ClusterTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutClusterCapacityProvidersResponseTypeDef = TypedDict(
     "PutClusterCapacityProvidersResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterSettingsResponseTypeDef = TypedDict(
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskDefinitionsResponseTypeDef = TypedDict(
     "DeleteTaskDefinitionsResponseTypeDef",
     {
         "taskDefinitions": List[TaskDefinitionTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
-        "loadBalancers": List[LoadBalancerOutputTypeDef],
-        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
         "status": str,
         "desiredCount": int,
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
         "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
-        "placementConstraints": List[PlacementConstraintOutputTypeDef],
-        "placementStrategy": List[PlacementStrategyOutputTypeDef],
+        "placementConstraints": List[PlacementConstraintTypeDef],
+        "placementStrategy": List[PlacementStrategyTypeDef],
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerOutputTypeDef,
-        "tags": List[TagOutputTypeDef],
+        "deploymentController": DeploymentControllerTypeDef,
+        "tags": List[TagTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
     },
     total=False,
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -69,63 +69,46 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentStateChangeTypeDef",
-    "KeyValuePairOutputTypeDef",
-    "AttributeOutputTypeDef",
+    "KeyValuePairTypeDef",
     "AttributeTypeDef",
-    "ManagedScalingOutputTypeDef",
     "ManagedScalingTypeDef",
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
-    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
-    "ClusterSettingOutputTypeDef",
     "ClusterSettingTypeDef",
-    "ContainerDependencyOutputTypeDef",
-    "EnvironmentFileOutputTypeDef",
-    "FirelensConfigurationOutputTypeDef",
-    "HealthCheckOutputTypeDef",
-    "HostEntryOutputTypeDef",
-    "MountPointOutputTypeDef",
-    "PortMappingOutputTypeDef",
-    "RepositoryCredentialsOutputTypeDef",
-    "ResourceRequirementOutputTypeDef",
-    "SecretOutputTypeDef",
-    "SystemControlOutputTypeDef",
-    "UlimitOutputTypeDef",
-    "VolumeFromOutputTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
-    "FirelensConfigurationTypeDef",
-    "HealthCheckTypeDef",
+    "FirelensConfigurationOutputTypeDef",
+    "HealthCheckOutputTypeDef",
     "HostEntryTypeDef",
-    "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
+    "FirelensConfigurationTypeDef",
+    "HealthCheckTypeDef",
     "InstanceHealthCheckResultTypeDef",
     "ResourceOutputTypeDef",
-    "VersionInfoOutputTypeDef",
+    "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
-    "NetworkBindingOutputTypeDef",
     "NetworkInterfaceTypeDef",
-    "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
@@ -134,172 +117,148 @@
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
     "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
-    "DeploymentCircuitBreakerOutputTypeDef",
     "DeploymentCircuitBreakerTypeDef",
-    "DeploymentControllerOutputTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
     "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
-    "DiscoverPollEndpointResponseTypeDef",
     "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
-    "EFSAuthorizationConfigOutputTypeDef",
     "EFSAuthorizationConfigTypeDef",
-    "EphemeralStorageOutputTypeDef",
     "EphemeralStorageTypeDef",
-    "ExecuteCommandLogConfigurationOutputTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
-    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
-    "HostVolumePropertiesOutputTypeDef",
     "HostVolumePropertiesTypeDef",
-    "InferenceAcceleratorOutputTypeDef",
-    "InferenceAcceleratorOverrideOutputTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
     "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
     "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
-    "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
-    "ListContainerInstancesResponseTypeDef",
-    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
-    "ListServicesByNamespaceResponseTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
-    "ListServicesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
-    "ListTaskDefinitionsResponseTypeDef",
-    "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseTypeDef",
-    "LoadBalancerOutputTypeDef",
     "ManagedAgentStateChangeTypeDef",
-    "PaginatorConfigTypeDef",
-    "PlacementConstraintOutputTypeDef",
-    "PlacementStrategyOutputTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "ResourceTypeDef",
-    "VersionInfoTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
-    "ResponseMetadataTypeDef",
-    "RuntimePlatformOutputTypeDef",
-    "ScaleOutputTypeDef",
-    "ServiceConnectClientAliasOutputTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
-    "ServiceRegistryOutputTypeDef",
     "StopTaskRequestRequestTypeDef",
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    "SubmitContainerStateChangeResponseTypeDef",
-    "SubmitTaskStateChangeResponseTypeDef",
-    "TaskDefinitionPlacementConstraintOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
     "ProxyConfigurationOutputTypeDef",
-    "DeleteAttributesResponseTypeDef",
-    "ListAttributesResponseTypeDef",
-    "PutAttributesResponseTypeDef",
+    "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
     "PutAttributesRequestRequestTypeDef",
-    "AutoScalingGroupProviderOutputTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
     "ContainerOverrideOutputTypeDef",
-    "LogConfigurationOutputTypeDef",
-    "ProxyConfigurationTypeDef",
     "ContainerOverrideTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "DeleteAttributesResponseTypeDef",
+    "DiscoverPollEndpointResponseTypeDef",
+    "ListAttributesResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
+    "ListServicesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    "ListTaskDefinitionsResponseTypeDef",
+    "ListTasksResponseTypeDef",
+    "PutAttributesResponseTypeDef",
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    "SubmitContainerStateChangeResponseTypeDef",
+    "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
     "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
-    "EFSVolumeConfigurationOutputTypeDef",
     "EFSVolumeConfigurationTypeDef",
-    "ExecuteCommandConfigurationOutputTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
-    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
     "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "ListAttributesRequestListAttributesPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    "ListTasksRequestListTasksPaginateTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "TaskSetTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
     "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
-    "ClusterConfigurationOutputTypeDef",
     "ClusterConfigurationTypeDef",
     "VolumeOutputTypeDef",
     "VolumeTypeDef",
     "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
     "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
@@ -353,42 +312,23 @@
     "AttachmentStateChangeTypeDef",
     {
         "attachmentArn": str,
         "status": str,
     },
 )
 
-KeyValuePairOutputTypeDef = TypedDict(
-    "KeyValuePairOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-    total=False,
-)
-
-_RequiredAttributeOutputTypeDef = TypedDict(
-    "_RequiredAttributeOutputTypeDef",
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAttributeOutputTypeDef = TypedDict(
-    "_OptionalAttributeOutputTypeDef",
-    {
         "value": str,
-        "targetType": Literal["container-instance"],
-        "targetId": str,
     },
     total=False,
 )
 
-class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
-    pass
-
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "name": str,
     },
 )
 _OptionalAttributeTypeDef = TypedDict(
@@ -400,26 +340,14 @@
     },
     total=False,
 )
 
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-ManagedScalingOutputTypeDef = TypedDict(
-    "ManagedScalingOutputTypeDef",
-    {
-        "status": ManagedScalingStatusType,
-        "targetCapacity": int,
-        "minimumScalingStepSize": int,
-        "maximumScalingStepSize": int,
-        "instanceWarmupPeriod": int,
-    },
-    total=False,
-)
-
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
@@ -464,35 +392,14 @@
 )
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
-_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "capacityProvider": str,
-    },
-)
-_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "weight": int,
-        "base": int,
-    },
-    total=False,
-)
-
-class CapacityProviderStrategyItemOutputTypeDef(
-    _RequiredCapacityProviderStrategyItemOutputTypeDef,
-    _OptionalCapacityProviderStrategyItemOutputTypeDef,
-):
-    pass
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -505,16 +412,16 @@
 )
 
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
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
 
@@ -529,42 +436,33 @@
     "ClusterServiceConnectDefaultsTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
-ClusterSettingOutputTypeDef = TypedDict(
-    "ClusterSettingOutputTypeDef",
-    {
-        "name": Literal["containerInsights"],
-        "value": str,
-    },
-    total=False,
-)
-
 ClusterSettingTypeDef = TypedDict(
     "ClusterSettingTypeDef",
     {
         "name": Literal["containerInsights"],
         "value": str,
     },
     total=False,
 )
 
-ContainerDependencyOutputTypeDef = TypedDict(
-    "ContainerDependencyOutputTypeDef",
+ContainerDependencyTypeDef = TypedDict(
+    "ContainerDependencyTypeDef",
     {
         "containerName": str,
         "condition": ContainerConditionType,
     },
 )
 
-EnvironmentFileOutputTypeDef = TypedDict(
-    "EnvironmentFileOutputTypeDef",
+EnvironmentFileTypeDef = TypedDict(
+    "EnvironmentFileTypeDef",
     {
         "value": str,
         "type": Literal["s3"],
     },
 )
 
 _RequiredFirelensConfigurationOutputTypeDef = TypedDict(
@@ -604,111 +502,95 @@
 )
 
 class HealthCheckOutputTypeDef(
     _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
 ):
     pass
 
-HostEntryOutputTypeDef = TypedDict(
-    "HostEntryOutputTypeDef",
+HostEntryTypeDef = TypedDict(
+    "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
 
-MountPointOutputTypeDef = TypedDict(
-    "MountPointOutputTypeDef",
+MountPointTypeDef = TypedDict(
+    "MountPointTypeDef",
     {
         "sourceVolume": str,
         "containerPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-PortMappingOutputTypeDef = TypedDict(
-    "PortMappingOutputTypeDef",
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
     {
         "containerPort": int,
         "hostPort": int,
         "protocol": TransportProtocolType,
         "name": str,
         "appProtocol": ApplicationProtocolType,
         "containerPortRange": str,
     },
     total=False,
 )
 
-RepositoryCredentialsOutputTypeDef = TypedDict(
-    "RepositoryCredentialsOutputTypeDef",
+RepositoryCredentialsTypeDef = TypedDict(
+    "RepositoryCredentialsTypeDef",
     {
         "credentialsParameter": str,
     },
 )
 
-ResourceRequirementOutputTypeDef = TypedDict(
-    "ResourceRequirementOutputTypeDef",
+ResourceRequirementTypeDef = TypedDict(
+    "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
-SecretOutputTypeDef = TypedDict(
-    "SecretOutputTypeDef",
+SecretTypeDef = TypedDict(
+    "SecretTypeDef",
     {
         "name": str,
         "valueFrom": str,
     },
 )
 
-SystemControlOutputTypeDef = TypedDict(
-    "SystemControlOutputTypeDef",
+SystemControlTypeDef = TypedDict(
+    "SystemControlTypeDef",
     {
         "namespace": str,
         "value": str,
     },
     total=False,
 )
 
-UlimitOutputTypeDef = TypedDict(
-    "UlimitOutputTypeDef",
+UlimitTypeDef = TypedDict(
+    "UlimitTypeDef",
     {
         "name": UlimitNameType,
         "softLimit": int,
         "hardLimit": int,
     },
 )
 
-VolumeFromOutputTypeDef = TypedDict(
-    "VolumeFromOutputTypeDef",
+VolumeFromTypeDef = TypedDict(
+    "VolumeFromTypeDef",
     {
         "sourceContainer": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-ContainerDependencyTypeDef = TypedDict(
-    "ContainerDependencyTypeDef",
-    {
-        "containerName": str,
-        "condition": ContainerConditionType,
-    },
-)
-
-EnvironmentFileTypeDef = TypedDict(
-    "EnvironmentFileTypeDef",
-    {
-        "value": str,
-        "type": Literal["s3"],
-    },
-)
-
 _RequiredFirelensConfigurationTypeDef = TypedDict(
     "_RequiredFirelensConfigurationTypeDef",
     {
         "type": FirelensConfigurationTypeType,
     },
 )
 _OptionalFirelensConfigurationTypeDef = TypedDict(
@@ -740,104 +622,14 @@
     },
     total=False,
 )
 
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
-HostEntryTypeDef = TypedDict(
-    "HostEntryTypeDef",
-    {
-        "hostname": str,
-        "ipAddress": str,
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
-MountPointTypeDef = TypedDict(
-    "MountPointTypeDef",
-    {
-        "sourceVolume": str,
-        "containerPath": str,
-        "readOnly": bool,
-    },
-    total=False,
-)
-
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "containerPort": int,
-        "hostPort": int,
-        "protocol": TransportProtocolType,
-        "name": str,
-        "appProtocol": ApplicationProtocolType,
-        "containerPortRange": str,
-    },
-    total=False,
-)
-
-RepositoryCredentialsTypeDef = TypedDict(
-    "RepositoryCredentialsTypeDef",
-    {
-        "credentialsParameter": str,
-    },
-)
-
-ResourceRequirementTypeDef = TypedDict(
-    "ResourceRequirementTypeDef",
-    {
-        "value": str,
-        "type": ResourceTypeType,
-    },
-)
-
-SecretTypeDef = TypedDict(
-    "SecretTypeDef",
-    {
-        "name": str,
-        "valueFrom": str,
-    },
-)
-
-SystemControlTypeDef = TypedDict(
-    "SystemControlTypeDef",
-    {
-        "namespace": str,
-        "value": str,
-    },
-    total=False,
-)
-
-UlimitTypeDef = TypedDict(
-    "UlimitTypeDef",
-    {
-        "name": UlimitNameType,
-        "softLimit": int,
-        "hardLimit": int,
-    },
-)
-
-VolumeFromTypeDef = TypedDict(
-    "VolumeFromTypeDef",
-    {
-        "sourceContainer": str,
-        "readOnly": bool,
-    },
-    total=False,
-)
-
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
@@ -854,16 +646,16 @@
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
     },
     total=False,
 )
 
-VersionInfoOutputTypeDef = TypedDict(
-    "VersionInfoOutputTypeDef",
+VersionInfoTypeDef = TypedDict(
+    "VersionInfoTypeDef",
     {
         "agentVersion": str,
         "agentHash": str,
         "dockerVersion": str,
     },
     total=False,
 )
@@ -888,44 +680,33 @@
         "name": Literal["ExecuteCommandAgent"],
         "reason": str,
         "lastStatus": str,
     },
     total=False,
 )
 
-NetworkBindingOutputTypeDef = TypedDict(
-    "NetworkBindingOutputTypeDef",
-    {
-        "bindIP": str,
-        "containerPort": int,
-        "hostPort": int,
-        "protocol": TransportProtocolType,
-        "containerPortRange": str,
-        "hostPortRange": str,
-    },
-    total=False,
-)
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "key": str,
-        "value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
@@ -1096,37 +877,22 @@
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
     },
 )
 
-DeploymentCircuitBreakerOutputTypeDef = TypedDict(
-    "DeploymentCircuitBreakerOutputTypeDef",
-    {
-        "enable": bool,
-        "rollback": bool,
-    },
-)
-
 DeploymentCircuitBreakerTypeDef = TypedDict(
     "DeploymentCircuitBreakerTypeDef",
     {
         "enable": bool,
         "rollback": bool,
     },
 )
 
-DeploymentControllerOutputTypeDef = TypedDict(
-    "DeploymentControllerOutputTypeDef",
-    {
-        "type": DeploymentControllerTypeType,
-    },
-)
-
 ServiceConnectServiceResourceTypeDef = TypedDict(
     "ServiceConnectServiceResourceTypeDef",
     {
         "discoveryName": str,
         "discoveryArn": str,
     },
     total=False,
@@ -1332,24 +1098,14 @@
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
-DiscoverPollEndpointResponseTypeDef = TypedDict(
-    "DiscoverPollEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "telemetryEndpoint": str,
-        "serviceConnectEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DockerVolumeConfigurationOutputTypeDef = TypedDict(
     "DockerVolumeConfigurationOutputTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
         "driverOpts": Dict[str, str],
@@ -1366,58 +1122,30 @@
         "driver": str,
         "driverOpts": Mapping[str, str],
         "labels": Mapping[str, str],
     },
     total=False,
 )
 
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
 )
 
-EphemeralStorageOutputTypeDef = TypedDict(
-    "EphemeralStorageOutputTypeDef",
-    {
-        "sizeInGiB": int,
-    },
-)
-
 EphemeralStorageTypeDef = TypedDict(
     "EphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
-ExecuteCommandLogConfigurationOutputTypeDef = TypedDict(
-    "ExecuteCommandLogConfigurationOutputTypeDef",
-    {
-        "cloudWatchLogGroupName": str,
-        "cloudWatchEncryptionEnabled": bool,
-        "s3BucketName": str,
-        "s3EncryptionEnabled": bool,
-        "s3KeyPrefix": str,
-    },
-    total=False,
-)
-
 ExecuteCommandLogConfigurationTypeDef = TypedDict(
     "ExecuteCommandLogConfigurationTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "cloudWatchEncryptionEnabled": bool,
         "s3BucketName": str,
         "s3EncryptionEnabled": bool,
@@ -1454,22 +1182,14 @@
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
     total=False,
 )
 
-FSxWindowsFileServerAuthorizationConfigOutputTypeDef = TypedDict(
-    "FSxWindowsFileServerAuthorizationConfigOutputTypeDef",
-    {
-        "credentialsParameter": str,
-        "domain": str,
-    },
-)
-
 FSxWindowsFileServerAuthorizationConfigTypeDef = TypedDict(
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     {
         "credentialsParameter": str,
         "domain": str,
     },
 )
@@ -1499,47 +1219,22 @@
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
     total=False,
 )
 
-HostVolumePropertiesOutputTypeDef = TypedDict(
-    "HostVolumePropertiesOutputTypeDef",
-    {
-        "sourcePath": str,
-    },
-    total=False,
-)
-
 HostVolumePropertiesTypeDef = TypedDict(
     "HostVolumePropertiesTypeDef",
     {
         "sourcePath": str,
     },
     total=False,
 )
 
-InferenceAcceleratorOutputTypeDef = TypedDict(
-    "InferenceAcceleratorOutputTypeDef",
-    {
-        "deviceName": str,
-        "deviceType": str,
-    },
-)
-
-InferenceAcceleratorOverrideOutputTypeDef = TypedDict(
-    "InferenceAcceleratorOverrideOutputTypeDef",
-    {
-        "deviceName": str,
-        "deviceType": str,
-    },
-    total=False,
-)
-
 InferenceAcceleratorOverrideTypeDef = TypedDict(
     "InferenceAcceleratorOverrideTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
     total=False,
@@ -1603,22 +1298,20 @@
     },
     total=False,
 )
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
-ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "name": SettingNameType,
-        "value": str,
-        "principalArn": str,
-        "effectiveSettings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountSettingsRequestRequestTypeDef = TypedDict(
     "ListAccountSettingsRequestRequestTypeDef",
     {
@@ -1628,37 +1321,14 @@
         "effectiveSettings": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "targetType": Literal["container-instance"],
-    },
-)
-_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "cluster": str,
-        "attributeName": str,
-        "attributeValue": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttributesRequestListAttributesPaginateTypeDef(
-    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
-    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributesRequestRequestTypeDef",
     {
         "targetType": Literal["container-instance"],
     },
 )
 _OptionalListAttributesRequestRequestTypeDef = TypedDict(
@@ -1674,92 +1344,35 @@
 )
 
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusterArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    {
-        "cluster": str,
-        "filter": str,
-        "status": ContainerInstanceStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContainerInstancesRequestRequestTypeDef = TypedDict(
     "ListContainerInstancesRequestRequestTypeDef",
     {
         "cluster": str,
         "filter": str,
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
-ListContainerInstancesResponseTypeDef = TypedDict(
-    "ListContainerInstancesResponseTypeDef",
-    {
-        "containerInstanceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "namespace": str,
-    },
-)
-_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
-    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-):
-    pass
-
 _RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesByNamespaceRequestRequestTypeDef",
     {
         "namespace": str,
     },
 )
 _OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
@@ -1773,139 +1386,56 @@
 
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
-ListServicesByNamespaceResponseTypeDef = TypedDict(
-    "ListServicesByNamespaceResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "cluster": str,
-        "launchType": LaunchTypeType,
-        "schedulingStrategy": SchedulingStrategyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
     },
     total=False,
 )
 
-ListServicesResponseTypeDef = TypedDict(
-    "ListServicesResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionFamilyStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionFamiliesRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionFamilyStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    {
-        "families": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionStatusType,
-        "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionsRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionStatusType,
         "sort": SortOrderType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListTaskDefinitionsResponseTypeDef",
-    {
-        "taskDefinitionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTasksRequestListTasksPaginateTypeDef = TypedDict(
-    "ListTasksRequestListTasksPaginateTypeDef",
-    {
-        "cluster": str,
-        "containerInstance": str,
-        "family": str,
-        "startedBy": str,
-        "serviceName": str,
-        "desiredStatus": DesiredStatusType,
-        "launchType": LaunchTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTasksRequestRequestTypeDef = TypedDict(
     "ListTasksRequestRequestTypeDef",
     {
         "cluster": str,
         "containerInstance": str,
         "family": str,
         "nextToken": str,
@@ -1914,34 +1444,14 @@
         "serviceName": str,
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
     },
     total=False,
 )
 
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
-    {
-        "taskArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LoadBalancerOutputTypeDef = TypedDict(
-    "LoadBalancerOutputTypeDef",
-    {
-        "targetGroupArn": str,
-        "loadBalancerName": str,
-        "containerName": str,
-        "containerPort": int,
-    },
-    total=False,
-)
-
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -1955,42 +1465,14 @@
 )
 
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
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
-PlacementConstraintOutputTypeDef = TypedDict(
-    "PlacementConstraintOutputTypeDef",
-    {
-        "type": PlacementConstraintTypeType,
-        "expression": str,
-    },
-    total=False,
-)
-
-PlacementStrategyOutputTypeDef = TypedDict(
-    "PlacementStrategyOutputTypeDef",
-    {
-        "type": PlacementStrategyTypeType,
-        "field": str,
-    },
-    total=False,
-)
-
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -2032,24 +1514,14 @@
         "longValue": int,
         "integerValue": int,
         "stringSetValue": Sequence[str],
     },
     total=False,
 )
 
-VersionInfoTypeDef = TypedDict(
-    "VersionInfoTypeDef",
-    {
-        "agentVersion": str,
-        "agentHash": str,
-        "dockerVersion": str,
-    },
-    total=False,
-)
-
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -2060,62 +1532,14 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
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
-RuntimePlatformOutputTypeDef = TypedDict(
-    "RuntimePlatformOutputTypeDef",
-    {
-        "cpuArchitecture": CPUArchitectureType,
-        "operatingSystemFamily": OSFamilyType,
-    },
-    total=False,
-)
-
-ScaleOutputTypeDef = TypedDict(
-    "ScaleOutputTypeDef",
-    {
-        "value": float,
-        "unit": Literal["PERCENT"],
-    },
-    total=False,
-)
-
-_RequiredServiceConnectClientAliasOutputTypeDef = TypedDict(
-    "_RequiredServiceConnectClientAliasOutputTypeDef",
-    {
-        "port": int,
-    },
-)
-_OptionalServiceConnectClientAliasOutputTypeDef = TypedDict(
-    "_OptionalServiceConnectClientAliasOutputTypeDef",
-    {
-        "dnsName": str,
-    },
-    total=False,
-)
-
-class ServiceConnectClientAliasOutputTypeDef(
-    _RequiredServiceConnectClientAliasOutputTypeDef, _OptionalServiceConnectClientAliasOutputTypeDef
-):
-    pass
-
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -2137,25 +1561,14 @@
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
     total=False,
 )
 
-ServiceRegistryOutputTypeDef = TypedDict(
-    "ServiceRegistryOutputTypeDef",
-    {
-        "registryArn": str,
-        "port": int,
-        "containerName": str,
-        "containerPort": int,
-    },
-    total=False,
-)
-
 _RequiredStopTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStopTaskRequestRequestTypeDef",
     {
         "task": str,
     },
 )
 _OptionalStopTaskRequestRequestTypeDef = TypedDict(
@@ -2168,47 +1581,14 @@
 )
 
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
-SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitContainerStateChangeResponseTypeDef = TypedDict(
-    "SubmitContainerStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitTaskStateChangeResponseTypeDef = TypedDict(
-    "SubmitTaskStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TaskDefinitionPlacementConstraintOutputTypeDef = TypedDict(
-    "TaskDefinitionPlacementConstraintOutputTypeDef",
-    {
-        "type": Literal["memberOf"],
-        "expression": str,
-    },
-    total=False,
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -2307,63 +1687,58 @@
 
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
-        "details": List[KeyValuePairOutputTypeDef],
+        "details": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
 _RequiredProxyConfigurationOutputTypeDef = TypedDict(
     "_RequiredProxyConfigurationOutputTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationOutputTypeDef = TypedDict(
     "_OptionalProxyConfigurationOutputTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairOutputTypeDef],
+        "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
 class ProxyConfigurationOutputTypeDef(
     _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
 ):
     pass
 
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
+_RequiredProxyConfigurationTypeDef = TypedDict(
+    "_RequiredProxyConfigurationTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "containerName": str,
     },
 )
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
+_OptionalProxyConfigurationTypeDef = TypedDict(
+    "_OptionalProxyConfigurationTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "type": Literal["APPMESH"],
+        "properties": Sequence[KeyValuePairTypeDef],
     },
+    total=False,
 )
 
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ProxyConfigurationTypeDef(
+    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
+):
+    pass
 
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
@@ -2395,34 +1770,14 @@
 )
 
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
-_RequiredAutoScalingGroupProviderOutputTypeDef = TypedDict(
-    "_RequiredAutoScalingGroupProviderOutputTypeDef",
-    {
-        "autoScalingGroupArn": str,
-    },
-)
-_OptionalAutoScalingGroupProviderOutputTypeDef = TypedDict(
-    "_OptionalAutoScalingGroupProviderOutputTypeDef",
-    {
-        "managedScaling": ManagedScalingOutputTypeDef,
-        "managedTerminationProtection": ManagedTerminationProtectionType,
-    },
-    total=False,
-)
-
-class AutoScalingGroupProviderOutputTypeDef(
-    _RequiredAutoScalingGroupProviderOutputTypeDef, _OptionalAutoScalingGroupProviderOutputTypeDef
-):
-    pass
-
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -2469,19 +1824,19 @@
     {
         "cluster": str,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 UpdateClusterSettingsRequestRequestTypeDef = TypedDict(
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
@@ -2490,79 +1845,59 @@
 )
 
 ContainerOverrideOutputTypeDef = TypedDict(
     "ContainerOverrideOutputTypeDef",
     {
         "name": str,
         "command": List[str],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "environmentFiles": List[EnvironmentFileOutputTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "environmentFiles": List[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
+    },
+    total=False,
+)
+
+ContainerOverrideTypeDef = TypedDict(
+    "ContainerOverrideTypeDef",
+    {
+        "name": str,
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
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
 
-_RequiredProxyConfigurationTypeDef = TypedDict(
-    "_RequiredProxyConfigurationTypeDef",
-    {
-        "containerName": str,
-    },
-)
-_OptionalProxyConfigurationTypeDef = TypedDict(
-    "_OptionalProxyConfigurationTypeDef",
-    {
-        "type": Literal["APPMESH"],
-        "properties": Sequence[KeyValuePairTypeDef],
-    },
-    total=False,
-)
-
-class ProxyConfigurationTypeDef(
-    _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
-):
-    pass
-
-ContainerOverrideTypeDef = TypedDict(
-    "ContainerOverrideTypeDef",
-    {
-        "name": str,
-        "command": Sequence[str],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "environmentFiles": Sequence[EnvironmentFileTypeDef],
-        "cpu": int,
-        "memory": int,
-        "memoryReservation": int,
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
@@ -2623,31 +1958,153 @@
         "name": str,
         "image": str,
         "imageDigest": str,
         "runtimeId": str,
         "lastStatus": str,
         "exitCode": int,
         "reason": str,
-        "networkBindings": List[NetworkBindingOutputTypeDef],
+        "networkBindings": List[NetworkBindingTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "healthStatus": HealthStatusType,
         "managedAgents": List[ManagedAgentTypeDef],
         "cpu": str,
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DiscoverPollEndpointResponseTypeDef = TypedDict(
+    "DiscoverPollEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusterArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainerInstancesResponseTypeDef = TypedDict(
+    "ListContainerInstancesResponseTypeDef",
+    {
+        "containerInstanceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesResponseTypeDef = TypedDict(
+    "ListServicesResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    {
+        "families": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
+    {
+        "taskArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitContainerStateChangeResponseTypeDef = TypedDict(
+    "SubmitContainerStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitTaskStateChangeResponseTypeDef = TypedDict(
+    "SubmitTaskStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
@@ -2657,47 +2114,47 @@
     },
 )
 
 DeleteAccountSettingResponseTypeDef = TypedDict(
     "DeleteAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountSettingsResponseTypeDef = TypedDict(
     "ListAccountSettingsResponseTypeDef",
     {
         "settings": List[SettingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingDefaultResponseTypeDef = TypedDict(
     "PutAccountSettingDefaultResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingResponseTypeDef = TypedDict(
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentConfigurationOutputTypeDef = TypedDict(
     "DeploymentConfigurationOutputTypeDef",
     {
-        "deploymentCircuitBreaker": DeploymentCircuitBreakerOutputTypeDef,
+        "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsOutputTypeDef,
     },
     total=False,
 )
 
@@ -2796,36 +2253,14 @@
 
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
-_RequiredEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEFSVolumeConfigurationOutputTypeDef",
-    {
-        "fileSystemId": str,
-    },
-)
-_OptionalEFSVolumeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEFSVolumeConfigurationOutputTypeDef",
-    {
-        "rootDirectory": str,
-        "transitEncryption": EFSTransitEncryptionType,
-        "transitEncryptionPort": int,
-        "authorizationConfig": EFSAuthorizationConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class EFSVolumeConfigurationOutputTypeDef(
-    _RequiredEFSVolumeConfigurationOutputTypeDef, _OptionalEFSVolumeConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -2840,24 +2275,14 @@
 )
 
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
-ExecuteCommandConfigurationOutputTypeDef = TypedDict(
-    "ExecuteCommandConfigurationOutputTypeDef",
-    {
-        "kmsKeyId": str,
-        "logging": ExecuteCommandLoggingType,
-        "logConfiguration": ExecuteCommandLogConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2869,24 +2294,15 @@
     {
         "clusterArn": str,
         "containerArn": str,
         "containerName": str,
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-FSxWindowsFileServerVolumeConfigurationOutputTypeDef = TypedDict(
-    "FSxWindowsFileServerVolumeConfigurationOutputTypeDef",
-    {
-        "fileSystemId": str,
-        "rootDirectory": str,
-        "authorizationConfig": FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
@@ -2896,24 +2312,24 @@
 )
 
 GetTaskProtectionResponseTypeDef = TypedDict(
     "GetTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskProtectionResponseTypeDef = TypedDict(
     "UpdateTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LinuxParametersOutputTypeDef = TypedDict(
     "LinuxParametersOutputTypeDef",
     {
         "capabilities": KernelCapabilitiesOutputTypeDef,
@@ -2937,14 +2353,135 @@
         "tmpfs": Sequence[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
+ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    {
+        "name": SettingNameType,
+        "value": str,
+        "principalArn": str,
+        "effectiveSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "targetType": Literal["container-instance"],
+    },
+)
+_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "cluster": str,
+        "attributeName": str,
+        "attributeValue": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttributesRequestListAttributesPaginateTypeDef(
+    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
+    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
+):
+    pass
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    {
+        "cluster": str,
+        "filter": str,
+        "status": ContainerInstanceStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "cluster": str,
+        "launchType": LaunchTypeType,
+        "schedulingStrategy": SchedulingStrategyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionFamilyStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionStatusType,
+        "sort": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTasksRequestListTasksPaginateTypeDef = TypedDict(
+    "ListTasksRequestListTasksPaginateTypeDef",
+    {
+        "cluster": str,
+        "containerInstance": str,
+        "family": str,
+        "startedBy": str,
+        "serviceName": str,
+        "desiredStatus": DesiredStatusType,
+        "launchType": LaunchTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "RegisterContainerInstanceRequestRequestTypeDef",
     {
         "cluster": str,
         "instanceIdentityDocument": str,
         "instanceIdentityDocumentSignature": str,
         "totalResources": Sequence[ResourceTypeDef],
@@ -2963,15 +2500,15 @@
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceOutputTypeDef = TypedDict(
     "_OptionalServiceConnectServiceOutputTypeDef",
     {
         "discoveryName": str,
-        "clientAliases": List[ServiceConnectClientAliasOutputTypeDef],
+        "clientAliases": List[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
 class ServiceConnectServiceOutputTypeDef(
     _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
@@ -3001,18 +2538,18 @@
 
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
-        "autoScalingGroupProvider": AutoScalingGroupProviderOutputTypeDef,
+        "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
         "updateStatus": CapacityProviderUpdateStatusType,
         "updateStatusReason": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateCapacityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCapacityProviderRequestRequestTypeDef",
     {
@@ -3055,24 +2592,24 @@
         "taskDefinition": str,
         "computedDesiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "createdAt": datetime,
         "updatedAt": datetime,
         "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "loadBalancers": List[LoadBalancerOutputTypeDef],
-        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
-        "scale": ScaleOutputTypeDef,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "scale": ScaleTypeDef,
         "stabilityStatus": StabilityStatusType,
         "stabilityStatusAt": datetime,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
@@ -3104,19 +2641,19 @@
     pass
 
 TaskOverrideOutputTypeDef = TypedDict(
     "TaskOverrideOutputTypeDef",
     {
         "containerOverrides": List[ContainerOverrideOutputTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideOutputTypeDef],
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
@@ -3134,27 +2671,27 @@
 ContainerInstanceTypeDef = TypedDict(
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
-        "versionInfo": VersionInfoOutputTypeDef,
+        "versionInfo": VersionInfoTypeDef,
         "remainingResources": List[ResourceOutputTypeDef],
         "registeredResources": List[ResourceOutputTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
         "registeredAt": datetime,
         "attachments": List[AttachmentTypeDef],
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "healthStatus": ContainerInstanceHealthStatusTypeDef,
     },
     total=False,
 )
 
 SubmitTaskStateChangeRequestRequestTypeDef = TypedDict(
     "SubmitTaskStateChangeRequestRequestTypeDef",
@@ -3169,40 +2706,30 @@
         "pullStartedAt": Union[datetime, str],
         "pullStoppedAt": Union[datetime, str],
         "executionStoppedAt": Union[datetime, str],
     },
     total=False,
 )
 
-ClusterConfigurationOutputTypeDef = TypedDict(
-    "ClusterConfigurationOutputTypeDef",
-    {
-        "executeCommandConfiguration": ExecuteCommandConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
 VolumeOutputTypeDef = TypedDict(
     "VolumeOutputTypeDef",
     {
         "name": str,
-        "host": HostVolumePropertiesOutputTypeDef,
+        "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
-        "efsVolumeConfiguration": EFSVolumeConfigurationOutputTypeDef,
-        "fsxWindowsFileServerVolumeConfiguration": (
-            FSxWindowsFileServerVolumeConfigurationOutputTypeDef
-        ),
+        "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
+        "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
@@ -3216,50 +2743,50 @@
 )
 
 ContainerDefinitionOutputTypeDef = TypedDict(
     "ContainerDefinitionOutputTypeDef",
     {
         "name": str,
         "image": str,
-        "repositoryCredentials": RepositoryCredentialsOutputTypeDef,
+        "repositoryCredentials": RepositoryCredentialsTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "links": List[str],
-        "portMappings": List[PortMappingOutputTypeDef],
+        "portMappings": List[PortMappingTypeDef],
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
-        "environment": List[KeyValuePairOutputTypeDef],
-        "environmentFiles": List[EnvironmentFileOutputTypeDef],
-        "mountPoints": List[MountPointOutputTypeDef],
-        "volumesFrom": List[VolumeFromOutputTypeDef],
+        "environment": List[KeyValuePairTypeDef],
+        "environmentFiles": List[EnvironmentFileTypeDef],
+        "mountPoints": List[MountPointTypeDef],
+        "volumesFrom": List[VolumeFromTypeDef],
         "linuxParameters": LinuxParametersOutputTypeDef,
-        "secrets": List[SecretOutputTypeDef],
-        "dependsOn": List[ContainerDependencyOutputTypeDef],
+        "secrets": List[SecretTypeDef],
+        "dependsOn": List[ContainerDependencyTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
         "disableNetworking": bool,
         "privileged": bool,
         "readonlyRootFilesystem": bool,
         "dnsServers": List[str],
         "dnsSearchDomains": List[str],
-        "extraHosts": List[HostEntryOutputTypeDef],
+        "extraHosts": List[HostEntryTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
-        "ulimits": List[UlimitOutputTypeDef],
+        "ulimits": List[UlimitTypeDef],
         "logConfiguration": LogConfigurationOutputTypeDef,
         "healthCheck": HealthCheckOutputTypeDef,
-        "systemControls": List[SystemControlOutputTypeDef],
-        "resourceRequirements": List[ResourceRequirementOutputTypeDef],
+        "systemControls": List[SystemControlTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationOutputTypeDef,
         "credentialSpecs": List[str],
     },
     total=False,
 )
 
 ContainerDefinitionTypeDef = TypedDict(
@@ -3352,124 +2879,124 @@
 ):
     pass
 
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCapacityProviderResponseTypeDef = TypedDict(
     "DeleteCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCapacityProvidersResponseTypeDef = TypedDict(
     "DescribeCapacityProvidersResponseTypeDef",
     {
         "capacityProviders": List[CapacityProviderTypeDef],
         "failures": List[FailureTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCapacityProviderResponseTypeDef = TypedDict(
     "UpdateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTaskSetResponseTypeDef = TypedDict(
     "CreateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskSetResponseTypeDef = TypedDict(
     "DeleteTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskSetsResponseTypeDef = TypedDict(
     "DescribeTaskSetsResponseTypeDef",
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskSetResponseTypeDef = TypedDict(
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaskTypeDef = TypedDict(
     "TaskTypeDef",
     {
         "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
         "availabilityZone": str,
         "capacityProviderName": str,
         "clusterArn": str,
         "connectivity": ConnectivityType,
         "connectivityAt": datetime,
         "containerInstanceArn": str,
         "containers": List[ContainerTypeDef],
         "cpu": str,
         "createdAt": datetime,
         "desiredStatus": str,
         "enableExecuteCommand": bool,
         "executionStoppedAt": datetime,
         "group": str,
         "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "lastStatus": str,
         "launchType": LaunchTypeType,
         "memory": str,
         "overrides": TaskOverrideOutputTypeDef,
         "platformVersion": str,
         "platformFamily": str,
         "pullStartedAt": datetime,
         "pullStoppedAt": datetime,
         "startedAt": datetime,
         "startedBy": str,
         "stopCode": TaskStopCodeType,
         "stoppedAt": datetime,
         "stoppedReason": str,
         "stoppingAt": datetime,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "taskArn": str,
         "taskDefinitionArn": str,
         "version": int,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
@@ -3533,68 +3060,68 @@
 ):
     pass
 
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContainerInstancesResponseTypeDef = TypedDict(
     "DescribeContainerInstancesResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterContainerInstanceResponseTypeDef = TypedDict(
     "RegisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerAgentResponseTypeDef = TypedDict(
     "UpdateContainerAgentResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerInstancesStateResponseTypeDef = TypedDict(
     "UpdateContainerInstancesStateResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
-        "configuration": ClusterConfigurationOutputTypeDef,
+        "configuration": ClusterConfigurationTypeDef,
         "status": str,
         "registeredContainerInstancesCount": int,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "activeServicesCount": int,
-        "statistics": List[KeyValuePairOutputTypeDef],
-        "tags": List[TagOutputTypeDef],
-        "settings": List[ClusterSettingOutputTypeDef],
+        "statistics": List[KeyValuePairTypeDef],
+        "tags": List[TagTypeDef],
+        "settings": List[ClusterSettingTypeDef],
         "capacityProviders": List[str],
-        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "attachments": List[AttachmentTypeDef],
         "attachmentsStatus": str,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsTypeDef,
     },
     total=False,
 )
 
@@ -3641,29 +3168,29 @@
         "family": str,
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
         "revision": int,
         "volumes": List[VolumeOutputTypeDef],
         "status": TaskDefinitionStatusType,
-        "requiresAttributes": List[AttributeOutputTypeDef],
-        "placementConstraints": List[TaskDefinitionPlacementConstraintOutputTypeDef],
+        "requiresAttributes": List[AttributeTypeDef],
+        "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
         "compatibilities": List[CompatibilityType],
-        "runtimePlatform": RuntimePlatformOutputTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
         "requiresCompatibilities": List[CompatibilityType],
         "cpu": str,
         "memory": str,
-        "inferenceAccelerators": List[InferenceAcceleratorOutputTypeDef],
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
         "proxyConfiguration": ProxyConfigurationOutputTypeDef,
         "registeredAt": datetime,
         "deregisteredAt": datetime,
         "registeredBy": str,
-        "ephemeralStorage": EphemeralStorageOutputTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
@@ -3707,15 +3234,15 @@
         "taskDefinition": str,
         "desiredCount": int,
         "pendingCount": int,
         "runningCount": int,
         "failedTasks": int,
         "createdAt": datetime,
         "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "launchType": LaunchTypeType,
         "platformVersion": str,
         "platformFamily": str,
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "rolloutState": DeploymentRolloutStateType,
         "rolloutStateReason": str,
         "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
@@ -3800,191 +3327,191 @@
     pass
 
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RunTaskResponseTypeDef = TypedDict(
     "RunTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTaskResponseTypeDef = TypedDict(
     "StartTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopTaskResponseTypeDef = TypedDict(
     "StopTaskResponseTypeDef",
     {
         "task": TaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "clusters": List[ClusterTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutClusterCapacityProvidersResponseTypeDef = TypedDict(
     "PutClusterCapacityProvidersResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterSettingsResponseTypeDef = TypedDict(
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskDefinitionsResponseTypeDef = TypedDict(
     "DeleteTaskDefinitionsResponseTypeDef",
     {
         "taskDefinitions": List[TaskDefinitionTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
-        "loadBalancers": List[LoadBalancerOutputTypeDef],
-        "serviceRegistries": List[ServiceRegistryOutputTypeDef],
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
         "status": str,
         "desiredCount": int,
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
         "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
-        "placementConstraints": List[PlacementConstraintOutputTypeDef],
-        "placementStrategy": List[PlacementStrategyOutputTypeDef],
+        "placementConstraints": List[PlacementConstraintTypeDef],
+        "placementStrategy": List[PlacementStrategyTypeDef],
         "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerOutputTypeDef,
-        "tags": List[TagOutputTypeDef],
+        "deploymentController": DeploymentControllerTypeDef,
+        "tags": List[TagTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
     },
     total=False,
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/PKG-INFO` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.12
-Summary: Type annotations for boto3.ECS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -445,63 +445,46 @@
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
-    KeyValuePairOutputTypeDef,
-    AttributeOutputTypeDef,
+    KeyValuePairTypeDef,
     AttributeTypeDef,
-    ManagedScalingOutputTypeDef,
     ManagedScalingTypeDef,
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
-    ClusterSettingOutputTypeDef,
     ClusterSettingTypeDef,
-    ContainerDependencyOutputTypeDef,
-    EnvironmentFileOutputTypeDef,
-    FirelensConfigurationOutputTypeDef,
-    HealthCheckOutputTypeDef,
-    HostEntryOutputTypeDef,
-    MountPointOutputTypeDef,
-    PortMappingOutputTypeDef,
-    RepositoryCredentialsOutputTypeDef,
-    ResourceRequirementOutputTypeDef,
-    SecretOutputTypeDef,
-    SystemControlOutputTypeDef,
-    UlimitOutputTypeDef,
-    VolumeFromOutputTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
-    FirelensConfigurationTypeDef,
-    HealthCheckTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
     HostEntryTypeDef,
-    KeyValuePairTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
+    FirelensConfigurationTypeDef,
+    HealthCheckTypeDef,
     InstanceHealthCheckResultTypeDef,
     ResourceOutputTypeDef,
-    VersionInfoOutputTypeDef,
+    VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
-    NetworkBindingOutputTypeDef,
     NetworkInterfaceTypeDef,
-    TagTypeDef,
+    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
@@ -510,172 +493,148 @@
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
     DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
-    DeploymentCircuitBreakerOutputTypeDef,
     DeploymentCircuitBreakerTypeDef,
-    DeploymentControllerOutputTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
     DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
     DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
-    EFSAuthorizationConfigOutputTypeDef,
     EFSAuthorizationConfigTypeDef,
-    EphemeralStorageOutputTypeDef,
     EphemeralStorageTypeDef,
-    ExecuteCommandLogConfigurationOutputTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
-    FSxWindowsFileServerAuthorizationConfigOutputTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
-    HostVolumePropertiesOutputTypeDef,
     HostVolumePropertiesTypeDef,
-    InferenceAcceleratorOutputTypeDef,
-    InferenceAcceleratorOverrideOutputTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
     KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
     TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
-    LoadBalancerOutputTypeDef,
     ManagedAgentStateChangeTypeDef,
-    PaginatorConfigTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     ResourceTypeDef,
-    VersionInfoTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    ResponseMetadataTypeDef,
-    RuntimePlatformOutputTypeDef,
-    ScaleOutputTypeDef,
-    ServiceConnectClientAliasOutputTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
-    ServiceRegistryOutputTypeDef,
     StopTaskRequestRequestTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
-    TaskDefinitionPlacementConstraintOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
     ProxyConfigurationOutputTypeDef,
-    DeleteAttributesResponseTypeDef,
-    ListAttributesResponseTypeDef,
-    PutAttributesResponseTypeDef,
+    ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
     PutAttributesRequestRequestTypeDef,
-    AutoScalingGroupProviderOutputTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
     ContainerOverrideOutputTypeDef,
-    LogConfigurationOutputTypeDef,
-    ProxyConfigurationTypeDef,
     ContainerOverrideTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DeleteAttributesResponseTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
+    ListAttributesResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksResponseTypeDef,
+    PutAttributesResponseTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
-    EFSVolumeConfigurationOutputTypeDef,
     EFSVolumeConfigurationTypeDef,
-    ExecuteCommandConfigurationOutputTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
-    FSxWindowsFileServerVolumeConfigurationOutputTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     TaskSetTypeDef,
     CreateTaskSetRequestRequestTypeDef,
     TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
-    ClusterConfigurationOutputTypeDef,
     ClusterConfigurationTypeDef,
     VolumeOutputTypeDef,
     VolumeTypeDef,
     ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
     ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
```

### Comparing `mypy-boto3-ecs-1.28.12/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.28.15/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.12/setup.py` & `mypy-boto3-ecs-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

