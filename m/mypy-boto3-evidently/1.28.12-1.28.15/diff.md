# Comparing `tmp/mypy-boto3-evidently-1.28.12.tar.gz` & `tmp/mypy-boto3-evidently-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-evidently-1.28.12.tar", last modified: Thu Jul 27 05:34:41 2023, max compression
+gzip compressed data, was "mypy-boto3-evidently-1.28.15.tar", last modified: Fri Jul 28 20:42:47 2023, max compression
```

## Comparing `mypy-boto3-evidently-1.28.12.tar` & `mypy-boto3-evidently-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.216512 mypy-boto3-evidently-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-07-27 05:34:41.212512 mypy-boto3-evidently-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16911 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.204512 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-27 05:22:12.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46024 2023-07-27 05:22:13.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45939 2023-07-27 05:22:13.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:11.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.212512 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:41.000000 mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:41.216512 mypy-boto3-evidently-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-27 05:22:10.000000 mypy-boto3-evidently-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.129087 mypy-boto3-evidently-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18384 2023-07-28 20:42:47.129087 mypy-boto3-evidently-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.125087 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30404 2023-07-28 20:25:45.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-28 20:25:44.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-28 20:25:45.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-28 20:25:45.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-28 20:25:45.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-28 20:25:45.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45680 2023-07-28 20:25:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45595 2023-07-28 20:25:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.129087 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18384 2023-07-28 20:42:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:46.000000 mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:47.133087 mypy-boto3-evidently-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-28 20:25:43.000000 mypy-boto3-evidently-1.28.15/setup.py
```

### Comparing `mypy-boto3-evidently-1.28.12/LICENSE` & `mypy-boto3-evidently-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/PKG-INFO` & `mypy-boto3-evidently-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatchEvidently 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatchEvidently 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,29 +356,30 @@
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
     SegmentTypeDef,
     DeleteExperimentRequestRequestTypeDef,
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
-    VariableValueOutputTypeDef,
+    VariableValueTypeDef,
     EvaluationRuleTypeDef,
     EventTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
@@ -387,88 +388,86 @@
     GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExperimentsRequestRequestTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
-    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
     SegmentOverrideOutputTypeDef,
     StartExperimentRequestRequestTypeDef,
-    StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
-    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
-    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    VariableValueTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartExperimentResponseTypeDef,
+    StopExperimentResponseTypeDef,
+    StopLaunchResponseTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
+    VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
     UpdateProjectDataDeliveryRequestRequestTypeDef,
     ProjectDataDeliveryTypeDef,
     PutProjectEventsResponseTypeDef,
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
-    VariationConfigTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
+    CreateFeatureRequestRequestTypeDef,
+    UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
-    CreateFeatureRequestRequestTypeDef,
-    UpdateFeatureRequestRequestTypeDef,
     CreateFeatureResponseTypeDef,
     GetFeatureResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     CreateExperimentResponseTypeDef,
     GetExperimentResponseTypeDef,
     ListExperimentsResponseTypeDef,
     UpdateExperimentResponseTypeDef,
```

### Comparing `mypy-boto3-evidently-1.28.12/README.md` & `mypy-boto3-evidently-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,29 +324,30 @@
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
     SegmentTypeDef,
     DeleteExperimentRequestRequestTypeDef,
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
-    VariableValueOutputTypeDef,
+    VariableValueTypeDef,
     EvaluationRuleTypeDef,
     EventTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
@@ -355,88 +356,86 @@
     GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExperimentsRequestRequestTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
-    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
     SegmentOverrideOutputTypeDef,
     StartExperimentRequestRequestTypeDef,
-    StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
-    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
-    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    VariableValueTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartExperimentResponseTypeDef,
+    StopExperimentResponseTypeDef,
+    StopLaunchResponseTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
+    VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
     UpdateProjectDataDeliveryRequestRequestTypeDef,
     ProjectDataDeliveryTypeDef,
     PutProjectEventsResponseTypeDef,
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
-    VariationConfigTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
+    CreateFeatureRequestRequestTypeDef,
+    UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
-    CreateFeatureRequestRequestTypeDef,
-    UpdateFeatureRequestRequestTypeDef,
     CreateFeatureResponseTypeDef,
     GetFeatureResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     CreateExperimentResponseTypeDef,
     GetExperimentResponseTypeDef,
     ListExperimentsResponseTypeDef,
     UpdateExperimentResponseTypeDef,
```

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.py` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__init__.pyi` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/__main__.py` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchEvidently 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudWatchEvidently 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently\nOther"
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

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.py` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/client.pyi` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.py` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/literals.pyi` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.py` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,118 +49,110 @@
     "ListFeaturesPaginator",
     "ListLaunchesPaginator",
     "ListProjectsPaginator",
     "ListSegmentReferencesPaginator",
     "ListSegmentsPaginator",
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
 class ListExperimentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listexperimentspaginator)
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listexperimentspaginator)
         """
 
-
 class ListFeaturesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
     """
 
     def paginate(
-        self, *, project: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, project: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFeaturesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
         """
 
-
 class ListLaunchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listlaunchespaginator)
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLaunchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listlaunchespaginator)
         """
 
-
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
         """
 
-
 class ListSegmentReferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentreferencespaginator)
         """
 
-
 class ListSegmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSegmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
         """
```

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/paginator.pyi` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,110 +49,118 @@
     "ListFeaturesPaginator",
     "ListLaunchesPaginator",
     "ListProjectsPaginator",
     "ListSegmentReferencesPaginator",
     "ListSegmentsPaginator",
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
 class ListExperimentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listexperimentspaginator)
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listexperimentspaginator)
         """
 
+
 class ListFeaturesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
     """
 
     def paginate(
-        self, *, project: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, project: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFeaturesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listfeaturespaginator)
         """
 
+
 class ListLaunchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listlaunchespaginator)
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLaunchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listlaunchespaginator)
         """
 
+
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listprojectspaginator)
         """
 
+
 class ListSegmentReferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentreferencespaginator)
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentreferencespaginator)
         """
 
+
 class ListSegmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSegmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/paginators/#listsegmentspaginator)
         """
```

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.py` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,30 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "EvaluationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CloudWatchLogsDestinationConfigTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "OnlineAbConfigTypeDef",
     "TreatmentConfigTypeDef",
     "LaunchGroupConfigTypeDef",
     "ProjectAppConfigResourceConfigTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "SegmentTypeDef",
     "DeleteExperimentRequestRequestTypeDef",
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
-    "VariableValueOutputTypeDef",
+    "VariableValueTypeDef",
     "EvaluationRuleTypeDef",
     "EventTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
@@ -70,88 +71,86 @@
     "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
-    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExperimentsRequestRequestTypeDef",
-    "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListFeaturesRequestRequestTypeDef",
-    "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListLaunchesRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentReferencesRequestRequestTypeDef",
     "RefResourceTypeDef",
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListSegmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
     "SegmentOverrideOutputTypeDef",
     "StartExperimentRequestRequestTypeDef",
-    "StartExperimentResponseTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
-    "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
-    "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
-    "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "VariableValueTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartExperimentResponseTypeDef",
+    "StopExperimentResponseTypeDef",
+    "StopLaunchResponseTypeDef",
+    "TestSegmentPatternResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
+    "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
     "PutProjectEventsRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
+    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "ListFeaturesRequestListFeaturesPaginateTypeDef",
+    "ListLaunchesRequestListLaunchesPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
     "MetricMonitorConfigTypeDef",
     "MetricGoalTypeDef",
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
     "UpdateProjectDataDeliveryRequestRequestTypeDef",
     "ProjectDataDeliveryTypeDef",
     "PutProjectEventsResponseTypeDef",
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
-    "VariationConfigTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
+    "CreateFeatureRequestRequestTypeDef",
+    "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
-    "CreateFeatureRequestRequestTypeDef",
-    "UpdateFeatureRequestRequestTypeDef",
     "CreateFeatureResponseTypeDef",
     "GetFeatureResponseTypeDef",
     "UpdateFeatureResponseTypeDef",
     "CreateExperimentResponseTypeDef",
     "GetExperimentResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "UpdateExperimentResponseTypeDef",
@@ -187,14 +186,25 @@
 
 class EvaluationRequestTypeDef(
     _RequiredEvaluationRequestTypeDef, _OptionalEvaluationRequestTypeDef
 ):
     pass
 
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 CloudWatchLogsDestinationConfigTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
@@ -375,16 +385,16 @@
 
 class EvaluateFeatureRequestRequestTypeDef(
     _RequiredEvaluateFeatureRequestRequestTypeDef, _OptionalEvaluateFeatureRequestRequestTypeDef
 ):
     pass
 
 
-VariableValueOutputTypeDef = TypedDict(
-    "VariableValueOutputTypeDef",
+VariableValueTypeDef = TypedDict(
+    "VariableValueTypeDef",
     {
         "boolValue": bool,
         "doubleValue": float,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
@@ -579,37 +589,24 @@
 )
 
 
 class LaunchGroupTypeDef(_RequiredLaunchGroupTypeDef, _OptionalLaunchGroupTypeDef):
     pass
 
 
-_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": ExperimentStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListExperimentsRequestListExperimentsPaginateTypeDef(
-    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
-    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExperimentsRequestRequestTypeDef = TypedDict(
     "_RequiredListExperimentsRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListExperimentsRequestRequestTypeDef = TypedDict(
@@ -625,36 +622,14 @@
 
 class ListExperimentsRequestRequestTypeDef(
     _RequiredListExperimentsRequestRequestTypeDef, _OptionalListExperimentsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFeaturesRequestListFeaturesPaginateTypeDef(
-    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
-    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFeaturesRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListFeaturesRequestRequestTypeDef = TypedDict(
@@ -669,37 +644,14 @@
 
 class ListFeaturesRequestRequestTypeDef(
     _RequiredListFeaturesRequestRequestTypeDef, _OptionalListFeaturesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "status": LaunchStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLaunchesRequestListLaunchesPaginateTypeDef(
-    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
-    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLaunchesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListLaunchesRequestRequestTypeDef = TypedDict(
@@ -715,22 +667,14 @@
 
 class ListLaunchesRequestRequestTypeDef(
     _RequiredListLaunchesRequestRequestTypeDef, _OptionalListLaunchesRequestRequestTypeDef
 ):
     pass
 
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -761,37 +705,14 @@
 )
 
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
 
-_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "segment": str,
-        "type": SegmentReferenceResourceTypeType,
-    },
-)
-_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
-    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSegmentReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListSegmentReferencesRequestRequestTypeDef",
     {
         "segment": str,
         "type": SegmentReferenceResourceTypeType,
     },
 )
@@ -832,22 +753,14 @@
 )
 
 
 class RefResourceTypeDef(_RequiredRefResourceTypeDef, _OptionalRefResourceTypeDef):
     pass
 
 
-ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSegmentsRequestRequestTypeDef = TypedDict(
     "ListSegmentsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -856,22 +769,14 @@
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
 _RequiredMetricDefinitionConfigTypeDef = TypedDict(
     "_RequiredMetricDefinitionConfigTypeDef",
     {
         "entityIdKey": str,
         "name": str,
         "valueKey": str,
     },
@@ -900,24 +805,14 @@
         "name": str,
         "unitLabel": str,
         "valueKey": str,
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
 ProjectAppConfigResourceTypeDef = TypedDict(
     "ProjectAppConfigResourceTypeDef",
     {
         "applicationId": str,
         "configurationProfileId": str,
         "environmentId": str,
     },
@@ -947,25 +842,14 @@
         "errorCode": str,
         "errorMessage": str,
         "eventId": str,
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
 SegmentOverrideTypeDef = TypedDict(
     "SegmentOverrideTypeDef",
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
@@ -985,22 +869,14 @@
     {
         "analysisCompleteTime": Union[datetime, str],
         "experiment": str,
         "project": str,
     },
 )
 
-StartExperimentResponseTypeDef = TypedDict(
-    "StartExperimentResponseTypeDef",
-    {
-        "startedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1024,22 +900,14 @@
 
 class StopExperimentRequestRequestTypeDef(
     _RequiredStopExperimentRequestRequestTypeDef, _OptionalStopExperimentRequestRequestTypeDef
 ):
     pass
 
 
-StopExperimentResponseTypeDef = TypedDict(
-    "StopExperimentResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredStopLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1055,22 +923,14 @@
 
 class StopLaunchRequestRequestTypeDef(
     _RequiredStopLaunchRequestRequestTypeDef, _OptionalStopLaunchRequestRequestTypeDef
 ):
     pass
 
 
-StopLaunchResponseTypeDef = TypedDict(
-    "StopLaunchResponseTypeDef",
-    {
-        "endedTime": datetime,
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
@@ -1079,49 +939,70 @@
     "TestSegmentPatternRequestRequestTypeDef",
     {
         "pattern": str,
         "payload": str,
     },
 )
 
-TestSegmentPatternResponseTypeDef = TypedDict(
-    "TestSegmentPatternResponseTypeDef",
-    {
-        "match": bool,
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
 
-VariableValueTypeDef = TypedDict(
-    "VariableValueTypeDef",
-    {
-        "boolValue": bool,
-        "doubleValue": float,
-        "longValue": int,
-        "stringValue": str,
-    },
-    total=False,
-)
-
 BatchEvaluateFeatureRequestRequestTypeDef = TypedDict(
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExperimentResponseTypeDef = TypedDict(
+    "StartExperimentResponseTypeDef",
+    {
+        "startedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopExperimentResponseTypeDef = TypedDict(
+    "StopExperimentResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopLaunchResponseTypeDef = TypedDict(
+    "StopLaunchResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestSegmentPatternResponseTypeDef = TypedDict(
+    "TestSegmentPatternResponseTypeDef",
+    {
+        "match": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1140,43 +1021,43 @@
     pass
 
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentsResponseTypeDef = TypedDict(
     "ListSegmentsResponseTypeDef",
     {
         "nextToken": str,
         "segments": List[SegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
-        "value": VariableValueOutputTypeDef,
+        "value": VariableValueTypeDef,
         "variation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "entityId": str,
@@ -1185,30 +1066,38 @@
 )
 _OptionalEvaluationResultTypeDef = TypedDict(
     "_OptionalEvaluationResultTypeDef",
     {
         "details": str,
         "project": str,
         "reason": str,
-        "value": VariableValueOutputTypeDef,
+        "value": VariableValueTypeDef,
         "variation": str,
     },
     total=False,
 )
 
 
 class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
     pass
 
 
+VariationConfigTypeDef = TypedDict(
+    "VariationConfigTypeDef",
+    {
+        "name": str,
+        "value": VariableValueTypeDef,
+    },
+)
+
 VariationTypeDef = TypedDict(
     "VariationTypeDef",
     {
         "name": str,
-        "value": VariableValueOutputTypeDef,
+        "value": VariableValueTypeDef,
     },
     total=False,
 )
 
 _RequiredFeatureSummaryTypeDef = TypedDict(
     "_RequiredFeatureSummaryTypeDef",
     {
@@ -1247,33 +1136,140 @@
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
         "details": str,
         "reports": List[ExperimentReportTypeDef],
         "resultsData": List[ExperimentResultsDataTypeDef],
         "timestamps": List[datetime],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "status": ExperimentStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExperimentsRequestListExperimentsPaginateTypeDef(
+    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
+    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "project": str,
     },
 )
+_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFeaturesRequestListFeaturesPaginateTypeDef(
+    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
+    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "status": LaunchStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLaunchesRequestListLaunchesPaginateTypeDef(
+    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
+    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
+):
+    pass
+
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "segment": str,
+        "type": SegmentReferenceResourceTypeType,
+    },
+)
+_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
+    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+):
+    pass
+
+
+ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "projects": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentReferencesResponseTypeDef = TypedDict(
     "ListSegmentReferencesResponseTypeDef",
     {
         "nextToken": str,
         "referencedBy": List[RefResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricGoalConfigTypeDef = TypedDict(
     "_RequiredMetricGoalConfigTypeDef",
     {
         "metricDefinition": MetricDefinitionConfigTypeDef,
@@ -1367,15 +1363,15 @@
 )
 
 PutProjectEventsResponseTypeDef = TypedDict(
     "PutProjectEventsResponseTypeDef",
     {
         "eventResults": List[PutProjectEventsResultEntryTypeDef],
         "failedEventCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
@@ -1413,29 +1409,75 @@
 )
 
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
 
 
-VariationConfigTypeDef = TypedDict(
-    "VariationConfigTypeDef",
+BatchEvaluateFeatureResponseTypeDef = TypedDict(
+    "BatchEvaluateFeatureResponseTypeDef",
+    {
+        "results": List[EvaluationResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFeatureRequestRequestTypeDef",
     {
         "name": str,
-        "value": VariableValueTypeDef,
+        "project": str,
+        "variations": Sequence[VariationConfigTypeDef],
     },
 )
+_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFeatureRequestRequestTypeDef",
+    {
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
 
-BatchEvaluateFeatureResponseTypeDef = TypedDict(
-    "BatchEvaluateFeatureResponseTypeDef",
+
+class CreateFeatureRequestRequestTypeDef(
+    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeatureRequestRequestTypeDef",
     {
-        "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "feature": str,
+        "project": str,
     },
 )
+_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeatureRequestRequestTypeDef",
+    {
+        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "removeVariations": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateFeatureRequestRequestTypeDef(
+    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredFeatureTypeDef = TypedDict(
     "_RequiredFeatureTypeDef",
     {
         "arn": str,
         "createdTime": datetime,
         "evaluationStrategy": FeatureEvaluationStrategyType,
@@ -1465,15 +1507,15 @@
 
 
 ListFeaturesResponseTypeDef = TypedDict(
     "ListFeaturesResponseTypeDef",
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
@@ -1632,154 +1674,100 @@
     "ScheduledSplitsLaunchDefinitionTypeDef",
     {
         "steps": List[ScheduledSplitTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFeatureRequestRequestTypeDef",
-    {
-        "name": str,
-        "project": str,
-        "variations": Sequence[VariationConfigTypeDef],
-    },
-)
-_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFeatureRequestRequestTypeDef",
-    {
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateFeatureRequestRequestTypeDef(
-    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFeatureRequestRequestTypeDef",
-    {
-        "feature": str,
-        "project": str,
-    },
-)
-_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFeatureRequestRequestTypeDef",
-    {
-        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "removeVariations": Sequence[str],
-    },
-    total=False,
-)
-
-
-class UpdateFeatureRequestRequestTypeDef(
-    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
-):
-    pass
-
-
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFeatureResponseTypeDef = TypedDict(
     "GetFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFeatureResponseTypeDef = TypedDict(
     "UpdateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExperimentResponseTypeDef = TypedDict(
     "CreateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateExperimentResponseTypeDef = TypedDict(
     "UpdateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectDataDeliveryResponseTypeDef = TypedDict(
     "UpdateProjectDataDeliveryResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResponseTypeDef = TypedDict(
     "UpdateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchRequestRequestTypeDef",
     {
         "groups": Sequence[LaunchGroupConfigTypeDef],
@@ -1864,43 +1852,43 @@
     pass
 
 
 CreateLaunchResponseTypeDef = TypedDict(
     "CreateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchResponseTypeDef = TypedDict(
     "GetLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchesResponseTypeDef = TypedDict(
     "ListLaunchesResponseTypeDef",
     {
         "launches": List[LaunchTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLaunchResponseTypeDef = TypedDict(
     "StartLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchResponseTypeDef = TypedDict(
     "UpdateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently/type_defs.pyi` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "EvaluationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CloudWatchLogsDestinationConfigTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "OnlineAbConfigTypeDef",
     "TreatmentConfigTypeDef",
     "LaunchGroupConfigTypeDef",
     "ProjectAppConfigResourceConfigTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "SegmentTypeDef",
     "DeleteExperimentRequestRequestTypeDef",
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
-    "VariableValueOutputTypeDef",
+    "VariableValueTypeDef",
     "EvaluationRuleTypeDef",
     "EventTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
@@ -69,88 +70,86 @@
     "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
-    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExperimentsRequestRequestTypeDef",
-    "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListFeaturesRequestRequestTypeDef",
-    "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListLaunchesRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentReferencesRequestRequestTypeDef",
     "RefResourceTypeDef",
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListSegmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
     "SegmentOverrideOutputTypeDef",
     "StartExperimentRequestRequestTypeDef",
-    "StartExperimentResponseTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
-    "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
-    "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
-    "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "VariableValueTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartExperimentResponseTypeDef",
+    "StopExperimentResponseTypeDef",
+    "StopLaunchResponseTypeDef",
+    "TestSegmentPatternResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
+    "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
     "PutProjectEventsRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
+    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "ListFeaturesRequestListFeaturesPaginateTypeDef",
+    "ListLaunchesRequestListLaunchesPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
     "MetricMonitorConfigTypeDef",
     "MetricGoalTypeDef",
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
     "UpdateProjectDataDeliveryRequestRequestTypeDef",
     "ProjectDataDeliveryTypeDef",
     "PutProjectEventsResponseTypeDef",
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
-    "VariationConfigTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
+    "CreateFeatureRequestRequestTypeDef",
+    "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
-    "CreateFeatureRequestRequestTypeDef",
-    "UpdateFeatureRequestRequestTypeDef",
     "CreateFeatureResponseTypeDef",
     "GetFeatureResponseTypeDef",
     "UpdateFeatureResponseTypeDef",
     "CreateExperimentResponseTypeDef",
     "GetExperimentResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "UpdateExperimentResponseTypeDef",
@@ -184,14 +183,25 @@
 )
 
 class EvaluationRequestTypeDef(
     _RequiredEvaluationRequestTypeDef, _OptionalEvaluationRequestTypeDef
 ):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 CloudWatchLogsDestinationConfigTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
@@ -362,16 +372,16 @@
 )
 
 class EvaluateFeatureRequestRequestTypeDef(
     _RequiredEvaluateFeatureRequestRequestTypeDef, _OptionalEvaluateFeatureRequestRequestTypeDef
 ):
     pass
 
-VariableValueOutputTypeDef = TypedDict(
-    "VariableValueOutputTypeDef",
+VariableValueTypeDef = TypedDict(
+    "VariableValueTypeDef",
     {
         "boolValue": bool,
         "doubleValue": float,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
@@ -558,35 +568,24 @@
     },
     total=False,
 )
 
 class LaunchGroupTypeDef(_RequiredLaunchGroupTypeDef, _OptionalLaunchGroupTypeDef):
     pass
 
-_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": ExperimentStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListExperimentsRequestListExperimentsPaginateTypeDef(
-    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
-    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExperimentsRequestRequestTypeDef = TypedDict(
     "_RequiredListExperimentsRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListExperimentsRequestRequestTypeDef = TypedDict(
@@ -600,34 +599,14 @@
 )
 
 class ListExperimentsRequestRequestTypeDef(
     _RequiredListExperimentsRequestRequestTypeDef, _OptionalListExperimentsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFeaturesRequestListFeaturesPaginateTypeDef(
-    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
-    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFeaturesRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListFeaturesRequestRequestTypeDef = TypedDict(
@@ -640,35 +619,14 @@
 )
 
 class ListFeaturesRequestRequestTypeDef(
     _RequiredListFeaturesRequestRequestTypeDef, _OptionalListFeaturesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "status": LaunchStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLaunchesRequestListLaunchesPaginateTypeDef(
-    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
-    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
-):
-    pass
-
 _RequiredListLaunchesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListLaunchesRequestRequestTypeDef = TypedDict(
@@ -682,22 +640,14 @@
 )
 
 class ListLaunchesRequestRequestTypeDef(
     _RequiredListLaunchesRequestRequestTypeDef, _OptionalListLaunchesRequestRequestTypeDef
 ):
     pass
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -726,35 +676,14 @@
     },
     total=False,
 )
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
-_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "segment": str,
-        "type": SegmentReferenceResourceTypeType,
-    },
-)
-_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
-    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSegmentReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListSegmentReferencesRequestRequestTypeDef",
     {
         "segment": str,
         "type": SegmentReferenceResourceTypeType,
     },
 )
@@ -791,22 +720,14 @@
     },
     total=False,
 )
 
 class RefResourceTypeDef(_RequiredRefResourceTypeDef, _OptionalRefResourceTypeDef):
     pass
 
-ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSegmentsRequestRequestTypeDef = TypedDict(
     "ListSegmentsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -815,22 +736,14 @@
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
 _RequiredMetricDefinitionConfigTypeDef = TypedDict(
     "_RequiredMetricDefinitionConfigTypeDef",
     {
         "entityIdKey": str,
         "name": str,
         "valueKey": str,
     },
@@ -857,24 +770,14 @@
         "name": str,
         "unitLabel": str,
         "valueKey": str,
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
 ProjectAppConfigResourceTypeDef = TypedDict(
     "ProjectAppConfigResourceTypeDef",
     {
         "applicationId": str,
         "configurationProfileId": str,
         "environmentId": str,
     },
@@ -904,25 +807,14 @@
         "errorCode": str,
         "errorMessage": str,
         "eventId": str,
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
 SegmentOverrideTypeDef = TypedDict(
     "SegmentOverrideTypeDef",
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
@@ -942,22 +834,14 @@
     {
         "analysisCompleteTime": Union[datetime, str],
         "experiment": str,
         "project": str,
     },
 )
 
-StartExperimentResponseTypeDef = TypedDict(
-    "StartExperimentResponseTypeDef",
-    {
-        "startedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -979,22 +863,14 @@
 )
 
 class StopExperimentRequestRequestTypeDef(
     _RequiredStopExperimentRequestRequestTypeDef, _OptionalStopExperimentRequestRequestTypeDef
 ):
     pass
 
-StopExperimentResponseTypeDef = TypedDict(
-    "StopExperimentResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredStopLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1008,22 +884,14 @@
 )
 
 class StopLaunchRequestRequestTypeDef(
     _RequiredStopLaunchRequestRequestTypeDef, _OptionalStopLaunchRequestRequestTypeDef
 ):
     pass
 
-StopLaunchResponseTypeDef = TypedDict(
-    "StopLaunchResponseTypeDef",
-    {
-        "endedTime": datetime,
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
@@ -1032,49 +900,70 @@
     "TestSegmentPatternRequestRequestTypeDef",
     {
         "pattern": str,
         "payload": str,
     },
 )
 
-TestSegmentPatternResponseTypeDef = TypedDict(
-    "TestSegmentPatternResponseTypeDef",
-    {
-        "match": bool,
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
 
-VariableValueTypeDef = TypedDict(
-    "VariableValueTypeDef",
-    {
-        "boolValue": bool,
-        "doubleValue": float,
-        "longValue": int,
-        "stringValue": str,
-    },
-    total=False,
-)
-
 BatchEvaluateFeatureRequestRequestTypeDef = TypedDict(
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExperimentResponseTypeDef = TypedDict(
+    "StartExperimentResponseTypeDef",
+    {
+        "startedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopExperimentResponseTypeDef = TypedDict(
+    "StopExperimentResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopLaunchResponseTypeDef = TypedDict(
+    "StopLaunchResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestSegmentPatternResponseTypeDef = TypedDict(
+    "TestSegmentPatternResponseTypeDef",
+    {
+        "match": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1091,43 +980,43 @@
 ):
     pass
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentsResponseTypeDef = TypedDict(
     "ListSegmentsResponseTypeDef",
     {
         "nextToken": str,
         "segments": List[SegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
-        "value": VariableValueOutputTypeDef,
+        "value": VariableValueTypeDef,
         "variation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "entityId": str,
@@ -1136,28 +1025,36 @@
 )
 _OptionalEvaluationResultTypeDef = TypedDict(
     "_OptionalEvaluationResultTypeDef",
     {
         "details": str,
         "project": str,
         "reason": str,
-        "value": VariableValueOutputTypeDef,
+        "value": VariableValueTypeDef,
         "variation": str,
     },
     total=False,
 )
 
 class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
     pass
 
+VariationConfigTypeDef = TypedDict(
+    "VariationConfigTypeDef",
+    {
+        "name": str,
+        "value": VariableValueTypeDef,
+    },
+)
+
 VariationTypeDef = TypedDict(
     "VariationTypeDef",
     {
         "name": str,
-        "value": VariableValueOutputTypeDef,
+        "value": VariableValueTypeDef,
     },
     total=False,
 )
 
 _RequiredFeatureSummaryTypeDef = TypedDict(
     "_RequiredFeatureSummaryTypeDef",
     {
@@ -1194,33 +1091,132 @@
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
         "details": str,
         "reports": List[ExperimentReportTypeDef],
         "resultsData": List[ExperimentResultsDataTypeDef],
         "timestamps": List[datetime],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "status": ExperimentStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExperimentsRequestListExperimentsPaginateTypeDef(
+    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
+    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFeaturesRequestListFeaturesPaginateTypeDef(
+    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
+    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
+):
+    pass
+
+_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "status": LaunchStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLaunchesRequestListLaunchesPaginateTypeDef(
+    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
+    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
+):
+    pass
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "segment": str,
+        "type": SegmentReferenceResourceTypeType,
+    },
+)
+_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
+    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+):
+    pass
+
+ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "projects": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentReferencesResponseTypeDef = TypedDict(
     "ListSegmentReferencesResponseTypeDef",
     {
         "nextToken": str,
         "referencedBy": List[RefResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricGoalConfigTypeDef = TypedDict(
     "_RequiredMetricGoalConfigTypeDef",
     {
         "metricDefinition": MetricDefinitionConfigTypeDef,
@@ -1308,15 +1304,15 @@
 )
 
 PutProjectEventsResponseTypeDef = TypedDict(
     "PutProjectEventsResponseTypeDef",
     {
         "eventResults": List[PutProjectEventsResultEntryTypeDef],
         "failedEventCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
@@ -1350,30 +1346,72 @@
     },
     total=False,
 )
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
 
-VariationConfigTypeDef = TypedDict(
-    "VariationConfigTypeDef",
+BatchEvaluateFeatureResponseTypeDef = TypedDict(
+    "BatchEvaluateFeatureResponseTypeDef",
+    {
+        "results": List[EvaluationResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFeatureRequestRequestTypeDef",
     {
         "name": str,
-        "value": VariableValueTypeDef,
+        "project": str,
+        "variations": Sequence[VariationConfigTypeDef],
+    },
+)
+_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFeatureRequestRequestTypeDef",
+    {
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
-BatchEvaluateFeatureResponseTypeDef = TypedDict(
-    "BatchEvaluateFeatureResponseTypeDef",
+class CreateFeatureRequestRequestTypeDef(
+    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeatureRequestRequestTypeDef",
     {
-        "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "feature": str,
+        "project": str,
+    },
+)
+_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeatureRequestRequestTypeDef",
+    {
+        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
+        "defaultVariation": str,
+        "description": str,
+        "entityOverrides": Mapping[str, str],
+        "evaluationStrategy": FeatureEvaluationStrategyType,
+        "removeVariations": Sequence[str],
     },
+    total=False,
 )
 
+class UpdateFeatureRequestRequestTypeDef(
+    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
+):
+    pass
+
 _RequiredFeatureTypeDef = TypedDict(
     "_RequiredFeatureTypeDef",
     {
         "arn": str,
         "createdTime": datetime,
         "evaluationStrategy": FeatureEvaluationStrategyType,
         "lastUpdatedTime": datetime,
@@ -1400,15 +1438,15 @@
     pass
 
 ListFeaturesResponseTypeDef = TypedDict(
     "ListFeaturesResponseTypeDef",
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
@@ -1557,150 +1595,100 @@
     "ScheduledSplitsLaunchDefinitionTypeDef",
     {
         "steps": List[ScheduledSplitTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFeatureRequestRequestTypeDef",
-    {
-        "name": str,
-        "project": str,
-        "variations": Sequence[VariationConfigTypeDef],
-    },
-)
-_OptionalCreateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFeatureRequestRequestTypeDef",
-    {
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateFeatureRequestRequestTypeDef(
-    _RequiredCreateFeatureRequestRequestTypeDef, _OptionalCreateFeatureRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFeatureRequestRequestTypeDef",
-    {
-        "feature": str,
-        "project": str,
-    },
-)
-_OptionalUpdateFeatureRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFeatureRequestRequestTypeDef",
-    {
-        "addOrUpdateVariations": Sequence[VariationConfigTypeDef],
-        "defaultVariation": str,
-        "description": str,
-        "entityOverrides": Mapping[str, str],
-        "evaluationStrategy": FeatureEvaluationStrategyType,
-        "removeVariations": Sequence[str],
-    },
-    total=False,
-)
-
-class UpdateFeatureRequestRequestTypeDef(
-    _RequiredUpdateFeatureRequestRequestTypeDef, _OptionalUpdateFeatureRequestRequestTypeDef
-):
-    pass
-
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFeatureResponseTypeDef = TypedDict(
     "GetFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFeatureResponseTypeDef = TypedDict(
     "UpdateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExperimentResponseTypeDef = TypedDict(
     "CreateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateExperimentResponseTypeDef = TypedDict(
     "UpdateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectDataDeliveryResponseTypeDef = TypedDict(
     "UpdateProjectDataDeliveryResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResponseTypeDef = TypedDict(
     "UpdateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchRequestRequestTypeDef",
     {
         "groups": Sequence[LaunchGroupConfigTypeDef],
@@ -1779,43 +1767,43 @@
 class LaunchTypeDef(_RequiredLaunchTypeDef, _OptionalLaunchTypeDef):
     pass
 
 CreateLaunchResponseTypeDef = TypedDict(
     "CreateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchResponseTypeDef = TypedDict(
     "GetLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchesResponseTypeDef = TypedDict(
     "ListLaunchesResponseTypeDef",
     {
         "launches": List[LaunchTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLaunchResponseTypeDef = TypedDict(
     "StartLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchResponseTypeDef = TypedDict(
     "UpdateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/PKG-INFO` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-evidently
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatchEvidently 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatchEvidently 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-evidently.svg?color=blue)](https://pypi.org/project/mypy-boto3-evidently)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-evidently)](https://pepy.tech/project/mypy-boto3-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchEvidently 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[boto3.CloudWatchEvidently 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [mypy-boto3-evidently docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,29 +356,30 @@
 
 `mypy_boto3_evidently.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_evidently.type_defs import (
     EvaluationRequestTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
     SegmentTypeDef,
     DeleteExperimentRequestRequestTypeDef,
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
-    VariableValueOutputTypeDef,
+    VariableValueTypeDef,
     EvaluationRuleTypeDef,
     EventTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
@@ -387,88 +388,86 @@
     GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExperimentsRequestRequestTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
-    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
     SegmentOverrideOutputTypeDef,
     StartExperimentRequestRequestTypeDef,
-    StartExperimentResponseTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
-    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
-    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    VariableValueTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartExperimentResponseTypeDef,
+    StopExperimentResponseTypeDef,
+    StopLaunchResponseTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
+    VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
     PutProjectEventsRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
     UpdateProjectDataDeliveryRequestRequestTypeDef,
     ProjectDataDeliveryTypeDef,
     PutProjectEventsResponseTypeDef,
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
-    VariationConfigTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
+    CreateFeatureRequestRequestTypeDef,
+    UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
-    CreateFeatureRequestRequestTypeDef,
-    UpdateFeatureRequestRequestTypeDef,
     CreateFeatureResponseTypeDef,
     GetFeatureResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     CreateExperimentResponseTypeDef,
     GetExperimentResponseTypeDef,
     ListExperimentsResponseTypeDef,
     UpdateExperimentResponseTypeDef,
```

### Comparing `mypy-boto3-evidently-1.28.12/mypy_boto3_evidently.egg-info/SOURCES.txt` & `mypy-boto3-evidently-1.28.15/mypy_boto3_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-evidently-1.28.12/setup.py` & `mypy-boto3-evidently-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-evidently",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchEvidently 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CloudWatchEvidently 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

