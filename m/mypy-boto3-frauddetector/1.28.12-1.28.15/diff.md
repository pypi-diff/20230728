# Comparing `tmp/mypy-boto3-frauddetector-1.28.12.tar.gz` & `tmp/mypy-boto3-frauddetector-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-frauddetector-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
+gzip compressed data, was "mypy-boto3-frauddetector-1.28.15.tar", last modified: Fri Jul 28 20:42:50 2023, max compression
```

## Comparing `mypy-boto3-frauddetector-1.28.12.tar` & `mypy-boto3-frauddetector-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.968506 mypy-boto3-frauddetector-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-27 05:34:42.964506 mypy-boto3-frauddetector-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.964506 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46336 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63313 2023-07-27 05:22:30.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63238 2023-07-27 05:22:30.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.964506 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:42.000000 mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.968506 mypy-boto3-frauddetector-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:22:28.000000 mypy-boto3-frauddetector-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.197129 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46336 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-28 20:26:08.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60744 2023-07-28 20:26:11.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60673 2023-07-28 20:26:09.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:42:50.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:49.000000 mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:50.209129 mypy-boto3-frauddetector-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:26:07.000000 mypy-boto3-frauddetector-1.28.15/setup.py
```

### Comparing `mypy-boto3-frauddetector-1.28.12/LICENSE` & `mypy-boto3-frauddetector-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.12/PKG-INFO` & `mypy-boto3-frauddetector-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.12
-Summary: Type annotations for boto3.FraudDetector 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,180 +320,171 @@
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
     AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
-    CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
-    CreateModelVersionResultTypeDef,
-    RuleOutputTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
-    DeleteEventsByEventTypeResultTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
-    EntityOutputTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
-    EventOrchestrationOutputTypeDef,
     EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
-    ExternalEventsDetailOutputTypeDef,
     ExternalModelSummaryTypeDef,
-    ModelInputConfigurationOutputTypeDef,
+    ModelInputConfigurationTypeDef,
     ModelOutputConfigurationOutputTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
-    GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
-    ModelVersionOutputTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
     GetListElementsRequestRequestTypeDef,
-    GetListElementsResultTypeDef,
     GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
     GetVariablesRequestRequestTypeDef,
-    IngestedEventsTimeWindowOutputTypeDef,
     IngestedEventsTimeWindowTypeDef,
     LabelSchemaOutputTypeDef,
     LabelSchemaTypeDef,
     PredictionTimeRangeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
-    ModelInputConfigurationTypeDef,
     ModelOutputConfigurationTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
     UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelVersionResultTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
-    GetListsMetadataResultTypeDef,
-    BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
+    BatchCreateVariableResultTypeDef,
+    CreateDetectorVersionResultTypeDef,
+    CreateModelVersionResultTypeDef,
+    DeleteEventsByEventTypeResultTypeDef,
+    GetDeleteEventsByEventTypeStatusResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
+    ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
+    CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
+    GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
     UpdateRuleVersionRequestRequestTypeDef,
-    CreateRuleResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    GetDetectorVersionResultTypeDef,
-    ModelScoresTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
-    IngestedEventsDetailOutputTypeDef,
     IngestedEventsDetailTypeDef,
     TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
     PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
-    GetExternalModelsResultTypeDef,
     GetEventPredictionResultTypeDef,
+    GetExternalModelsResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
     CreateModelVersionRequestRequestTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.28.12/README.md` & `mypy-boto3-frauddetector-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,180 +288,171 @@
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
     AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
-    CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
-    CreateModelVersionResultTypeDef,
-    RuleOutputTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
-    DeleteEventsByEventTypeResultTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
-    EntityOutputTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
-    EventOrchestrationOutputTypeDef,
     EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
-    ExternalEventsDetailOutputTypeDef,
     ExternalModelSummaryTypeDef,
-    ModelInputConfigurationOutputTypeDef,
+    ModelInputConfigurationTypeDef,
     ModelOutputConfigurationOutputTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
-    GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
-    ModelVersionOutputTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
     GetListElementsRequestRequestTypeDef,
-    GetListElementsResultTypeDef,
     GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
     GetVariablesRequestRequestTypeDef,
-    IngestedEventsTimeWindowOutputTypeDef,
     IngestedEventsTimeWindowTypeDef,
     LabelSchemaOutputTypeDef,
     LabelSchemaTypeDef,
     PredictionTimeRangeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
-    ModelInputConfigurationTypeDef,
     ModelOutputConfigurationTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
     UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelVersionResultTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
-    GetListsMetadataResultTypeDef,
-    BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
+    BatchCreateVariableResultTypeDef,
+    CreateDetectorVersionResultTypeDef,
+    CreateModelVersionResultTypeDef,
+    DeleteEventsByEventTypeResultTypeDef,
+    GetDeleteEventsByEventTypeStatusResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
+    ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
+    CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
+    GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
     UpdateRuleVersionRequestRequestTypeDef,
-    CreateRuleResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    GetDetectorVersionResultTypeDef,
-    ModelScoresTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
-    IngestedEventsDetailOutputTypeDef,
     IngestedEventsDetailTypeDef,
     TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
     PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
-    GetExternalModelsResultTypeDef,
     GetEventPredictionResultTypeDef,
+    GetExternalModelsResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
     CreateModelVersionRequestRequestTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/__main__.py` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FraudDetector 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.FraudDetector 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
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

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.py` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/client.pyi` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.py` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/literals.pyi` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.py` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -38,190 +38,180 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ATIMetricDataPointTypeDef",
     "ATIModelPerformanceTypeDef",
     "AggregatedLogOddsMetricTypeDef",
     "AggregatedVariablesImpactExplanationTypeDef",
     "AllowDenyListTypeDef",
     "BatchCreateVariableErrorTypeDef",
     "TagTypeDef",
     "VariableEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
     "BatchImportTypeDef",
     "BatchPredictionTypeDef",
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
-    "CreateDetectorVersionResultTypeDef",
     "ExternalEventsDetailTypeDef",
-    "CreateModelVersionResultTypeDef",
-    "RuleOutputTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
     "DeleteBatchImportJobRequestRequestTypeDef",
     "DeleteBatchPredictionJobRequestRequestTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
     "DeleteEventRequestRequestTypeDef",
     "DeleteEventTypeRequestRequestTypeDef",
     "DeleteEventsByEventTypeRequestRequestTypeDef",
-    "DeleteEventsByEventTypeResultTypeDef",
     "DeleteExternalModelRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteListRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
     "DescribeDetectorRequestRequestTypeDef",
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
     "DetectorTypeDef",
-    "EntityOutputTypeDef",
     "EntityTypeDef",
     "EntityTypeTypeDef",
     "EvaluatedExternalModelTypeDef",
     "EvaluatedRuleTypeDef",
-    "EventOrchestrationOutputTypeDef",
     "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
-    "ExternalEventsDetailOutputTypeDef",
     "ExternalModelSummaryTypeDef",
-    "ModelInputConfigurationOutputTypeDef",
+    "ModelInputConfigurationTypeDef",
     "ModelOutputConfigurationOutputTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
-    "ModelVersionOutputTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
     "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
     "GetListElementsRequestRequestTypeDef",
-    "GetListElementsResultTypeDef",
     "GetListsMetadataRequestRequestTypeDef",
     "GetModelVersionRequestRequestTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
     "GetVariablesRequestRequestTypeDef",
-    "IngestedEventsTimeWindowOutputTypeDef",
     "IngestedEventsTimeWindowTypeDef",
     "LabelSchemaOutputTypeDef",
     "LabelSchemaTypeDef",
     "PredictionTimeRangeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
-    "ModelInputConfigurationTypeDef",
     "ModelOutputConfigurationTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
     "UpdateDetectorVersionStatusRequestRequestTypeDef",
     "UpdateEventLabelRequestRequestTypeDef",
     "UpdateListRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelVersionResultTypeDef",
     "UpdateModelVersionStatusRequestRequestTypeDef",
     "UpdateVariableRequestRequestTypeDef",
     "ATITrainingMetricsValueTypeDef",
     "AggregatedVariablesImportanceMetricsTypeDef",
-    "GetListsMetadataResultTypeDef",
-    "BatchCreateVariableResultTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
     "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
     "PutOutcomeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
+    "BatchCreateVariableResultTypeDef",
+    "CreateDetectorVersionResultTypeDef",
+    "CreateModelVersionResultTypeDef",
+    "DeleteEventsByEventTypeResultTypeDef",
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    "GetListElementsResultTypeDef",
+    "GetListsMetadataResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
+    "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
+    "CreateRuleResultTypeDef",
     "DeleteRuleRequestRequestTypeDef",
+    "GetDetectorVersionResultTypeDef",
     "UpdateDetectorVersionRequestRequestTypeDef",
     "UpdateRuleMetadataRequestRequestTypeDef",
     "UpdateRuleVersionRequestRequestTypeDef",
-    "CreateRuleResultTypeDef",
     "UpdateRuleVersionResultTypeDef",
     "DataValidationMetricsTypeDef",
     "DescribeDetectorResultTypeDef",
     "GetDetectorsResultTypeDef",
     "EventTypeDef",
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
-    "GetDetectorVersionResultTypeDef",
-    "ModelScoresTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
-    "IngestedEventsDetailOutputTypeDef",
     "IngestedEventsDetailTypeDef",
     "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
     "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
-    "GetExternalModelsResultTypeDef",
     "GetEventPredictionResultTypeDef",
+    "GetExternalModelsResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
     "GetModelVersionResultTypeDef",
     "CreateModelVersionRequestRequestTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
@@ -284,19 +274,17 @@
         "createdTime": str,
         "updatedTime": str,
         "arn": str,
     },
     total=False,
 )
 
-
 class AllowDenyListTypeDef(_RequiredAllowDenyListTypeDef, _OptionalAllowDenyListTypeDef):
     pass
 
-
 BatchCreateVariableErrorTypeDef = TypedDict(
     "BatchCreateVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -320,14 +308,25 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
 )
 
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
 BatchGetVariableErrorTypeDef = TypedDict(
     "BatchGetVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -425,66 +424,34 @@
     "_OptionalModelVersionTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
-
 class ModelVersionTypeDef(_RequiredModelVersionTypeDef, _OptionalModelVersionTypeDef):
     pass
 
-
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "detectorId": str,
         "ruleId": str,
         "ruleVersion": str,
     },
 )
 
-CreateDetectorVersionResultTypeDef = TypedDict(
-    "CreateDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "status": DetectorVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExternalEventsDetailTypeDef = TypedDict(
     "ExternalEventsDetailTypeDef",
     {
         "dataLocation": str,
         "dataAccessRoleArn": str,
     },
 )
 
-CreateModelVersionResultTypeDef = TypedDict(
-    "CreateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "detectorId": str,
-        "ruleId": str,
-        "ruleVersion": str,
-    },
-)
-
 FieldValidationMessageTypeDef = TypedDict(
     "FieldValidationMessageTypeDef",
     {
         "fieldName": str,
         "identifier": str,
         "title": str,
         "content": str,
@@ -550,44 +517,33 @@
     "_OptionalDeleteEventRequestRequestTypeDef",
     {
         "deleteAuditHistory": bool,
     },
     total=False,
 )
 
-
 class DeleteEventRequestRequestTypeDef(
     _RequiredDeleteEventRequestRequestTypeDef, _OptionalDeleteEventRequestRequestTypeDef
 ):
     pass
 
-
 DeleteEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
 DeleteEventsByEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventsByEventTypeRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
-DeleteEventsByEventTypeResultTypeDef = TypedDict(
-    "DeleteEventsByEventTypeResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteExternalModelRequestRequestTypeDef = TypedDict(
     "DeleteExternalModelRequestRequestTypeDef",
     {
         "modelEndpoint": str,
     },
 )
 
@@ -647,21 +603,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeDetectorRequestRequestTypeDef(
     _RequiredDescribeDetectorRequestRequestTypeDef, _OptionalDescribeDetectorRequestRequestTypeDef
 ):
     pass
 
-
 DetectorVersionSummaryTypeDef = TypedDict(
     "DetectorVersionSummaryTypeDef",
     {
         "detectorVersionId": str,
         "status": DetectorVersionStatusType,
         "description": str,
         "lastUpdatedTime": str,
@@ -690,22 +644,14 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-EntityOutputTypeDef = TypedDict(
-    "EntityOutputTypeDef",
-    {
-        "entityType": str,
-        "entityId": str,
-    },
-)
-
 EntityTypeDef = TypedDict(
     "EntityTypeDef",
     {
         "entityType": str,
         "entityId": str,
     },
 )
@@ -743,21 +689,14 @@
         "outcomes": List[str],
         "evaluated": bool,
         "matched": bool,
     },
     total=False,
 )
 
-EventOrchestrationOutputTypeDef = TypedDict(
-    "EventOrchestrationOutputTypeDef",
-    {
-        "eventBridgeEnabled": bool,
-    },
-)
-
 EventOrchestrationTypeDef = TypedDict(
     "EventOrchestrationTypeDef",
     {
         "eventBridgeEnabled": bool,
     },
 )
 
@@ -792,55 +731,45 @@
         "name": str,
         "value": str,
         "source": str,
     },
     total=False,
 )
 
-ExternalEventsDetailOutputTypeDef = TypedDict(
-    "ExternalEventsDetailOutputTypeDef",
-    {
-        "dataLocation": str,
-        "dataAccessRoleArn": str,
-    },
-)
-
 ExternalModelSummaryTypeDef = TypedDict(
     "ExternalModelSummaryTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
     },
     total=False,
 )
 
-_RequiredModelInputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredModelInputConfigurationOutputTypeDef",
+_RequiredModelInputConfigurationTypeDef = TypedDict(
+    "_RequiredModelInputConfigurationTypeDef",
     {
         "useEventVariables": bool,
     },
 )
-_OptionalModelInputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalModelInputConfigurationOutputTypeDef",
+_OptionalModelInputConfigurationTypeDef = TypedDict(
+    "_OptionalModelInputConfigurationTypeDef",
     {
         "eventTypeName": str,
         "format": ModelInputDataFormatType,
         "jsonInputTemplate": str,
         "csvInputTemplate": str,
     },
     total=False,
 )
 
-
-class ModelInputConfigurationOutputTypeDef(
-    _RequiredModelInputConfigurationOutputTypeDef, _OptionalModelInputConfigurationOutputTypeDef
+class ModelInputConfigurationTypeDef(
+    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
 ):
     pass
 
-
 _RequiredModelOutputConfigurationOutputTypeDef = TypedDict(
     "_RequiredModelOutputConfigurationOutputTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
 _OptionalModelOutputConfigurationOutputTypeDef = TypedDict(
@@ -848,21 +777,19 @@
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
-
 class ModelOutputConfigurationOutputTypeDef(
     _RequiredModelOutputConfigurationOutputTypeDef, _OptionalModelOutputConfigurationOutputTypeDef
 ):
     pass
 
-
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "value": str,
     },
     total=False,
 )
@@ -890,54 +817,22 @@
 GetDeleteEventsByEventTypeStatusRequestRequestTypeDef = TypedDict(
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
-GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": AsyncJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDetectorVersionRequestRequestTypeDef = TypedDict(
     "GetDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
     },
 )
 
-_RequiredModelVersionOutputTypeDef = TypedDict(
-    "_RequiredModelVersionOutputTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-    },
-)
-_OptionalModelVersionOutputTypeDef = TypedDict(
-    "_OptionalModelVersionOutputTypeDef",
-    {
-        "arn": str,
-    },
-    total=False,
-)
-
-
-class ModelVersionOutputTypeDef(
-    _RequiredModelVersionOutputTypeDef, _OptionalModelVersionOutputTypeDef
-):
-    pass
-
-
 GetDetectorsRequestRequestTypeDef = TypedDict(
     "GetDetectorsRequestRequestTypeDef",
     {
         "detectorId": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1052,30 +947,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetListElementsRequestRequestTypeDef(
     _RequiredGetListElementsRequestRequestTypeDef, _OptionalGetListElementsRequestRequestTypeDef
 ):
     pass
 
-
-GetListElementsResultTypeDef = TypedDict(
-    "GetListElementsResultTypeDef",
-    {
-        "elements": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetListsMetadataRequestRequestTypeDef = TypedDict(
     "GetListsMetadataRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1151,21 +1035,19 @@
         "ruleVersion": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetRulesRequestRequestTypeDef(
     _RequiredGetRulesRequestRequestTypeDef, _OptionalGetRulesRequestRequestTypeDef
 ):
     pass
 
-
 RuleDetailTypeDef = TypedDict(
     "RuleDetailTypeDef",
     {
         "ruleId": str,
         "description": str,
         "detectorId": str,
         "ruleVersion": str,
@@ -1185,22 +1067,14 @@
         "name": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-IngestedEventsTimeWindowOutputTypeDef = TypedDict(
-    "IngestedEventsTimeWindowOutputTypeDef",
-    {
-        "startTime": str,
-        "endTime": str,
-    },
-)
-
 IngestedEventsTimeWindowTypeDef = TypedDict(
     "IngestedEventsTimeWindowTypeDef",
     {
         "startTime": str,
         "endTime": str,
     },
 )
@@ -1242,30 +1116,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 LogOddsMetricTypeDef = TypedDict(
     "LogOddsMetricTypeDef",
     {
         "variableName": str,
         "variableType": str,
         "variableImportance": float,
     },
@@ -1278,38 +1142,14 @@
         "precision": float,
         "tpr": float,
         "threshold": float,
     },
     total=False,
 )
 
-_RequiredModelInputConfigurationTypeDef = TypedDict(
-    "_RequiredModelInputConfigurationTypeDef",
-    {
-        "useEventVariables": bool,
-    },
-)
-_OptionalModelInputConfigurationTypeDef = TypedDict(
-    "_OptionalModelInputConfigurationTypeDef",
-    {
-        "eventTypeName": str,
-        "format": ModelInputDataFormatType,
-        "jsonInputTemplate": str,
-        "csvInputTemplate": str,
-    },
-    total=False,
-)
-
-
-class ModelInputConfigurationTypeDef(
-    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
-):
-    pass
-
-
 _RequiredModelOutputConfigurationTypeDef = TypedDict(
     "_RequiredModelOutputConfigurationTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
 _OptionalModelOutputConfigurationTypeDef = TypedDict(
@@ -1317,21 +1157,19 @@
     {
         "jsonKeyToVariableMap": Mapping[str, str],
         "csvIndexToVariableMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ModelOutputConfigurationTypeDef(
     _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
 ):
     pass
 
-
 OFIMetricDataPointTypeDef = TypedDict(
     "OFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1360,25 +1198,14 @@
 PutKMSEncryptionKeyRequestRequestTypeDef = TypedDict(
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     {
         "kmsEncryptionKeyArn": str,
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
 TFIMetricDataPointTypeDef = TypedDict(
     "TFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1435,21 +1262,19 @@
         "description": str,
         "updateMode": ListUpdateModeType,
         "variableType": str,
     },
     total=False,
 )
 
-
 class UpdateListRequestRequestTypeDef(
     _RequiredUpdateListRequestRequestTypeDef, _OptionalUpdateListRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
     },
 )
@@ -1457,32 +1282,19 @@
     "_OptionalUpdateModelRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
-
-UpdateModelVersionResultTypeDef = TypedDict(
-    "UpdateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateModelVersionStatusRequestRequestTypeDef = TypedDict(
     "UpdateModelVersionStatusRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": ModelVersionStatusType,
@@ -1501,21 +1313,19 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
 )
 
-
 class UpdateVariableRequestRequestTypeDef(
     _RequiredUpdateVariableRequestRequestTypeDef, _OptionalUpdateVariableRequestRequestTypeDef
 ):
     pass
 
-
 ATITrainingMetricsValueTypeDef = TypedDict(
     "ATITrainingMetricsValueTypeDef",
     {
         "metricDataPoints": List[ATIMetricDataPointTypeDef],
         "modelPerformance": ATIModelPerformanceTypeDef,
     },
     total=False,
@@ -1525,31 +1335,14 @@
     "AggregatedVariablesImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[AggregatedLogOddsMetricTypeDef],
     },
     total=False,
 )
 
-GetListsMetadataResultTypeDef = TypedDict(
-    "GetListsMetadataResultTypeDef",
-    {
-        "lists": List[AllowDenyListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchCreateVariableResultTypeDef = TypedDict(
-    "BatchCreateVariableResultTypeDef",
-    {
-        "errors": List[BatchCreateVariableErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBatchImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchImportJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1560,22 +1353,20 @@
     "_OptionalCreateBatchImportJobRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBatchImportJobRequestRequestTypeDef(
     _RequiredCreateBatchImportJobRequestRequestTypeDef,
     _OptionalCreateBatchImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateBatchPredictionJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchPredictionJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1588,22 +1379,20 @@
     {
         "detectorVersion": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBatchPredictionJobRequestRequestTypeDef(
     _RequiredCreateBatchPredictionJobRequestRequestTypeDef,
     _OptionalCreateBatchPredictionJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateListRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateListRequestRequestTypeDef = TypedDict(
@@ -1613,21 +1402,19 @@
         "variableType": str,
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateListRequestRequestTypeDef(
     _RequiredCreateListRequestRequestTypeDef, _OptionalCreateListRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "eventTypeName": str,
     },
@@ -1637,21 +1424,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleRequestRequestTypeDef",
     {
         "ruleId": str,
         "detectorId": str,
         "expression": str,
         "language": Literal["DETECTORPL"],
@@ -1663,21 +1448,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVariableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVariableRequestRequestTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "dataSource": DataSourceType,
         "defaultValue": str,
@@ -1689,21 +1472,19 @@
         "description": str,
         "variableType": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1712,21 +1493,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutDetectorRequestRequestTypeDef(
     _RequiredPutDetectorRequestRequestTypeDef, _OptionalPutDetectorRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEntityTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutEntityTypeRequestRequestTypeDef = TypedDict(
@@ -1734,21 +1513,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutEntityTypeRequestRequestTypeDef(
     _RequiredPutEntityTypeRequestRequestTypeDef, _OptionalPutEntityTypeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutLabelRequestRequestTypeDef = TypedDict(
     "_RequiredPutLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutLabelRequestRequestTypeDef = TypedDict(
@@ -1756,21 +1533,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutLabelRequestRequestTypeDef(
     _RequiredPutLabelRequestRequestTypeDef, _OptionalPutLabelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutOutcomeRequestRequestTypeDef = TypedDict(
     "_RequiredPutOutcomeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutOutcomeRequestRequestTypeDef = TypedDict(
@@ -1778,21 +1553,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutOutcomeRequestRequestTypeDef(
     _RequiredPutOutcomeRequestRequestTypeDef, _OptionalPutOutcomeRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1807,58 +1580,150 @@
     "_OptionalBatchCreateVariableRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class BatchCreateVariableRequestRequestTypeDef(
     _RequiredBatchCreateVariableRequestRequestTypeDef,
     _OptionalBatchCreateVariableRequestRequestTypeDef,
 ):
     pass
 
+BatchCreateVariableResultTypeDef = TypedDict(
+    "BatchCreateVariableResultTypeDef",
+    {
+        "errors": List[BatchCreateVariableErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDetectorVersionResultTypeDef = TypedDict(
+    "CreateDetectorVersionResultTypeDef",
+    {
+        "detectorId": str,
+        "detectorVersionId": str,
+        "status": DetectorVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelVersionResultTypeDef = TypedDict(
+    "CreateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEventsByEventTypeResultTypeDef = TypedDict(
+    "DeleteEventsByEventTypeResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": AsyncJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetListElementsResultTypeDef = TypedDict(
+    "GetListElementsResultTypeDef",
+    {
+        "elements": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetListsMetadataResultTypeDef = TypedDict(
+    "GetListsMetadataResultTypeDef",
+    {
+        "lists": List[AllowDenyListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelVersionResultTypeDef = TypedDict(
+    "UpdateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 BatchGetVariableResultTypeDef = TypedDict(
     "BatchGetVariableResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "errors": List[BatchGetVariableErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariablesResultTypeDef = TypedDict(
     "GetVariablesResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBatchImportJobsResultTypeDef = TypedDict(
     "GetBatchImportJobsResultTypeDef",
     {
         "batchImports": List[BatchImportTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBatchPredictionJobsResultTypeDef = TypedDict(
     "GetBatchPredictionJobsResultTypeDef",
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ModelScoresTypeDef = TypedDict(
+    "ModelScoresTypeDef",
+    {
+        "modelVersion": ModelVersionTypeDef,
+        "scores": Dict[str, float],
+    },
+    total=False,
+)
+
 _RequiredCreateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "rules": Sequence[RuleTypeDef],
     },
 )
@@ -1870,29 +1735,53 @@
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDetectorVersionRequestRequestTypeDef(
     _RequiredCreateDetectorVersionRequestRequestTypeDef,
     _OptionalCreateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
+CreateRuleResultTypeDef = TypedDict(
+    "CreateRuleResultTypeDef",
+    {
+        "rule": RuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
     },
 )
 
+GetDetectorVersionResultTypeDef = TypedDict(
+    "GetDetectorVersionResultTypeDef",
+    {
+        "detectorId": str,
+        "detectorVersionId": str,
+        "description": str,
+        "externalModelEndpoints": List[str],
+        "modelVersions": List[ModelVersionTypeDef],
+        "rules": List[RuleTypeDef],
+        "status": DetectorVersionStatusType,
+        "lastUpdatedTime": str,
+        "createdTime": str,
+        "ruleExecutionMode": RuleExecutionModeType,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
         "externalModelEndpoints": Sequence[str],
         "rules": Sequence[RuleTypeDef],
@@ -1904,22 +1793,20 @@
         "description": str,
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
     },
     total=False,
 )
 
-
 class UpdateDetectorVersionRequestRequestTypeDef(
     _RequiredUpdateDetectorVersionRequestRequestTypeDef,
     _OptionalUpdateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateRuleMetadataRequestRequestTypeDef = TypedDict(
     "UpdateRuleMetadataRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
         "description": str,
     },
 )
@@ -1938,34 +1825,24 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateRuleVersionRequestRequestTypeDef(
     _RequiredUpdateRuleVersionRequestRequestTypeDef, _OptionalUpdateRuleVersionRequestRequestTypeDef
 ):
     pass
 
-
-CreateRuleResultTypeDef = TypedDict(
-    "CreateRuleResultTypeDef",
-    {
-        "rule": RuleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
-        "rule": RuleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "rule": RuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataValidationMetricsTypeDef = TypedDict(
     "DataValidationMetricsTypeDef",
     {
         "fileLevelMessages": List[FileValidationMessageTypeDef],
@@ -1977,37 +1854,37 @@
 DescribeDetectorResultTypeDef = TypedDict(
     "DescribeDetectorResultTypeDef",
     {
         "detectorId": str,
         "detectorVersionSummaries": List[DetectorVersionSummaryTypeDef],
         "nextToken": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDetectorsResultTypeDef = TypedDict(
     "GetDetectorsResultTypeDef",
     {
         "detectors": List[DetectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "eventId": str,
         "eventTypeName": str,
         "eventTimestamp": str,
         "eventVariables": Dict[str, str],
         "currentLabel": str,
         "labelTimestamp": str,
-        "entities": List[EntityOutputTypeDef],
+        "entities": List[EntityTypeDef],
     },
     total=False,
 )
 
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
@@ -2023,27 +1900,25 @@
     {
         "assignedLabel": str,
         "labelTimestamp": str,
     },
     total=False,
 )
 
-
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
-
 GetEntityTypesResultTypeDef = TypedDict(
     "GetEntityTypesResultTypeDef",
     {
         "entityTypes": List[EntityTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventTypeRequestRequestTypeDef",
     {
         "name": str,
@@ -2059,27 +1934,25 @@
         "eventIngestion": EventIngestionType,
         "tags": Sequence[TagTypeDef],
         "eventOrchestration": EventOrchestrationTypeDef,
     },
     total=False,
 )
 
-
 class PutEventTypeRequestRequestTypeDef(
     _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
 ):
     pass
 
-
 ListEventPredictionsResultTypeDef = TypedDict(
     "ListEventPredictionsResultTypeDef",
     {
         "eventPredictionSummaries": List[EventPredictionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeTypeDef = TypedDict(
     "EventTypeTypeDef",
     {
         "name": str,
@@ -2088,15 +1961,15 @@
         "labels": List[str],
         "entityTypes": List[str],
         "eventIngestion": EventIngestionType,
         "ingestedEventStatistics": IngestedEventStatisticsTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
-        "eventOrchestration": EventOrchestrationOutputTypeDef,
+        "eventOrchestration": EventOrchestrationTypeDef,
     },
     total=False,
 )
 
 ExternalModelOutputsTypeDef = TypedDict(
     "ExternalModelOutputsTypeDef",
     {
@@ -2108,51 +1981,24 @@
 
 ExternalModelTypeDef = TypedDict(
     "ExternalModelTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationOutputTypeDef,
+        "inputConfiguration": ModelInputConfigurationTypeDef,
         "outputConfiguration": ModelOutputConfigurationOutputTypeDef,
         "modelEndpointStatus": ModelEndpointStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-GetDetectorVersionResultTypeDef = TypedDict(
-    "GetDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "description": str,
-        "externalModelEndpoints": List[str],
-        "modelVersions": List[ModelVersionOutputTypeDef],
-        "rules": List[RuleOutputTypeDef],
-        "status": DetectorVersionStatusType,
-        "lastUpdatedTime": str,
-        "createdTime": str,
-        "ruleExecutionMode": RuleExecutionModeType,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModelScoresTypeDef = TypedDict(
-    "ModelScoresTypeDef",
-    {
-        "modelVersion": ModelVersionOutputTypeDef,
-        "scores": Dict[str, float],
-    },
-    total=False,
-)
-
 _RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
     "_RequiredGetEventPredictionRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventId": str,
         "eventTypeName": str,
         "entities": Sequence[EntityTypeDef],
@@ -2165,70 +2011,61 @@
     {
         "detectorVersionId": str,
         "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
     },
     total=False,
 )
 
-
 class GetEventPredictionRequestRequestTypeDef(
     _RequiredGetEventPredictionRequestRequestTypeDef,
     _OptionalGetEventPredictionRequestRequestTypeDef,
 ):
     pass
 
-
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLabelsResultTypeDef = TypedDict(
     "GetLabelsResultTypeDef",
     {
         "labels": List[LabelTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResultTypeDef = TypedDict(
     "GetModelsResultTypeDef",
     {
         "nextToken": str,
         "models": List[ModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOutcomesResultTypeDef = TypedDict(
     "GetOutcomesResultTypeDef",
     {
         "outcomes": List[OutcomeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRulesResultTypeDef = TypedDict(
     "GetRulesResultTypeDef",
     {
         "ruleDetails": List[RuleDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IngestedEventsDetailOutputTypeDef = TypedDict(
-    "IngestedEventsDetailOutputTypeDef",
-    {
-        "ingestedEventsTimeWindow": IngestedEventsTimeWindowOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
@@ -2245,65 +2082,52 @@
     "_OptionalTrainingDataSchemaOutputTypeDef",
     {
         "labelSchema": LabelSchemaOutputTypeDef,
     },
     total=False,
 )
 
-
 class TrainingDataSchemaOutputTypeDef(
     _RequiredTrainingDataSchemaOutputTypeDef, _OptionalTrainingDataSchemaOutputTypeDef
 ):
     pass
 
-
 _RequiredTrainingDataSchemaTypeDef = TypedDict(
     "_RequiredTrainingDataSchemaTypeDef",
     {
         "modelVariables": Sequence[str],
     },
 )
 _OptionalTrainingDataSchemaTypeDef = TypedDict(
     "_OptionalTrainingDataSchemaTypeDef",
     {
         "labelSchema": LabelSchemaTypeDef,
     },
     total=False,
 )
 
-
 class TrainingDataSchemaTypeDef(
     _RequiredTrainingDataSchemaTypeDef, _OptionalTrainingDataSchemaTypeDef
 ):
     pass
 
-
 ListEventPredictionsRequestRequestTypeDef = TypedDict(
     "ListEventPredictionsRequestRequestTypeDef",
     {
         "eventId": FilterConditionTypeDef,
         "eventType": FilterConditionTypeDef,
         "detectorId": FilterConditionTypeDef,
         "detectorVersionId": FilterConditionTypeDef,
         "predictionTimeRange": PredictionTimeRangeTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VariableImportanceMetricsTypeDef = TypedDict(
     "VariableImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[LogOddsMetricTypeDef],
     },
     total=False,
 )
@@ -2332,21 +2156,19 @@
     "_OptionalPutExternalModelRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutExternalModelRequestRequestTypeDef(
     _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
 ):
     pass
 
-
 OFIModelPerformanceTypeDef = TypedDict(
     "OFIModelPerformanceTypeDef",
     {
         "auc": float,
         "uncertaintyRange": UncertaintyRangeTypeDef,
     },
     total=False,
@@ -2370,43 +2192,43 @@
     total=False,
 )
 
 GetEventResultTypeDef = TypedDict(
     "GetEventResultTypeDef",
     {
         "event": EventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventTypesResultTypeDef = TypedDict(
     "GetEventTypesResultTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetExternalModelsResultTypeDef = TypedDict(
-    "GetExternalModelsResultTypeDef",
-    {
-        "externalModels": List[ExternalModelTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventPredictionResultTypeDef = TypedDict(
     "GetEventPredictionResultTypeDef",
     {
         "modelScores": List[ModelScoresTypeDef],
         "ruleResults": List[RuleResultTypeDef],
         "externalModelOutputs": List[ExternalModelOutputsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetExternalModelsResultTypeDef = TypedDict(
+    "GetExternalModelsResultTypeDef",
+    {
+        "externalModels": List[ExternalModelTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
@@ -2420,35 +2242,33 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetModelVersionResultTypeDef = TypedDict(
     "GetModelVersionResultTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
-        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "status": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
@@ -2463,22 +2283,20 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
-
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
@@ -2559,39 +2377,39 @@
         "eventVariables": List[EventVariableSummaryTypeDef],
         "rules": List[EvaluatedRuleTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "outcomes": List[str],
         "evaluatedModelVersions": List[EvaluatedModelVersionTypeDef],
         "evaluatedExternalModels": List[EvaluatedExternalModelTypeDef],
         "predictionTimestamp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelVersionDetailTypeDef = TypedDict(
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
-        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "trainingResult": TrainingResultTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
         "trainingResultV2": TrainingResultV2TypeDef,
     },
     total=False,
 )
 
 DescribeModelVersionsResultTypeDef = TypedDict(
     "DescribeModelVersionsResultTypeDef",
     {
         "modelVersionDetails": List[ModelVersionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector/type_defs.pyi` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,189 +38,181 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ATIMetricDataPointTypeDef",
     "ATIModelPerformanceTypeDef",
     "AggregatedLogOddsMetricTypeDef",
     "AggregatedVariablesImpactExplanationTypeDef",
     "AllowDenyListTypeDef",
     "BatchCreateVariableErrorTypeDef",
     "TagTypeDef",
     "VariableEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
     "BatchImportTypeDef",
     "BatchPredictionTypeDef",
     "CancelBatchImportJobRequestRequestTypeDef",
     "CancelBatchPredictionJobRequestRequestTypeDef",
     "ModelVersionTypeDef",
     "RuleTypeDef",
-    "CreateDetectorVersionResultTypeDef",
     "ExternalEventsDetailTypeDef",
-    "CreateModelVersionResultTypeDef",
-    "RuleOutputTypeDef",
     "FieldValidationMessageTypeDef",
     "FileValidationMessageTypeDef",
     "DeleteBatchImportJobRequestRequestTypeDef",
     "DeleteBatchPredictionJobRequestRequestTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
     "DeleteEventRequestRequestTypeDef",
     "DeleteEventTypeRequestRequestTypeDef",
     "DeleteEventsByEventTypeRequestRequestTypeDef",
-    "DeleteEventsByEventTypeResultTypeDef",
     "DeleteExternalModelRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteListRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
     "DescribeDetectorRequestRequestTypeDef",
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
     "DetectorTypeDef",
-    "EntityOutputTypeDef",
     "EntityTypeDef",
     "EntityTypeTypeDef",
     "EvaluatedExternalModelTypeDef",
     "EvaluatedRuleTypeDef",
-    "EventOrchestrationOutputTypeDef",
     "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
-    "ExternalEventsDetailOutputTypeDef",
     "ExternalModelSummaryTypeDef",
-    "ModelInputConfigurationOutputTypeDef",
+    "ModelInputConfigurationTypeDef",
     "ModelOutputConfigurationOutputTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
-    "ModelVersionOutputTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
     "GetEventPredictionMetadataRequestRequestTypeDef",
     "ModelEndpointDataBlobTypeDef",
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
     "GetListElementsRequestRequestTypeDef",
-    "GetListElementsResultTypeDef",
     "GetListsMetadataRequestRequestTypeDef",
     "GetModelVersionRequestRequestTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
     "GetVariablesRequestRequestTypeDef",
-    "IngestedEventsTimeWindowOutputTypeDef",
     "IngestedEventsTimeWindowTypeDef",
     "LabelSchemaOutputTypeDef",
     "LabelSchemaTypeDef",
     "PredictionTimeRangeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
-    "ModelInputConfigurationTypeDef",
     "ModelOutputConfigurationTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
     "UpdateDetectorVersionStatusRequestRequestTypeDef",
     "UpdateEventLabelRequestRequestTypeDef",
     "UpdateListRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelVersionResultTypeDef",
     "UpdateModelVersionStatusRequestRequestTypeDef",
     "UpdateVariableRequestRequestTypeDef",
     "ATITrainingMetricsValueTypeDef",
     "AggregatedVariablesImportanceMetricsTypeDef",
-    "GetListsMetadataResultTypeDef",
-    "BatchCreateVariableResultTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
     "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
     "PutOutcomeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
+    "BatchCreateVariableResultTypeDef",
+    "CreateDetectorVersionResultTypeDef",
+    "CreateModelVersionResultTypeDef",
+    "DeleteEventsByEventTypeResultTypeDef",
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    "GetListElementsResultTypeDef",
+    "GetListsMetadataResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
+    "ModelScoresTypeDef",
     "CreateDetectorVersionRequestRequestTypeDef",
+    "CreateRuleResultTypeDef",
     "DeleteRuleRequestRequestTypeDef",
+    "GetDetectorVersionResultTypeDef",
     "UpdateDetectorVersionRequestRequestTypeDef",
     "UpdateRuleMetadataRequestRequestTypeDef",
     "UpdateRuleVersionRequestRequestTypeDef",
-    "CreateRuleResultTypeDef",
     "UpdateRuleVersionResultTypeDef",
     "DataValidationMetricsTypeDef",
     "DescribeDetectorResultTypeDef",
     "GetDetectorsResultTypeDef",
     "EventTypeDef",
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
-    "GetDetectorVersionResultTypeDef",
-    "ModelScoresTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
-    "IngestedEventsDetailOutputTypeDef",
     "IngestedEventsDetailTypeDef",
     "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
     "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
-    "GetExternalModelsResultTypeDef",
     "GetEventPredictionResultTypeDef",
+    "GetExternalModelsResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
     "GetModelVersionResultTypeDef",
     "CreateModelVersionRequestRequestTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
@@ -283,17 +275,19 @@
         "createdTime": str,
         "updatedTime": str,
         "arn": str,
     },
     total=False,
 )
 
+
 class AllowDenyListTypeDef(_RequiredAllowDenyListTypeDef, _OptionalAllowDenyListTypeDef):
     pass
 
+
 BatchCreateVariableErrorTypeDef = TypedDict(
     "BatchCreateVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -317,14 +311,25 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
 )
 
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
 BatchGetVariableErrorTypeDef = TypedDict(
     "BatchGetVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -422,64 +427,36 @@
     "_OptionalModelVersionTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
+
 class ModelVersionTypeDef(_RequiredModelVersionTypeDef, _OptionalModelVersionTypeDef):
     pass
 
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "detectorId": str,
         "ruleId": str,
         "ruleVersion": str,
     },
 )
 
-CreateDetectorVersionResultTypeDef = TypedDict(
-    "CreateDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "status": DetectorVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExternalEventsDetailTypeDef = TypedDict(
     "ExternalEventsDetailTypeDef",
     {
         "dataLocation": str,
         "dataAccessRoleArn": str,
     },
 )
 
-CreateModelVersionResultTypeDef = TypedDict(
-    "CreateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "detectorId": str,
-        "ruleId": str,
-        "ruleVersion": str,
-    },
-)
-
 FieldValidationMessageTypeDef = TypedDict(
     "FieldValidationMessageTypeDef",
     {
         "fieldName": str,
         "identifier": str,
         "title": str,
         "content": str,
@@ -545,42 +522,35 @@
     "_OptionalDeleteEventRequestRequestTypeDef",
     {
         "deleteAuditHistory": bool,
     },
     total=False,
 )
 
+
 class DeleteEventRequestRequestTypeDef(
     _RequiredDeleteEventRequestRequestTypeDef, _OptionalDeleteEventRequestRequestTypeDef
 ):
     pass
 
+
 DeleteEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
 DeleteEventsByEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventsByEventTypeRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
-DeleteEventsByEventTypeResultTypeDef = TypedDict(
-    "DeleteEventsByEventTypeResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteExternalModelRequestRequestTypeDef = TypedDict(
     "DeleteExternalModelRequestRequestTypeDef",
     {
         "modelEndpoint": str,
     },
 )
 
@@ -640,19 +610,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeDetectorRequestRequestTypeDef(
     _RequiredDescribeDetectorRequestRequestTypeDef, _OptionalDescribeDetectorRequestRequestTypeDef
 ):
     pass
 
+
 DetectorVersionSummaryTypeDef = TypedDict(
     "DetectorVersionSummaryTypeDef",
     {
         "detectorVersionId": str,
         "status": DetectorVersionStatusType,
         "description": str,
         "lastUpdatedTime": str,
@@ -681,22 +653,14 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-EntityOutputTypeDef = TypedDict(
-    "EntityOutputTypeDef",
-    {
-        "entityType": str,
-        "entityId": str,
-    },
-)
-
 EntityTypeDef = TypedDict(
     "EntityTypeDef",
     {
         "entityType": str,
         "entityId": str,
     },
 )
@@ -734,21 +698,14 @@
         "outcomes": List[str],
         "evaluated": bool,
         "matched": bool,
     },
     total=False,
 )
 
-EventOrchestrationOutputTypeDef = TypedDict(
-    "EventOrchestrationOutputTypeDef",
-    {
-        "eventBridgeEnabled": bool,
-    },
-)
-
 EventOrchestrationTypeDef = TypedDict(
     "EventOrchestrationTypeDef",
     {
         "eventBridgeEnabled": bool,
     },
 )
 
@@ -783,53 +740,47 @@
         "name": str,
         "value": str,
         "source": str,
     },
     total=False,
 )
 
-ExternalEventsDetailOutputTypeDef = TypedDict(
-    "ExternalEventsDetailOutputTypeDef",
-    {
-        "dataLocation": str,
-        "dataAccessRoleArn": str,
-    },
-)
-
 ExternalModelSummaryTypeDef = TypedDict(
     "ExternalModelSummaryTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
     },
     total=False,
 )
 
-_RequiredModelInputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredModelInputConfigurationOutputTypeDef",
+_RequiredModelInputConfigurationTypeDef = TypedDict(
+    "_RequiredModelInputConfigurationTypeDef",
     {
         "useEventVariables": bool,
     },
 )
-_OptionalModelInputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalModelInputConfigurationOutputTypeDef",
+_OptionalModelInputConfigurationTypeDef = TypedDict(
+    "_OptionalModelInputConfigurationTypeDef",
     {
         "eventTypeName": str,
         "format": ModelInputDataFormatType,
         "jsonInputTemplate": str,
         "csvInputTemplate": str,
     },
     total=False,
 )
 
-class ModelInputConfigurationOutputTypeDef(
-    _RequiredModelInputConfigurationOutputTypeDef, _OptionalModelInputConfigurationOutputTypeDef
+
+class ModelInputConfigurationTypeDef(
+    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
 ):
     pass
 
+
 _RequiredModelOutputConfigurationOutputTypeDef = TypedDict(
     "_RequiredModelOutputConfigurationOutputTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
 _OptionalModelOutputConfigurationOutputTypeDef = TypedDict(
@@ -837,19 +788,21 @@
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
+
 class ModelOutputConfigurationOutputTypeDef(
     _RequiredModelOutputConfigurationOutputTypeDef, _OptionalModelOutputConfigurationOutputTypeDef
 ):
     pass
 
+
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "value": str,
     },
     total=False,
 )
@@ -877,52 +830,22 @@
 GetDeleteEventsByEventTypeStatusRequestRequestTypeDef = TypedDict(
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     {
         "eventTypeName": str,
     },
 )
 
-GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
-    "GetDeleteEventsByEventTypeStatusResultTypeDef",
-    {
-        "eventTypeName": str,
-        "eventsDeletionStatus": AsyncJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDetectorVersionRequestRequestTypeDef = TypedDict(
     "GetDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
     },
 )
 
-_RequiredModelVersionOutputTypeDef = TypedDict(
-    "_RequiredModelVersionOutputTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-    },
-)
-_OptionalModelVersionOutputTypeDef = TypedDict(
-    "_OptionalModelVersionOutputTypeDef",
-    {
-        "arn": str,
-    },
-    total=False,
-)
-
-class ModelVersionOutputTypeDef(
-    _RequiredModelVersionOutputTypeDef, _OptionalModelVersionOutputTypeDef
-):
-    pass
-
 GetDetectorsRequestRequestTypeDef = TypedDict(
     "GetDetectorsRequestRequestTypeDef",
     {
         "detectorId": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1037,27 +960,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetListElementsRequestRequestTypeDef(
     _RequiredGetListElementsRequestRequestTypeDef, _OptionalGetListElementsRequestRequestTypeDef
 ):
     pass
 
-GetListElementsResultTypeDef = TypedDict(
-    "GetListElementsResultTypeDef",
-    {
-        "elements": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetListsMetadataRequestRequestTypeDef = TypedDict(
     "GetListsMetadataRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
         "maxResults": int,
@@ -1134,19 +1050,21 @@
         "ruleVersion": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetRulesRequestRequestTypeDef(
     _RequiredGetRulesRequestRequestTypeDef, _OptionalGetRulesRequestRequestTypeDef
 ):
     pass
 
+
 RuleDetailTypeDef = TypedDict(
     "RuleDetailTypeDef",
     {
         "ruleId": str,
         "description": str,
         "detectorId": str,
         "ruleVersion": str,
@@ -1166,22 +1084,14 @@
         "name": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-IngestedEventsTimeWindowOutputTypeDef = TypedDict(
-    "IngestedEventsTimeWindowOutputTypeDef",
-    {
-        "startTime": str,
-        "endTime": str,
-    },
-)
-
 IngestedEventsTimeWindowTypeDef = TypedDict(
     "IngestedEventsTimeWindowTypeDef",
     {
         "startTime": str,
         "endTime": str,
     },
 )
@@ -1223,27 +1133,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
 
 LogOddsMetricTypeDef = TypedDict(
     "LogOddsMetricTypeDef",
     {
         "variableName": str,
         "variableType": str,
         "variableImportance": float,
@@ -1257,36 +1161,14 @@
         "precision": float,
         "tpr": float,
         "threshold": float,
     },
     total=False,
 )
 
-_RequiredModelInputConfigurationTypeDef = TypedDict(
-    "_RequiredModelInputConfigurationTypeDef",
-    {
-        "useEventVariables": bool,
-    },
-)
-_OptionalModelInputConfigurationTypeDef = TypedDict(
-    "_OptionalModelInputConfigurationTypeDef",
-    {
-        "eventTypeName": str,
-        "format": ModelInputDataFormatType,
-        "jsonInputTemplate": str,
-        "csvInputTemplate": str,
-    },
-    total=False,
-)
-
-class ModelInputConfigurationTypeDef(
-    _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
-):
-    pass
-
 _RequiredModelOutputConfigurationTypeDef = TypedDict(
     "_RequiredModelOutputConfigurationTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
 _OptionalModelOutputConfigurationTypeDef = TypedDict(
@@ -1294,19 +1176,21 @@
     {
         "jsonKeyToVariableMap": Mapping[str, str],
         "csvIndexToVariableMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ModelOutputConfigurationTypeDef(
     _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
 ):
     pass
 
+
 OFIMetricDataPointTypeDef = TypedDict(
     "OFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1335,25 +1219,14 @@
 PutKMSEncryptionKeyRequestRequestTypeDef = TypedDict(
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     {
         "kmsEncryptionKeyArn": str,
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
 TFIMetricDataPointTypeDef = TypedDict(
     "TFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1410,19 +1283,21 @@
         "description": str,
         "updateMode": ListUpdateModeType,
         "variableType": str,
     },
     total=False,
 )
 
+
 class UpdateListRequestRequestTypeDef(
     _RequiredUpdateListRequestRequestTypeDef, _OptionalUpdateListRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
     },
 )
@@ -1430,29 +1305,20 @@
     "_OptionalUpdateModelRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
-UpdateModelVersionResultTypeDef = TypedDict(
-    "UpdateModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateModelVersionStatusRequestRequestTypeDef = TypedDict(
     "UpdateModelVersionStatusRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
@@ -1472,19 +1338,21 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
 )
 
+
 class UpdateVariableRequestRequestTypeDef(
     _RequiredUpdateVariableRequestRequestTypeDef, _OptionalUpdateVariableRequestRequestTypeDef
 ):
     pass
 
+
 ATITrainingMetricsValueTypeDef = TypedDict(
     "ATITrainingMetricsValueTypeDef",
     {
         "metricDataPoints": List[ATIMetricDataPointTypeDef],
         "modelPerformance": ATIModelPerformanceTypeDef,
     },
     total=False,
@@ -1494,31 +1362,14 @@
     "AggregatedVariablesImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[AggregatedLogOddsMetricTypeDef],
     },
     total=False,
 )
 
-GetListsMetadataResultTypeDef = TypedDict(
-    "GetListsMetadataResultTypeDef",
-    {
-        "lists": List[AllowDenyListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchCreateVariableResultTypeDef = TypedDict(
-    "BatchCreateVariableResultTypeDef",
-    {
-        "errors": List[BatchCreateVariableErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBatchImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchImportJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1529,20 +1380,22 @@
     "_OptionalCreateBatchImportJobRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBatchImportJobRequestRequestTypeDef(
     _RequiredCreateBatchImportJobRequestRequestTypeDef,
     _OptionalCreateBatchImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateBatchPredictionJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchPredictionJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1555,20 +1408,22 @@
     {
         "detectorVersion": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBatchPredictionJobRequestRequestTypeDef(
     _RequiredCreateBatchPredictionJobRequestRequestTypeDef,
     _OptionalCreateBatchPredictionJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateListRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateListRequestRequestTypeDef = TypedDict(
@@ -1578,19 +1433,21 @@
         "variableType": str,
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateListRequestRequestTypeDef(
     _RequiredCreateListRequestRequestTypeDef, _OptionalCreateListRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "eventTypeName": str,
     },
@@ -1600,19 +1457,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleRequestRequestTypeDef",
     {
         "ruleId": str,
         "detectorId": str,
         "expression": str,
         "language": Literal["DETECTORPL"],
@@ -1624,19 +1483,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVariableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVariableRequestRequestTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "dataSource": DataSourceType,
         "defaultValue": str,
@@ -1648,19 +1509,21 @@
         "description": str,
         "variableType": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1669,19 +1532,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutDetectorRequestRequestTypeDef(
     _RequiredPutDetectorRequestRequestTypeDef, _OptionalPutDetectorRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEntityTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutEntityTypeRequestRequestTypeDef = TypedDict(
@@ -1689,19 +1554,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutEntityTypeRequestRequestTypeDef(
     _RequiredPutEntityTypeRequestRequestTypeDef, _OptionalPutEntityTypeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutLabelRequestRequestTypeDef = TypedDict(
     "_RequiredPutLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutLabelRequestRequestTypeDef = TypedDict(
@@ -1709,19 +1576,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutLabelRequestRequestTypeDef(
     _RequiredPutLabelRequestRequestTypeDef, _OptionalPutLabelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutOutcomeRequestRequestTypeDef = TypedDict(
     "_RequiredPutOutcomeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutOutcomeRequestRequestTypeDef = TypedDict(
@@ -1729,19 +1598,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutOutcomeRequestRequestTypeDef(
     _RequiredPutOutcomeRequestRequestTypeDef, _OptionalPutOutcomeRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1756,56 +1627,152 @@
     "_OptionalBatchCreateVariableRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class BatchCreateVariableRequestRequestTypeDef(
     _RequiredBatchCreateVariableRequestRequestTypeDef,
     _OptionalBatchCreateVariableRequestRequestTypeDef,
 ):
     pass
 
+
+BatchCreateVariableResultTypeDef = TypedDict(
+    "BatchCreateVariableResultTypeDef",
+    {
+        "errors": List[BatchCreateVariableErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDetectorVersionResultTypeDef = TypedDict(
+    "CreateDetectorVersionResultTypeDef",
+    {
+        "detectorId": str,
+        "detectorVersionId": str,
+        "status": DetectorVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelVersionResultTypeDef = TypedDict(
+    "CreateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEventsByEventTypeResultTypeDef = TypedDict(
+    "DeleteEventsByEventTypeResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeleteEventsByEventTypeStatusResultTypeDef = TypedDict(
+    "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    {
+        "eventTypeName": str,
+        "eventsDeletionStatus": AsyncJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetListElementsResultTypeDef = TypedDict(
+    "GetListElementsResultTypeDef",
+    {
+        "elements": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetListsMetadataResultTypeDef = TypedDict(
+    "GetListsMetadataResultTypeDef",
+    {
+        "lists": List[AllowDenyListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelVersionResultTypeDef = TypedDict(
+    "UpdateModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetVariableResultTypeDef = TypedDict(
     "BatchGetVariableResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "errors": List[BatchGetVariableErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariablesResultTypeDef = TypedDict(
     "GetVariablesResultTypeDef",
     {
         "variables": List[VariableTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBatchImportJobsResultTypeDef = TypedDict(
     "GetBatchImportJobsResultTypeDef",
     {
         "batchImports": List[BatchImportTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBatchPredictionJobsResultTypeDef = TypedDict(
     "GetBatchPredictionJobsResultTypeDef",
     {
         "batchPredictions": List[BatchPredictionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ModelScoresTypeDef = TypedDict(
+    "ModelScoresTypeDef",
+    {
+        "modelVersion": ModelVersionTypeDef,
+        "scores": Dict[str, float],
+    },
+    total=False,
+)
+
 _RequiredCreateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "rules": Sequence[RuleTypeDef],
     },
 )
@@ -1817,27 +1784,55 @@
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDetectorVersionRequestRequestTypeDef(
     _RequiredCreateDetectorVersionRequestRequestTypeDef,
     _OptionalCreateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
+
+CreateRuleResultTypeDef = TypedDict(
+    "CreateRuleResultTypeDef",
+    {
+        "rule": RuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
     },
 )
 
+GetDetectorVersionResultTypeDef = TypedDict(
+    "GetDetectorVersionResultTypeDef",
+    {
+        "detectorId": str,
+        "detectorVersionId": str,
+        "description": str,
+        "externalModelEndpoints": List[str],
+        "modelVersions": List[ModelVersionTypeDef],
+        "rules": List[RuleTypeDef],
+        "status": DetectorVersionStatusType,
+        "lastUpdatedTime": str,
+        "createdTime": str,
+        "ruleExecutionMode": RuleExecutionModeType,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDetectorVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDetectorVersionRequestRequestTypeDef",
     {
         "detectorId": str,
         "detectorVersionId": str,
         "externalModelEndpoints": Sequence[str],
         "rules": Sequence[RuleTypeDef],
@@ -1849,20 +1844,22 @@
         "description": str,
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
     },
     total=False,
 )
 
+
 class UpdateDetectorVersionRequestRequestTypeDef(
     _RequiredUpdateDetectorVersionRequestRequestTypeDef,
     _OptionalUpdateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateRuleMetadataRequestRequestTypeDef = TypedDict(
     "UpdateRuleMetadataRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
         "description": str,
     },
 )
@@ -1881,32 +1878,26 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateRuleVersionRequestRequestTypeDef(
     _RequiredUpdateRuleVersionRequestRequestTypeDef, _OptionalUpdateRuleVersionRequestRequestTypeDef
 ):
     pass
 
-CreateRuleResultTypeDef = TypedDict(
-    "CreateRuleResultTypeDef",
-    {
-        "rule": RuleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
-        "rule": RuleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "rule": RuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataValidationMetricsTypeDef = TypedDict(
     "DataValidationMetricsTypeDef",
     {
         "fileLevelMessages": List[FileValidationMessageTypeDef],
@@ -1918,37 +1909,37 @@
 DescribeDetectorResultTypeDef = TypedDict(
     "DescribeDetectorResultTypeDef",
     {
         "detectorId": str,
         "detectorVersionSummaries": List[DetectorVersionSummaryTypeDef],
         "nextToken": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDetectorsResultTypeDef = TypedDict(
     "GetDetectorsResultTypeDef",
     {
         "detectors": List[DetectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "eventId": str,
         "eventTypeName": str,
         "eventTimestamp": str,
         "eventVariables": Dict[str, str],
         "currentLabel": str,
         "labelTimestamp": str,
-        "entities": List[EntityOutputTypeDef],
+        "entities": List[EntityTypeDef],
     },
     total=False,
 )
 
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
@@ -1964,25 +1955,27 @@
     {
         "assignedLabel": str,
         "labelTimestamp": str,
     },
     total=False,
 )
 
+
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
+
 GetEntityTypesResultTypeDef = TypedDict(
     "GetEntityTypesResultTypeDef",
     {
         "entityTypes": List[EntityTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventTypeRequestRequestTypeDef",
     {
         "name": str,
@@ -1998,25 +1991,27 @@
         "eventIngestion": EventIngestionType,
         "tags": Sequence[TagTypeDef],
         "eventOrchestration": EventOrchestrationTypeDef,
     },
     total=False,
 )
 
+
 class PutEventTypeRequestRequestTypeDef(
     _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
 ):
     pass
 
+
 ListEventPredictionsResultTypeDef = TypedDict(
     "ListEventPredictionsResultTypeDef",
     {
         "eventPredictionSummaries": List[EventPredictionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeTypeDef = TypedDict(
     "EventTypeTypeDef",
     {
         "name": str,
@@ -2025,15 +2020,15 @@
         "labels": List[str],
         "entityTypes": List[str],
         "eventIngestion": EventIngestionType,
         "ingestedEventStatistics": IngestedEventStatisticsTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
-        "eventOrchestration": EventOrchestrationOutputTypeDef,
+        "eventOrchestration": EventOrchestrationTypeDef,
     },
     total=False,
 )
 
 ExternalModelOutputsTypeDef = TypedDict(
     "ExternalModelOutputsTypeDef",
     {
@@ -2045,51 +2040,24 @@
 
 ExternalModelTypeDef = TypedDict(
     "ExternalModelTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationOutputTypeDef,
+        "inputConfiguration": ModelInputConfigurationTypeDef,
         "outputConfiguration": ModelOutputConfigurationOutputTypeDef,
         "modelEndpointStatus": ModelEndpointStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
-GetDetectorVersionResultTypeDef = TypedDict(
-    "GetDetectorVersionResultTypeDef",
-    {
-        "detectorId": str,
-        "detectorVersionId": str,
-        "description": str,
-        "externalModelEndpoints": List[str],
-        "modelVersions": List[ModelVersionOutputTypeDef],
-        "rules": List[RuleOutputTypeDef],
-        "status": DetectorVersionStatusType,
-        "lastUpdatedTime": str,
-        "createdTime": str,
-        "ruleExecutionMode": RuleExecutionModeType,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModelScoresTypeDef = TypedDict(
-    "ModelScoresTypeDef",
-    {
-        "modelVersion": ModelVersionOutputTypeDef,
-        "scores": Dict[str, float],
-    },
-    total=False,
-)
-
 _RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
     "_RequiredGetEventPredictionRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventId": str,
         "eventTypeName": str,
         "entities": Sequence[EntityTypeDef],
@@ -2102,68 +2070,63 @@
     {
         "detectorVersionId": str,
         "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
     },
     total=False,
 )
 
+
 class GetEventPredictionRequestRequestTypeDef(
     _RequiredGetEventPredictionRequestRequestTypeDef,
     _OptionalGetEventPredictionRequestRequestTypeDef,
 ):
     pass
 
+
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLabelsResultTypeDef = TypedDict(
     "GetLabelsResultTypeDef",
     {
         "labels": List[LabelTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResultTypeDef = TypedDict(
     "GetModelsResultTypeDef",
     {
         "nextToken": str,
         "models": List[ModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOutcomesResultTypeDef = TypedDict(
     "GetOutcomesResultTypeDef",
     {
         "outcomes": List[OutcomeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRulesResultTypeDef = TypedDict(
     "GetRulesResultTypeDef",
     {
         "ruleDetails": List[RuleDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IngestedEventsDetailOutputTypeDef = TypedDict(
-    "IngestedEventsDetailOutputTypeDef",
-    {
-        "ingestedEventsTimeWindow": IngestedEventsTimeWindowOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
@@ -2180,61 +2143,56 @@
     "_OptionalTrainingDataSchemaOutputTypeDef",
     {
         "labelSchema": LabelSchemaOutputTypeDef,
     },
     total=False,
 )
 
+
 class TrainingDataSchemaOutputTypeDef(
     _RequiredTrainingDataSchemaOutputTypeDef, _OptionalTrainingDataSchemaOutputTypeDef
 ):
     pass
 
+
 _RequiredTrainingDataSchemaTypeDef = TypedDict(
     "_RequiredTrainingDataSchemaTypeDef",
     {
         "modelVariables": Sequence[str],
     },
 )
 _OptionalTrainingDataSchemaTypeDef = TypedDict(
     "_OptionalTrainingDataSchemaTypeDef",
     {
         "labelSchema": LabelSchemaTypeDef,
     },
     total=False,
 )
 
+
 class TrainingDataSchemaTypeDef(
     _RequiredTrainingDataSchemaTypeDef, _OptionalTrainingDataSchemaTypeDef
 ):
     pass
 
+
 ListEventPredictionsRequestRequestTypeDef = TypedDict(
     "ListEventPredictionsRequestRequestTypeDef",
     {
         "eventId": FilterConditionTypeDef,
         "eventType": FilterConditionTypeDef,
         "detectorId": FilterConditionTypeDef,
         "detectorVersionId": FilterConditionTypeDef,
         "predictionTimeRange": PredictionTimeRangeTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VariableImportanceMetricsTypeDef = TypedDict(
     "VariableImportanceMetricsTypeDef",
     {
         "logOddsMetrics": List[LogOddsMetricTypeDef],
     },
     total=False,
 )
@@ -2263,19 +2221,21 @@
     "_OptionalPutExternalModelRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutExternalModelRequestRequestTypeDef(
     _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
 ):
     pass
 
+
 OFIModelPerformanceTypeDef = TypedDict(
     "OFIModelPerformanceTypeDef",
     {
         "auc": float,
         "uncertaintyRange": UncertaintyRangeTypeDef,
     },
     total=False,
@@ -2299,43 +2259,43 @@
     total=False,
 )
 
 GetEventResultTypeDef = TypedDict(
     "GetEventResultTypeDef",
     {
         "event": EventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventTypesResultTypeDef = TypedDict(
     "GetEventTypesResultTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetExternalModelsResultTypeDef = TypedDict(
-    "GetExternalModelsResultTypeDef",
-    {
-        "externalModels": List[ExternalModelTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEventPredictionResultTypeDef = TypedDict(
     "GetEventPredictionResultTypeDef",
     {
         "modelScores": List[ModelScoresTypeDef],
         "ruleResults": List[RuleResultTypeDef],
         "externalModelOutputs": List[ExternalModelOutputsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetExternalModelsResultTypeDef = TypedDict(
+    "GetExternalModelsResultTypeDef",
+    {
+        "externalModels": List[ExternalModelTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
@@ -2349,33 +2309,35 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetModelVersionResultTypeDef = TypedDict(
     "GetModelVersionResultTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
-        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "status": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
@@ -2390,20 +2352,22 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
+
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
@@ -2484,39 +2448,39 @@
         "eventVariables": List[EventVariableSummaryTypeDef],
         "rules": List[EvaluatedRuleTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "outcomes": List[str],
         "evaluatedModelVersions": List[EvaluatedModelVersionTypeDef],
         "evaluatedExternalModels": List[EvaluatedExternalModelTypeDef],
         "predictionTimestamp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelVersionDetailTypeDef = TypedDict(
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
-        "externalEventsDetail": ExternalEventsDetailOutputTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailOutputTypeDef,
+        "externalEventsDetail": ExternalEventsDetailTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "trainingResult": TrainingResultTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
         "trainingResultV2": TrainingResultV2TypeDef,
     },
     total=False,
 )
 
 DescribeModelVersionsResultTypeDef = TypedDict(
     "DescribeModelVersionsResultTypeDef",
     {
         "modelVersionDetails": List[ModelVersionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/PKG-INFO` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.28.12
-Summary: Type annotations for boto3.FraudDetector 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-frauddetector)](https://pepy.tech/project/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
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
 [mypy-boto3-frauddetector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,180 +320,171 @@
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
     AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
     BatchImportTypeDef,
     BatchPredictionTypeDef,
     CancelBatchImportJobRequestRequestTypeDef,
     CancelBatchPredictionJobRequestRequestTypeDef,
     ModelVersionTypeDef,
     RuleTypeDef,
-    CreateDetectorVersionResultTypeDef,
     ExternalEventsDetailTypeDef,
-    CreateModelVersionResultTypeDef,
-    RuleOutputTypeDef,
     FieldValidationMessageTypeDef,
     FileValidationMessageTypeDef,
     DeleteBatchImportJobRequestRequestTypeDef,
     DeleteBatchPredictionJobRequestRequestTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
-    DeleteEventsByEventTypeResultTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
     DetectorTypeDef,
-    EntityOutputTypeDef,
     EntityTypeDef,
     EntityTypeTypeDef,
     EvaluatedExternalModelTypeDef,
     EvaluatedRuleTypeDef,
-    EventOrchestrationOutputTypeDef,
     EventOrchestrationTypeDef,
     EventPredictionSummaryTypeDef,
     IngestedEventStatisticsTypeDef,
     EventVariableSummaryTypeDef,
-    ExternalEventsDetailOutputTypeDef,
     ExternalModelSummaryTypeDef,
-    ModelInputConfigurationOutputTypeDef,
+    ModelInputConfigurationTypeDef,
     ModelOutputConfigurationOutputTypeDef,
     FilterConditionTypeDef,
     GetBatchImportJobsRequestRequestTypeDef,
     GetBatchPredictionJobsRequestRequestTypeDef,
     GetDeleteEventsByEventTypeStatusRequestRequestTypeDef,
-    GetDeleteEventsByEventTypeStatusResultTypeDef,
     GetDetectorVersionRequestRequestTypeDef,
-    ModelVersionOutputTypeDef,
     GetDetectorsRequestRequestTypeDef,
     GetEntityTypesRequestRequestTypeDef,
     GetEventPredictionMetadataRequestRequestTypeDef,
     ModelEndpointDataBlobTypeDef,
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
     GetListElementsRequestRequestTypeDef,
-    GetListElementsResultTypeDef,
     GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
     GetVariablesRequestRequestTypeDef,
-    IngestedEventsTimeWindowOutputTypeDef,
     IngestedEventsTimeWindowTypeDef,
     LabelSchemaOutputTypeDef,
     LabelSchemaTypeDef,
     PredictionTimeRangeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     LogOddsMetricTypeDef,
     MetricDataPointTypeDef,
-    ModelInputConfigurationTypeDef,
     ModelOutputConfigurationTypeDef,
     OFIMetricDataPointTypeDef,
     UncertaintyRangeTypeDef,
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
     UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelVersionResultTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
-    GetListsMetadataResultTypeDef,
-    BatchCreateVariableResultTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
     CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
     PutOutcomeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
+    BatchCreateVariableResultTypeDef,
+    CreateDetectorVersionResultTypeDef,
+    CreateModelVersionResultTypeDef,
+    DeleteEventsByEventTypeResultTypeDef,
+    GetDeleteEventsByEventTypeStatusResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
+    ModelScoresTypeDef,
     CreateDetectorVersionRequestRequestTypeDef,
+    CreateRuleResultTypeDef,
     DeleteRuleRequestRequestTypeDef,
+    GetDetectorVersionResultTypeDef,
     UpdateDetectorVersionRequestRequestTypeDef,
     UpdateRuleMetadataRequestRequestTypeDef,
     UpdateRuleVersionRequestRequestTypeDef,
-    CreateRuleResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     DataValidationMetricsTypeDef,
     DescribeDetectorResultTypeDef,
     GetDetectorsResultTypeDef,
     EventTypeDef,
     SendEventRequestRequestTypeDef,
     GetEntityTypesResultTypeDef,
     PutEventTypeRequestRequestTypeDef,
     ListEventPredictionsResultTypeDef,
     EventTypeTypeDef,
     ExternalModelOutputsTypeDef,
     ExternalModelTypeDef,
-    GetDetectorVersionResultTypeDef,
-    ModelScoresTypeDef,
     GetEventPredictionRequestRequestTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
     GetModelsResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
-    IngestedEventsDetailOutputTypeDef,
     IngestedEventsDetailTypeDef,
     TrainingDataSchemaOutputTypeDef,
     TrainingDataSchemaTypeDef,
     ListEventPredictionsRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     VariableImportanceMetricsTypeDef,
     TrainingMetricsTypeDef,
     PutExternalModelRequestRequestTypeDef,
     OFIModelPerformanceTypeDef,
     TFIModelPerformanceTypeDef,
     PredictionExplanationsTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
-    GetExternalModelsResultTypeDef,
     GetEventPredictionResultTypeDef,
+    GetExternalModelsResultTypeDef,
     UpdateModelVersionRequestRequestTypeDef,
     GetModelVersionResultTypeDef,
     CreateModelVersionRequestRequestTypeDef,
     TrainingResultTypeDef,
     OFITrainingMetricsValueTypeDef,
     TFITrainingMetricsValueTypeDef,
     ModelVersionEvaluationTypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.28.12/mypy_boto3_frauddetector.egg-info/SOURCES.txt` & `mypy-boto3-frauddetector-1.28.15/mypy_boto3_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.28.12/setup.py` & `mypy-boto3-frauddetector-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-frauddetector",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FraudDetector 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.FraudDetector 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

