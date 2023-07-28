# Comparing `tmp/mypy-boto3-autoscaling-plans-1.28.12.tar.gz` & `tmp/mypy-boto3-autoscaling-plans-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-plans-1.28.12.tar` & `mypy-boto3-autoscaling-plans-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.648572 mypy-boto3-autoscaling-plans-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-27 05:34:20.640572 mypy-boto3-autoscaling-plans-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.640572 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-07-27 05:17:51.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-07-27 05:17:51.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.640572 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.648572 mypy-boto3-autoscaling-plans-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.376697 mypy-boto3-autoscaling-plans-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-28 20:42:19.364697 mypy-boto3-autoscaling-plans-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.364697 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-07-28 20:20:01.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-07-28 20:20:01.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:00.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.364697 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:19.000000 mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.376697 mypy-boto3-autoscaling-plans-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:19:59.000000 mypy-boto3-autoscaling-plans-1.28.15/setup.py
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/LICENSE` & `mypy-boto3-autoscaling-plans-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.12
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,35 +343,32 @@
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterOutputTypeDef,
     TagFilterTypeDef,
-    CreateScalingPlanResponseTypeDef,
-    MetricDimensionOutputTypeDef,
+    ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PredefinedLoadMetricSpecificationOutputTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
-    PredefinedScalingMetricSpecificationOutputTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
-    ResponseMetadataTypeDef,
     ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationOutputTypeDef,
-    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
     TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
     ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
     ScalingInstructionTypeDef,
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/README.md` & `mypy-boto3-autoscaling-plans-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,35 +311,32 @@
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterOutputTypeDef,
     TagFilterTypeDef,
-    CreateScalingPlanResponseTypeDef,
-    MetricDimensionOutputTypeDef,
+    ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PredefinedLoadMetricSpecificationOutputTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
-    PredefinedScalingMetricSpecificationOutputTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
-    ResponseMetadataTypeDef,
     ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationOutputTypeDef,
-    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
     TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
     ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
     ScalingInstructionTypeDef,
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.py` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.pyi` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__main__.py` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScalingPlans 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AutoScalingPlans 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.py` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.pyi` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.py` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.pyi` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.py` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlanResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 
@@ -72,13 +72,13 @@
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.pyi` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlanResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 class DescribeScalingPlansPaginator(Paginator):
@@ -68,13 +68,13 @@
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.py` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,35 +38,32 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
-    "CreateScalingPlanResponseTypeDef",
-    "MetricDimensionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
-    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "PredefinedLoadMetricSpecificationOutputTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
-    "PredefinedScalingMetricSpecificationOutputTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
-    "ResponseMetadataTypeDef",
     "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
+    "CreateScalingPlanResponseTypeDef",
     "CustomizedLoadMetricSpecificationOutputTypeDef",
-    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
+    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
+    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
     "TargetTrackingConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
     "ScalingInstructionTypeDef",
@@ -92,27 +89,22 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-CreateScalingPlanResponseTypeDef = TypedDict(
-    "CreateScalingPlanResponseTypeDef",
-    {
-        "ScalingPlanVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "Value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
@@ -133,37 +125,24 @@
     "DeleteScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 
-_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
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
-class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
-    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -194,46 +173,14 @@
         "ScalableDimension": ScalableDimensionType,
         "ForecastDataType": ForecastDataTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
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
-_RequiredPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredefinedLoadMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedLoadMetricType": LoadMetricTypeType,
-    },
-)
-_OptionalPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredefinedLoadMetricSpecificationOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-
-class PredefinedLoadMetricSpecificationOutputTypeDef(
-    _RequiredPredefinedLoadMetricSpecificationOutputTypeDef,
-    _OptionalPredefinedLoadMetricSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -248,36 +195,14 @@
 class PredefinedLoadMetricSpecificationTypeDef(
     _RequiredPredefinedLoadMetricSpecificationTypeDef,
     _OptionalPredefinedLoadMetricSpecificationTypeDef,
 ):
     pass
 
 
-_RequiredPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredefinedScalingMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedScalingMetricType": ScalingMetricTypeType,
-    },
-)
-_OptionalPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredefinedScalingMetricSpecificationOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-
-class PredefinedScalingMetricSpecificationOutputTypeDef(
-    _RequiredPredefinedScalingMetricSpecificationOutputTypeDef,
-    _OptionalPredefinedScalingMetricSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredPredefinedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedScalingMetricSpecificationTypeDef",
     {
         "PredefinedScalingMetricType": ScalingMetricTypeType,
     },
 )
 _OptionalPredefinedScalingMetricSpecificationTypeDef = TypedDict(
@@ -292,25 +217,14 @@
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
 
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
 ApplicationSourceOutputTypeDef = TypedDict(
     "ApplicationSourceOutputTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": List[TagFilterOutputTypeDef],
     },
     total=False,
@@ -321,85 +235,93 @@
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
+CreateScalingPlanResponseTypeDef = TypedDict(
+    "CreateScalingPlanResponseTypeDef",
+    {
+        "ScalingPlanVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
 )
 _OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
     "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
     {
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
 
 class CustomizedLoadMetricSpecificationOutputTypeDef(
     _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
     _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
 ):
     pass
 
 
-_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
+_RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
+    "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
 )
-_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
+_OptionalCustomizedLoadMetricSpecificationTypeDef = TypedDict(
+    "_OptionalCustomizedLoadMetricSpecificationTypeDef",
     {
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
 
-class CustomizedScalingMetricSpecificationOutputTypeDef(
-    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
-    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
+class CustomizedLoadMetricSpecificationTypeDef(
+    _RequiredCustomizedLoadMetricSpecificationTypeDef,
+    _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
 
-_RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
-    "_RequiredCustomizedLoadMetricSpecificationTypeDef",
+_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
 )
-_OptionalCustomizedLoadMetricSpecificationTypeDef = TypedDict(
-    "_OptionalCustomizedLoadMetricSpecificationTypeDef",
+_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
     {
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
 
-class CustomizedLoadMetricSpecificationTypeDef(
-    _RequiredCustomizedLoadMetricSpecificationTypeDef,
-    _OptionalCustomizedLoadMetricSpecificationTypeDef,
+class CustomizedScalingMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
 ):
     pass
 
 
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
@@ -425,25 +347,48 @@
     pass
 
 
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
+    },
+)
+_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
+    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+):
+    pass
+
+
 DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
         "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScalingPlansRequestRequestTypeDef = TypedDict(
     "DescribeScalingPlansRequestRequestTypeDef",
     {
@@ -461,15 +406,15 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_OptionalTargetTrackingConfigurationOutputTypeDef",
     {
-        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationOutputTypeDef,
+        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationTypeDef,
         "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
         "DisableScaleIn": bool,
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "EstimatedInstanceWarmup": int,
     },
     total=False,
@@ -519,15 +464,15 @@
         "MaxCapacity": int,
         "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
     },
 )
 _OptionalScalingInstructionOutputTypeDef = TypedDict(
     "_OptionalScalingInstructionOutputTypeDef",
     {
-        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationOutputTypeDef,
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
         "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
@@ -680,19 +625,19 @@
 
 
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.pyi` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -37,35 +37,32 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
-    "CreateScalingPlanResponseTypeDef",
-    "MetricDimensionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
-    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "PredefinedLoadMetricSpecificationOutputTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
-    "PredefinedScalingMetricSpecificationOutputTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
-    "ResponseMetadataTypeDef",
     "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
+    "CreateScalingPlanResponseTypeDef",
     "CustomizedLoadMetricSpecificationOutputTypeDef",
-    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
+    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
+    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
     "TargetTrackingConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
     "ScalingInstructionTypeDef",
@@ -91,27 +88,22 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-CreateScalingPlanResponseTypeDef = TypedDict(
-    "CreateScalingPlanResponseTypeDef",
-    {
-        "ScalingPlanVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "Value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
@@ -132,35 +124,24 @@
     "DeleteScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 
-_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
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
 
-class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
-    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -189,44 +170,14 @@
         "ScalableDimension": ScalableDimensionType,
         "ForecastDataType": ForecastDataTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
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
-_RequiredPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredefinedLoadMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedLoadMetricType": LoadMetricTypeType,
-    },
-)
-_OptionalPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredefinedLoadMetricSpecificationOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-class PredefinedLoadMetricSpecificationOutputTypeDef(
-    _RequiredPredefinedLoadMetricSpecificationOutputTypeDef,
-    _OptionalPredefinedLoadMetricSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -239,34 +190,14 @@
 
 class PredefinedLoadMetricSpecificationTypeDef(
     _RequiredPredefinedLoadMetricSpecificationTypeDef,
     _OptionalPredefinedLoadMetricSpecificationTypeDef,
 ):
     pass
 
-_RequiredPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredefinedScalingMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedScalingMetricType": ScalingMetricTypeType,
-    },
-)
-_OptionalPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredefinedScalingMetricSpecificationOutputTypeDef",
-    {
-        "ResourceLabel": str,
-    },
-    total=False,
-)
-
-class PredefinedScalingMetricSpecificationOutputTypeDef(
-    _RequiredPredefinedScalingMetricSpecificationOutputTypeDef,
-    _OptionalPredefinedScalingMetricSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredPredefinedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedScalingMetricSpecificationTypeDef",
     {
         "PredefinedScalingMetricType": ScalingMetricTypeType,
     },
 )
 _OptionalPredefinedScalingMetricSpecificationTypeDef = TypedDict(
@@ -279,25 +210,14 @@
 
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
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
 ApplicationSourceOutputTypeDef = TypedDict(
     "ApplicationSourceOutputTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": List[TagFilterOutputTypeDef],
     },
     total=False,
@@ -308,80 +228,88 @@
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
+CreateScalingPlanResponseTypeDef = TypedDict(
+    "CreateScalingPlanResponseTypeDef",
+    {
+        "ScalingPlanVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
 )
 _OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
     "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
     {
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
 class CustomizedLoadMetricSpecificationOutputTypeDef(
     _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
     _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
 ):
     pass
 
-_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
+_RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
+    "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
 )
-_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
+_OptionalCustomizedLoadMetricSpecificationTypeDef = TypedDict(
+    "_OptionalCustomizedLoadMetricSpecificationTypeDef",
     {
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
-class CustomizedScalingMetricSpecificationOutputTypeDef(
-    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
-    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
+class CustomizedLoadMetricSpecificationTypeDef(
+    _RequiredCustomizedLoadMetricSpecificationTypeDef,
+    _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
-_RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
-    "_RequiredCustomizedLoadMetricSpecificationTypeDef",
+_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
 )
-_OptionalCustomizedLoadMetricSpecificationTypeDef = TypedDict(
-    "_OptionalCustomizedLoadMetricSpecificationTypeDef",
+_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
     {
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
-class CustomizedLoadMetricSpecificationTypeDef(
-    _RequiredCustomizedLoadMetricSpecificationTypeDef,
-    _OptionalCustomizedLoadMetricSpecificationTypeDef,
+class CustomizedScalingMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
 ):
     pass
 
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
         "MetricName": str,
@@ -404,25 +332,46 @@
 ):
     pass
 
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
     },
 )
+_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
+    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+):
+    pass
 
 DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
         "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScalingPlansRequestRequestTypeDef = TypedDict(
     "DescribeScalingPlansRequestRequestTypeDef",
     {
@@ -440,15 +389,15 @@
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
     "_OptionalTargetTrackingConfigurationOutputTypeDef",
     {
-        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationOutputTypeDef,
+        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationTypeDef,
         "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
         "DisableScaleIn": bool,
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "EstimatedInstanceWarmup": int,
     },
     total=False,
@@ -494,15 +443,15 @@
         "MaxCapacity": int,
         "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
     },
 )
 _OptionalScalingInstructionOutputTypeDef = TypedDict(
     "_OptionalScalingInstructionOutputTypeDef",
     {
-        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationOutputTypeDef,
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
         "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
@@ -643,19 +592,19 @@
     pass
 
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.12
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,35 +343,32 @@
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterOutputTypeDef,
     TagFilterTypeDef,
-    CreateScalingPlanResponseTypeDef,
-    MetricDimensionOutputTypeDef,
+    ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PredefinedLoadMetricSpecificationOutputTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
-    PredefinedScalingMetricSpecificationOutputTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
-    ResponseMetadataTypeDef,
     ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationOutputTypeDef,
-    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
     TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
     ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
     ScalingInstructionTypeDef,
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-plans-1.28.15/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.12/setup.py` & `mypy-boto3-autoscaling-plans-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling-plans",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScalingPlans 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.AutoScalingPlans 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

