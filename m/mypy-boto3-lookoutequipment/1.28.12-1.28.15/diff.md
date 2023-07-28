# Comparing `tmp/mypy-boto3-lookoutequipment-1.28.12.tar.gz` & `tmp/mypy-boto3-lookoutequipment-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutequipment-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutequipment-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
```

## Comparing `mypy-boto3-lookoutequipment-1.28.12.tar` & `mypy-boto3-lookoutequipment-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-27 05:25:35.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-07-27 05:25:37.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40437 2023-07-27 05:25:36.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:57.000000 mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.828453 mypy-boto3-lookoutequipment-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:25:34.000000 mypy-boto3-lookoutequipment-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.661424 mypy-boto3-lookoutequipment-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-28 20:43:11.661424 mypy-boto3-lookoutequipment-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.657424 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-07-28 20:30:32.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-28 20:30:33.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-28 20:30:32.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35906 2023-07-28 20:30:33.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-07-28 20:30:33.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.661424 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-28 20:43:11.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 20:43:11.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:11.000000 mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.661424 mypy-boto3-lookoutequipment-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:30:30.000000 mypy-boto3-lookoutequipment-1.28.15/setup.py
```

### Comparing `mypy-boto3-lookoutequipment-1.28.12/LICENSE` & `mypy-boto3-lookoutequipment-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.12/PKG-INFO` & `mypy-boto3-lookoutequipment-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutequipment
-Version: 1.28.12
-Summary: Type annotations for boto3.LookoutEquipment 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LookoutEquipment 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutequipment)](https://pepy.tech/project/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,111 +312,100 @@
 
 ```python
 from mypy_boto3_lookoutequipment.type_defs import (
     CategoricalValuesTypeDef,
     CountPercentTypeDef,
     DatasetSchemaTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateInferenceSchedulerResponseTypeDef,
-    CreateLabelGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLabelRequestRequestTypeDef,
-    CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
-    CreateModelResponseTypeDef,
-    DataPreProcessingConfigurationOutputTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
     DeleteLabelGroupRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DescribeDataIngestionJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeInferenceSchedulerRequestRequestTypeDef,
     DescribeLabelGroupRequestRequestTypeDef,
-    DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
-    DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
-    InferenceInputNameConfigurationOutputTypeDef,
-    InferenceS3InputConfigurationOutputTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
-    InferenceS3OutputConfigurationOutputTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
-    IngestionS3InputConfigurationOutputTypeDef,
     IngestionS3InputConfigurationTypeDef,
     MissingCompleteSensorDataTypeDef,
     SensorsWithShortDateRangeTypeDef,
     LabelGroupSummaryTypeDef,
     LabelSummaryTypeDef,
-    LabelsS3InputConfigurationOutputTypeDef,
     LabelsS3InputConfigurationTypeDef,
     LargeTimestampGapsTypeDef,
     ListDataIngestionJobsRequestRequestTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListInferenceEventsRequestRequestTypeDef,
     ListInferenceExecutionsRequestRequestTypeDef,
     ListInferenceSchedulersRequestRequestTypeDef,
     ListLabelGroupsRequestRequestTypeDef,
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
-    ResponseMetadataTypeDef,
-    StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
-    StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
-    StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateInferenceSchedulerResponseTypeDef,
+    CreateLabelGroupResponseTypeDef,
+    CreateLabelResponseTypeDef,
+    CreateModelResponseTypeDef,
+    DescribeLabelGroupResponseTypeDef,
+    DescribeLabelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDataIngestionJobResponseTypeDef,
+    StartInferenceSchedulerResponseTypeDef,
+    StopInferenceSchedulerResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
-    InferenceInputConfigurationOutputTypeDef,
     InferenceInputConfigurationTypeDef,
-    InferenceOutputConfigurationOutputTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
-    IngestionInputConfigurationOutputTypeDef,
     IngestionInputConfigurationTypeDef,
     InsufficientSensorDataTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
-    LabelsInputConfigurationOutputTypeDef,
     LabelsInputConfigurationTypeDef,
     ListModelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SensorStatisticsSummaryTypeDef,
+    CreateInferenceSchedulerRequestRequestTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     InferenceExecutionSummaryTypeDef,
-    CreateInferenceSchedulerRequestRequestTypeDef,
     UpdateInferenceSchedulerRequestRequestTypeDef,
     DataIngestionJobSummaryTypeDef,
     StartDataIngestionJobRequestRequestTypeDef,
     DataQualitySummaryTypeDef,
-    DescribeModelResponseTypeDef,
     CreateModelRequestRequestTypeDef,
+    DescribeModelResponseTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.12/README.md` & `mypy-boto3-lookoutequipment-1.28.15/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutequipment)](https://pepy.tech/project/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,111 +280,100 @@
 
 ```python
 from mypy_boto3_lookoutequipment.type_defs import (
     CategoricalValuesTypeDef,
     CountPercentTypeDef,
     DatasetSchemaTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateInferenceSchedulerResponseTypeDef,
-    CreateLabelGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLabelRequestRequestTypeDef,
-    CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
-    CreateModelResponseTypeDef,
-    DataPreProcessingConfigurationOutputTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
     DeleteLabelGroupRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DescribeDataIngestionJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeInferenceSchedulerRequestRequestTypeDef,
     DescribeLabelGroupRequestRequestTypeDef,
-    DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
-    DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
-    InferenceInputNameConfigurationOutputTypeDef,
-    InferenceS3InputConfigurationOutputTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
-    InferenceS3OutputConfigurationOutputTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
-    IngestionS3InputConfigurationOutputTypeDef,
     IngestionS3InputConfigurationTypeDef,
     MissingCompleteSensorDataTypeDef,
     SensorsWithShortDateRangeTypeDef,
     LabelGroupSummaryTypeDef,
     LabelSummaryTypeDef,
-    LabelsS3InputConfigurationOutputTypeDef,
     LabelsS3InputConfigurationTypeDef,
     LargeTimestampGapsTypeDef,
     ListDataIngestionJobsRequestRequestTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListInferenceEventsRequestRequestTypeDef,
     ListInferenceExecutionsRequestRequestTypeDef,
     ListInferenceSchedulersRequestRequestTypeDef,
     ListLabelGroupsRequestRequestTypeDef,
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
-    ResponseMetadataTypeDef,
-    StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
-    StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
-    StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateInferenceSchedulerResponseTypeDef,
+    CreateLabelGroupResponseTypeDef,
+    CreateLabelResponseTypeDef,
+    CreateModelResponseTypeDef,
+    DescribeLabelGroupResponseTypeDef,
+    DescribeLabelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDataIngestionJobResponseTypeDef,
+    StartInferenceSchedulerResponseTypeDef,
+    StopInferenceSchedulerResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
-    InferenceInputConfigurationOutputTypeDef,
     InferenceInputConfigurationTypeDef,
-    InferenceOutputConfigurationOutputTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
-    IngestionInputConfigurationOutputTypeDef,
     IngestionInputConfigurationTypeDef,
     InsufficientSensorDataTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
-    LabelsInputConfigurationOutputTypeDef,
     LabelsInputConfigurationTypeDef,
     ListModelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SensorStatisticsSummaryTypeDef,
+    CreateInferenceSchedulerRequestRequestTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     InferenceExecutionSummaryTypeDef,
-    CreateInferenceSchedulerRequestRequestTypeDef,
     UpdateInferenceSchedulerRequestRequestTypeDef,
     DataIngestionJobSummaryTypeDef,
     StartDataIngestionJobRequestRequestTypeDef,
     DataQualitySummaryTypeDef,
-    DescribeModelResponseTypeDef,
     CreateModelRequestRequestTypeDef,
+    DescribeModelResponseTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/__main__.py` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutEquipment 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LookoutEquipment 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment\nOther"
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

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.py` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/client.pyi` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.py` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/literals.pyi` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.py` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,111 +36,100 @@
 
 
 __all__ = (
     "CategoricalValuesTypeDef",
     "CountPercentTypeDef",
     "DatasetSchemaTypeDef",
     "TagTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateInferenceSchedulerResponseTypeDef",
-    "CreateLabelGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLabelRequestRequestTypeDef",
-    "CreateLabelResponseTypeDef",
     "DataPreProcessingConfigurationTypeDef",
-    "CreateModelResponseTypeDef",
-    "DataPreProcessingConfigurationOutputTypeDef",
     "DuplicateTimestampsTypeDef",
     "InvalidSensorDataTypeDef",
     "MissingSensorDataTypeDef",
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
     "DeleteLabelGroupRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DescribeDataIngestionJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeInferenceSchedulerRequestRequestTypeDef",
     "DescribeLabelGroupRequestRequestTypeDef",
-    "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelRequestRequestTypeDef",
-    "DescribeLabelResponseTypeDef",
     "DescribeModelRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
-    "InferenceInputNameConfigurationOutputTypeDef",
-    "InferenceS3InputConfigurationOutputTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
-    "InferenceS3OutputConfigurationOutputTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
-    "IngestionS3InputConfigurationOutputTypeDef",
     "IngestionS3InputConfigurationTypeDef",
     "MissingCompleteSensorDataTypeDef",
     "SensorsWithShortDateRangeTypeDef",
     "LabelGroupSummaryTypeDef",
     "LabelSummaryTypeDef",
-    "LabelsS3InputConfigurationOutputTypeDef",
     "LabelsS3InputConfigurationTypeDef",
     "LargeTimestampGapsTypeDef",
     "ListDataIngestionJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListInferenceEventsRequestRequestTypeDef",
     "ListInferenceExecutionsRequestRequestTypeDef",
     "ListInferenceSchedulersRequestRequestTypeDef",
     "ListLabelGroupsRequestRequestTypeDef",
     "ListLabelsRequestRequestTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
-    "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
-    "StopInferenceSchedulerResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateInferenceSchedulerResponseTypeDef",
+    "CreateLabelGroupResponseTypeDef",
+    "CreateLabelResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "DescribeLabelGroupResponseTypeDef",
+    "DescribeLabelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDataIngestionJobResponseTypeDef",
+    "StartInferenceSchedulerResponseTypeDef",
+    "StopInferenceSchedulerResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
-    "InferenceInputConfigurationOutputTypeDef",
     "InferenceInputConfigurationTypeDef",
-    "InferenceOutputConfigurationOutputTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
-    "IngestionInputConfigurationOutputTypeDef",
     "IngestionInputConfigurationTypeDef",
     "InsufficientSensorDataTypeDef",
     "ListLabelGroupsResponseTypeDef",
     "ListLabelsResponseTypeDef",
-    "LabelsInputConfigurationOutputTypeDef",
     "LabelsInputConfigurationTypeDef",
     "ListModelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SensorStatisticsSummaryTypeDef",
+    "CreateInferenceSchedulerRequestRequestTypeDef",
     "DescribeInferenceSchedulerResponseTypeDef",
     "InferenceExecutionSummaryTypeDef",
-    "CreateInferenceSchedulerRequestRequestTypeDef",
     "UpdateInferenceSchedulerRequestRequestTypeDef",
     "DataIngestionJobSummaryTypeDef",
     "StartDataIngestionJobRequestRequestTypeDef",
     "DataQualitySummaryTypeDef",
-    "DescribeModelResponseTypeDef",
     "CreateModelRequestRequestTypeDef",
+    "DescribeModelResponseTypeDef",
     "ListSensorStatisticsResponseTypeDef",
     "ListInferenceExecutionsResponseTypeDef",
     "ListDataIngestionJobsResponseTypeDef",
     "DescribeDataIngestionJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
@@ -185,40 +174,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Status": DatasetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateInferenceSchedulerResponseTypeDef = TypedDict(
-    "CreateInferenceSchedulerResponseTypeDef",
-    {
-        "InferenceSchedulerArn": str,
-        "InferenceSchedulerName": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLabelGroupResponseTypeDef = TypedDict(
-    "CreateLabelGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
@@ -241,47 +212,22 @@
 
 class CreateLabelRequestRequestTypeDef(
     _RequiredCreateLabelRequestRequestTypeDef, _OptionalCreateLabelRequestRequestTypeDef
 ):
     pass
 
 
-CreateLabelResponseTypeDef = TypedDict(
-    "CreateLabelResponseTypeDef",
-    {
-        "LabelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataPreProcessingConfigurationTypeDef = TypedDict(
     "DataPreProcessingConfigurationTypeDef",
     {
         "TargetSamplingRate": TargetSamplingRateType,
     },
     total=False,
 )
 
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "Status": ModelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataPreProcessingConfigurationOutputTypeDef = TypedDict(
-    "DataPreProcessingConfigurationOutputTypeDef",
-    {
-        "TargetSamplingRate": TargetSamplingRateType,
-    },
-    total=False,
-)
-
 DuplicateTimestampsTypeDef = TypedDict(
     "DuplicateTimestampsTypeDef",
     {
         "TotalNumberOfDuplicateTimestamps": int,
     },
 )
 
@@ -379,65 +325,29 @@
 DescribeLabelGroupRequestRequestTypeDef = TypedDict(
     "DescribeLabelGroupRequestRequestTypeDef",
     {
         "LabelGroupName": str,
     },
 )
 
-DescribeLabelGroupResponseTypeDef = TypedDict(
-    "DescribeLabelGroupResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "FaultCodes": List[str],
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeLabelRequestRequestTypeDef = TypedDict(
     "DescribeLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
         "LabelId": str,
     },
 )
 
-DescribeLabelResponseTypeDef = TypedDict(
-    "DescribeLabelResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "LabelId": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "Rating": LabelRatingType,
-        "FaultCode": str,
-        "Notes": str,
-        "Equipment": str,
-        "CreatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeModelRequestRequestTypeDef = TypedDict(
     "DescribeModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InferenceEventSummaryTypeDef = TypedDict(
     "InferenceEventSummaryTypeDef",
     {
         "InferenceSchedulerArn": str,
         "InferenceSchedulerName": str,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
@@ -451,45 +361,14 @@
     "S3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-InferenceInputNameConfigurationOutputTypeDef = TypedDict(
-    "InferenceInputNameConfigurationOutputTypeDef",
-    {
-        "TimestampFormat": str,
-        "ComponentTimestampDelimiter": str,
-    },
-    total=False,
-)
-
-_RequiredInferenceS3InputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInferenceS3InputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalInferenceS3InputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInferenceS3InputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-
-class InferenceS3InputConfigurationOutputTypeDef(
-    _RequiredInferenceS3InputConfigurationOutputTypeDef,
-    _OptionalInferenceS3InputConfigurationOutputTypeDef,
-):
-    pass
-
-
 InferenceInputNameConfigurationTypeDef = TypedDict(
     "InferenceInputNameConfigurationTypeDef",
     {
         "TimestampFormat": str,
         "ComponentTimestampDelimiter": str,
     },
     total=False,
@@ -512,36 +391,14 @@
 
 class InferenceS3InputConfigurationTypeDef(
     _RequiredInferenceS3InputConfigurationTypeDef, _OptionalInferenceS3InputConfigurationTypeDef
 ):
     pass
 
 
-_RequiredInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInferenceS3OutputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInferenceS3OutputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-
-class InferenceS3OutputConfigurationOutputTypeDef(
-    _RequiredInferenceS3OutputConfigurationOutputTypeDef,
-    _OptionalInferenceS3OutputConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredInferenceS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceS3OutputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalInferenceS3OutputConfigurationTypeDef = TypedDict(
@@ -570,37 +427,14 @@
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "LatestInferenceResult": LatestInferenceResultType,
     },
     total=False,
 )
 
-_RequiredIngestionS3InputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredIngestionS3InputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalIngestionS3InputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalIngestionS3InputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "KeyPattern": str,
-    },
-    total=False,
-)
-
-
-class IngestionS3InputConfigurationOutputTypeDef(
-    _RequiredIngestionS3InputConfigurationOutputTypeDef,
-    _OptionalIngestionS3InputConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredIngestionS3InputConfigurationTypeDef = TypedDict(
     "_RequiredIngestionS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalIngestionS3InputConfigurationTypeDef = TypedDict(
@@ -656,36 +490,14 @@
         "FaultCode": str,
         "Equipment": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
-_RequiredLabelsS3InputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLabelsS3InputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalLabelsS3InputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLabelsS3InputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-
-class LabelsS3InputConfigurationOutputTypeDef(
-    _RequiredLabelsS3InputConfigurationOutputTypeDef,
-    _OptionalLabelsS3InputConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredLabelsS3InputConfigurationTypeDef = TypedDict(
     "_RequiredLabelsS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalLabelsS3InputConfigurationTypeDef = TypedDict(
@@ -897,22 +709,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredMonotonicValuesTypeDef = TypedDict(
     "_RequiredMonotonicValuesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
     },
 )
 _OptionalMonotonicValuesTypeDef = TypedDict(
@@ -931,72 +735,28 @@
 MultipleOperatingModesTypeDef = TypedDict(
     "MultipleOperatingModesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
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
-StartDataIngestionJobResponseTypeDef = TypedDict(
-    "StartDataIngestionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "Status": IngestionJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StartInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
-StartInferenceSchedulerResponseTypeDef = TypedDict(
-    "StartInferenceSchedulerResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StopInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
-StopInferenceSchedulerResponseTypeDef = TypedDict(
-    "StopInferenceSchedulerResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1073,29 +833,152 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Status": DatasetStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInferenceSchedulerResponseTypeDef = TypedDict(
+    "CreateInferenceSchedulerResponseTypeDef",
+    {
+        "InferenceSchedulerArn": str,
+        "InferenceSchedulerName": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLabelGroupResponseTypeDef = TypedDict(
+    "CreateLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLabelResponseTypeDef = TypedDict(
+    "CreateLabelResponseTypeDef",
+    {
+        "LabelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "Status": ModelStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLabelGroupResponseTypeDef = TypedDict(
+    "DescribeLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "FaultCodes": List[str],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLabelResponseTypeDef = TypedDict(
+    "DescribeLabelResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "LabelId": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "Rating": LabelRatingType,
+        "FaultCode": str,
+        "Notes": str,
+        "Equipment": str,
+        "CreatedAt": datetime,
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
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataIngestionJobResponseTypeDef = TypedDict(
+    "StartDataIngestionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "Status": IngestionJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartInferenceSchedulerResponseTypeDef = TypedDict(
+    "StartInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopInferenceSchedulerResponseTypeDef = TypedDict(
+    "StopInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "NextToken": str,
         "DatasetSummaries": List[DatasetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInferenceEventsResponseTypeDef = TypedDict(
     "ListInferenceEventsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceEventSummaries": List[InferenceEventSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIngestedFilesSummaryTypeDef = TypedDict(
     "_RequiredIngestedFilesSummaryTypeDef",
     {
         "TotalNumberOfFiles": int,
@@ -1113,56 +996,24 @@
 
 class IngestedFilesSummaryTypeDef(
     _RequiredIngestedFilesSummaryTypeDef, _OptionalIngestedFilesSummaryTypeDef
 ):
     pass
 
 
-InferenceInputConfigurationOutputTypeDef = TypedDict(
-    "InferenceInputConfigurationOutputTypeDef",
-    {
-        "S3InputConfiguration": InferenceS3InputConfigurationOutputTypeDef,
-        "InputTimeZoneOffset": str,
-        "InferenceInputNameConfiguration": InferenceInputNameConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 InferenceInputConfigurationTypeDef = TypedDict(
     "InferenceInputConfigurationTypeDef",
     {
         "S3InputConfiguration": InferenceS3InputConfigurationTypeDef,
         "InputTimeZoneOffset": str,
         "InferenceInputNameConfiguration": InferenceInputNameConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredInferenceOutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInferenceOutputConfigurationOutputTypeDef",
-    {
-        "S3OutputConfiguration": InferenceS3OutputConfigurationOutputTypeDef,
-    },
-)
-_OptionalInferenceOutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInferenceOutputConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class InferenceOutputConfigurationOutputTypeDef(
-    _RequiredInferenceOutputConfigurationOutputTypeDef,
-    _OptionalInferenceOutputConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredInferenceOutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceOutputConfigurationTypeDef",
     {
         "S3OutputConfiguration": InferenceS3OutputConfigurationTypeDef,
     },
 )
 _OptionalInferenceOutputConfigurationTypeDef = TypedDict(
@@ -1181,22 +1032,15 @@
 
 
 ListInferenceSchedulersResponseTypeDef = TypedDict(
     "ListInferenceSchedulersResponseTypeDef",
     {
         "NextToken": str,
         "InferenceSchedulerSummaries": List[InferenceSchedulerSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IngestionInputConfigurationOutputTypeDef = TypedDict(
-    "IngestionInputConfigurationOutputTypeDef",
-    {
-        "S3InputConfiguration": IngestionS3InputConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestionInputConfigurationTypeDef = TypedDict(
     "IngestionInputConfigurationTypeDef",
     {
         "S3InputConfiguration": IngestionS3InputConfigurationTypeDef,
@@ -1212,59 +1056,42 @@
 )
 
 ListLabelGroupsResponseTypeDef = TypedDict(
     "ListLabelGroupsResponseTypeDef",
     {
         "NextToken": str,
         "LabelGroupSummaries": List[LabelGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLabelsResponseTypeDef = TypedDict(
     "ListLabelsResponseTypeDef",
     {
         "NextToken": str,
         "LabelSummaries": List[LabelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LabelsInputConfigurationOutputTypeDef = TypedDict(
-    "LabelsInputConfigurationOutputTypeDef",
-    {
-        "S3InputConfiguration": LabelsS3InputConfigurationOutputTypeDef,
-        "LabelGroupName": str,
-    },
-    total=False,
-)
-
 LabelsInputConfigurationTypeDef = TypedDict(
     "LabelsInputConfigurationTypeDef",
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
         "LabelGroupName": str,
     },
     total=False,
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SensorStatisticsSummaryTypeDef = TypedDict(
     "SensorStatisticsSummaryTypeDef",
     {
         "ComponentName": str,
@@ -1280,84 +1107,84 @@
         "MonotonicValues": MonotonicValuesTypeDef,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
     },
     total=False,
 )
 
+_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "DataUploadFrequency": DataUploadFrequencyType,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "RoleArn": str,
+        "ClientToken": str,
+    },
+)
+_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "DataDelayOffsetInMinutes": int,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateInferenceSchedulerRequestRequestTypeDef(
+    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
+    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeInferenceSchedulerResponseTypeDef = TypedDict(
     "DescribeInferenceSchedulerResponseTypeDef",
     {
         "ModelArn": str,
         "ModelName": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "Status": InferenceSchedulerStatusType,
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
         "RoleArn": str,
         "ServerSideKmsKeyId": str,
         "LatestInferenceResult": LatestInferenceResultType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferenceExecutionSummaryTypeDef = TypedDict(
     "InferenceExecutionSummaryTypeDef",
     {
         "ModelName": str,
         "ModelArn": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "ScheduledStartTime": datetime,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
         "CustomerResultObject": S3ObjectTypeDef,
         "Status": InferenceExecutionStatusType,
         "FailedReason": str,
     },
     total=False,
 )
 
-_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "DataUploadFrequency": DataUploadFrequencyType,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
-        "RoleArn": str,
-        "ClientToken": str,
-    },
-)
-_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "DataDelayOffsetInMinutes": int,
-        "ServerSideKmsKeyId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateInferenceSchedulerRequestRequestTypeDef(
-    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
-    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 _OptionalUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
@@ -1382,15 +1209,15 @@
 
 DataIngestionJobSummaryTypeDef = TypedDict(
     "DataIngestionJobSummaryTypeDef",
     {
         "JobId": str,
         "DatasetName": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "Status": IngestionJobStatusType,
     },
     total=False,
 )
 
 StartDataIngestionJobRequestRequestTypeDef = TypedDict(
     "StartDataIngestionJobRequestRequestTypeDef",
@@ -1409,42 +1236,14 @@
         "MissingSensorData": MissingSensorDataTypeDef,
         "InvalidSensorData": InvalidSensorDataTypeDef,
         "UnsupportedTimestamps": UnsupportedTimestampsTypeDef,
         "DuplicateTimestamps": DuplicateTimestampsTypeDef,
     },
 )
 
-DescribeModelResponseTypeDef = TypedDict(
-    "DescribeModelResponseTypeDef",
-    {
-        "ModelName": str,
-        "ModelArn": str,
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Schema": str,
-        "LabelsInputConfiguration": LabelsInputConfigurationOutputTypeDef,
-        "TrainingDataStartTime": datetime,
-        "TrainingDataEndTime": datetime,
-        "EvaluationDataStartTime": datetime,
-        "EvaluationDataEndTime": datetime,
-        "RoleArn": str,
-        "DataPreProcessingConfiguration": DataPreProcessingConfigurationOutputTypeDef,
-        "Status": ModelStatusType,
-        "TrainingExecutionStartTime": datetime,
-        "TrainingExecutionEndTime": datetime,
-        "FailedReason": str,
-        "ModelMetrics": str,
-        "LastUpdatedTime": datetime,
-        "CreatedAt": datetime,
-        "ServerSideKmsKeyId": str,
-        "OffCondition": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ModelName": str,
         "DatasetName": str,
         "ClientToken": str,
     },
@@ -1470,73 +1269,101 @@
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
 
+DescribeModelResponseTypeDef = TypedDict(
+    "DescribeModelResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Schema": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
+        "TrainingDataStartTime": datetime,
+        "TrainingDataEndTime": datetime,
+        "EvaluationDataStartTime": datetime,
+        "EvaluationDataEndTime": datetime,
+        "RoleArn": str,
+        "DataPreProcessingConfiguration": DataPreProcessingConfigurationTypeDef,
+        "Status": ModelStatusType,
+        "TrainingExecutionStartTime": datetime,
+        "TrainingExecutionEndTime": datetime,
+        "FailedReason": str,
+        "ModelMetrics": str,
+        "LastUpdatedTime": datetime,
+        "CreatedAt": datetime,
+        "ServerSideKmsKeyId": str,
+        "OffCondition": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInferenceExecutionsResponseTypeDef = TypedDict(
     "ListInferenceExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceExecutionSummaries": List[InferenceExecutionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataIngestionJobsResponseTypeDef = TypedDict(
     "ListDataIngestionJobsResponseTypeDef",
     {
         "NextToken": str,
         "DataIngestionJobSummaries": List[DataIngestionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataIngestionJobResponseTypeDef = TypedDict(
     "DescribeDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "RoleArn": str,
         "CreatedAt": datetime,
         "Status": IngestionJobStatusType,
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
         "IngestedDataSize": int,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetName": str,
         "DatasetArn": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Status": DatasetStatusType,
         "Schema": str,
         "ServerSideKmsKeyId": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment/type_defs.pyi` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -35,111 +35,100 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "CategoricalValuesTypeDef",
     "CountPercentTypeDef",
     "DatasetSchemaTypeDef",
     "TagTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateInferenceSchedulerResponseTypeDef",
-    "CreateLabelGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLabelRequestRequestTypeDef",
-    "CreateLabelResponseTypeDef",
     "DataPreProcessingConfigurationTypeDef",
-    "CreateModelResponseTypeDef",
-    "DataPreProcessingConfigurationOutputTypeDef",
     "DuplicateTimestampsTypeDef",
     "InvalidSensorDataTypeDef",
     "MissingSensorDataTypeDef",
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
     "DeleteLabelGroupRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DescribeDataIngestionJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeInferenceSchedulerRequestRequestTypeDef",
     "DescribeLabelGroupRequestRequestTypeDef",
-    "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelRequestRequestTypeDef",
-    "DescribeLabelResponseTypeDef",
     "DescribeModelRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
-    "InferenceInputNameConfigurationOutputTypeDef",
-    "InferenceS3InputConfigurationOutputTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
-    "InferenceS3OutputConfigurationOutputTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
-    "IngestionS3InputConfigurationOutputTypeDef",
     "IngestionS3InputConfigurationTypeDef",
     "MissingCompleteSensorDataTypeDef",
     "SensorsWithShortDateRangeTypeDef",
     "LabelGroupSummaryTypeDef",
     "LabelSummaryTypeDef",
-    "LabelsS3InputConfigurationOutputTypeDef",
     "LabelsS3InputConfigurationTypeDef",
     "LargeTimestampGapsTypeDef",
     "ListDataIngestionJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListInferenceEventsRequestRequestTypeDef",
     "ListInferenceExecutionsRequestRequestTypeDef",
     "ListInferenceSchedulersRequestRequestTypeDef",
     "ListLabelGroupsRequestRequestTypeDef",
     "ListLabelsRequestRequestTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
-    "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
-    "StopInferenceSchedulerResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateInferenceSchedulerResponseTypeDef",
+    "CreateLabelGroupResponseTypeDef",
+    "CreateLabelResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "DescribeLabelGroupResponseTypeDef",
+    "DescribeLabelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDataIngestionJobResponseTypeDef",
+    "StartInferenceSchedulerResponseTypeDef",
+    "StopInferenceSchedulerResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
-    "InferenceInputConfigurationOutputTypeDef",
     "InferenceInputConfigurationTypeDef",
-    "InferenceOutputConfigurationOutputTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
-    "IngestionInputConfigurationOutputTypeDef",
     "IngestionInputConfigurationTypeDef",
     "InsufficientSensorDataTypeDef",
     "ListLabelGroupsResponseTypeDef",
     "ListLabelsResponseTypeDef",
-    "LabelsInputConfigurationOutputTypeDef",
     "LabelsInputConfigurationTypeDef",
     "ListModelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SensorStatisticsSummaryTypeDef",
+    "CreateInferenceSchedulerRequestRequestTypeDef",
     "DescribeInferenceSchedulerResponseTypeDef",
     "InferenceExecutionSummaryTypeDef",
-    "CreateInferenceSchedulerRequestRequestTypeDef",
     "UpdateInferenceSchedulerRequestRequestTypeDef",
     "DataIngestionJobSummaryTypeDef",
     "StartDataIngestionJobRequestRequestTypeDef",
     "DataQualitySummaryTypeDef",
-    "DescribeModelResponseTypeDef",
     "CreateModelRequestRequestTypeDef",
+    "DescribeModelResponseTypeDef",
     "ListSensorStatisticsResponseTypeDef",
     "ListInferenceExecutionsResponseTypeDef",
     "ListDataIngestionJobsResponseTypeDef",
     "DescribeDataIngestionJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
@@ -182,40 +171,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Status": DatasetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateInferenceSchedulerResponseTypeDef = TypedDict(
-    "CreateInferenceSchedulerResponseTypeDef",
-    {
-        "InferenceSchedulerArn": str,
-        "InferenceSchedulerName": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLabelGroupResponseTypeDef = TypedDict(
-    "CreateLabelGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
@@ -236,47 +207,22 @@
 )
 
 class CreateLabelRequestRequestTypeDef(
     _RequiredCreateLabelRequestRequestTypeDef, _OptionalCreateLabelRequestRequestTypeDef
 ):
     pass
 
-CreateLabelResponseTypeDef = TypedDict(
-    "CreateLabelResponseTypeDef",
-    {
-        "LabelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataPreProcessingConfigurationTypeDef = TypedDict(
     "DataPreProcessingConfigurationTypeDef",
     {
         "TargetSamplingRate": TargetSamplingRateType,
     },
     total=False,
 )
 
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "Status": ModelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataPreProcessingConfigurationOutputTypeDef = TypedDict(
-    "DataPreProcessingConfigurationOutputTypeDef",
-    {
-        "TargetSamplingRate": TargetSamplingRateType,
-    },
-    total=False,
-)
-
 DuplicateTimestampsTypeDef = TypedDict(
     "DuplicateTimestampsTypeDef",
     {
         "TotalNumberOfDuplicateTimestamps": int,
     },
 )
 
@@ -374,65 +320,29 @@
 DescribeLabelGroupRequestRequestTypeDef = TypedDict(
     "DescribeLabelGroupRequestRequestTypeDef",
     {
         "LabelGroupName": str,
     },
 )
 
-DescribeLabelGroupResponseTypeDef = TypedDict(
-    "DescribeLabelGroupResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "FaultCodes": List[str],
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeLabelRequestRequestTypeDef = TypedDict(
     "DescribeLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
         "LabelId": str,
     },
 )
 
-DescribeLabelResponseTypeDef = TypedDict(
-    "DescribeLabelResponseTypeDef",
-    {
-        "LabelGroupName": str,
-        "LabelGroupArn": str,
-        "LabelId": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "Rating": LabelRatingType,
-        "FaultCode": str,
-        "Notes": str,
-        "Equipment": str,
-        "CreatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeModelRequestRequestTypeDef = TypedDict(
     "DescribeModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InferenceEventSummaryTypeDef = TypedDict(
     "InferenceEventSummaryTypeDef",
     {
         "InferenceSchedulerArn": str,
         "InferenceSchedulerName": str,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
@@ -446,43 +356,14 @@
     "S3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-InferenceInputNameConfigurationOutputTypeDef = TypedDict(
-    "InferenceInputNameConfigurationOutputTypeDef",
-    {
-        "TimestampFormat": str,
-        "ComponentTimestampDelimiter": str,
-    },
-    total=False,
-)
-
-_RequiredInferenceS3InputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInferenceS3InputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalInferenceS3InputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInferenceS3InputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-class InferenceS3InputConfigurationOutputTypeDef(
-    _RequiredInferenceS3InputConfigurationOutputTypeDef,
-    _OptionalInferenceS3InputConfigurationOutputTypeDef,
-):
-    pass
-
 InferenceInputNameConfigurationTypeDef = TypedDict(
     "InferenceInputNameConfigurationTypeDef",
     {
         "TimestampFormat": str,
         "ComponentTimestampDelimiter": str,
     },
     total=False,
@@ -503,34 +384,14 @@
 )
 
 class InferenceS3InputConfigurationTypeDef(
     _RequiredInferenceS3InputConfigurationTypeDef, _OptionalInferenceS3InputConfigurationTypeDef
 ):
     pass
 
-_RequiredInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInferenceS3OutputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalInferenceS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInferenceS3OutputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-class InferenceS3OutputConfigurationOutputTypeDef(
-    _RequiredInferenceS3OutputConfigurationOutputTypeDef,
-    _OptionalInferenceS3OutputConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredInferenceS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceS3OutputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalInferenceS3OutputConfigurationTypeDef = TypedDict(
@@ -557,35 +418,14 @@
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "LatestInferenceResult": LatestInferenceResultType,
     },
     total=False,
 )
 
-_RequiredIngestionS3InputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredIngestionS3InputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalIngestionS3InputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalIngestionS3InputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "KeyPattern": str,
-    },
-    total=False,
-)
-
-class IngestionS3InputConfigurationOutputTypeDef(
-    _RequiredIngestionS3InputConfigurationOutputTypeDef,
-    _OptionalIngestionS3InputConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredIngestionS3InputConfigurationTypeDef = TypedDict(
     "_RequiredIngestionS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalIngestionS3InputConfigurationTypeDef = TypedDict(
@@ -639,34 +479,14 @@
         "FaultCode": str,
         "Equipment": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
-_RequiredLabelsS3InputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLabelsS3InputConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalLabelsS3InputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLabelsS3InputConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-    },
-    total=False,
-)
-
-class LabelsS3InputConfigurationOutputTypeDef(
-    _RequiredLabelsS3InputConfigurationOutputTypeDef,
-    _OptionalLabelsS3InputConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredLabelsS3InputConfigurationTypeDef = TypedDict(
     "_RequiredLabelsS3InputConfigurationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalLabelsS3InputConfigurationTypeDef = TypedDict(
@@ -866,22 +686,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredMonotonicValuesTypeDef = TypedDict(
     "_RequiredMonotonicValuesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
     },
 )
 _OptionalMonotonicValuesTypeDef = TypedDict(
@@ -898,72 +710,28 @@
 MultipleOperatingModesTypeDef = TypedDict(
     "MultipleOperatingModesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
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
-StartDataIngestionJobResponseTypeDef = TypedDict(
-    "StartDataIngestionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "Status": IngestionJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StartInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
-StartInferenceSchedulerResponseTypeDef = TypedDict(
-    "StartInferenceSchedulerResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StopInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
-StopInferenceSchedulerResponseTypeDef = TypedDict(
-    "StopInferenceSchedulerResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "InferenceSchedulerArn": str,
-        "Status": InferenceSchedulerStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1034,29 +802,152 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Status": DatasetStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInferenceSchedulerResponseTypeDef = TypedDict(
+    "CreateInferenceSchedulerResponseTypeDef",
+    {
+        "InferenceSchedulerArn": str,
+        "InferenceSchedulerName": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLabelGroupResponseTypeDef = TypedDict(
+    "CreateLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLabelResponseTypeDef = TypedDict(
+    "CreateLabelResponseTypeDef",
+    {
+        "LabelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "Status": ModelStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLabelGroupResponseTypeDef = TypedDict(
+    "DescribeLabelGroupResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "FaultCodes": List[str],
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLabelResponseTypeDef = TypedDict(
+    "DescribeLabelResponseTypeDef",
+    {
+        "LabelGroupName": str,
+        "LabelGroupArn": str,
+        "LabelId": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "Rating": LabelRatingType,
+        "FaultCode": str,
+        "Notes": str,
+        "Equipment": str,
+        "CreatedAt": datetime,
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
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataIngestionJobResponseTypeDef = TypedDict(
+    "StartDataIngestionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "Status": IngestionJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartInferenceSchedulerResponseTypeDef = TypedDict(
+    "StartInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopInferenceSchedulerResponseTypeDef = TypedDict(
+    "StopInferenceSchedulerResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "InferenceSchedulerArn": str,
+        "Status": InferenceSchedulerStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "NextToken": str,
         "DatasetSummaries": List[DatasetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInferenceEventsResponseTypeDef = TypedDict(
     "ListInferenceEventsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceEventSummaries": List[InferenceEventSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIngestedFilesSummaryTypeDef = TypedDict(
     "_RequiredIngestedFilesSummaryTypeDef",
     {
         "TotalNumberOfFiles": int,
@@ -1072,54 +963,24 @@
 )
 
 class IngestedFilesSummaryTypeDef(
     _RequiredIngestedFilesSummaryTypeDef, _OptionalIngestedFilesSummaryTypeDef
 ):
     pass
 
-InferenceInputConfigurationOutputTypeDef = TypedDict(
-    "InferenceInputConfigurationOutputTypeDef",
-    {
-        "S3InputConfiguration": InferenceS3InputConfigurationOutputTypeDef,
-        "InputTimeZoneOffset": str,
-        "InferenceInputNameConfiguration": InferenceInputNameConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 InferenceInputConfigurationTypeDef = TypedDict(
     "InferenceInputConfigurationTypeDef",
     {
         "S3InputConfiguration": InferenceS3InputConfigurationTypeDef,
         "InputTimeZoneOffset": str,
         "InferenceInputNameConfiguration": InferenceInputNameConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredInferenceOutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInferenceOutputConfigurationOutputTypeDef",
-    {
-        "S3OutputConfiguration": InferenceS3OutputConfigurationOutputTypeDef,
-    },
-)
-_OptionalInferenceOutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInferenceOutputConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class InferenceOutputConfigurationOutputTypeDef(
-    _RequiredInferenceOutputConfigurationOutputTypeDef,
-    _OptionalInferenceOutputConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredInferenceOutputConfigurationTypeDef = TypedDict(
     "_RequiredInferenceOutputConfigurationTypeDef",
     {
         "S3OutputConfiguration": InferenceS3OutputConfigurationTypeDef,
     },
 )
 _OptionalInferenceOutputConfigurationTypeDef = TypedDict(
@@ -1136,22 +997,15 @@
     pass
 
 ListInferenceSchedulersResponseTypeDef = TypedDict(
     "ListInferenceSchedulersResponseTypeDef",
     {
         "NextToken": str,
         "InferenceSchedulerSummaries": List[InferenceSchedulerSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IngestionInputConfigurationOutputTypeDef = TypedDict(
-    "IngestionInputConfigurationOutputTypeDef",
-    {
-        "S3InputConfiguration": IngestionS3InputConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestionInputConfigurationTypeDef = TypedDict(
     "IngestionInputConfigurationTypeDef",
     {
         "S3InputConfiguration": IngestionS3InputConfigurationTypeDef,
@@ -1167,59 +1021,42 @@
 )
 
 ListLabelGroupsResponseTypeDef = TypedDict(
     "ListLabelGroupsResponseTypeDef",
     {
         "NextToken": str,
         "LabelGroupSummaries": List[LabelGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLabelsResponseTypeDef = TypedDict(
     "ListLabelsResponseTypeDef",
     {
         "NextToken": str,
         "LabelSummaries": List[LabelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LabelsInputConfigurationOutputTypeDef = TypedDict(
-    "LabelsInputConfigurationOutputTypeDef",
-    {
-        "S3InputConfiguration": LabelsS3InputConfigurationOutputTypeDef,
-        "LabelGroupName": str,
-    },
-    total=False,
-)
-
 LabelsInputConfigurationTypeDef = TypedDict(
     "LabelsInputConfigurationTypeDef",
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
         "LabelGroupName": str,
     },
     total=False,
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SensorStatisticsSummaryTypeDef = TypedDict(
     "SensorStatisticsSummaryTypeDef",
     {
         "ComponentName": str,
@@ -1235,82 +1072,82 @@
         "MonotonicValues": MonotonicValuesTypeDef,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
     },
     total=False,
 )
 
+_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "InferenceSchedulerName": str,
+        "DataUploadFrequency": DataUploadFrequencyType,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
+        "RoleArn": str,
+        "ClientToken": str,
+    },
+)
+_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
+    {
+        "DataDelayOffsetInMinutes": int,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateInferenceSchedulerRequestRequestTypeDef(
+    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
+    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
+):
+    pass
+
 DescribeInferenceSchedulerResponseTypeDef = TypedDict(
     "DescribeInferenceSchedulerResponseTypeDef",
     {
         "ModelArn": str,
         "ModelName": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "Status": InferenceSchedulerStatusType,
         "DataDelayOffsetInMinutes": int,
         "DataUploadFrequency": DataUploadFrequencyType,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
         "RoleArn": str,
         "ServerSideKmsKeyId": str,
         "LatestInferenceResult": LatestInferenceResultType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InferenceExecutionSummaryTypeDef = TypedDict(
     "InferenceExecutionSummaryTypeDef",
     {
         "ModelName": str,
         "ModelArn": str,
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "ScheduledStartTime": datetime,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "DataInputConfiguration": InferenceInputConfigurationOutputTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationOutputTypeDef,
+        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
+        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
         "CustomerResultObject": S3ObjectTypeDef,
         "Status": InferenceExecutionStatusType,
         "FailedReason": str,
     },
     total=False,
 )
 
-_RequiredCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "ModelName": str,
-        "InferenceSchedulerName": str,
-        "DataUploadFrequency": DataUploadFrequencyType,
-        "DataInputConfiguration": InferenceInputConfigurationTypeDef,
-        "DataOutputConfiguration": InferenceOutputConfigurationTypeDef,
-        "RoleArn": str,
-        "ClientToken": str,
-    },
-)
-_OptionalCreateInferenceSchedulerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInferenceSchedulerRequestRequestTypeDef",
-    {
-        "DataDelayOffsetInMinutes": int,
-        "ServerSideKmsKeyId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateInferenceSchedulerRequestRequestTypeDef(
-    _RequiredCreateInferenceSchedulerRequestRequestTypeDef,
-    _OptionalCreateInferenceSchedulerRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 _OptionalUpdateInferenceSchedulerRequestRequestTypeDef = TypedDict(
@@ -1333,15 +1170,15 @@
 
 DataIngestionJobSummaryTypeDef = TypedDict(
     "DataIngestionJobSummaryTypeDef",
     {
         "JobId": str,
         "DatasetName": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "Status": IngestionJobStatusType,
     },
     total=False,
 )
 
 StartDataIngestionJobRequestRequestTypeDef = TypedDict(
     "StartDataIngestionJobRequestRequestTypeDef",
@@ -1360,42 +1197,14 @@
         "MissingSensorData": MissingSensorDataTypeDef,
         "InvalidSensorData": InvalidSensorDataTypeDef,
         "UnsupportedTimestamps": UnsupportedTimestampsTypeDef,
         "DuplicateTimestamps": DuplicateTimestampsTypeDef,
     },
 )
 
-DescribeModelResponseTypeDef = TypedDict(
-    "DescribeModelResponseTypeDef",
-    {
-        "ModelName": str,
-        "ModelArn": str,
-        "DatasetName": str,
-        "DatasetArn": str,
-        "Schema": str,
-        "LabelsInputConfiguration": LabelsInputConfigurationOutputTypeDef,
-        "TrainingDataStartTime": datetime,
-        "TrainingDataEndTime": datetime,
-        "EvaluationDataStartTime": datetime,
-        "EvaluationDataEndTime": datetime,
-        "RoleArn": str,
-        "DataPreProcessingConfiguration": DataPreProcessingConfigurationOutputTypeDef,
-        "Status": ModelStatusType,
-        "TrainingExecutionStartTime": datetime,
-        "TrainingExecutionEndTime": datetime,
-        "FailedReason": str,
-        "ModelMetrics": str,
-        "LastUpdatedTime": datetime,
-        "CreatedAt": datetime,
-        "ServerSideKmsKeyId": str,
-        "OffCondition": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ModelName": str,
         "DatasetName": str,
         "ClientToken": str,
     },
@@ -1419,73 +1228,101 @@
 )
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
+DescribeModelResponseTypeDef = TypedDict(
+    "DescribeModelResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Schema": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
+        "TrainingDataStartTime": datetime,
+        "TrainingDataEndTime": datetime,
+        "EvaluationDataStartTime": datetime,
+        "EvaluationDataEndTime": datetime,
+        "RoleArn": str,
+        "DataPreProcessingConfiguration": DataPreProcessingConfigurationTypeDef,
+        "Status": ModelStatusType,
+        "TrainingExecutionStartTime": datetime,
+        "TrainingExecutionEndTime": datetime,
+        "FailedReason": str,
+        "ModelMetrics": str,
+        "LastUpdatedTime": datetime,
+        "CreatedAt": datetime,
+        "ServerSideKmsKeyId": str,
+        "OffCondition": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInferenceExecutionsResponseTypeDef = TypedDict(
     "ListInferenceExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "InferenceExecutionSummaries": List[InferenceExecutionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataIngestionJobsResponseTypeDef = TypedDict(
     "ListDataIngestionJobsResponseTypeDef",
     {
         "NextToken": str,
         "DataIngestionJobSummaries": List[DataIngestionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataIngestionJobResponseTypeDef = TypedDict(
     "DescribeDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
         "DatasetArn": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "RoleArn": str,
         "CreatedAt": datetime,
         "Status": IngestionJobStatusType,
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
         "IngestedDataSize": int,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetName": str,
         "DatasetArn": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Status": DatasetStatusType,
         "Schema": str,
         "ServerSideKmsKeyId": str,
-        "IngestionInputConfiguration": IngestionInputConfigurationOutputTypeDef,
+        "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/PKG-INFO` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutequipment
-Version: 1.28.12
-Summary: Type annotations for boto3.LookoutEquipment 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LookoutEquipment 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutequipment.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutequipment)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutequipment)](https://pepy.tech/project/mypy-boto3-lookoutequipment)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutEquipment 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
+[boto3.LookoutEquipment 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment)
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
 [mypy-boto3-lookoutequipment docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutequipment/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,111 +312,100 @@
 
 ```python
 from mypy_boto3_lookoutequipment.type_defs import (
     CategoricalValuesTypeDef,
     CountPercentTypeDef,
     DatasetSchemaTypeDef,
     TagTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateInferenceSchedulerResponseTypeDef,
-    CreateLabelGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLabelRequestRequestTypeDef,
-    CreateLabelResponseTypeDef,
     DataPreProcessingConfigurationTypeDef,
-    CreateModelResponseTypeDef,
-    DataPreProcessingConfigurationOutputTypeDef,
     DuplicateTimestampsTypeDef,
     InvalidSensorDataTypeDef,
     MissingSensorDataTypeDef,
     UnsupportedTimestampsTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteInferenceSchedulerRequestRequestTypeDef,
     DeleteLabelGroupRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DescribeDataIngestionJobRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeInferenceSchedulerRequestRequestTypeDef,
     DescribeLabelGroupRequestRequestTypeDef,
-    DescribeLabelGroupResponseTypeDef,
     DescribeLabelRequestRequestTypeDef,
-    DescribeLabelResponseTypeDef,
     DescribeModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     InferenceEventSummaryTypeDef,
     S3ObjectTypeDef,
-    InferenceInputNameConfigurationOutputTypeDef,
-    InferenceS3InputConfigurationOutputTypeDef,
     InferenceInputNameConfigurationTypeDef,
     InferenceS3InputConfigurationTypeDef,
-    InferenceS3OutputConfigurationOutputTypeDef,
     InferenceS3OutputConfigurationTypeDef,
     InferenceSchedulerSummaryTypeDef,
-    IngestionS3InputConfigurationOutputTypeDef,
     IngestionS3InputConfigurationTypeDef,
     MissingCompleteSensorDataTypeDef,
     SensorsWithShortDateRangeTypeDef,
     LabelGroupSummaryTypeDef,
     LabelSummaryTypeDef,
-    LabelsS3InputConfigurationOutputTypeDef,
     LabelsS3InputConfigurationTypeDef,
     LargeTimestampGapsTypeDef,
     ListDataIngestionJobsRequestRequestTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListInferenceEventsRequestRequestTypeDef,
     ListInferenceExecutionsRequestRequestTypeDef,
     ListInferenceSchedulersRequestRequestTypeDef,
     ListLabelGroupsRequestRequestTypeDef,
     ListLabelsRequestRequestTypeDef,
     ListModelsRequestRequestTypeDef,
     ModelSummaryTypeDef,
     ListSensorStatisticsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     MonotonicValuesTypeDef,
     MultipleOperatingModesTypeDef,
-    ResponseMetadataTypeDef,
-    StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerRequestRequestTypeDef,
-    StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerRequestRequestTypeDef,
-    StopInferenceSchedulerResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLabelGroupRequestRequestTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateLabelGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateInferenceSchedulerResponseTypeDef,
+    CreateLabelGroupResponseTypeDef,
+    CreateLabelResponseTypeDef,
+    CreateModelResponseTypeDef,
+    DescribeLabelGroupResponseTypeDef,
+    DescribeLabelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDataIngestionJobResponseTypeDef,
+    StartInferenceSchedulerResponseTypeDef,
+    StopInferenceSchedulerResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     IngestedFilesSummaryTypeDef,
-    InferenceInputConfigurationOutputTypeDef,
     InferenceInputConfigurationTypeDef,
-    InferenceOutputConfigurationOutputTypeDef,
     InferenceOutputConfigurationTypeDef,
     ListInferenceSchedulersResponseTypeDef,
-    IngestionInputConfigurationOutputTypeDef,
     IngestionInputConfigurationTypeDef,
     InsufficientSensorDataTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
-    LabelsInputConfigurationOutputTypeDef,
     LabelsInputConfigurationTypeDef,
     ListModelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SensorStatisticsSummaryTypeDef,
+    CreateInferenceSchedulerRequestRequestTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     InferenceExecutionSummaryTypeDef,
-    CreateInferenceSchedulerRequestRequestTypeDef,
     UpdateInferenceSchedulerRequestRequestTypeDef,
     DataIngestionJobSummaryTypeDef,
     StartDataIngestionJobRequestRequestTypeDef,
     DataQualitySummaryTypeDef,
-    DescribeModelResponseTypeDef,
     CreateModelRequestRequestTypeDef,
+    DescribeModelResponseTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lookoutequipment-1.28.12/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt` & `mypy-boto3-lookoutequipment-1.28.15/mypy_boto3_lookoutequipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutequipment-1.28.12/setup.py` & `mypy-boto3-lookoutequipment-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutequipment",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lookoutequipment"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutEquipment 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LookoutEquipment 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

