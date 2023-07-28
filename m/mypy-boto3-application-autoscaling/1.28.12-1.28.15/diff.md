# Comparing `tmp/mypy-boto3-application-autoscaling-1.28.12.tar.gz` & `tmp/mypy-boto3-application-autoscaling-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-autoscaling-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-application-autoscaling-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-application-autoscaling-1.28.12.tar` & `mypy-boto3-application-autoscaling-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.468577 mypy-boto3-application-autoscaling-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-07-27 05:34:18.468577 mypy-boto3-application-autoscaling-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.468577 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-27 05:17:24.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-27 05:17:24.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-07-27 05:17:25.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-07-27 05:17:24.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.468577 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-07-27 05:34:18.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:34:18.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 05:34:18.000000 mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.468577 mypy-boto3-application-autoscaling-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-27 05:17:23.000000 mypy-boto3-application-autoscaling-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.212654 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26057 2023-07-28 20:19:25.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-07-28 20:19:24.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:42:16.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:42:15.000000 mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.216654 mypy-boto3-application-autoscaling-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-28 20:19:23.000000 mypy-boto3-application-autoscaling-1.28.15/setup.py
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/LICENSE` & `mypy-boto3-application-autoscaling-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-autoscaling)](https://pepy.tech/project/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,50 +348,44 @@
 
 `mypy_boto3_application_autoscaling.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
-    PaginatorConfigTypeDef,
-    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ResponseMetadataTypeDef,
-    ScalableTargetActionOutputTypeDef,
-    SuspendedStateOutputTypeDef,
-    StepAdjustmentOutputTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
-    TargetTrackingMetricDimensionOutputTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
-    RegisterScalableTargetRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/README.md` & `mypy-boto3-application-autoscaling-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-autoscaling)](https://pepy.tech/project/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,50 +316,44 @@
 
 `mypy_boto3_application_autoscaling.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
-    PaginatorConfigTypeDef,
-    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ResponseMetadataTypeDef,
-    ScalableTargetActionOutputTypeDef,
-    SuspendedStateOutputTypeDef,
-    StepAdjustmentOutputTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
-    TargetTrackingMetricDimensionOutputTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
-    RegisterScalableTargetRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/__init__.py` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/__init__.pyi` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/__main__.py` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationAutoScaling 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ApplicationAutoScaling 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/client.py` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/client.pyi` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/literals.py` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/literals.pyi` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/paginator.py` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -41,99 +41,93 @@
 __all__ = (
     "DescribeScalableTargetsPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScalingPoliciesPaginator",
     "DescribeScheduledActionsPaginator",
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
 class DescribeScalableTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalabletargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
-
 class DescribeScalingActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
-
 class DescribeScalingPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
-
 class DescribeScheduledActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescheduledactionspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/paginator.pyi` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,93 +41,99 @@
 __all__ = (
     "DescribeScalableTargetsPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScalingPoliciesPaginator",
     "DescribeScheduledActionsPaginator",
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
 class DescribeScalableTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalabletargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
+
 class DescribeScalingActivitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
+
 class DescribeScalingPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
+
 class DescribeScheduledActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescheduledactionspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/type_defs.py` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,53 +27,46 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlarmTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
-    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
-    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
-    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
-    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotScaledReasonTypeDef",
-    "PaginatorConfigTypeDef",
-    "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
     "SuspendedStateTypeDef",
-    "RegisterScalableTargetResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScalableTargetActionOutputTypeDef",
-    "SuspendedStateOutputTypeDef",
-    "StepAdjustmentOutputTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TargetTrackingMetricDimensionOutputTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
-    "RegisterScalableTargetRequestRequestTypeDef",
     "ScheduledActionTypeDef",
+    "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
@@ -95,22 +88,14 @@
     "AlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmARN": str,
     },
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
@@ -140,38 +125,24 @@
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
 )
 
-_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResourceIds": Sequence[str],
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
-    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
@@ -181,47 +152,31 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "IncludeNotScaledActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
-    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
@@ -232,47 +187,20 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeNotScaledActivities": bool,
     },
     total=False,
 )
 
-
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "PolicyNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
-    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -283,47 +211,20 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ScheduledActionNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
-    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -334,37 +235,27 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScheduledActionsRequestRequestTypeDef(
     _RequiredDescribeScheduledActionsRequestRequestTypeDef,
     _OptionalDescribeScheduledActionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
 _OptionalNotScaledReasonTypeDef = TypedDict(
@@ -373,72 +264,36 @@
         "MaxCapacity": int,
         "MinCapacity": int,
         "CurrentCapacity": int,
     },
     total=False,
 )
 
-
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
     pass
 
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
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
-
 ScalableTargetActionTypeDef = TypedDict(
     "ScalableTargetActionTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
@@ -450,132 +305,169 @@
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
     total=False,
 )
 
-RegisterScalableTargetResponseTypeDef = TypedDict(
-    "RegisterScalableTargetResponseTypeDef",
+_RequiredStepAdjustmentTypeDef = TypedDict(
+    "_RequiredStepAdjustmentTypeDef",
     {
-        "ScalableTargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ScalingAdjustment": int,
     },
 )
+_OptionalStepAdjustmentTypeDef = TypedDict(
+    "_OptionalStepAdjustmentTypeDef",
+    {
+        "MetricIntervalLowerBound": float,
+        "MetricIntervalUpperBound": float,
+    },
+    total=False,
+)
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
+    pass
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResourceARN": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-ScalableTargetActionOutputTypeDef = TypedDict(
-    "ScalableTargetActionOutputTypeDef",
+TargetTrackingMetricDimensionTypeDef = TypedDict(
+    "TargetTrackingMetricDimensionTypeDef",
     {
-        "MinCapacity": int,
-        "MaxCapacity": int,
+        "Name": str,
+        "Value": str,
     },
-    total=False,
 )
 
-SuspendedStateOutputTypeDef = TypedDict(
-    "SuspendedStateOutputTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "DynamicScalingInSuspended": bool,
-        "DynamicScalingOutSuspended": bool,
-        "ScheduledScalingSuspended": bool,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
-    total=False,
 )
 
-_RequiredStepAdjustmentOutputTypeDef = TypedDict(
-    "_RequiredStepAdjustmentOutputTypeDef",
+_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
-        "ScalingAdjustment": int,
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
-_OptionalStepAdjustmentOutputTypeDef = TypedDict(
-    "_OptionalStepAdjustmentOutputTypeDef",
+_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
-        "MetricIntervalLowerBound": float,
-        "MetricIntervalUpperBound": float,
+        "ResourceIds": Sequence[str],
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class StepAdjustmentOutputTypeDef(
-    _RequiredStepAdjustmentOutputTypeDef, _OptionalStepAdjustmentOutputTypeDef
+class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
+    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
 ):
     pass
 
-
-_RequiredStepAdjustmentTypeDef = TypedDict(
-    "_RequiredStepAdjustmentTypeDef",
+_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
-        "ScalingAdjustment": int,
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
-_OptionalStepAdjustmentTypeDef = TypedDict(
-    "_OptionalStepAdjustmentTypeDef",
+_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
-        "MetricIntervalLowerBound": float,
-        "MetricIntervalUpperBound": float,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "IncludeNotScaledActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
+class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
+    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+):
     pass
 
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Mapping[str, str],
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
-
-TargetTrackingMetricDimensionOutputTypeDef = TypedDict(
-    "TargetTrackingMetricDimensionOutputTypeDef",
+_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
-        "Name": str,
-        "Value": str,
+        "PolicyNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-TargetTrackingMetricDimensionTypeDef = TypedDict(
-    "TargetTrackingMetricDimensionTypeDef",
+class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
+    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     {
-        "Name": str,
-        "Value": str,
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ScheduledActionNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
+    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
@@ -595,19 +487,17 @@
         "StatusMessage": str,
         "Details": str,
         "NotScaledReasons": List[NotScaledReasonTypeDef],
     },
     total=False,
 )
 
-
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
-
 _RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
     "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -621,21 +511,45 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-
 class PutScheduledActionRequestRequestTypeDef(
     _RequiredPutScheduledActionRequestRequestTypeDef,
     _OptionalPutScheduledActionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
+    {
+        "ScheduledActionName": str,
+        "ScheduledActionARN": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "Schedule": str,
+        "ResourceId": str,
+        "CreationTime": datetime,
+    },
+)
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
+    {
+        "Timezone": str,
+        "ScalableDimension": ScalableDimensionType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ScalableTargetAction": ScalableTargetActionTypeDef,
+    },
+    total=False,
+)
+
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+    pass
 
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -649,50 +563,20 @@
         "RoleARN": str,
         "SuspendedState": SuspendedStateTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RegisterScalableTargetRequestRequestTypeDef(
     _RequiredRegisterScalableTargetRequestRequestTypeDef,
     _OptionalRegisterScalableTargetRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredScheduledActionTypeDef = TypedDict(
-    "_RequiredScheduledActionTypeDef",
-    {
-        "ScheduledActionName": str,
-        "ScheduledActionARN": str,
-        "ServiceNamespace": ServiceNamespaceType,
-        "Schedule": str,
-        "ResourceId": str,
-        "CreationTime": datetime,
-    },
-)
-_OptionalScheduledActionTypeDef = TypedDict(
-    "_OptionalScheduledActionTypeDef",
-    {
-        "Timezone": str,
-        "ScalableDimension": ScalableDimensionType,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ScalableTargetAction": ScalableTargetActionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
-    pass
-
-
 _RequiredScalableTargetTypeDef = TypedDict(
     "_RequiredScalableTargetTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
@@ -700,30 +584,28 @@
         "RoleARN": str,
         "CreationTime": datetime,
     },
 )
 _OptionalScalableTargetTypeDef = TypedDict(
     "_OptionalScalableTargetTypeDef",
     {
-        "SuspendedState": SuspendedStateOutputTypeDef,
+        "SuspendedState": SuspendedStateTypeDef,
         "ScalableTargetARN": str,
     },
     total=False,
 )
 
-
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
-
 StepScalingPolicyConfigurationOutputTypeDef = TypedDict(
     "StepScalingPolicyConfigurationOutputTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": List[StepAdjustmentOutputTypeDef],
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
         "MetricAggregationType": MetricAggregationTypeType,
     },
     total=False,
 )
 
@@ -738,15 +620,15 @@
     },
     total=False,
 )
 
 TargetTrackingMetricOutputTypeDef = TypedDict(
     "TargetTrackingMetricOutputTypeDef",
     {
-        "Dimensions": List[TargetTrackingMetricDimensionOutputTypeDef],
+        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
         "MetricName": str,
         "Namespace": str,
     },
     total=False,
 )
 
 TargetTrackingMetricTypeDef = TypedDict(
@@ -760,33 +642,33 @@
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
     "DescribeScalingActivitiesResponseTypeDef",
     {
         "ScalingActivities": List[ScalingActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsResponseTypeDef = TypedDict(
     "DescribeScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalableTargetsResponseTypeDef = TypedDict(
     "DescribeScalableTargetsResponseTypeDef",
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatOutputTypeDef",
     {
         "Metric": TargetTrackingMetricOutputTypeDef,
@@ -797,21 +679,19 @@
     "_OptionalTargetTrackingMetricStatOutputTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricStatOutputTypeDef(
     _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
 ):
     pass
 
-
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
         "Stat": str,
     },
 )
@@ -819,21 +699,19 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
-
 _RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
@@ -843,22 +721,20 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatOutputTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricDataQueryOutputTypeDef(
     _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
     _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
 ):
     pass
 
-
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -868,27 +744,25 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
-
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
 
@@ -910,31 +784,29 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
     "_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef",
     {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationOutputTypeDef,
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingScalingPolicyConfigurationOutputTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
@@ -945,22 +817,20 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -977,19 +847,17 @@
             TargetTrackingScalingPolicyConfigurationOutputTypeDef
         ),
         "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-
 _RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -1001,22 +869,20 @@
         "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class PutScalingPolicyRequestRequestTypeDef(
     _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
 ):
     pass
 
-
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling/type_defs.pyi` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,52 +27,47 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlarmTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
-    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
-    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
-    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
-    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotScaledReasonTypeDef",
-    "PaginatorConfigTypeDef",
-    "PredefinedMetricSpecificationOutputTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
     "SuspendedStateTypeDef",
-    "RegisterScalableTargetResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScalableTargetActionOutputTypeDef",
-    "SuspendedStateOutputTypeDef",
-    "StepAdjustmentOutputTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TargetTrackingMetricDimensionOutputTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
-    "RegisterScalableTargetRequestRequestTypeDef",
     "ScheduledActionTypeDef",
+    "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
@@ -94,22 +89,14 @@
     "AlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmARN": str,
     },
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
@@ -139,36 +126,24 @@
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
 )
 
-_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResourceIds": Sequence[str],
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
-    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
@@ -178,43 +153,33 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "IncludeNotScaledActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
-    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
@@ -225,42 +190,21 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeNotScaledActivities": bool,
     },
     total=False,
 )
 
+
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "PolicyNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
-    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
@@ -272,42 +216,21 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ScheduledActionNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
-    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
@@ -319,35 +242,29 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScheduledActionsRequestRequestTypeDef(
     _RequiredDescribeScheduledActionsRequestRequestTypeDef,
     _OptionalDescribeScheduledActionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
 _OptionalNotScaledReasonTypeDef = TypedDict(
@@ -356,46 +273,18 @@
         "MaxCapacity": int,
         "MinCapacity": int,
         "CurrentCapacity": int,
     },
     total=False,
 )
 
+
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
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
 
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
@@ -403,19 +292,21 @@
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
+
 ScalableTargetActionTypeDef = TypedDict(
     "ScalableTargetActionTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
@@ -427,128 +318,179 @@
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
     total=False,
 )
 
-RegisterScalableTargetResponseTypeDef = TypedDict(
-    "RegisterScalableTargetResponseTypeDef",
+_RequiredStepAdjustmentTypeDef = TypedDict(
+    "_RequiredStepAdjustmentTypeDef",
     {
-        "ScalableTargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ScalingAdjustment": int,
+    },
+)
+_OptionalStepAdjustmentTypeDef = TypedDict(
+    "_OptionalStepAdjustmentTypeDef",
+    {
+        "MetricIntervalLowerBound": float,
+        "MetricIntervalUpperBound": float,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
+    pass
+
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResourceARN": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-ScalableTargetActionOutputTypeDef = TypedDict(
-    "ScalableTargetActionOutputTypeDef",
+TargetTrackingMetricDimensionTypeDef = TypedDict(
+    "TargetTrackingMetricDimensionTypeDef",
     {
-        "MinCapacity": int,
-        "MaxCapacity": int,
+        "Name": str,
+        "Value": str,
     },
-    total=False,
 )
 
-SuspendedStateOutputTypeDef = TypedDict(
-    "SuspendedStateOutputTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "DynamicScalingInSuspended": bool,
-        "DynamicScalingOutSuspended": bool,
-        "ScheduledScalingSuspended": bool,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
-    total=False,
 )
 
-_RequiredStepAdjustmentOutputTypeDef = TypedDict(
-    "_RequiredStepAdjustmentOutputTypeDef",
+_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
-        "ScalingAdjustment": int,
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
-_OptionalStepAdjustmentOutputTypeDef = TypedDict(
-    "_OptionalStepAdjustmentOutputTypeDef",
+_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
-        "MetricIntervalLowerBound": float,
-        "MetricIntervalUpperBound": float,
+        "ResourceIds": Sequence[str],
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class StepAdjustmentOutputTypeDef(
-    _RequiredStepAdjustmentOutputTypeDef, _OptionalStepAdjustmentOutputTypeDef
+
+class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
+    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
 ):
     pass
 
-_RequiredStepAdjustmentTypeDef = TypedDict(
-    "_RequiredStepAdjustmentTypeDef",
+
+_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
-        "ScalingAdjustment": int,
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
-_OptionalStepAdjustmentTypeDef = TypedDict(
-    "_OptionalStepAdjustmentTypeDef",
+_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
-        "MetricIntervalLowerBound": float,
-        "MetricIntervalUpperBound": float,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "IncludeNotScaledActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
+
+class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
+    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+
+_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Mapping[str, str],
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
-
-TargetTrackingMetricDimensionOutputTypeDef = TypedDict(
-    "TargetTrackingMetricDimensionOutputTypeDef",
+_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
-        "Name": str,
-        "Value": str,
+        "PolicyNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-TargetTrackingMetricDimensionTypeDef = TypedDict(
-    "TargetTrackingMetricDimensionTypeDef",
+
+class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
+    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     {
-        "Name": str,
-        "Value": str,
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
+_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ScheduledActionNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+
+class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
+    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
@@ -568,17 +510,19 @@
         "StatusMessage": str,
         "Details": str,
         "NotScaledReasons": List[NotScaledReasonTypeDef],
     },
     total=False,
 )
 
+
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
+
 _RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
     "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -592,20 +536,50 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
+
 class PutScheduledActionRequestRequestTypeDef(
     _RequiredPutScheduledActionRequestRequestTypeDef,
     _OptionalPutScheduledActionRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
+    {
+        "ScheduledActionName": str,
+        "ScheduledActionARN": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "Schedule": str,
+        "ResourceId": str,
+        "CreationTime": datetime,
+    },
+)
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
+    {
+        "Timezone": str,
+        "ScalableDimension": ScalableDimensionType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ScalableTargetAction": ScalableTargetActionTypeDef,
+    },
+    total=False,
+)
+
+
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+    pass
+
+
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
@@ -618,45 +592,21 @@
         "RoleARN": str,
         "SuspendedState": SuspendedStateTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RegisterScalableTargetRequestRequestTypeDef(
     _RequiredRegisterScalableTargetRequestRequestTypeDef,
     _OptionalRegisterScalableTargetRequestRequestTypeDef,
 ):
     pass
 
-_RequiredScheduledActionTypeDef = TypedDict(
-    "_RequiredScheduledActionTypeDef",
-    {
-        "ScheduledActionName": str,
-        "ScheduledActionARN": str,
-        "ServiceNamespace": ServiceNamespaceType,
-        "Schedule": str,
-        "ResourceId": str,
-        "CreationTime": datetime,
-    },
-)
-_OptionalScheduledActionTypeDef = TypedDict(
-    "_OptionalScheduledActionTypeDef",
-    {
-        "Timezone": str,
-        "ScalableDimension": ScalableDimensionType,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ScalableTargetAction": ScalableTargetActionOutputTypeDef,
-    },
-    total=False,
-)
-
-class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
-    pass
 
 _RequiredScalableTargetTypeDef = TypedDict(
     "_RequiredScalableTargetTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -665,28 +615,30 @@
         "RoleARN": str,
         "CreationTime": datetime,
     },
 )
 _OptionalScalableTargetTypeDef = TypedDict(
     "_OptionalScalableTargetTypeDef",
     {
-        "SuspendedState": SuspendedStateOutputTypeDef,
+        "SuspendedState": SuspendedStateTypeDef,
         "ScalableTargetARN": str,
     },
     total=False,
 )
 
+
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
+
 StepScalingPolicyConfigurationOutputTypeDef = TypedDict(
     "StepScalingPolicyConfigurationOutputTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": List[StepAdjustmentOutputTypeDef],
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
         "MetricAggregationType": MetricAggregationTypeType,
     },
     total=False,
 )
 
@@ -701,15 +653,15 @@
     },
     total=False,
 )
 
 TargetTrackingMetricOutputTypeDef = TypedDict(
     "TargetTrackingMetricOutputTypeDef",
     {
-        "Dimensions": List[TargetTrackingMetricDimensionOutputTypeDef],
+        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
         "MetricName": str,
         "Namespace": str,
     },
     total=False,
 )
 
 TargetTrackingMetricTypeDef = TypedDict(
@@ -723,33 +675,33 @@
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
     "DescribeScalingActivitiesResponseTypeDef",
     {
         "ScalingActivities": List[ScalingActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsResponseTypeDef = TypedDict(
     "DescribeScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalableTargetsResponseTypeDef = TypedDict(
     "DescribeScalableTargetsResponseTypeDef",
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatOutputTypeDef",
     {
         "Metric": TargetTrackingMetricOutputTypeDef,
@@ -760,19 +712,21 @@
     "_OptionalTargetTrackingMetricStatOutputTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricStatOutputTypeDef(
     _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
 ):
     pass
 
+
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
         "Stat": str,
     },
 )
@@ -780,19 +734,21 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
+
 _RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
@@ -802,20 +758,22 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatOutputTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricDataQueryOutputTypeDef(
     _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
     _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
 ):
     pass
 
+
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -825,25 +783,27 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
+
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
 
@@ -865,29 +825,31 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
     "_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef",
     {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationOutputTypeDef,
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
         "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingScalingPolicyConfigurationOutputTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
@@ -898,20 +860,22 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -928,17 +892,19 @@
             TargetTrackingScalingPolicyConfigurationOutputTypeDef
         ),
         "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
+
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
+
 _RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -950,20 +916,22 @@
         "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class PutScalingPolicyRequestRequestTypeDef(
     _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
 ):
     pass
 
+
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-autoscaling)](https://pepy.tech/project/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,50 +348,44 @@
 
 `mypy_boto3_application_autoscaling.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
-    PaginatorConfigTypeDef,
-    PredefinedMetricSpecificationOutputTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ResponseMetadataTypeDef,
-    ScalableTargetActionOutputTypeDef,
-    SuspendedStateOutputTypeDef,
-    StepAdjustmentOutputTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
-    TargetTrackingMetricDimensionOutputTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
-    RegisterScalableTargetRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
```

### Comparing `mypy-boto3-application-autoscaling-1.28.12/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-application-autoscaling-1.28.15/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.28.12/setup.py` & `mypy-boto3-application-autoscaling-1.28.15/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-autoscaling",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationAutoScaling 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ApplicationAutoScaling 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

