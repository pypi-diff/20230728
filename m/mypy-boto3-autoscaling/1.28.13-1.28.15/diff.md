# Comparing `tmp/mypy-boto3-autoscaling-1.28.13.tar.gz` & `tmp/mypy-boto3-autoscaling-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.28.13.tar", last modified: Thu Jul 27 19:34:20 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.28.13.tar` & `mypy-boto3-autoscaling-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.119558 mypy-boto3-autoscaling-1.28.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-27 19:34:20.115558 mypy-boto3-autoscaling-1.28.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.111558 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52899 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-27 19:32:15.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-27 19:32:13.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    95018 2023-07-27 19:32:17.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94863 2023-07-27 19:32:16.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.115558 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 19:34:19.000000 mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:34:20.119558 mypy-boto3-autoscaling-1.28.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 19:32:12.000000 mypy-boto3-autoscaling-1.28.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.288696 mypy-boto3-autoscaling-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-07-28 20:42:19.276696 mypy-boto3-autoscaling-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22206 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.272696 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52899 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-28 20:19:56.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-07-28 20:19:59.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86078 2023-07-28 20:19:58.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.276696 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.288696 mypy-boto3-autoscaling-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:19:55.000000 mypy-boto3-autoscaling-1.28.15/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.28.13/LICENSE` & `mypy-boto3-autoscaling-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/PKG-INFO` & `mypy-boto3-autoscaling-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.13
-Summary: Type annotations for boto3.AutoScaling 1.28.13 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,49 +392,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
-    AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
-    AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
-    LaunchTemplateSpecificationOutputTypeDef,
+    LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
-    TrafficSourceIdentifierOutputTypeDef,
-    BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
-    EbsOutputTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
-    LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
@@ -461,54 +454,39 @@
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
-    InstanceMetadataOptionsOutputTypeDef,
-    InstanceMonitoringOutputTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
     RefreshPreferencesOutputTypeDef,
-    MemoryGiBPerVCpuRequestOutputTypeDef,
-    MemoryMiBRequestOutputTypeDef,
-    NetworkBandwidthGbpsRequestOutputTypeDef,
-    NetworkInterfaceCountRequestOutputTypeDef,
-    TotalLocalStorageGBRequestOutputTypeDef,
-    VCpuCountRequestOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
-    InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
-    InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
-    PredictiveScalingPredefinedLoadMetricOutputTypeDef,
-    PredictiveScalingPredefinedMetricPairOutputTypeDef,
-    PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
-    StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
@@ -543,36 +521,35 @@
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
-    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
-    WarmPoolConfigurationTypeDef,
     PutWarmPoolTypeRequestTypeDef,
+    WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
-    LaunchConfigurationTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
+    LaunchConfigurationTypeDef,
     MetricStatOutputTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
     RollbackDetailsTypeDef,
     LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
@@ -613,15 +590,15 @@
     ScalingPolicyTypeDef,
     PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestOutputTypeDef:
+def get_structure() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.13/README.md` & `mypy-boto3-autoscaling-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,49 +360,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
-    AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
-    AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
-    LaunchTemplateSpecificationOutputTypeDef,
+    LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
-    TrafficSourceIdentifierOutputTypeDef,
-    BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
-    EbsOutputTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
-    LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
@@ -429,54 +422,39 @@
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
-    InstanceMetadataOptionsOutputTypeDef,
-    InstanceMonitoringOutputTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
     RefreshPreferencesOutputTypeDef,
-    MemoryGiBPerVCpuRequestOutputTypeDef,
-    MemoryMiBRequestOutputTypeDef,
-    NetworkBandwidthGbpsRequestOutputTypeDef,
-    NetworkInterfaceCountRequestOutputTypeDef,
-    TotalLocalStorageGBRequestOutputTypeDef,
-    VCpuCountRequestOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
-    InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
-    InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
-    PredictiveScalingPredefinedLoadMetricOutputTypeDef,
-    PredictiveScalingPredefinedMetricPairOutputTypeDef,
-    PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
-    StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
@@ -511,36 +489,35 @@
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
-    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
-    WarmPoolConfigurationTypeDef,
     PutWarmPoolTypeRequestTypeDef,
+    WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
-    LaunchConfigurationTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
+    LaunchConfigurationTypeDef,
     MetricStatOutputTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
     RollbackDetailsTypeDef,
     LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
@@ -581,15 +558,15 @@
     ScalingPolicyTypeDef,
     PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestOutputTypeDef:
+def get_structure() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.28.13\nVersion:         1.28.13\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.AutoScaling 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.13")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestOutputTypeDef
+    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestTypeDef
 
-    data: AcceleratorCountRequestOutputTypeDef = {...}
+    data: AcceleratorCountRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -49,49 +49,42 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AcceleratorCountRequestOutputTypeDef",
     "AcceleratorCountRequestTypeDef",
-    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
-    "LaunchTemplateSpecificationOutputTypeDef",
+    "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
-    "TrafficSourceIdentifierOutputTypeDef",
-    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
-    "EbsOutputTypeDef",
     "EbsTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
-    "LaunchTemplateSpecificationTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
@@ -118,54 +111,39 @@
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
-    "InstanceMetadataOptionsOutputTypeDef",
-    "InstanceMonitoringOutputTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
     "RefreshPreferencesOutputTypeDef",
-    "MemoryGiBPerVCpuRequestOutputTypeDef",
-    "MemoryMiBRequestOutputTypeDef",
-    "NetworkBandwidthGbpsRequestOutputTypeDef",
-    "NetworkInterfaceCountRequestOutputTypeDef",
-    "TotalLocalStorageGBRequestOutputTypeDef",
-    "VCpuCountRequestOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
-    "InstanceReusePolicyOutputTypeDef",
     "InstanceReusePolicyTypeDef",
-    "InstancesDistributionOutputTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
-    "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
-    "PredictiveScalingPredefinedLoadMetricOutputTypeDef",
-    "PredictiveScalingPredefinedMetricPairOutputTypeDef",
-    "PredictiveScalingPredefinedScalingMetricOutputTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
     "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
-    "StepAdjustmentOutputTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
@@ -200,36 +178,35 @@
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
     "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
-    "WarmPoolConfigurationTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
+    "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
-    "LaunchConfigurationTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
+    "LaunchConfigurationTypeDef",
     "MetricStatOutputTypeDef",
     "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "RollbackDetailsTypeDef",
     "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
@@ -269,41 +246,23 @@
     "GetPredictiveScalingForecastAnswerTypeDef",
     "ScalingPolicyTypeDef",
     "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
-AcceleratorCountRequestOutputTypeDef = TypedDict(
-    "AcceleratorCountRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
-AcceleratorTotalMemoryMiBRequestOutputTypeDef = TypedDict(
-    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
 AcceleratorTotalMemoryMiBRequestTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -448,16 +407,16 @@
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
 )
 
-LaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "LaunchTemplateSpecificationOutputTypeDef",
+LaunchTemplateSpecificationTypeDef = TypedDict(
+    "LaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
     total=False,
 )
@@ -479,44 +438,14 @@
         "Key": str,
         "Value": str,
         "PropagateAtLaunch": bool,
     },
     total=False,
 )
 
-_RequiredTrafficSourceIdentifierOutputTypeDef = TypedDict(
-    "_RequiredTrafficSourceIdentifierOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-_OptionalTrafficSourceIdentifierOutputTypeDef = TypedDict(
-    "_OptionalTrafficSourceIdentifierOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-
-class TrafficSourceIdentifierOutputTypeDef(
-    _RequiredTrafficSourceIdentifierOutputTypeDef, _OptionalTrafficSourceIdentifierOutputTypeDef
-):
-    pass
-
-
-BaselineEbsBandwidthMbpsRequestOutputTypeDef = TypedDict(
-    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
 BaselineEbsBandwidthMbpsRequestTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -577,28 +506,14 @@
 class ScheduledUpdateGroupActionRequestTypeDef(
     _RequiredScheduledUpdateGroupActionRequestTypeDef,
     _OptionalScheduledUpdateGroupActionRequestTypeDef,
 ):
     pass
 
 
-EbsOutputTypeDef = TypedDict(
-    "EbsOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeSize": int,
-        "VolumeType": str,
-        "DeleteOnTermination": bool,
-        "Iops": int,
-        "Encrypted": bool,
-        "Throughput": int,
-    },
-    total=False,
-)
-
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
@@ -645,24 +560,14 @@
 class CompleteLifecycleActionTypeRequestTypeDef(
     _RequiredCompleteLifecycleActionTypeRequestTypeDef,
     _OptionalCompleteLifecycleActionTypeRequestTypeDef,
 ):
     pass
 
 
-LaunchTemplateSpecificationTypeDef = TypedDict(
-    "LaunchTemplateSpecificationTypeDef",
-    {
-        "LaunchTemplateId": str,
-        "LaunchTemplateName": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 _RequiredLifecycleHookSpecificationTypeDef = TypedDict(
     "_RequiredLifecycleHookSpecificationTypeDef",
     {
         "LifecycleHookName": str,
         "LifecycleTransition": str,
     },
 )
@@ -721,22 +626,14 @@
     "InstanceMonitoringTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1251,32 +1148,14 @@
         "AutoScalingGroupName": str,
         "PolicyName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-InstanceMetadataOptionsOutputTypeDef = TypedDict(
-    "InstanceMetadataOptionsOutputTypeDef",
-    {
-        "HttpTokens": InstanceMetadataHttpTokensStateType,
-        "HttpPutResponseHopLimit": int,
-        "HttpEndpoint": InstanceMetadataEndpointStateType,
-    },
-    total=False,
-)
-
-InstanceMonitoringOutputTypeDef = TypedDict(
-    "InstanceMonitoringOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
@@ -1302,92 +1181,14 @@
         "AutoRollback": bool,
         "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
         "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
-MemoryGiBPerVCpuRequestOutputTypeDef = TypedDict(
-    "MemoryGiBPerVCpuRequestOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
-_RequiredMemoryMiBRequestOutputTypeDef = TypedDict(
-    "_RequiredMemoryMiBRequestOutputTypeDef",
-    {
-        "Min": int,
-    },
-)
-_OptionalMemoryMiBRequestOutputTypeDef = TypedDict(
-    "_OptionalMemoryMiBRequestOutputTypeDef",
-    {
-        "Max": int,
-    },
-    total=False,
-)
-
-
-class MemoryMiBRequestOutputTypeDef(
-    _RequiredMemoryMiBRequestOutputTypeDef, _OptionalMemoryMiBRequestOutputTypeDef
-):
-    pass
-
-
-NetworkBandwidthGbpsRequestOutputTypeDef = TypedDict(
-    "NetworkBandwidthGbpsRequestOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
-NetworkInterfaceCountRequestOutputTypeDef = TypedDict(
-    "NetworkInterfaceCountRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
-TotalLocalStorageGBRequestOutputTypeDef = TypedDict(
-    "TotalLocalStorageGBRequestOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
-_RequiredVCpuCountRequestOutputTypeDef = TypedDict(
-    "_RequiredVCpuCountRequestOutputTypeDef",
-    {
-        "Min": int,
-    },
-)
-_OptionalVCpuCountRequestOutputTypeDef = TypedDict(
-    "_OptionalVCpuCountRequestOutputTypeDef",
-    {
-        "Max": int,
-    },
-    total=False,
-)
-
-
-class VCpuCountRequestOutputTypeDef(
-    _RequiredVCpuCountRequestOutputTypeDef, _OptionalVCpuCountRequestOutputTypeDef
-):
-    pass
-
-
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1454,43 +1255,22 @@
 )
 
 
 class VCpuCountRequestTypeDef(_RequiredVCpuCountRequestTypeDef, _OptionalVCpuCountRequestTypeDef):
     pass
 
 
-InstanceReusePolicyOutputTypeDef = TypedDict(
-    "InstanceReusePolicyOutputTypeDef",
-    {
-        "ReuseOnScaleIn": bool,
-    },
-    total=False,
-)
-
 InstanceReusePolicyTypeDef = TypedDict(
     "InstanceReusePolicyTypeDef",
     {
         "ReuseOnScaleIn": bool,
     },
     total=False,
 )
 
-InstancesDistributionOutputTypeDef = TypedDict(
-    "InstancesDistributionOutputTypeDef",
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
 InstancesDistributionTypeDef = TypedDict(
     "InstancesDistributionTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
@@ -1513,36 +1293,14 @@
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-_RequiredPredefinedMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredefinedMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedMetricType": MetricTypeType,
-    },
-)
-_OptionalPredefinedMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredefinedMetricSpecificationOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-
-class PredefinedMetricSpecificationOutputTypeDef(
-    _RequiredPredefinedMetricSpecificationOutputTypeDef,
-    _OptionalPredefinedMetricSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1556,80 +1314,14 @@
 
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
 
-_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef",
-    {
-        "PredefinedMetricType": PredefinedLoadMetricTypeType,
-    },
-)
-_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-
-class PredictiveScalingPredefinedLoadMetricOutputTypeDef(
-    _RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef,
-    _OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef,
-):
-    pass
-
-
-_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef",
-    {
-        "PredefinedMetricType": PredefinedMetricPairTypeType,
-    },
-)
-_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-
-class PredictiveScalingPredefinedMetricPairOutputTypeDef(
-    _RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef,
-    _OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef,
-):
-    pass
-
-
-_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef",
-    {
-        "PredefinedMetricType": PredefinedScalingMetricTypeType,
-    },
-)
-_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-
-class PredictiveScalingPredefinedScalingMetricOutputTypeDef(
-    _RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef,
-    _OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef,
-):
-    pass
-
-
 _RequiredPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedLoadMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
@@ -1827,36 +1519,14 @@
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
-_RequiredStepAdjustmentOutputTypeDef = TypedDict(
-    "_RequiredStepAdjustmentOutputTypeDef",
-    {
-        "ScalingAdjustment": int,
-    },
-)
-_OptionalStepAdjustmentOutputTypeDef = TypedDict(
-    "_OptionalStepAdjustmentOutputTypeDef",
-    {
-        "MetricIntervalLowerBound": float,
-        "MetricIntervalUpperBound": float,
-    },
-    total=False,
-)
-
-
-class StepAdjustmentOutputTypeDef(
-    _RequiredStepAdjustmentOutputTypeDef, _OptionalStepAdjustmentOutputTypeDef
-):
-    pass
-
-
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalScalingProcessQueryRequestTypeDef = TypedDict(
@@ -2272,15 +1942,15 @@
     },
 )
 _OptionalAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_OptionalAutoScalingInstanceDetailsTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 
 class AutoScalingInstanceDetailsTypeDef(
@@ -2300,15 +1970,15 @@
     },
 )
 _OptionalInstanceTypeDef = TypedDict(
     "_OptionalInstanceTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
@@ -2344,37 +2014,14 @@
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
     },
 )
 
-_RequiredBlockDeviceMappingOutputTypeDef = TypedDict(
-    "_RequiredBlockDeviceMappingOutputTypeDef",
-    {
-        "DeviceName": str,
-    },
-)
-_OptionalBlockDeviceMappingOutputTypeDef = TypedDict(
-    "_OptionalBlockDeviceMappingOutputTypeDef",
-    {
-        "VirtualName": str,
-        "Ebs": EbsOutputTypeDef,
-        "NoDevice": bool,
-    },
-    total=False,
-)
-
-
-class BlockDeviceMappingOutputTypeDef(
-    _RequiredBlockDeviceMappingOutputTypeDef, _OptionalBlockDeviceMappingOutputTypeDef
-):
-    pass
-
-
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
     },
 )
 _OptionalBlockDeviceMappingTypeDef = TypedDict(
@@ -2414,15 +2061,15 @@
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricOutputTypeDef = TypedDict(
     "_OptionalMetricOutputTypeDef",
     {
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 
 class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
     pass
@@ -2509,41 +2156,41 @@
     },
     total=False,
 )
 
 _RequiredInstanceRequirementsOutputTypeDef = TypedDict(
     "_RequiredInstanceRequirementsOutputTypeDef",
     {
-        "VCpuCount": VCpuCountRequestOutputTypeDef,
-        "MemoryMiB": MemoryMiBRequestOutputTypeDef,
+        "VCpuCount": VCpuCountRequestTypeDef,
+        "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
 _OptionalInstanceRequirementsOutputTypeDef = TypedDict(
     "_OptionalInstanceRequirementsOutputTypeDef",
     {
         "CpuManufacturers": List[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestOutputTypeDef,
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestTypeDef,
         "ExcludedInstanceTypes": List[str],
         "InstanceGenerations": List[InstanceGenerationType],
         "SpotMaxPricePercentageOverLowestPrice": int,
         "OnDemandMaxPricePercentageOverLowestPrice": int,
         "BareMetal": BareMetalType,
         "BurstablePerformance": BurstablePerformanceType,
         "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountRequestOutputTypeDef,
+        "NetworkInterfaceCount": NetworkInterfaceCountRequestTypeDef,
         "LocalStorage": LocalStorageType,
         "LocalStorageTypes": List[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBRequestOutputTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestOutputTypeDef,
+        "TotalLocalStorageGB": TotalLocalStorageGBRequestTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestTypeDef,
         "AcceleratorTypes": List[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountRequestOutputTypeDef,
+        "AcceleratorCount": AcceleratorCountRequestTypeDef,
         "AcceleratorManufacturers": List[AcceleratorManufacturerType],
         "AcceleratorNames": List[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestOutputTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestOutputTypeDef,
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
         "AllowedInstanceTypes": List[str],
     },
     total=False,
 )
 
 
 class InstanceRequirementsOutputTypeDef(
@@ -2590,26 +2237,14 @@
 
 class InstanceRequirementsTypeDef(
     _RequiredInstanceRequirementsTypeDef, _OptionalInstanceRequirementsTypeDef
 ):
     pass
 
 
-WarmPoolConfigurationTypeDef = TypedDict(
-    "WarmPoolConfigurationTypeDef",
-    {
-        "MaxGroupPreparedCapacity": int,
-        "MinSize": int,
-        "PoolState": WarmPoolStateType,
-        "Status": Literal["PendingDelete"],
-        "InstanceReusePolicy": InstanceReusePolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredPutWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredPutWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalPutWarmPoolTypeRequestTypeDef = TypedDict(
@@ -2626,14 +2261,26 @@
 
 class PutWarmPoolTypeRequestTypeDef(
     _RequiredPutWarmPoolTypeRequestTypeDef, _OptionalPutWarmPoolTypeRequestTypeDef
 ):
     pass
 
 
+WarmPoolConfigurationTypeDef = TypedDict(
+    "WarmPoolConfigurationTypeDef",
+    {
+        "MaxGroupPreparedCapacity": int,
+        "MinSize": int,
+        "PoolState": WarmPoolStateType,
+        "Status": Literal["PendingDelete"],
+        "InstanceReusePolicy": InstanceReusePolicyTypeDef,
+    },
+    total=False,
+)
+
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2652,88 +2299,88 @@
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLaunchConfigurationTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTypeDef",
+_RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
+    "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
-        "ImageId": str,
-        "InstanceType": str,
-        "CreatedTime": datetime,
     },
 )
-_OptionalLaunchConfigurationTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTypeDef",
+_OptionalCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
+    "_OptionalCreateLaunchConfigurationTypeRequestTypeDef",
     {
-        "LaunchConfigurationARN": str,
+        "ImageId": str,
         "KeyName": str,
-        "SecurityGroups": List[str],
+        "SecurityGroups": Sequence[str],
         "ClassicLinkVPCId": str,
-        "ClassicLinkVPCSecurityGroups": List[str],
+        "ClassicLinkVPCSecurityGroups": Sequence[str],
         "UserData": str,
+        "InstanceId": str,
+        "InstanceType": str,
         "KernelId": str,
         "RamdiskId": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
-        "InstanceMonitoring": InstanceMonitoringOutputTypeDef,
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "InstanceMonitoring": InstanceMonitoringTypeDef,
         "SpotPrice": str,
         "IamInstanceProfile": str,
         "EbsOptimized": bool,
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
-        "MetadataOptions": InstanceMetadataOptionsOutputTypeDef,
+        "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
 
-class LaunchConfigurationTypeDef(
-    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
+class CreateLaunchConfigurationTypeRequestTypeDef(
+    _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
+    _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
-    "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
+_RequiredLaunchConfigurationTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTypeDef",
     {
         "LaunchConfigurationName": str,
+        "ImageId": str,
+        "InstanceType": str,
+        "CreatedTime": datetime,
     },
 )
-_OptionalCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
-    "_OptionalCreateLaunchConfigurationTypeRequestTypeDef",
+_OptionalLaunchConfigurationTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTypeDef",
     {
-        "ImageId": str,
+        "LaunchConfigurationARN": str,
         "KeyName": str,
-        "SecurityGroups": Sequence[str],
+        "SecurityGroups": List[str],
         "ClassicLinkVPCId": str,
-        "ClassicLinkVPCSecurityGroups": Sequence[str],
+        "ClassicLinkVPCSecurityGroups": List[str],
         "UserData": str,
-        "InstanceId": str,
-        "InstanceType": str,
         "KernelId": str,
         "RamdiskId": str,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "InstanceMonitoring": InstanceMonitoringTypeDef,
         "SpotPrice": str,
         "IamInstanceProfile": str,
         "EbsOptimized": bool,
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
         "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
 
-class CreateLaunchConfigurationTypeRequestTypeDef(
-    _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
-    _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
+class LaunchConfigurationTypeDef(
+    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
 
 _RequiredMetricStatOutputTypeDef = TypedDict(
     "_RequiredMetricStatOutputTypeDef",
     {
@@ -2831,15 +2478,15 @@
 )
 
 LaunchTemplateOverridesOutputTypeDef = TypedDict(
     "LaunchTemplateOverridesOutputTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsOutputTypeDef,
     },
     total=False,
 )
 
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
@@ -2965,15 +2612,15 @@
 ):
     pass
 
 
 LaunchTemplateOutputTypeDef = TypedDict(
     "LaunchTemplateOutputTypeDef",
     {
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
     },
     total=False,
 )
 
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
@@ -3006,15 +2653,15 @@
 )
 
 CustomizedMetricSpecificationOutputTypeDef = TypedDict(
     "CustomizedMetricSpecificationOutputTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
         "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
     },
     total=False,
 )
 
@@ -3052,15 +2699,15 @@
     total=False,
 )
 
 MixedInstancesPolicyOutputTypeDef = TypedDict(
     "MixedInstancesPolicyOutputTypeDef",
     {
         "LaunchTemplate": LaunchTemplateOutputTypeDef,
-        "InstancesDistribution": InstancesDistributionOutputTypeDef,
+        "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
@@ -3075,19 +2722,17 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
     "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
     {
-        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairOutputTypeDef,
-        "PredefinedScalingMetricSpecification": (
-            PredictiveScalingPredefinedScalingMetricOutputTypeDef
-        ),
-        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricOutputTypeDef,
+        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairTypeDef,
+        "PredefinedScalingMetricSpecification": PredictiveScalingPredefinedScalingMetricTypeDef,
+        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricTypeDef,
         "CustomizedScalingMetricSpecification": (
             PredictiveScalingCustomizedScalingMetricOutputTypeDef
         ),
         "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
         "CustomizedCapacityMetricSpecification": (
             PredictiveScalingCustomizedCapacityMetricOutputTypeDef
         ),
@@ -3108,15 +2753,15 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_OptionalTargetTrackingConfigurationOutputTypeDef",
     {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationOutputTypeDef,
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
 
@@ -3191,15 +2836,15 @@
     },
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
@@ -3214,28 +2859,28 @@
         "MaxInstanceLifetime": int,
         "CapacityRebalance": bool,
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "WarmPoolSize": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
-        "TrafficSources": List[TrafficSourceIdentifierOutputTypeDef],
+        "TrafficSources": List[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
 
 DesiredConfigurationOutputTypeDef = TypedDict(
     "DesiredConfigurationOutputTypeDef",
     {
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
@@ -3461,15 +3106,15 @@
         "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentOutputTypeDef],
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
         "EstimatedInstanceWarmup": int,
         "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestOutputTypeDef
+    from mypy_boto3_autoscaling.type_defs import AcceleratorCountRequestTypeDef
 
-    data: AcceleratorCountRequestOutputTypeDef = {...}
+    data: AcceleratorCountRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -48,49 +48,42 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AcceleratorCountRequestOutputTypeDef",
     "AcceleratorCountRequestTypeDef",
-    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
-    "LaunchTemplateSpecificationOutputTypeDef",
+    "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
-    "TrafficSourceIdentifierOutputTypeDef",
-    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
-    "EbsOutputTypeDef",
     "EbsTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
-    "LaunchTemplateSpecificationTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
@@ -117,54 +110,39 @@
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
-    "InstanceMetadataOptionsOutputTypeDef",
-    "InstanceMonitoringOutputTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
     "RefreshPreferencesOutputTypeDef",
-    "MemoryGiBPerVCpuRequestOutputTypeDef",
-    "MemoryMiBRequestOutputTypeDef",
-    "NetworkBandwidthGbpsRequestOutputTypeDef",
-    "NetworkInterfaceCountRequestOutputTypeDef",
-    "TotalLocalStorageGBRequestOutputTypeDef",
-    "VCpuCountRequestOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
-    "InstanceReusePolicyOutputTypeDef",
     "InstanceReusePolicyTypeDef",
-    "InstancesDistributionOutputTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
-    "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
-    "PredictiveScalingPredefinedLoadMetricOutputTypeDef",
-    "PredictiveScalingPredefinedMetricPairOutputTypeDef",
-    "PredictiveScalingPredefinedScalingMetricOutputTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
     "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
-    "StepAdjustmentOutputTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
@@ -199,36 +177,35 @@
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    "BlockDeviceMappingOutputTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
     "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
-    "WarmPoolConfigurationTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
+    "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
-    "LaunchConfigurationTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
+    "LaunchConfigurationTypeDef",
     "MetricStatOutputTypeDef",
     "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "RollbackDetailsTypeDef",
     "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
@@ -268,41 +245,23 @@
     "GetPredictiveScalingForecastAnswerTypeDef",
     "ScalingPolicyTypeDef",
     "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
-AcceleratorCountRequestOutputTypeDef = TypedDict(
-    "AcceleratorCountRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
-AcceleratorTotalMemoryMiBRequestOutputTypeDef = TypedDict(
-    "AcceleratorTotalMemoryMiBRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
 AcceleratorTotalMemoryMiBRequestTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -441,16 +400,16 @@
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
 )
 
-LaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "LaunchTemplateSpecificationOutputTypeDef",
+LaunchTemplateSpecificationTypeDef = TypedDict(
+    "LaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
     total=False,
 )
@@ -472,42 +431,14 @@
         "Key": str,
         "Value": str,
         "PropagateAtLaunch": bool,
     },
     total=False,
 )
 
-_RequiredTrafficSourceIdentifierOutputTypeDef = TypedDict(
-    "_RequiredTrafficSourceIdentifierOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-_OptionalTrafficSourceIdentifierOutputTypeDef = TypedDict(
-    "_OptionalTrafficSourceIdentifierOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-class TrafficSourceIdentifierOutputTypeDef(
-    _RequiredTrafficSourceIdentifierOutputTypeDef, _OptionalTrafficSourceIdentifierOutputTypeDef
-):
-    pass
-
-BaselineEbsBandwidthMbpsRequestOutputTypeDef = TypedDict(
-    "BaselineEbsBandwidthMbpsRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
 BaselineEbsBandwidthMbpsRequestTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
@@ -564,28 +495,14 @@
 
 class ScheduledUpdateGroupActionRequestTypeDef(
     _RequiredScheduledUpdateGroupActionRequestTypeDef,
     _OptionalScheduledUpdateGroupActionRequestTypeDef,
 ):
     pass
 
-EbsOutputTypeDef = TypedDict(
-    "EbsOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeSize": int,
-        "VolumeType": str,
-        "DeleteOnTermination": bool,
-        "Iops": int,
-        "Encrypted": bool,
-        "Throughput": int,
-    },
-    total=False,
-)
-
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
@@ -630,24 +547,14 @@
 
 class CompleteLifecycleActionTypeRequestTypeDef(
     _RequiredCompleteLifecycleActionTypeRequestTypeDef,
     _OptionalCompleteLifecycleActionTypeRequestTypeDef,
 ):
     pass
 
-LaunchTemplateSpecificationTypeDef = TypedDict(
-    "LaunchTemplateSpecificationTypeDef",
-    {
-        "LaunchTemplateId": str,
-        "LaunchTemplateName": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 _RequiredLifecycleHookSpecificationTypeDef = TypedDict(
     "_RequiredLifecycleHookSpecificationTypeDef",
     {
         "LifecycleHookName": str,
         "LifecycleTransition": str,
     },
 )
@@ -702,22 +609,14 @@
     "InstanceMonitoringTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1202,32 +1101,14 @@
         "AutoScalingGroupName": str,
         "PolicyName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-InstanceMetadataOptionsOutputTypeDef = TypedDict(
-    "InstanceMetadataOptionsOutputTypeDef",
-    {
-        "HttpTokens": InstanceMetadataHttpTokensStateType,
-        "HttpPutResponseHopLimit": int,
-        "HttpEndpoint": InstanceMetadataEndpointStateType,
-    },
-    total=False,
-)
-
-InstanceMonitoringOutputTypeDef = TypedDict(
-    "InstanceMonitoringOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
@@ -1253,88 +1134,14 @@
         "AutoRollback": bool,
         "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
         "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
-MemoryGiBPerVCpuRequestOutputTypeDef = TypedDict(
-    "MemoryGiBPerVCpuRequestOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
-_RequiredMemoryMiBRequestOutputTypeDef = TypedDict(
-    "_RequiredMemoryMiBRequestOutputTypeDef",
-    {
-        "Min": int,
-    },
-)
-_OptionalMemoryMiBRequestOutputTypeDef = TypedDict(
-    "_OptionalMemoryMiBRequestOutputTypeDef",
-    {
-        "Max": int,
-    },
-    total=False,
-)
-
-class MemoryMiBRequestOutputTypeDef(
-    _RequiredMemoryMiBRequestOutputTypeDef, _OptionalMemoryMiBRequestOutputTypeDef
-):
-    pass
-
-NetworkBandwidthGbpsRequestOutputTypeDef = TypedDict(
-    "NetworkBandwidthGbpsRequestOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
-NetworkInterfaceCountRequestOutputTypeDef = TypedDict(
-    "NetworkInterfaceCountRequestOutputTypeDef",
-    {
-        "Min": int,
-        "Max": int,
-    },
-    total=False,
-)
-
-TotalLocalStorageGBRequestOutputTypeDef = TypedDict(
-    "TotalLocalStorageGBRequestOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
-_RequiredVCpuCountRequestOutputTypeDef = TypedDict(
-    "_RequiredVCpuCountRequestOutputTypeDef",
-    {
-        "Min": int,
-    },
-)
-_OptionalVCpuCountRequestOutputTypeDef = TypedDict(
-    "_OptionalVCpuCountRequestOutputTypeDef",
-    {
-        "Max": int,
-    },
-    total=False,
-)
-
-class VCpuCountRequestOutputTypeDef(
-    _RequiredVCpuCountRequestOutputTypeDef, _OptionalVCpuCountRequestOutputTypeDef
-):
-    pass
-
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1397,43 +1204,22 @@
     },
     total=False,
 )
 
 class VCpuCountRequestTypeDef(_RequiredVCpuCountRequestTypeDef, _OptionalVCpuCountRequestTypeDef):
     pass
 
-InstanceReusePolicyOutputTypeDef = TypedDict(
-    "InstanceReusePolicyOutputTypeDef",
-    {
-        "ReuseOnScaleIn": bool,
-    },
-    total=False,
-)
-
 InstanceReusePolicyTypeDef = TypedDict(
     "InstanceReusePolicyTypeDef",
     {
         "ReuseOnScaleIn": bool,
     },
     total=False,
 )
 
-InstancesDistributionOutputTypeDef = TypedDict(
-    "InstancesDistributionOutputTypeDef",
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
 InstancesDistributionTypeDef = TypedDict(
     "InstancesDistributionTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
@@ -1456,34 +1242,14 @@
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-_RequiredPredefinedMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredefinedMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedMetricType": MetricTypeType,
-    },
-)
-_OptionalPredefinedMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredefinedMetricSpecificationOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-class PredefinedMetricSpecificationOutputTypeDef(
-    _RequiredPredefinedMetricSpecificationOutputTypeDef,
-    _OptionalPredefinedMetricSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1495,74 +1261,14 @@
 )
 
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
-_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef",
-    {
-        "PredefinedMetricType": PredefinedLoadMetricTypeType,
-    },
-)
-_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-class PredictiveScalingPredefinedLoadMetricOutputTypeDef(
-    _RequiredPredictiveScalingPredefinedLoadMetricOutputTypeDef,
-    _OptionalPredictiveScalingPredefinedLoadMetricOutputTypeDef,
-):
-    pass
-
-_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef",
-    {
-        "PredefinedMetricType": PredefinedMetricPairTypeType,
-    },
-)
-_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-class PredictiveScalingPredefinedMetricPairOutputTypeDef(
-    _RequiredPredictiveScalingPredefinedMetricPairOutputTypeDef,
-    _OptionalPredictiveScalingPredefinedMetricPairOutputTypeDef,
-):
-    pass
-
-_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef",
-    {
-        "PredefinedMetricType": PredefinedScalingMetricTypeType,
-    },
-)
-_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-class PredictiveScalingPredefinedScalingMetricOutputTypeDef(
-    _RequiredPredictiveScalingPredefinedScalingMetricOutputTypeDef,
-    _OptionalPredictiveScalingPredefinedScalingMetricOutputTypeDef,
-):
-    pass
-
 _RequiredPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
     "_RequiredPredictiveScalingPredefinedLoadMetricTypeDef",
     {
         "PredefinedMetricType": PredefinedLoadMetricTypeType,
     },
 )
 _OptionalPredictiveScalingPredefinedLoadMetricTypeDef = TypedDict(
@@ -1746,34 +1452,14 @@
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
-_RequiredStepAdjustmentOutputTypeDef = TypedDict(
-    "_RequiredStepAdjustmentOutputTypeDef",
-    {
-        "ScalingAdjustment": int,
-    },
-)
-_OptionalStepAdjustmentOutputTypeDef = TypedDict(
-    "_OptionalStepAdjustmentOutputTypeDef",
-    {
-        "MetricIntervalLowerBound": float,
-        "MetricIntervalUpperBound": float,
-    },
-    total=False,
-)
-
-class StepAdjustmentOutputTypeDef(
-    _RequiredStepAdjustmentOutputTypeDef, _OptionalStepAdjustmentOutputTypeDef
-):
-    pass
-
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalScalingProcessQueryRequestTypeDef = TypedDict(
@@ -2177,15 +1863,15 @@
     },
 )
 _OptionalAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_OptionalAutoScalingInstanceDetailsTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 class AutoScalingInstanceDetailsTypeDef(
     _RequiredAutoScalingInstanceDetailsTypeDef, _OptionalAutoScalingInstanceDetailsTypeDef
@@ -2203,15 +1889,15 @@
     },
 )
 _OptionalInstanceTypeDef = TypedDict(
     "_OptionalInstanceTypeDef",
     {
         "InstanceType": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
@@ -2245,35 +1931,14 @@
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
     },
 )
 
-_RequiredBlockDeviceMappingOutputTypeDef = TypedDict(
-    "_RequiredBlockDeviceMappingOutputTypeDef",
-    {
-        "DeviceName": str,
-    },
-)
-_OptionalBlockDeviceMappingOutputTypeDef = TypedDict(
-    "_OptionalBlockDeviceMappingOutputTypeDef",
-    {
-        "VirtualName": str,
-        "Ebs": EbsOutputTypeDef,
-        "NoDevice": bool,
-    },
-    total=False,
-)
-
-class BlockDeviceMappingOutputTypeDef(
-    _RequiredBlockDeviceMappingOutputTypeDef, _OptionalBlockDeviceMappingOutputTypeDef
-):
-    pass
-
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
     },
 )
 _OptionalBlockDeviceMappingTypeDef = TypedDict(
@@ -2311,15 +1976,15 @@
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricOutputTypeDef = TypedDict(
     "_OptionalMetricOutputTypeDef",
     {
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
     pass
 
@@ -2402,41 +2067,41 @@
     },
     total=False,
 )
 
 _RequiredInstanceRequirementsOutputTypeDef = TypedDict(
     "_RequiredInstanceRequirementsOutputTypeDef",
     {
-        "VCpuCount": VCpuCountRequestOutputTypeDef,
-        "MemoryMiB": MemoryMiBRequestOutputTypeDef,
+        "VCpuCount": VCpuCountRequestTypeDef,
+        "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
 _OptionalInstanceRequirementsOutputTypeDef = TypedDict(
     "_OptionalInstanceRequirementsOutputTypeDef",
     {
         "CpuManufacturers": List[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestOutputTypeDef,
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestTypeDef,
         "ExcludedInstanceTypes": List[str],
         "InstanceGenerations": List[InstanceGenerationType],
         "SpotMaxPricePercentageOverLowestPrice": int,
         "OnDemandMaxPricePercentageOverLowestPrice": int,
         "BareMetal": BareMetalType,
         "BurstablePerformance": BurstablePerformanceType,
         "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountRequestOutputTypeDef,
+        "NetworkInterfaceCount": NetworkInterfaceCountRequestTypeDef,
         "LocalStorage": LocalStorageType,
         "LocalStorageTypes": List[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBRequestOutputTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestOutputTypeDef,
+        "TotalLocalStorageGB": TotalLocalStorageGBRequestTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestTypeDef,
         "AcceleratorTypes": List[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountRequestOutputTypeDef,
+        "AcceleratorCount": AcceleratorCountRequestTypeDef,
         "AcceleratorManufacturers": List[AcceleratorManufacturerType],
         "AcceleratorNames": List[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestOutputTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestOutputTypeDef,
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
         "AllowedInstanceTypes": List[str],
     },
     total=False,
 )
 
 class InstanceRequirementsOutputTypeDef(
     _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
@@ -2479,26 +2144,14 @@
 )
 
 class InstanceRequirementsTypeDef(
     _RequiredInstanceRequirementsTypeDef, _OptionalInstanceRequirementsTypeDef
 ):
     pass
 
-WarmPoolConfigurationTypeDef = TypedDict(
-    "WarmPoolConfigurationTypeDef",
-    {
-        "MaxGroupPreparedCapacity": int,
-        "MinSize": int,
-        "PoolState": WarmPoolStateType,
-        "Status": Literal["PendingDelete"],
-        "InstanceReusePolicy": InstanceReusePolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredPutWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredPutWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalPutWarmPoolTypeRequestTypeDef = TypedDict(
@@ -2513,14 +2166,26 @@
 )
 
 class PutWarmPoolTypeRequestTypeDef(
     _RequiredPutWarmPoolTypeRequestTypeDef, _OptionalPutWarmPoolTypeRequestTypeDef
 ):
     pass
 
+WarmPoolConfigurationTypeDef = TypedDict(
+    "WarmPoolConfigurationTypeDef",
+    {
+        "MaxGroupPreparedCapacity": int,
+        "MinSize": int,
+        "PoolState": WarmPoolStateType,
+        "Status": Literal["PendingDelete"],
+        "InstanceReusePolicy": InstanceReusePolicyTypeDef,
+    },
+    total=False,
+)
+
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2539,85 +2204,85 @@
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLaunchConfigurationTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTypeDef",
+_RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
+    "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
-        "ImageId": str,
-        "InstanceType": str,
-        "CreatedTime": datetime,
     },
 )
-_OptionalLaunchConfigurationTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTypeDef",
+_OptionalCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
+    "_OptionalCreateLaunchConfigurationTypeRequestTypeDef",
     {
-        "LaunchConfigurationARN": str,
+        "ImageId": str,
         "KeyName": str,
-        "SecurityGroups": List[str],
+        "SecurityGroups": Sequence[str],
         "ClassicLinkVPCId": str,
-        "ClassicLinkVPCSecurityGroups": List[str],
+        "ClassicLinkVPCSecurityGroups": Sequence[str],
         "UserData": str,
+        "InstanceId": str,
+        "InstanceType": str,
         "KernelId": str,
         "RamdiskId": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingOutputTypeDef],
-        "InstanceMonitoring": InstanceMonitoringOutputTypeDef,
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "InstanceMonitoring": InstanceMonitoringTypeDef,
         "SpotPrice": str,
         "IamInstanceProfile": str,
         "EbsOptimized": bool,
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
-        "MetadataOptions": InstanceMetadataOptionsOutputTypeDef,
+        "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
-class LaunchConfigurationTypeDef(
-    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
+class CreateLaunchConfigurationTypeRequestTypeDef(
+    _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
+    _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
 ):
     pass
 
-_RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
-    "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
+_RequiredLaunchConfigurationTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTypeDef",
     {
         "LaunchConfigurationName": str,
+        "ImageId": str,
+        "InstanceType": str,
+        "CreatedTime": datetime,
     },
 )
-_OptionalCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
-    "_OptionalCreateLaunchConfigurationTypeRequestTypeDef",
+_OptionalLaunchConfigurationTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTypeDef",
     {
-        "ImageId": str,
+        "LaunchConfigurationARN": str,
         "KeyName": str,
-        "SecurityGroups": Sequence[str],
+        "SecurityGroups": List[str],
         "ClassicLinkVPCId": str,
-        "ClassicLinkVPCSecurityGroups": Sequence[str],
+        "ClassicLinkVPCSecurityGroups": List[str],
         "UserData": str,
-        "InstanceId": str,
-        "InstanceType": str,
         "KernelId": str,
         "RamdiskId": str,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "InstanceMonitoring": InstanceMonitoringTypeDef,
         "SpotPrice": str,
         "IamInstanceProfile": str,
         "EbsOptimized": bool,
         "AssociatePublicIpAddress": bool,
         "PlacementTenancy": str,
         "MetadataOptions": InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
-class CreateLaunchConfigurationTypeRequestTypeDef(
-    _RequiredCreateLaunchConfigurationTypeRequestTypeDef,
-    _OptionalCreateLaunchConfigurationTypeRequestTypeDef,
+class LaunchConfigurationTypeDef(
+    _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
 _RequiredMetricStatOutputTypeDef = TypedDict(
     "_RequiredMetricStatOutputTypeDef",
     {
         "Metric": MetricOutputTypeDef,
@@ -2706,15 +2371,15 @@
 )
 
 LaunchTemplateOverridesOutputTypeDef = TypedDict(
     "LaunchTemplateOverridesOutputTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsOutputTypeDef,
     },
     total=False,
 )
 
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
@@ -2832,15 +2497,15 @@
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
 LaunchTemplateOutputTypeDef = TypedDict(
     "LaunchTemplateOutputTypeDef",
     {
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
     },
     total=False,
 )
 
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
@@ -2873,15 +2538,15 @@
 )
 
 CustomizedMetricSpecificationOutputTypeDef = TypedDict(
     "CustomizedMetricSpecificationOutputTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
         "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
     },
     total=False,
 )
 
@@ -2919,15 +2584,15 @@
     total=False,
 )
 
 MixedInstancesPolicyOutputTypeDef = TypedDict(
     "MixedInstancesPolicyOutputTypeDef",
     {
         "LaunchTemplate": LaunchTemplateOutputTypeDef,
-        "InstancesDistribution": InstancesDistributionOutputTypeDef,
+        "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
@@ -2942,19 +2607,17 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
     "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
     {
-        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairOutputTypeDef,
-        "PredefinedScalingMetricSpecification": (
-            PredictiveScalingPredefinedScalingMetricOutputTypeDef
-        ),
-        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricOutputTypeDef,
+        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairTypeDef,
+        "PredefinedScalingMetricSpecification": PredictiveScalingPredefinedScalingMetricTypeDef,
+        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricTypeDef,
         "CustomizedScalingMetricSpecification": (
             PredictiveScalingCustomizedScalingMetricOutputTypeDef
         ),
         "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
         "CustomizedCapacityMetricSpecification": (
             PredictiveScalingCustomizedCapacityMetricOutputTypeDef
         ),
@@ -2973,15 +2636,15 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_OptionalTargetTrackingConfigurationOutputTypeDef",
     {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationOutputTypeDef,
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
 class TargetTrackingConfigurationOutputTypeDef(
@@ -3050,15 +2713,15 @@
     },
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
@@ -3073,26 +2736,26 @@
         "MaxInstanceLifetime": int,
         "CapacityRebalance": bool,
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "WarmPoolSize": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
-        "TrafficSources": List[TrafficSourceIdentifierOutputTypeDef],
+        "TrafficSources": List[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
 DesiredConfigurationOutputTypeDef = TypedDict(
     "DesiredConfigurationOutputTypeDef",
     {
-        "LaunchTemplate": LaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
@@ -3308,15 +2971,15 @@
         "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentOutputTypeDef],
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
         "EstimatedInstanceWarmup": int,
         "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
```

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.28.13
-Summary: Type annotations for boto3.AutoScaling 1.28.13 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling)](https://pepy.tech/project/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,49 +392,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
-    AcceleratorCountRequestOutputTypeDef,
     AcceleratorCountRequestTypeDef,
-    AcceleratorTotalMemoryMiBRequestOutputTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
     ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
-    LaunchTemplateSpecificationOutputTypeDef,
+    LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
-    TrafficSourceIdentifierOutputTypeDef,
-    BaselineEbsBandwidthMbpsRequestOutputTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
-    EbsOutputTypeDef,
     EbsTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
-    LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
@@ -461,54 +454,39 @@
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
-    InstanceMetadataOptionsOutputTypeDef,
-    InstanceMonitoringOutputTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
     RefreshPreferencesOutputTypeDef,
-    MemoryGiBPerVCpuRequestOutputTypeDef,
-    MemoryMiBRequestOutputTypeDef,
-    NetworkBandwidthGbpsRequestOutputTypeDef,
-    NetworkInterfaceCountRequestOutputTypeDef,
-    TotalLocalStorageGBRequestOutputTypeDef,
-    VCpuCountRequestOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
-    InstanceReusePolicyOutputTypeDef,
     InstanceReusePolicyTypeDef,
-    InstancesDistributionOutputTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
-    PredictiveScalingPredefinedLoadMetricOutputTypeDef,
-    PredictiveScalingPredefinedMetricPairOutputTypeDef,
-    PredictiveScalingPredefinedScalingMetricOutputTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
     RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
-    StepAdjustmentOutputTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
@@ -543,36 +521,35 @@
     LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
-    BlockDeviceMappingOutputTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
-    WarmPoolConfigurationTypeDef,
     PutWarmPoolTypeRequestTypeDef,
+    WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
-    LaunchConfigurationTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
+    LaunchConfigurationTypeDef,
     MetricStatOutputTypeDef,
     TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
     RollbackDetailsTypeDef,
     LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
@@ -613,15 +590,15 @@
     ScalingPolicyTypeDef,
     PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestOutputTypeDef:
+def get_structure() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-1.28.13/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.28.15/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.28.13/setup.py` & `mypy-boto3-autoscaling-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.28.13",
+    version="1.28.15",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScaling 1.28.13 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AutoScaling 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

