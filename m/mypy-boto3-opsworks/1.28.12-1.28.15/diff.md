# Comparing `tmp/mypy-boto3-opsworks-1.28.12.tar.gz` & `tmp/mypy-boto3-opsworks-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworks-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-opsworks-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
```

## Comparing `mypy-boto3-opsworks-1.28.12.tar` & `mypy-boto3-opsworks-1.28.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.829133 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51761 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51673 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19590 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    70410 2023-07-27 11:41:02.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70335 2023-07-27 11:41:01.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-27 11:41:00.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:21.000000 mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.833133 mypy-boto3-opsworks-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:40:59.000000 mypy-boto3-opsworks-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21429 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51761 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51673 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    65356 2023-07-28 20:32:59.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65287 2023-07-28 20:32:58.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-28 20:32:57.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:24.000000 mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.489600 mypy-boto3-opsworks-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:32:56.000000 mypy-boto3-opsworks-1.28.15/setup.py
```

### Comparing `mypy-boto3-opsworks-1.28.12/LICENSE` & `mypy-boto3-opsworks-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/PKG-INFO` & `mypy-boto3-opsworks-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.12
-Summary: Type annotations for boto3.OpsWorks 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,40 +438,31 @@
 ### Typed dictionaries
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
-    StackConfigurationManagerOutputTypeDef,
-    DataSourceOutputTypeDef,
-    EnvironmentVariableOutputTypeDef,
-    SourceOutputTypeDef,
-    SslConfigurationOutputTypeDef,
+    StackConfigurationManagerTypeDef,
+    DataSourceTypeDef,
+    EnvironmentVariableTypeDef,
+    SourceTypeDef,
+    SslConfigurationTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
     AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
-    EbsBlockDeviceOutputTypeDef,
     EbsBlockDeviceTypeDef,
-    ChefConfigurationOutputTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
-    SourceTypeDef,
-    StackConfigurationManagerTypeDef,
-    CloudWatchLogsLogStreamOutputTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
-    DataSourceTypeDef,
-    EnvironmentVariableTypeDef,
-    SslConfigurationTypeDef,
     DeploymentCommandTypeDef,
-    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -517,16 +508,14 @@
     GetHostnameSuggestionRequestRequestTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
     InstancesCountTypeDef,
     RecipesOutputTypeDef,
-    VolumeConfigurationOutputTypeDef,
-    ShutdownEventConfigurationOutputTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
@@ -545,51 +534,49 @@
     UpdateElasticIpRequestRequestTypeDef,
     UpdateInstanceRequestRequestTypeDef,
     UpdateMyUserProfileRequestRequestTypeDef,
     UpdateRdsDbInstanceRequestRequestTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
+    DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
-    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
-    StackTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationResponseTypeDef,
     CloneStackResultTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
-    InstancesCountResponseMetadataTypeDef,
+    InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
-    RecipesResponseMetadataTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
+    SourceResponseTypeDef,
+    StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
-    DescribeAgentVersionsRequestRequestTypeDef,
+    StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationOutputTypeDef,
-    CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
@@ -604,40 +591,39 @@
     DescribeRdsDbInstancesResultTypeDef,
     DescribeServiceErrorsResultTypeDef,
     DescribeUserProfilesResultTypeDef,
     DescribeVolumesResultTypeDef,
     GrantAccessResultTypeDef,
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
-    LifecycleEventConfigurationOutputTypeDef,
-    LifecycleEventConfigurationResponseMetadataTypeDef,
+    LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
-    InstanceTypeDef,
     CreateInstanceRequestRequestTypeDef,
+    InstanceTypeDef,
     DescribeStacksResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
-    LayerTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
+    LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerOutputTypeDef:
+def get_structure() -> StackConfigurationManagerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.12/README.md` & `mypy-boto3-opsworks-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,40 +406,31 @@
 ### Typed dictionaries
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
-    StackConfigurationManagerOutputTypeDef,
-    DataSourceOutputTypeDef,
-    EnvironmentVariableOutputTypeDef,
-    SourceOutputTypeDef,
-    SslConfigurationOutputTypeDef,
+    StackConfigurationManagerTypeDef,
+    DataSourceTypeDef,
+    EnvironmentVariableTypeDef,
+    SourceTypeDef,
+    SslConfigurationTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
     AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
-    EbsBlockDeviceOutputTypeDef,
     EbsBlockDeviceTypeDef,
-    ChefConfigurationOutputTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
-    SourceTypeDef,
-    StackConfigurationManagerTypeDef,
-    CloudWatchLogsLogStreamOutputTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
-    DataSourceTypeDef,
-    EnvironmentVariableTypeDef,
-    SslConfigurationTypeDef,
     DeploymentCommandTypeDef,
-    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -485,16 +476,14 @@
     GetHostnameSuggestionRequestRequestTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
     InstancesCountTypeDef,
     RecipesOutputTypeDef,
-    VolumeConfigurationOutputTypeDef,
-    ShutdownEventConfigurationOutputTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
@@ -513,51 +502,49 @@
     UpdateElasticIpRequestRequestTypeDef,
     UpdateInstanceRequestRequestTypeDef,
     UpdateMyUserProfileRequestRequestTypeDef,
     UpdateRdsDbInstanceRequestRequestTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
+    DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
-    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
-    StackTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationResponseTypeDef,
     CloneStackResultTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
-    InstancesCountResponseMetadataTypeDef,
+    InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
-    RecipesResponseMetadataTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
+    SourceResponseTypeDef,
+    StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
-    DescribeAgentVersionsRequestRequestTypeDef,
+    StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationOutputTypeDef,
-    CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
@@ -572,40 +559,39 @@
     DescribeRdsDbInstancesResultTypeDef,
     DescribeServiceErrorsResultTypeDef,
     DescribeUserProfilesResultTypeDef,
     DescribeVolumesResultTypeDef,
     GrantAccessResultTypeDef,
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
-    LifecycleEventConfigurationOutputTypeDef,
-    LifecycleEventConfigurationResponseMetadataTypeDef,
+    LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
-    InstanceTypeDef,
     CreateInstanceRequestRequestTypeDef,
+    InstanceTypeDef,
     DescribeStacksResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
-    LayerTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
+    LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerOutputTypeDef:
+def get_structure() -> StackConfigurationManagerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__init__.pyi` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/__main__.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorks 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.OpsWorks 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
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

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/client.pyi` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/literals.pyi` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/paginator.pyi` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,25 @@
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import OpsWorksClient
 from .literals import LayerAttributesKeysType, LayerTypeType, RootDeviceTypeType
 from .type_defs import (
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationResponseTypeDef,
     ChefConfigurationTypeDef,
-    CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
-    InstancesCountResponseMetadataTypeDef,
-    LifecycleEventConfigurationResponseMetadataTypeDef,
+    InstancesCountResponseTypeDef,
+    LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
-    RecipesResponseMetadataTypeDef,
     RecipesTypeDef,
-    SourceResponseMetadataTypeDef,
+    SourceResponseTypeDef,
     SourceTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
+    StackConfigurationManagerResponseTypeDef,
     StackConfigurationManagerTypeDef,
-    VolumeConfigurationOutputTypeDef,
     VolumeConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -161,30 +158,30 @@
     arn: str
     stack_id: str
     layer_id: str
     type: LayerTypeType
     name: str
     shortname: str
     attributes: Dict[LayerAttributesKeysType, str]
-    cloud_watch_logs_configuration: CloudWatchLogsConfigurationResponseMetadataTypeDef
+    cloud_watch_logs_configuration: CloudWatchLogsConfigurationTypeDef
     custom_instance_profile_arn: str
     custom_json: str
     custom_security_group_ids: List[str]
     default_security_group_names: List[str]
     packages: List[str]
-    volume_configurations: List[VolumeConfigurationOutputTypeDef]
+    volume_configurations: List[VolumeConfigurationTypeDef]
     enable_auto_healing: bool
     auto_assign_elastic_ips: bool
     auto_assign_public_ips: bool
-    default_recipes: RecipesResponseMetadataTypeDef
-    custom_recipes: RecipesResponseMetadataTypeDef
+    default_recipes: RecipesTypeDef
+    custom_recipes: RecipesTypeDef
     created_at: str
     install_updates_on_boot: bool
     use_ebs_optimized_instances: bool
-    lifecycle_event_configuration: LifecycleEventConfigurationResponseMetadataTypeDef
+    lifecycle_event_configuration: LifecycleEventConfigurationResponseTypeDef
     id: str
     stack: "Stack"
 
     def delete(self) -> None:
         """
         Deletes a specified layer.
 
@@ -228,15 +225,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stacksummary)
     """
 
     name: str
     arn: str
     layers_count: int
     apps_count: int
-    instances_count: InstancesCountResponseMetadataTypeDef
+    instances_count: InstancesCountResponseTypeDef
     stack_id: str
 
     def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.Stack)
@@ -288,19 +285,19 @@
     service_role_arn: str
     default_instance_profile_arn: str
     default_os: str
     hostname_theme: str
     default_availability_zone: str
     default_subnet_id: str
     custom_json: str
-    configuration_manager: StackConfigurationManagerResponseMetadataTypeDef
-    chef_configuration: ChefConfigurationResponseMetadataTypeDef
+    configuration_manager: StackConfigurationManagerResponseTypeDef
+    chef_configuration: ChefConfigurationResponseTypeDef
     use_custom_cookbooks: bool
     use_opsworks_security_groups: bool
-    custom_cookbooks_source: SourceResponseMetadataTypeDef
+    custom_cookbooks_source: SourceResponseTypeDef
     default_ssh_key_name: str
     created_at: str
     default_root_device_type: RootDeviceTypeType
     agent_version: str
     id: str
     layers: StackLayersCollection
```

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/service_resource.pyi` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/service_resource.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,25 @@
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import OpsWorksClient
 from .literals import LayerAttributesKeysType, LayerTypeType, RootDeviceTypeType
 from .type_defs import (
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationResponseTypeDef,
     ChefConfigurationTypeDef,
-    CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
-    InstancesCountResponseMetadataTypeDef,
-    LifecycleEventConfigurationResponseMetadataTypeDef,
+    InstancesCountResponseTypeDef,
+    LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
-    RecipesResponseMetadataTypeDef,
     RecipesTypeDef,
-    SourceResponseMetadataTypeDef,
+    SourceResponseTypeDef,
     SourceTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
+    StackConfigurationManagerResponseTypeDef,
     StackConfigurationManagerTypeDef,
-    VolumeConfigurationOutputTypeDef,
     VolumeConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -147,30 +144,30 @@
     arn: str
     stack_id: str
     layer_id: str
     type: LayerTypeType
     name: str
     shortname: str
     attributes: Dict[LayerAttributesKeysType, str]
-    cloud_watch_logs_configuration: CloudWatchLogsConfigurationResponseMetadataTypeDef
+    cloud_watch_logs_configuration: CloudWatchLogsConfigurationTypeDef
     custom_instance_profile_arn: str
     custom_json: str
     custom_security_group_ids: List[str]
     default_security_group_names: List[str]
     packages: List[str]
-    volume_configurations: List[VolumeConfigurationOutputTypeDef]
+    volume_configurations: List[VolumeConfigurationTypeDef]
     enable_auto_healing: bool
     auto_assign_elastic_ips: bool
     auto_assign_public_ips: bool
-    default_recipes: RecipesResponseMetadataTypeDef
-    custom_recipes: RecipesResponseMetadataTypeDef
+    default_recipes: RecipesTypeDef
+    custom_recipes: RecipesTypeDef
     created_at: str
     install_updates_on_boot: bool
     use_ebs_optimized_instances: bool
-    lifecycle_event_configuration: LifecycleEventConfigurationResponseMetadataTypeDef
+    lifecycle_event_configuration: LifecycleEventConfigurationResponseTypeDef
     id: str
     stack: "Stack"
 
     def delete(self) -> None:
         """
         Deletes a specified layer.
 
@@ -209,15 +206,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stacksummary)
     """
 
     name: str
     arn: str
     layers_count: int
     apps_count: int
-    instances_count: InstancesCountResponseMetadataTypeDef
+    instances_count: InstancesCountResponseTypeDef
     stack_id: str
 
     def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.Stack)
@@ -264,19 +261,19 @@
     service_role_arn: str
     default_instance_profile_arn: str
     default_os: str
     hostname_theme: str
     default_availability_zone: str
     default_subnet_id: str
     custom_json: str
-    configuration_manager: StackConfigurationManagerResponseMetadataTypeDef
-    chef_configuration: ChefConfigurationResponseMetadataTypeDef
+    configuration_manager: StackConfigurationManagerResponseTypeDef
+    chef_configuration: ChefConfigurationResponseTypeDef
     use_custom_cookbooks: bool
     use_opsworks_security_groups: bool
-    custom_cookbooks_source: SourceResponseMetadataTypeDef
+    custom_cookbooks_source: SourceResponseTypeDef
     default_ssh_key_name: str
     created_at: str
     default_root_device_type: RootDeviceTypeType
     agent_version: str
     id: str
     layers: StackLayersCollection
```

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opsworks service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerOutputTypeDef
+    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
 
-    data: StackConfigurationManagerOutputTypeDef = {...}
+    data: StackConfigurationManagerTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AppAttributesKeysType,
@@ -38,40 +38,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "StackConfigurationManagerOutputTypeDef",
-    "DataSourceOutputTypeDef",
-    "EnvironmentVariableOutputTypeDef",
-    "SourceOutputTypeDef",
-    "SslConfigurationOutputTypeDef",
+    "StackConfigurationManagerTypeDef",
+    "DataSourceTypeDef",
+    "EnvironmentVariableTypeDef",
+    "SourceTypeDef",
+    "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
-    "EbsBlockDeviceOutputTypeDef",
     "EbsBlockDeviceTypeDef",
-    "ChefConfigurationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
-    "SourceTypeDef",
-    "StackConfigurationManagerTypeDef",
-    "CloudWatchLogsLogStreamOutputTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
-    "DataSourceTypeDef",
-    "EnvironmentVariableTypeDef",
-    "SslConfigurationTypeDef",
     "DeploymentCommandTypeDef",
-    "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
@@ -117,16 +108,14 @@
     "GetHostnameSuggestionRequestRequestTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
     "InstancesCountTypeDef",
     "RecipesOutputTypeDef",
-    "VolumeConfigurationOutputTypeDef",
-    "ShutdownEventConfigurationOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
@@ -145,51 +134,49 @@
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
+    "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
-    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
-    "StackTypeDef",
-    "ChefConfigurationResponseMetadataTypeDef",
+    "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
     "CreateLayerResultTypeDef",
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
-    "InstancesCountResponseMetadataTypeDef",
+    "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
-    "RecipesResponseMetadataTypeDef",
+    "RecipesTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
-    "SourceResponseMetadataTypeDef",
-    "StackConfigurationManagerResponseMetadataTypeDef",
+    "SourceResponseTypeDef",
+    "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
-    "DescribeAgentVersionsRequestRequestTypeDef",
+    "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "CloudWatchLogsConfigurationOutputTypeDef",
-    "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
@@ -204,111 +191,108 @@
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
-    "LifecycleEventConfigurationOutputTypeDef",
-    "LifecycleEventConfigurationResponseMetadataTypeDef",
+    "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
-    "InstanceTypeDef",
     "CreateInstanceRequestRequestTypeDef",
+    "InstanceTypeDef",
     "DescribeStacksResultTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
-    "LayerTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
+    "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
     "DescribeTimeBasedAutoScalingResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "DescribeLayersResultTypeDef",
 )
 
-StackConfigurationManagerOutputTypeDef = TypedDict(
-    "StackConfigurationManagerOutputTypeDef",
+StackConfigurationManagerTypeDef = TypedDict(
+    "StackConfigurationManagerTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
     {
         "Type": str,
         "Arn": str,
         "DatabaseName": str,
     },
     total=False,
 )
 
-_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableOutputTypeDef",
+_RequiredEnvironmentVariableTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
-_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableOutputTypeDef",
+_OptionalEnvironmentVariableTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableTypeDef",
     {
         "Secure": bool,
     },
     total=False,
 )
 
 
-class EnvironmentVariableOutputTypeDef(
-    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
+class EnvironmentVariableTypeDef(
+    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
         "SshKey": str,
         "Revision": str,
     },
     total=False,
 )
 
-_RequiredSslConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSslConfigurationOutputTypeDef",
+_RequiredSslConfigurationTypeDef = TypedDict(
+    "_RequiredSslConfigurationTypeDef",
     {
         "Certificate": str,
         "PrivateKey": str,
     },
 )
-_OptionalSslConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSslConfigurationOutputTypeDef",
+_OptionalSslConfigurationTypeDef = TypedDict(
+    "_OptionalSslConfigurationTypeDef",
     {
         "Chain": str,
     },
     total=False,
 )
 
 
-class SslConfigurationOutputTypeDef(
-    _RequiredSslConfigurationOutputTypeDef, _OptionalSslConfigurationOutputTypeDef
-):
+class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
     pass
 
 
 AssignInstanceRequestRequestTypeDef = TypedDict(
     "AssignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
@@ -391,47 +375,26 @@
         "MemoryThreshold": float,
         "LoadThreshold": float,
         "Alarms": Sequence[str],
     },
     total=False,
 )
 
-EbsBlockDeviceOutputTypeDef = TypedDict(
-    "EbsBlockDeviceOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "Iops": int,
-        "VolumeSize": int,
-        "VolumeType": VolumeTypeType,
-        "DeleteOnTermination": bool,
-    },
-    total=False,
-)
-
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
         "SnapshotId": str,
         "Iops": int,
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "DeleteOnTermination": bool,
     },
     total=False,
 )
 
-ChefConfigurationOutputTypeDef = TypedDict(
-    "ChefConfigurationOutputTypeDef",
-    {
-        "ManageBerkshelf": bool,
-        "BerkshelfVersion": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -444,54 +407,14 @@
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
-    {
-        "Type": SourceTypeType,
-        "Url": str,
-        "Username": str,
-        "Password": str,
-        "SshKey": str,
-        "Revision": str,
-    },
-    total=False,
-)
-
-StackConfigurationManagerTypeDef = TypedDict(
-    "StackConfigurationManagerTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-CloudWatchLogsLogStreamOutputTypeDef = TypedDict(
-    "CloudWatchLogsLogStreamOutputTypeDef",
-    {
-        "LogGroupName": str,
-        "DatetimeFormat": str,
-        "TimeZone": CloudWatchLogsTimeZoneType,
-        "File": str,
-        "FileFingerprintLines": str,
-        "MultiLineStartPattern": str,
-        "InitialPosition": CloudWatchLogsInitialPositionType,
-        "Encoding": CloudWatchLogsEncodingType,
-        "BufferDuration": int,
-        "BatchCount": int,
-        "BatchSize": int,
-    },
-    total=False,
-)
-
 CloudWatchLogsLogStreamTypeDef = TypedDict(
     "CloudWatchLogsLogStreamTypeDef",
     {
         "LogGroupName": str,
         "DatetimeFormat": str,
         "TimeZone": CloudWatchLogsTimeZoneType,
         "File": str,
@@ -519,66 +442,14 @@
         "ExitCode": int,
         "LogUrl": str,
         "Type": str,
     },
     total=False,
 )
 
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "Type": str,
-        "Arn": str,
-        "DatabaseName": str,
-    },
-    total=False,
-)
-
-_RequiredEnvironmentVariableTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-_OptionalEnvironmentVariableTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableTypeDef",
-    {
-        "Secure": bool,
-    },
-    total=False,
-)
-
-
-class EnvironmentVariableTypeDef(
-    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
-):
-    pass
-
-
-_RequiredSslConfigurationTypeDef = TypedDict(
-    "_RequiredSslConfigurationTypeDef",
-    {
-        "Certificate": str,
-        "PrivateKey": str,
-    },
-)
-_OptionalSslConfigurationTypeDef = TypedDict(
-    "_OptionalSslConfigurationTypeDef",
-    {
-        "Chain": str,
-    },
-    total=False,
-)
-
-
-class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
-    pass
-
-
 _RequiredDeploymentCommandTypeDef = TypedDict(
     "_RequiredDeploymentCommandTypeDef",
     {
         "Name": DeploymentCommandNameType,
     },
 )
 _OptionalDeploymentCommandTypeDef = TypedDict(
@@ -592,26 +463,14 @@
 
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
 
-RecipesTypeDef = TypedDict(
-    "RecipesTypeDef",
-    {
-        "Setup": Sequence[str],
-        "Configure": Sequence[str],
-        "Deploy": Sequence[str],
-        "Undeploy": Sequence[str],
-        "Shutdown": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredVolumeConfigurationTypeDef = TypedDict(
     "_RequiredVolumeConfigurationTypeDef",
     {
         "MountPoint": str,
         "NumberOfDisks": int,
         "Size": int,
     },
@@ -1218,49 +1077,14 @@
         "Deploy": List[str],
         "Undeploy": List[str],
         "Shutdown": List[str],
     },
     total=False,
 )
 
-_RequiredVolumeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVolumeConfigurationOutputTypeDef",
-    {
-        "MountPoint": str,
-        "NumberOfDisks": int,
-        "Size": int,
-    },
-)
-_OptionalVolumeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVolumeConfigurationOutputTypeDef",
-    {
-        "RaidLevel": int,
-        "VolumeType": str,
-        "Iops": int,
-        "Encrypted": bool,
-    },
-    total=False,
-)
-
-
-class VolumeConfigurationOutputTypeDef(
-    _RequiredVolumeConfigurationOutputTypeDef, _OptionalVolumeConfigurationOutputTypeDef
-):
-    pass
-
-
-ShutdownEventConfigurationOutputTypeDef = TypedDict(
-    "ShutdownEventConfigurationOutputTypeDef",
-    {
-        "ExecutionTimeout": int,
-        "DelayUntilElbConnectionsDrained": bool,
-    },
-    total=False,
-)
-
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
         "ExecutionTimeout": int,
         "DelayUntilElbConnectionsDrained": bool,
     },
     total=False,
@@ -1603,40 +1427,110 @@
     pass
 
 
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "Version": str,
-        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
+        "ConfigurationManager": StackConfigurationManagerTypeDef,
+    },
+    total=False,
+)
+
+DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentVersionsRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "ConfigurationManager": StackConfigurationManagerTypeDef,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppId": str,
         "StackId": str,
         "Shortname": str,
         "Name": str,
         "Description": str,
-        "DataSources": List[DataSourceOutputTypeDef],
+        "DataSources": List[DataSourceTypeDef],
         "Type": AppTypeType,
-        "AppSource": SourceOutputTypeDef,
+        "AppSource": SourceTypeDef,
         "Domains": List[str],
         "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationOutputTypeDef,
+        "SslConfiguration": SslConfigurationTypeDef,
         "Attributes": Dict[AppAttributesKeysType, str],
         "CreatedAt": str,
-        "Environment": List[EnvironmentVariableOutputTypeDef],
+        "Environment": List[EnvironmentVariableTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "Name": str,
+        "Type": AppTypeType,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "Shortname": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "AppId": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "Type": AppTypeType,
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
+
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": str,
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsOutputTypeDef,
         "DownScaling": AutoScalingThresholdsOutputTypeDef,
@@ -1664,67 +1558,27 @@
 class SetLoadBasedAutoScalingRequestRequestTypeDef(
     _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef,
     _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
 
-BlockDeviceMappingOutputTypeDef = TypedDict(
-    "BlockDeviceMappingOutputTypeDef",
-    {
-        "DeviceName": str,
-        "NoDevice": str,
-        "VirtualName": str,
-        "Ebs": EbsBlockDeviceOutputTypeDef,
-    },
-    total=False,
-)
-
 BlockDeviceMappingTypeDef = TypedDict(
     "BlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "NoDevice": str,
         "VirtualName": str,
         "Ebs": EbsBlockDeviceTypeDef,
     },
     total=False,
 )
 
-StackTypeDef = TypedDict(
-    "StackTypeDef",
-    {
-        "StackId": str,
-        "Name": str,
-        "Arn": str,
-        "Region": str,
-        "VpcId": str,
-        "Attributes": Dict[Literal["Color"], str],
-        "ServiceRoleArn": str,
-        "DefaultInstanceProfileArn": str,
-        "DefaultOs": str,
-        "HostnameTheme": str,
-        "DefaultAvailabilityZone": str,
-        "DefaultSubnetId": str,
-        "CustomJson": str,
-        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
-        "ChefConfiguration": ChefConfigurationOutputTypeDef,
-        "UseCustomCookbooks": bool,
-        "UseOpsworksSecurityGroups": bool,
-        "CustomCookbooksSource": SourceOutputTypeDef,
-        "DefaultSshKeyName": str,
-        "CreatedAt": str,
-        "DefaultRootDeviceType": RootDeviceTypeType,
-        "AgentVersion": str,
-    },
-    total=False,
-)
-
-ChefConfigurationResponseMetadataTypeDef = TypedDict(
-    "ChefConfigurationResponseMetadataTypeDef",
+ChefConfigurationResponseTypeDef = TypedDict(
+    "ChefConfigurationResponseTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1805,16 +1659,16 @@
     {
         "LayerId": str,
         "Hostname": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstancesCountResponseMetadataTypeDef = TypedDict(
-    "InstancesCountResponseMetadataTypeDef",
+InstancesCountResponseTypeDef = TypedDict(
+    "InstancesCountResponseTypeDef",
     {
         "Assigning": int,
         "Booting": int,
         "ConnectionLost": int,
         "Deregistering": int,
         "Online": int,
         "Pending": int,
@@ -1841,16 +1695,16 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecipesResponseMetadataTypeDef = TypedDict(
-    "RecipesResponseMetadataTypeDef",
+RecipesTypeDef = TypedDict(
+    "RecipesTypeDef",
     {
         "Setup": List[str],
         "Configure": List[str],
         "Deploy": List[str],
         "Undeploy": List[str],
         "Shutdown": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1885,29 +1739,29 @@
     "RegisterVolumeResultTypeDef",
     {
         "VolumeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceResponseMetadataTypeDef = TypedDict(
-    "SourceResponseMetadataTypeDef",
+SourceResponseTypeDef = TypedDict(
+    "SourceResponseTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
         "SshKey": str,
         "Revision": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
-    "StackConfigurationManagerResponseMetadataTypeDef",
+StackConfigurationManagerResponseTypeDef = TypedDict(
+    "StackConfigurationManagerResponseTypeDef",
     {
         "Name": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2025,19 +1879,39 @@
 class CreateStackRequestServiceResourceCreateStackTypeDef(
     _RequiredCreateStackRequestServiceResourceCreateStackTypeDef,
     _OptionalCreateStackRequestServiceResourceCreateStackTypeDef,
 ):
     pass
 
 
-DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentVersionsRequestRequestTypeDef",
+StackTypeDef = TypedDict(
+    "StackTypeDef",
     {
         "StackId": str,
+        "Name": str,
+        "Arn": str,
+        "Region": str,
+        "VpcId": str,
+        "Attributes": Dict[Literal["Color"], str],
+        "ServiceRoleArn": str,
+        "DefaultInstanceProfileArn": str,
+        "DefaultOs": str,
+        "HostnameTheme": str,
+        "DefaultAvailabilityZone": str,
+        "DefaultSubnetId": str,
+        "CustomJson": str,
         "ConfigurationManager": StackConfigurationManagerTypeDef,
+        "ChefConfiguration": ChefConfigurationTypeDef,
+        "UseCustomCookbooks": bool,
+        "UseOpsworksSecurityGroups": bool,
+        "CustomCookbooksSource": SourceTypeDef,
+        "DefaultSshKeyName": str,
+        "CreatedAt": str,
+        "DefaultRootDeviceType": RootDeviceTypeType,
+        "AgentVersion": str,
     },
     total=False,
 )
 
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
@@ -2075,28 +1949,19 @@
     pass
 
 
 CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
     "CloudWatchLogsConfigurationOutputTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
+        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
     },
     total=False,
 )
 
-CloudWatchLogsConfigurationResponseMetadataTypeDef = TypedDict(
-    "CloudWatchLogsConfigurationResponseMetadataTypeDef",
-    {
-        "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
         "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
     },
     total=False,
@@ -2106,75 +1971,14 @@
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "Name": str,
-        "Type": AppTypeType,
-    },
-)
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
-    {
-        "Shortname": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "AppId": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "Type": AppTypeType,
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "StackId": str,
         "Command": DeploymentCommandTypeDef,
     },
 )
@@ -2415,26 +2219,18 @@
         "LayersCount": int,
         "AppsCount": int,
         "InstancesCount": InstancesCountTypeDef,
     },
     total=False,
 )
 
-LifecycleEventConfigurationOutputTypeDef = TypedDict(
-    "LifecycleEventConfigurationOutputTypeDef",
-    {
-        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-LifecycleEventConfigurationResponseMetadataTypeDef = TypedDict(
-    "LifecycleEventConfigurationResponseMetadataTypeDef",
+LifecycleEventConfigurationResponseTypeDef = TypedDict(
+    "LifecycleEventConfigurationResponseTypeDef",
     {
-        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
+        "Shutdown": ShutdownEventConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleEventConfigurationTypeDef = TypedDict(
     "LifecycleEventConfigurationTypeDef",
     {
@@ -2508,24 +2304,61 @@
     "DescribeLoadBasedAutoScalingResultTypeDef",
     {
         "LoadBasedAutoScalingConfigurations": List[LoadBasedAutoScalingConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "LayerIds": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceRequestRequestTypeDef",
+    {
+        "AutoScalingType": AutoScalingTypeType,
+        "Hostname": str,
+        "Os": str,
+        "AmiId": str,
+        "SshKeyName": str,
+        "AvailabilityZone": str,
+        "VirtualizationType": str,
+        "SubnetId": str,
+        "Architecture": ArchitectureType,
+        "RootDeviceType": RootDeviceTypeType,
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "InstallUpdatesOnBoot": bool,
+        "EbsOptimized": bool,
+        "AgentVersion": str,
+        "Tenancy": str,
+    },
+    total=False,
+)
+
+
+class CreateInstanceRequestRequestTypeDef(
+    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
+):
+    pass
+
+
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AgentVersion": str,
         "AmiId": str,
         "Architecture": ArchitectureType,
         "Arn": str,
         "AutoScalingType": AutoScalingTypeType,
         "AvailabilityZone": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
+        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "CreatedAt": str,
         "EbsOptimized": bool,
         "Ec2InstanceId": str,
         "EcsClusterArn": str,
         "EcsContainerInstanceArn": str,
         "ElasticIp": str,
         "Hostname": str,
@@ -2556,51 +2389,14 @@
         "SubnetId": str,
         "Tenancy": str,
         "VirtualizationType": VirtualizationTypeType,
     },
     total=False,
 )
 
-_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "LayerIds": Sequence[str],
-        "InstanceType": str,
-    },
-)
-_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceRequestRequestTypeDef",
-    {
-        "AutoScalingType": AutoScalingTypeType,
-        "Hostname": str,
-        "Os": str,
-        "AmiId": str,
-        "SshKeyName": str,
-        "AvailabilityZone": str,
-        "VirtualizationType": str,
-        "SubnetId": str,
-        "Architecture": ArchitectureType,
-        "RootDeviceType": RootDeviceTypeType,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "InstallUpdatesOnBoot": bool,
-        "EbsOptimized": bool,
-        "AgentVersion": str,
-        "Tenancy": str,
-    },
-    total=False,
-)
-
-
-class CreateInstanceRequestRequestTypeDef(
-    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
-):
-    pass
-
-
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2617,44 +2413,14 @@
     "DescribeStackSummaryResultTypeDef",
     {
         "StackSummary": StackSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LayerTypeDef = TypedDict(
-    "LayerTypeDef",
-    {
-        "Arn": str,
-        "StackId": str,
-        "LayerId": str,
-        "Type": LayerTypeType,
-        "Name": str,
-        "Shortname": str,
-        "Attributes": Dict[LayerAttributesKeysType, str],
-        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
-        "CustomInstanceProfileArn": str,
-        "CustomJson": str,
-        "CustomSecurityGroupIds": List[str],
-        "DefaultSecurityGroupNames": List[str],
-        "Packages": List[str],
-        "VolumeConfigurations": List[VolumeConfigurationOutputTypeDef],
-        "EnableAutoHealing": bool,
-        "AutoAssignElasticIps": bool,
-        "AutoAssignPublicIps": bool,
-        "DefaultRecipes": RecipesOutputTypeDef,
-        "CustomRecipes": RecipesOutputTypeDef,
-        "CreatedAt": str,
-        "InstallUpdatesOnBoot": bool,
-        "UseEbsOptimizedInstances": bool,
-        "LifecycleEventConfiguration": LifecycleEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLayerRequestRequestTypeDef",
     {
         "StackId": str,
         "Type": LayerTypeType,
         "Name": str,
         "Shortname": str,
@@ -2721,14 +2487,44 @@
 class CreateLayerRequestStackCreateLayerTypeDef(
     _RequiredCreateLayerRequestStackCreateLayerTypeDef,
     _OptionalCreateLayerRequestStackCreateLayerTypeDef,
 ):
     pass
 
 
+LayerTypeDef = TypedDict(
+    "LayerTypeDef",
+    {
+        "Arn": str,
+        "StackId": str,
+        "LayerId": str,
+        "Type": LayerTypeType,
+        "Name": str,
+        "Shortname": str,
+        "Attributes": Dict[LayerAttributesKeysType, str],
+        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
+        "CustomInstanceProfileArn": str,
+        "CustomJson": str,
+        "CustomSecurityGroupIds": List[str],
+        "DefaultSecurityGroupNames": List[str],
+        "Packages": List[str],
+        "VolumeConfigurations": List[VolumeConfigurationTypeDef],
+        "EnableAutoHealing": bool,
+        "AutoAssignElasticIps": bool,
+        "AutoAssignPublicIps": bool,
+        "DefaultRecipes": RecipesOutputTypeDef,
+        "CustomRecipes": RecipesOutputTypeDef,
+        "CreatedAt": str,
+        "InstallUpdatesOnBoot": bool,
+        "UseEbsOptimizedInstances": bool,
+        "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayerRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalUpdateLayerRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/type_defs.pyi` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opsworks service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerOutputTypeDef
+    from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
 
-    data: StackConfigurationManagerOutputTypeDef = {...}
+    data: StackConfigurationManagerTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AppAttributesKeysType,
@@ -37,40 +37,31 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "StackConfigurationManagerOutputTypeDef",
-    "DataSourceOutputTypeDef",
-    "EnvironmentVariableOutputTypeDef",
-    "SourceOutputTypeDef",
-    "SslConfigurationOutputTypeDef",
+    "StackConfigurationManagerTypeDef",
+    "DataSourceTypeDef",
+    "EnvironmentVariableTypeDef",
+    "SourceTypeDef",
+    "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
-    "EbsBlockDeviceOutputTypeDef",
     "EbsBlockDeviceTypeDef",
-    "ChefConfigurationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
-    "SourceTypeDef",
-    "StackConfigurationManagerTypeDef",
-    "CloudWatchLogsLogStreamOutputTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
-    "DataSourceTypeDef",
-    "EnvironmentVariableTypeDef",
-    "SslConfigurationTypeDef",
     "DeploymentCommandTypeDef",
-    "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
@@ -116,16 +107,14 @@
     "GetHostnameSuggestionRequestRequestTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
     "InstancesCountTypeDef",
     "RecipesOutputTypeDef",
-    "VolumeConfigurationOutputTypeDef",
-    "ShutdownEventConfigurationOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
@@ -144,51 +133,49 @@
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
+    "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
-    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
-    "StackTypeDef",
-    "ChefConfigurationResponseMetadataTypeDef",
+    "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
     "CreateLayerResultTypeDef",
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
-    "InstancesCountResponseMetadataTypeDef",
+    "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
-    "RecipesResponseMetadataTypeDef",
+    "RecipesTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
-    "SourceResponseMetadataTypeDef",
-    "StackConfigurationManagerResponseMetadataTypeDef",
+    "SourceResponseTypeDef",
+    "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
-    "DescribeAgentVersionsRequestRequestTypeDef",
+    "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "CloudWatchLogsConfigurationOutputTypeDef",
-    "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
@@ -203,108 +190,105 @@
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
-    "LifecycleEventConfigurationOutputTypeDef",
-    "LifecycleEventConfigurationResponseMetadataTypeDef",
+    "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
-    "InstanceTypeDef",
     "CreateInstanceRequestRequestTypeDef",
+    "InstanceTypeDef",
     "DescribeStacksResultTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
-    "LayerTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
+    "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
     "DescribeTimeBasedAutoScalingResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "DescribeLayersResultTypeDef",
 )
 
-StackConfigurationManagerOutputTypeDef = TypedDict(
-    "StackConfigurationManagerOutputTypeDef",
+StackConfigurationManagerTypeDef = TypedDict(
+    "StackConfigurationManagerTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
     {
         "Type": str,
         "Arn": str,
         "DatabaseName": str,
     },
     total=False,
 )
 
-_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableOutputTypeDef",
+_RequiredEnvironmentVariableTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
-_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableOutputTypeDef",
+_OptionalEnvironmentVariableTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableTypeDef",
     {
         "Secure": bool,
     },
     total=False,
 )
 
-class EnvironmentVariableOutputTypeDef(
-    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
+class EnvironmentVariableTypeDef(
+    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
         "SshKey": str,
         "Revision": str,
     },
     total=False,
 )
 
-_RequiredSslConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSslConfigurationOutputTypeDef",
+_RequiredSslConfigurationTypeDef = TypedDict(
+    "_RequiredSslConfigurationTypeDef",
     {
         "Certificate": str,
         "PrivateKey": str,
     },
 )
-_OptionalSslConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSslConfigurationOutputTypeDef",
+_OptionalSslConfigurationTypeDef = TypedDict(
+    "_OptionalSslConfigurationTypeDef",
     {
         "Chain": str,
     },
     total=False,
 )
 
-class SslConfigurationOutputTypeDef(
-    _RequiredSslConfigurationOutputTypeDef, _OptionalSslConfigurationOutputTypeDef
-):
+class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
     pass
 
 AssignInstanceRequestRequestTypeDef = TypedDict(
     "AssignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LayerIds": Sequence[str],
@@ -382,47 +366,26 @@
         "MemoryThreshold": float,
         "LoadThreshold": float,
         "Alarms": Sequence[str],
     },
     total=False,
 )
 
-EbsBlockDeviceOutputTypeDef = TypedDict(
-    "EbsBlockDeviceOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "Iops": int,
-        "VolumeSize": int,
-        "VolumeType": VolumeTypeType,
-        "DeleteOnTermination": bool,
-    },
-    total=False,
-)
-
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
         "SnapshotId": str,
         "Iops": int,
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "DeleteOnTermination": bool,
     },
     total=False,
 )
 
-ChefConfigurationOutputTypeDef = TypedDict(
-    "ChefConfigurationOutputTypeDef",
-    {
-        "ManageBerkshelf": bool,
-        "BerkshelfVersion": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -435,54 +398,14 @@
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
-    {
-        "Type": SourceTypeType,
-        "Url": str,
-        "Username": str,
-        "Password": str,
-        "SshKey": str,
-        "Revision": str,
-    },
-    total=False,
-)
-
-StackConfigurationManagerTypeDef = TypedDict(
-    "StackConfigurationManagerTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-CloudWatchLogsLogStreamOutputTypeDef = TypedDict(
-    "CloudWatchLogsLogStreamOutputTypeDef",
-    {
-        "LogGroupName": str,
-        "DatetimeFormat": str,
-        "TimeZone": CloudWatchLogsTimeZoneType,
-        "File": str,
-        "FileFingerprintLines": str,
-        "MultiLineStartPattern": str,
-        "InitialPosition": CloudWatchLogsInitialPositionType,
-        "Encoding": CloudWatchLogsEncodingType,
-        "BufferDuration": int,
-        "BatchCount": int,
-        "BatchSize": int,
-    },
-    total=False,
-)
-
 CloudWatchLogsLogStreamTypeDef = TypedDict(
     "CloudWatchLogsLogStreamTypeDef",
     {
         "LogGroupName": str,
         "DatetimeFormat": str,
         "TimeZone": CloudWatchLogsTimeZoneType,
         "File": str,
@@ -510,62 +433,14 @@
         "ExitCode": int,
         "LogUrl": str,
         "Type": str,
     },
     total=False,
 )
 
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "Type": str,
-        "Arn": str,
-        "DatabaseName": str,
-    },
-    total=False,
-)
-
-_RequiredEnvironmentVariableTypeDef = TypedDict(
-    "_RequiredEnvironmentVariableTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-_OptionalEnvironmentVariableTypeDef = TypedDict(
-    "_OptionalEnvironmentVariableTypeDef",
-    {
-        "Secure": bool,
-    },
-    total=False,
-)
-
-class EnvironmentVariableTypeDef(
-    _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
-):
-    pass
-
-_RequiredSslConfigurationTypeDef = TypedDict(
-    "_RequiredSslConfigurationTypeDef",
-    {
-        "Certificate": str,
-        "PrivateKey": str,
-    },
-)
-_OptionalSslConfigurationTypeDef = TypedDict(
-    "_OptionalSslConfigurationTypeDef",
-    {
-        "Chain": str,
-    },
-    total=False,
-)
-
-class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
-    pass
-
 _RequiredDeploymentCommandTypeDef = TypedDict(
     "_RequiredDeploymentCommandTypeDef",
     {
         "Name": DeploymentCommandNameType,
     },
 )
 _OptionalDeploymentCommandTypeDef = TypedDict(
@@ -577,26 +452,14 @@
 )
 
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
-RecipesTypeDef = TypedDict(
-    "RecipesTypeDef",
-    {
-        "Setup": Sequence[str],
-        "Configure": Sequence[str],
-        "Deploy": Sequence[str],
-        "Undeploy": Sequence[str],
-        "Shutdown": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredVolumeConfigurationTypeDef = TypedDict(
     "_RequiredVolumeConfigurationTypeDef",
     {
         "MountPoint": str,
         "NumberOfDisks": int,
         "Size": int,
     },
@@ -1191,47 +1054,14 @@
         "Deploy": List[str],
         "Undeploy": List[str],
         "Shutdown": List[str],
     },
     total=False,
 )
 
-_RequiredVolumeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVolumeConfigurationOutputTypeDef",
-    {
-        "MountPoint": str,
-        "NumberOfDisks": int,
-        "Size": int,
-    },
-)
-_OptionalVolumeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVolumeConfigurationOutputTypeDef",
-    {
-        "RaidLevel": int,
-        "VolumeType": str,
-        "Iops": int,
-        "Encrypted": bool,
-    },
-    total=False,
-)
-
-class VolumeConfigurationOutputTypeDef(
-    _RequiredVolumeConfigurationOutputTypeDef, _OptionalVolumeConfigurationOutputTypeDef
-):
-    pass
-
-ShutdownEventConfigurationOutputTypeDef = TypedDict(
-    "ShutdownEventConfigurationOutputTypeDef",
-    {
-        "ExecutionTimeout": int,
-        "DelayUntilElbConnectionsDrained": bool,
-    },
-    total=False,
-)
-
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
         "ExecutionTimeout": int,
         "DelayUntilElbConnectionsDrained": bool,
     },
     total=False,
@@ -1556,40 +1386,106 @@
 ):
     pass
 
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "Version": str,
-        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
+        "ConfigurationManager": StackConfigurationManagerTypeDef,
+    },
+    total=False,
+)
+
+DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentVersionsRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "ConfigurationManager": StackConfigurationManagerTypeDef,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppId": str,
         "StackId": str,
         "Shortname": str,
         "Name": str,
         "Description": str,
-        "DataSources": List[DataSourceOutputTypeDef],
+        "DataSources": List[DataSourceTypeDef],
         "Type": AppTypeType,
-        "AppSource": SourceOutputTypeDef,
+        "AppSource": SourceTypeDef,
         "Domains": List[str],
         "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationOutputTypeDef,
+        "SslConfiguration": SslConfigurationTypeDef,
         "Attributes": Dict[AppAttributesKeysType, str],
         "CreatedAt": str,
-        "Environment": List[EnvironmentVariableOutputTypeDef],
+        "Environment": List[EnvironmentVariableTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "Name": str,
+        "Type": AppTypeType,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "Shortname": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "AppId": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "DataSources": Sequence[DataSourceTypeDef],
+        "Type": AppTypeType,
+        "AppSource": SourceTypeDef,
+        "Domains": Sequence[str],
+        "EnableSsl": bool,
+        "SslConfiguration": SslConfigurationTypeDef,
+        "Attributes": Mapping[AppAttributesKeysType, str],
+        "Environment": Sequence[EnvironmentVariableTypeDef],
+    },
+    total=False,
+)
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": str,
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsOutputTypeDef,
         "DownScaling": AutoScalingThresholdsOutputTypeDef,
@@ -1615,67 +1511,27 @@
 
 class SetLoadBasedAutoScalingRequestRequestTypeDef(
     _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef,
     _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
-BlockDeviceMappingOutputTypeDef = TypedDict(
-    "BlockDeviceMappingOutputTypeDef",
-    {
-        "DeviceName": str,
-        "NoDevice": str,
-        "VirtualName": str,
-        "Ebs": EbsBlockDeviceOutputTypeDef,
-    },
-    total=False,
-)
-
 BlockDeviceMappingTypeDef = TypedDict(
     "BlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "NoDevice": str,
         "VirtualName": str,
         "Ebs": EbsBlockDeviceTypeDef,
     },
     total=False,
 )
 
-StackTypeDef = TypedDict(
-    "StackTypeDef",
-    {
-        "StackId": str,
-        "Name": str,
-        "Arn": str,
-        "Region": str,
-        "VpcId": str,
-        "Attributes": Dict[Literal["Color"], str],
-        "ServiceRoleArn": str,
-        "DefaultInstanceProfileArn": str,
-        "DefaultOs": str,
-        "HostnameTheme": str,
-        "DefaultAvailabilityZone": str,
-        "DefaultSubnetId": str,
-        "CustomJson": str,
-        "ConfigurationManager": StackConfigurationManagerOutputTypeDef,
-        "ChefConfiguration": ChefConfigurationOutputTypeDef,
-        "UseCustomCookbooks": bool,
-        "UseOpsworksSecurityGroups": bool,
-        "CustomCookbooksSource": SourceOutputTypeDef,
-        "DefaultSshKeyName": str,
-        "CreatedAt": str,
-        "DefaultRootDeviceType": RootDeviceTypeType,
-        "AgentVersion": str,
-    },
-    total=False,
-)
-
-ChefConfigurationResponseMetadataTypeDef = TypedDict(
-    "ChefConfigurationResponseMetadataTypeDef",
+ChefConfigurationResponseTypeDef = TypedDict(
+    "ChefConfigurationResponseTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1756,16 +1612,16 @@
     {
         "LayerId": str,
         "Hostname": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstancesCountResponseMetadataTypeDef = TypedDict(
-    "InstancesCountResponseMetadataTypeDef",
+InstancesCountResponseTypeDef = TypedDict(
+    "InstancesCountResponseTypeDef",
     {
         "Assigning": int,
         "Booting": int,
         "ConnectionLost": int,
         "Deregistering": int,
         "Online": int,
         "Pending": int,
@@ -1792,16 +1648,16 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecipesResponseMetadataTypeDef = TypedDict(
-    "RecipesResponseMetadataTypeDef",
+RecipesTypeDef = TypedDict(
+    "RecipesTypeDef",
     {
         "Setup": List[str],
         "Configure": List[str],
         "Deploy": List[str],
         "Undeploy": List[str],
         "Shutdown": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1836,29 +1692,29 @@
     "RegisterVolumeResultTypeDef",
     {
         "VolumeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceResponseMetadataTypeDef = TypedDict(
-    "SourceResponseMetadataTypeDef",
+SourceResponseTypeDef = TypedDict(
+    "SourceResponseTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
         "SshKey": str,
         "Revision": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
-    "StackConfigurationManagerResponseMetadataTypeDef",
+StackConfigurationManagerResponseTypeDef = TypedDict(
+    "StackConfigurationManagerResponseTypeDef",
     {
         "Name": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1970,19 +1826,39 @@
 
 class CreateStackRequestServiceResourceCreateStackTypeDef(
     _RequiredCreateStackRequestServiceResourceCreateStackTypeDef,
     _OptionalCreateStackRequestServiceResourceCreateStackTypeDef,
 ):
     pass
 
-DescribeAgentVersionsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentVersionsRequestRequestTypeDef",
+StackTypeDef = TypedDict(
+    "StackTypeDef",
     {
         "StackId": str,
+        "Name": str,
+        "Arn": str,
+        "Region": str,
+        "VpcId": str,
+        "Attributes": Dict[Literal["Color"], str],
+        "ServiceRoleArn": str,
+        "DefaultInstanceProfileArn": str,
+        "DefaultOs": str,
+        "HostnameTheme": str,
+        "DefaultAvailabilityZone": str,
+        "DefaultSubnetId": str,
+        "CustomJson": str,
         "ConfigurationManager": StackConfigurationManagerTypeDef,
+        "ChefConfiguration": ChefConfigurationTypeDef,
+        "UseCustomCookbooks": bool,
+        "UseOpsworksSecurityGroups": bool,
+        "CustomCookbooksSource": SourceTypeDef,
+        "DefaultSshKeyName": str,
+        "CreatedAt": str,
+        "DefaultRootDeviceType": RootDeviceTypeType,
+        "AgentVersion": str,
     },
     total=False,
 )
 
 _RequiredUpdateStackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStackRequestRequestTypeDef",
     {
@@ -2018,28 +1894,19 @@
 ):
     pass
 
 CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
     "CloudWatchLogsConfigurationOutputTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
+        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
     },
     total=False,
 )
 
-CloudWatchLogsConfigurationResponseMetadataTypeDef = TypedDict(
-    "CloudWatchLogsConfigurationResponseMetadataTypeDef",
-    {
-        "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
         "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
     },
     total=False,
@@ -2049,71 +1916,14 @@
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "Name": str,
-        "Type": AppTypeType,
-    },
-)
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
-    {
-        "Shortname": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
-    },
-    total=False,
-)
-
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "AppId": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "DataSources": Sequence[DataSourceTypeDef],
-        "Type": AppTypeType,
-        "AppSource": SourceTypeDef,
-        "Domains": Sequence[str],
-        "EnableSsl": bool,
-        "SslConfiguration": SslConfigurationTypeDef,
-        "Attributes": Mapping[AppAttributesKeysType, str],
-        "Environment": Sequence[EnvironmentVariableTypeDef],
-    },
-    total=False,
-)
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "StackId": str,
         "Command": DeploymentCommandTypeDef,
     },
 )
@@ -2350,26 +2160,18 @@
         "LayersCount": int,
         "AppsCount": int,
         "InstancesCount": InstancesCountTypeDef,
     },
     total=False,
 )
 
-LifecycleEventConfigurationOutputTypeDef = TypedDict(
-    "LifecycleEventConfigurationOutputTypeDef",
+LifecycleEventConfigurationResponseTypeDef = TypedDict(
+    "LifecycleEventConfigurationResponseTypeDef",
     {
-        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-LifecycleEventConfigurationResponseMetadataTypeDef = TypedDict(
-    "LifecycleEventConfigurationResponseMetadataTypeDef",
-    {
-        "Shutdown": ShutdownEventConfigurationOutputTypeDef,
+        "Shutdown": ShutdownEventConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleEventConfigurationTypeDef = TypedDict(
     "LifecycleEventConfigurationTypeDef",
     {
@@ -2441,24 +2243,59 @@
     "DescribeLoadBasedAutoScalingResultTypeDef",
     {
         "LoadBasedAutoScalingConfigurations": List[LoadBasedAutoScalingConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceRequestRequestTypeDef",
+    {
+        "StackId": str,
+        "LayerIds": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceRequestRequestTypeDef",
+    {
+        "AutoScalingType": AutoScalingTypeType,
+        "Hostname": str,
+        "Os": str,
+        "AmiId": str,
+        "SshKeyName": str,
+        "AvailabilityZone": str,
+        "VirtualizationType": str,
+        "SubnetId": str,
+        "Architecture": ArchitectureType,
+        "RootDeviceType": RootDeviceTypeType,
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "InstallUpdatesOnBoot": bool,
+        "EbsOptimized": bool,
+        "AgentVersion": str,
+        "Tenancy": str,
+    },
+    total=False,
+)
+
+class CreateInstanceRequestRequestTypeDef(
+    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
+):
+    pass
+
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AgentVersion": str,
         "AmiId": str,
         "Architecture": ArchitectureType,
         "Arn": str,
         "AutoScalingType": AutoScalingTypeType,
         "AvailabilityZone": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
+        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "CreatedAt": str,
         "EbsOptimized": bool,
         "Ec2InstanceId": str,
         "EcsClusterArn": str,
         "EcsContainerInstanceArn": str,
         "ElasticIp": str,
         "Hostname": str,
@@ -2489,49 +2326,14 @@
         "SubnetId": str,
         "Tenancy": str,
         "VirtualizationType": VirtualizationTypeType,
     },
     total=False,
 )
 
-_RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceRequestRequestTypeDef",
-    {
-        "StackId": str,
-        "LayerIds": Sequence[str],
-        "InstanceType": str,
-    },
-)
-_OptionalCreateInstanceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceRequestRequestTypeDef",
-    {
-        "AutoScalingType": AutoScalingTypeType,
-        "Hostname": str,
-        "Os": str,
-        "AmiId": str,
-        "SshKeyName": str,
-        "AvailabilityZone": str,
-        "VirtualizationType": str,
-        "SubnetId": str,
-        "Architecture": ArchitectureType,
-        "RootDeviceType": RootDeviceTypeType,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "InstallUpdatesOnBoot": bool,
-        "EbsOptimized": bool,
-        "AgentVersion": str,
-        "Tenancy": str,
-    },
-    total=False,
-)
-
-class CreateInstanceRequestRequestTypeDef(
-    _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
-):
-    pass
-
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2548,44 +2350,14 @@
     "DescribeStackSummaryResultTypeDef",
     {
         "StackSummary": StackSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LayerTypeDef = TypedDict(
-    "LayerTypeDef",
-    {
-        "Arn": str,
-        "StackId": str,
-        "LayerId": str,
-        "Type": LayerTypeType,
-        "Name": str,
-        "Shortname": str,
-        "Attributes": Dict[LayerAttributesKeysType, str],
-        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
-        "CustomInstanceProfileArn": str,
-        "CustomJson": str,
-        "CustomSecurityGroupIds": List[str],
-        "DefaultSecurityGroupNames": List[str],
-        "Packages": List[str],
-        "VolumeConfigurations": List[VolumeConfigurationOutputTypeDef],
-        "EnableAutoHealing": bool,
-        "AutoAssignElasticIps": bool,
-        "AutoAssignPublicIps": bool,
-        "DefaultRecipes": RecipesOutputTypeDef,
-        "CustomRecipes": RecipesOutputTypeDef,
-        "CreatedAt": str,
-        "InstallUpdatesOnBoot": bool,
-        "UseEbsOptimizedInstances": bool,
-        "LifecycleEventConfiguration": LifecycleEventConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLayerRequestRequestTypeDef",
     {
         "StackId": str,
         "Type": LayerTypeType,
         "Name": str,
         "Shortname": str,
@@ -2648,14 +2420,44 @@
 
 class CreateLayerRequestStackCreateLayerTypeDef(
     _RequiredCreateLayerRequestStackCreateLayerTypeDef,
     _OptionalCreateLayerRequestStackCreateLayerTypeDef,
 ):
     pass
 
+LayerTypeDef = TypedDict(
+    "LayerTypeDef",
+    {
+        "Arn": str,
+        "StackId": str,
+        "LayerId": str,
+        "Type": LayerTypeType,
+        "Name": str,
+        "Shortname": str,
+        "Attributes": Dict[LayerAttributesKeysType, str],
+        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
+        "CustomInstanceProfileArn": str,
+        "CustomJson": str,
+        "CustomSecurityGroupIds": List[str],
+        "DefaultSecurityGroupNames": List[str],
+        "Packages": List[str],
+        "VolumeConfigurations": List[VolumeConfigurationTypeDef],
+        "EnableAutoHealing": bool,
+        "AutoAssignElasticIps": bool,
+        "AutoAssignPublicIps": bool,
+        "DefaultRecipes": RecipesOutputTypeDef,
+        "CustomRecipes": RecipesOutputTypeDef,
+        "CreatedAt": str,
+        "InstallUpdatesOnBoot": bool,
+        "UseEbsOptimizedInstances": bool,
+        "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayerRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalUpdateLayerRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.py` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks/waiter.pyi` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/PKG-INFO` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.12
-Summary: Type annotations for boto3.OpsWorks 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,40 +438,31 @@
 ### Typed dictionaries
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
-    StackConfigurationManagerOutputTypeDef,
-    DataSourceOutputTypeDef,
-    EnvironmentVariableOutputTypeDef,
-    SourceOutputTypeDef,
-    SslConfigurationOutputTypeDef,
+    StackConfigurationManagerTypeDef,
+    DataSourceTypeDef,
+    EnvironmentVariableTypeDef,
+    SourceTypeDef,
+    SslConfigurationTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
     AutoScalingThresholdsOutputTypeDef,
     AutoScalingThresholdsTypeDef,
-    EbsBlockDeviceOutputTypeDef,
     EbsBlockDeviceTypeDef,
-    ChefConfigurationOutputTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
-    SourceTypeDef,
-    StackConfigurationManagerTypeDef,
-    CloudWatchLogsLogStreamOutputTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
-    DataSourceTypeDef,
-    EnvironmentVariableTypeDef,
-    SslConfigurationTypeDef,
     DeploymentCommandTypeDef,
-    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -517,16 +508,14 @@
     GetHostnameSuggestionRequestRequestTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
     InstancesCountTypeDef,
     RecipesOutputTypeDef,
-    VolumeConfigurationOutputTypeDef,
-    ShutdownEventConfigurationOutputTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
@@ -545,51 +534,49 @@
     UpdateElasticIpRequestRequestTypeDef,
     UpdateInstanceRequestRequestTypeDef,
     UpdateMyUserProfileRequestRequestTypeDef,
     UpdateRdsDbInstanceRequestRequestTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
+    DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
-    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
-    StackTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
+    ChefConfigurationResponseTypeDef,
     CloneStackResultTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
-    InstancesCountResponseMetadataTypeDef,
+    InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
-    RecipesResponseMetadataTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
+    SourceResponseTypeDef,
+    StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
-    DescribeAgentVersionsRequestRequestTypeDef,
+    StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationOutputTypeDef,
-    CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
@@ -604,40 +591,39 @@
     DescribeRdsDbInstancesResultTypeDef,
     DescribeServiceErrorsResultTypeDef,
     DescribeUserProfilesResultTypeDef,
     DescribeVolumesResultTypeDef,
     GrantAccessResultTypeDef,
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
-    LifecycleEventConfigurationOutputTypeDef,
-    LifecycleEventConfigurationResponseMetadataTypeDef,
+    LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
-    InstanceTypeDef,
     CreateInstanceRequestRequestTypeDef,
+    InstanceTypeDef,
     DescribeStacksResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
-    LayerTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
+    LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerOutputTypeDef:
+def get_structure() -> StackConfigurationManagerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.12/mypy_boto3_opsworks.egg-info/SOURCES.txt` & `mypy-boto3-opsworks-1.28.15/mypy_boto3_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.12/setup.py` & `mypy-boto3-opsworks-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworks",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorks 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

