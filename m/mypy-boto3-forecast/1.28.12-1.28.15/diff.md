# Comparing `tmp/mypy-boto3-forecast-1.28.12.tar.gz` & `tmp/mypy-boto3-forecast-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-forecast-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
+gzip compressed data, was "mypy-boto3-forecast-1.28.15.tar", last modified: Fri Jul 28 20:42:50 2023, max compression
```

## Comparing `mypy-boto3-forecast-1.28.12.tar` & `mypy-boto3-forecast-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51565 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51481 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-27 05:22:25.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-27 05:22:25.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75342 2023-07-27 05:22:27.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75270 2023-07-27 05:22:26.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:24.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:42.000000 mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.548507 mypy-boto3-forecast-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:22:23.000000 mypy-boto3-forecast-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.081128 mypy-boto3-forecast-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23727 2023-07-28 20:42:50.077128 mypy-boto3-forecast-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.073128 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51565 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51481 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-28 20:26:03.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71201 2023-07-28 20:26:06.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71135 2023-07-28 20:26:04.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:02.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.073128 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23727 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:49.000000 mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:50.081128 mypy-boto3-forecast-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:26:01.000000 mypy-boto3-forecast-1.28.15/setup.py
```

### Comparing `mypy-boto3-forecast-1.28.12/LICENSE` & `mypy-boto3-forecast-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/PKG-INFO` & `mypy-boto3-forecast-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.28.12
-Summary: Type annotations for boto3.ForecastService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,46 +396,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
-    ActionOutputTypeDef,
     ActionTypeDef,
     AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
     AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
     CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
-    ContinuousParameterRangeOutputTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
+    ResponseMetadataTypeDef,
     ExplainabilityConfigTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
-    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -446,147 +430,149 @@
     DeletePredictorBacktestExportJobRequestRequestTypeDef,
     DeletePredictorRequestRequestTypeDef,
     DeleteResourceTreeRequestRequestTypeDef,
     DeleteWhatIfAnalysisRequestRequestTypeDef,
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
-    EncryptionConfigOutputTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
-    TimeAlignmentBoundaryOutputTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
-    ExplainabilityConfigOutputTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
-    EvaluationParametersOutputTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
     FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
-    SupplementaryFeatureOutputTypeDef,
     SupplementaryFeatureTypeDef,
-    IntegerParameterRangeOutputTypeDef,
     IntegerParameterRangeTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
-    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
-    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
-    SchemaAttributeOutputTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
-    TimeSeriesConditionOutputTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
     DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    DataDestinationOutputTypeDef,
-    DataSourceOutputTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
-    ExplainabilitySummaryTypeDef,
     FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
     InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     CreateAutoPredictorRequestRequestTypeDef,
     BaselineTypeDef,
+    ListExplainabilitiesResponseTypeDef,
+    CreateExplainabilityExportRequestRequestTypeDef,
+    CreateForecastExportJobRequestRequestTypeDef,
+    CreatePredictorBacktestExportJobRequestRequestTypeDef,
+    CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
     DescribeForecastExportJobResponseTypeDef,
     DescribePredictorBacktestExportJobResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     ExplainabilityExportSummaryTypeDef,
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
+    CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
-    CreateExplainabilityExportRequestRequestTypeDef,
-    CreateForecastExportJobRequestRequestTypeDef,
-    CreatePredictorBacktestExportJobRequestRequestTypeDef,
-    CreateWhatIfForecastExportRequestRequestTypeDef,
-    CreateDatasetImportJobRequestRequestTypeDef,
     ListPredictorsResponseTypeDef,
-    ListExplainabilitiesResponseTypeDef,
     FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
     HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
@@ -615,15 +601,15 @@
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
     CreateForecastRequestRequestTypeDef,
     CreateWhatIfAnalysisRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionOutputTypeDef:
+def get_structure() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.12/README.md` & `mypy-boto3-forecast-1.28.15/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,46 +364,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
-    ActionOutputTypeDef,
     ActionTypeDef,
     AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
     AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
     CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
-    ContinuousParameterRangeOutputTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
+    ResponseMetadataTypeDef,
     ExplainabilityConfigTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
-    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -414,147 +398,149 @@
     DeletePredictorBacktestExportJobRequestRequestTypeDef,
     DeletePredictorRequestRequestTypeDef,
     DeleteResourceTreeRequestRequestTypeDef,
     DeleteWhatIfAnalysisRequestRequestTypeDef,
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
-    EncryptionConfigOutputTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
-    TimeAlignmentBoundaryOutputTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
-    ExplainabilityConfigOutputTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
-    EvaluationParametersOutputTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
     FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
-    SupplementaryFeatureOutputTypeDef,
     SupplementaryFeatureTypeDef,
-    IntegerParameterRangeOutputTypeDef,
     IntegerParameterRangeTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
-    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
-    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
-    SchemaAttributeOutputTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
-    TimeSeriesConditionOutputTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
     DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    DataDestinationOutputTypeDef,
-    DataSourceOutputTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
-    ExplainabilitySummaryTypeDef,
     FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
     InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     CreateAutoPredictorRequestRequestTypeDef,
     BaselineTypeDef,
+    ListExplainabilitiesResponseTypeDef,
+    CreateExplainabilityExportRequestRequestTypeDef,
+    CreateForecastExportJobRequestRequestTypeDef,
+    CreatePredictorBacktestExportJobRequestRequestTypeDef,
+    CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
     DescribeForecastExportJobResponseTypeDef,
     DescribePredictorBacktestExportJobResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     ExplainabilityExportSummaryTypeDef,
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
+    CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
-    CreateExplainabilityExportRequestRequestTypeDef,
-    CreateForecastExportJobRequestRequestTypeDef,
-    CreatePredictorBacktestExportJobRequestRequestTypeDef,
-    CreateWhatIfForecastExportRequestRequestTypeDef,
-    CreateDatasetImportJobRequestRequestTypeDef,
     ListPredictorsResponseTypeDef,
-    ListExplainabilitiesResponseTypeDef,
     FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
     HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
@@ -583,15 +569,15 @@
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
     CreateForecastRequestRequestTypeDef,
     CreateWhatIfAnalysisRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionOutputTypeDef:
+def get_structure() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.py` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__init__.pyi` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/__main__.py` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ForecastService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ForecastService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
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

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.py` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/client.pyi` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.py` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/literals.pyi` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.py` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -81,263 +81,247 @@
     "ListPredictorBacktestExportJobsPaginator",
     "ListPredictorsPaginator",
     "ListWhatIfAnalysesPaginator",
     "ListWhatIfForecastExportsPaginator",
     "ListWhatIfForecastsPaginator",
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
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
         """
 
-
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
-
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
         """
 
-
 class ListExplainabilitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
         """
 
-
 class ListExplainabilityExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
-
 class ListForecastExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
         """
 
-
 class ListForecastsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
         """
 
-
 class ListMonitorEvaluationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
-
 class ListMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
         """
 
-
 class ListPredictorBacktestExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
-
 class ListPredictorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
         """
 
-
 class ListWhatIfAnalysesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
         """
 
-
 class ListWhatIfForecastExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
-
 class ListWhatIfForecastsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/paginator.pyi` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,247 +81,263 @@
     "ListPredictorBacktestExportJobsPaginator",
     "ListPredictorsPaginator",
     "ListWhatIfAnalysesPaginator",
     "ListWhatIfForecastExportsPaginator",
     "ListWhatIfForecastsPaginator",
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
 class ListDatasetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetgroupspaginator)
         """
 
+
 class ListDatasetImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
+
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listdatasetspaginator)
         """
 
+
 class ListExplainabilitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilitiespaginator)
         """
 
+
 class ListExplainabilityExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
+
 class ListForecastExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastexportjobspaginator)
         """
 
+
 class ListForecastsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listforecastspaginator)
         """
 
+
 class ListMonitorEvaluationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
+
 class ListMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listmonitorspaginator)
         """
 
+
 class ListPredictorBacktestExportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
+
 class ListPredictorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listpredictorspaginator)
         """
 
+
 class ListWhatIfAnalysesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifanalysespaginator)
         """
 
+
 class ListWhatIfForecastExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
+
 class ListWhatIfForecastsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.py` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for forecast service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_forecast.type_defs import ActionOutputTypeDef
+    from mypy_boto3_forecast.type_defs import ActionTypeDef
 
-    data: ActionOutputTypeDef = {...}
+    data: ActionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -41,46 +41,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
     "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
     "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
-    "ContinuousParameterRangeOutputTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
-    "CreateAutoPredictorResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateExplainabilityExportResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ExplainabilityConfigTypeDef",
-    "CreateExplainabilityResponseTypeDef",
-    "CreateForecastExportJobResponseTypeDef",
-    "CreateForecastResponseTypeDef",
-    "CreateMonitorResponseTypeDef",
-    "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
-    "CreatePredictorResponseTypeDef",
-    "CreateWhatIfAnalysisResponseTypeDef",
-    "CreateWhatIfForecastExportResponseTypeDef",
-    "CreateWhatIfForecastResponseTypeDef",
-    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -91,147 +75,149 @@
     "DeletePredictorBacktestExportJobRequestRequestTypeDef",
     "DeletePredictorRequestRequestTypeDef",
     "DeleteResourceTreeRequestRequestTypeDef",
     "DeleteWhatIfAnalysisRequestRequestTypeDef",
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
-    "EncryptionConfigOutputTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
-    "TimeAlignmentBoundaryOutputTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
-    "ExplainabilityConfigOutputTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
-    "EvaluationParametersOutputTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
     "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
-    "SupplementaryFeatureOutputTypeDef",
     "SupplementaryFeatureTypeDef",
-    "IntegerParameterRangeOutputTypeDef",
     "IntegerParameterRangeTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
-    "SchemaAttributeOutputTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
-    "TimeSeriesConditionOutputTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
     "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "DataDestinationOutputTypeDef",
-    "DataSourceOutputTypeDef",
+    "CreateAutoPredictorResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateExplainabilityExportResponseTypeDef",
+    "CreateExplainabilityResponseTypeDef",
+    "CreateForecastExportJobResponseTypeDef",
+    "CreateForecastResponseTypeDef",
+    "CreateMonitorResponseTypeDef",
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    "CreatePredictorResponseTypeDef",
+    "CreateWhatIfAnalysisResponseTypeDef",
+    "CreateWhatIfForecastExportResponseTypeDef",
+    "CreateWhatIfForecastResponseTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
-    "ExplainabilitySummaryTypeDef",
     "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
-    "ListForecastsRequestListForecastsPaginateTypeDef",
     "ListForecastsRequestRequestTypeDef",
-    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     "ListMonitorsRequestRequestTypeDef",
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     "ListPredictorsRequestRequestTypeDef",
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
     "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+    "ListForecastsRequestListForecastsPaginateTypeDef",
+    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
     "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
     "CreateAutoPredictorRequestRequestTypeDef",
     "BaselineTypeDef",
+    "ListExplainabilitiesResponseTypeDef",
+    "CreateExplainabilityExportRequestRequestTypeDef",
+    "CreateForecastExportJobRequestRequestTypeDef",
+    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
+    "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
     "DescribeForecastExportJobResponseTypeDef",
     "DescribePredictorBacktestExportJobResponseTypeDef",
     "DescribeWhatIfForecastExportResponseTypeDef",
     "ExplainabilityExportSummaryTypeDef",
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
+    "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
-    "CreateExplainabilityExportRequestRequestTypeDef",
-    "CreateForecastExportJobRequestRequestTypeDef",
-    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
-    "CreateWhatIfForecastExportRequestRequestTypeDef",
-    "CreateDatasetImportJobRequestRequestTypeDef",
     "ListPredictorsResponseTypeDef",
-    "ListExplainabilitiesResponseTypeDef",
     "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
     "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
@@ -259,23 +245,14 @@
     "GetAccuracyMetricsResponseTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
     "CreateForecastRequestRequestTypeDef",
     "CreateWhatIfAnalysisRequestRequestTypeDef",
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "Operation": OperationType,
-        "Value": float,
-    },
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
@@ -360,37 +337,14 @@
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
-_RequiredContinuousParameterRangeOutputTypeDef = TypedDict(
-    "_RequiredContinuousParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "MaxValue": float,
-        "MinValue": float,
-    },
-)
-_OptionalContinuousParameterRangeOutputTypeDef = TypedDict(
-    "_OptionalContinuousParameterRangeOutputTypeDef",
-    {
-        "ScalingType": ScalingTypeType,
-    },
-    total=False,
-)
-
-
-class ContinuousParameterRangeOutputTypeDef(
-    _RequiredContinuousParameterRangeOutputTypeDef, _OptionalContinuousParameterRangeOutputTypeDef
-):
-    pass
-
-
 _RequiredContinuousParameterRangeTypeDef = TypedDict(
     "_RequiredContinuousParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": float,
         "MinValue": float,
     },
@@ -440,163 +394,42 @@
         "DayOfMonth": int,
         "DayOfWeek": DayOfWeekType,
         "Hour": int,
     },
     total=False,
 )
 
-CreateAutoPredictorResponseTypeDef = TypedDict(
-    "CreateAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "DatasetImportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateExplainabilityExportResponseTypeDef = TypedDict(
-    "CreateExplainabilityExportResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ExplainabilityExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ExplainabilityConfigTypeDef = TypedDict(
     "ExplainabilityConfigTypeDef",
     {
         "TimeSeriesGranularity": TimeSeriesGranularityType,
         "TimePointGranularity": TimePointGranularityType,
     },
 )
 
-CreateExplainabilityResponseTypeDef = TypedDict(
-    "CreateExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastExportJobResponseTypeDef = TypedDict(
-    "CreateForecastExportJobResponseTypeDef",
-    {
-        "ForecastExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastResponseTypeDef = TypedDict(
-    "CreateForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMonitorResponseTypeDef = TypedDict(
-    "CreateMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    {
-        "PredictorBacktestExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluationParametersTypeDef = TypedDict(
     "EvaluationParametersTypeDef",
     {
         "NumberOfBacktestWindows": int,
         "BackTestWindowOffset": int,
     },
     total=False,
 )
 
-CreatePredictorResponseTypeDef = TypedDict(
-    "CreatePredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfAnalysisResponseTypeDef = TypedDict(
-    "CreateWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastExportResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastExportResponseTypeDef",
-    {
-        "WhatIfForecastExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3ConfigOutputTypeDef = TypedDict(
-    "_RequiredS3ConfigOutputTypeDef",
-    {
-        "Path": str,
-        "RoleArn": str,
-    },
-)
-_OptionalS3ConfigOutputTypeDef = TypedDict(
-    "_OptionalS3ConfigOutputTypeDef",
-    {
-        "KMSKeyArn": str,
-    },
-    total=False,
-)
-
-
-class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
-    pass
-
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -738,22 +571,14 @@
 DescribeAutoPredictorRequestRequestTypeDef = TypedDict(
     "DescribeAutoPredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
-EncryptionConfigOutputTypeDef = TypedDict(
-    "EncryptionConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "KMSKeyArn": str,
-    },
-)
-
 ExplainabilityInfoTypeDef = TypedDict(
     "ExplainabilityInfoTypeDef",
     {
         "ExplainabilityArn": str,
         "Status": str,
     },
     total=False,
@@ -773,46 +598,21 @@
     {
         "Arn": str,
         "State": StateType,
     },
     total=False,
 )
 
-TimeAlignmentBoundaryOutputTypeDef = TypedDict(
-    "TimeAlignmentBoundaryOutputTypeDef",
-    {
-        "Month": MonthType,
-        "DayOfMonth": int,
-        "DayOfWeek": DayOfWeekType,
-        "Hour": int,
-    },
-    total=False,
-)
-
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupName": str,
-        "DatasetGroupArn": str,
-        "DatasetArns": List[str],
-        "Domain": DomainType,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetImportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetImportJobRequestRequestTypeDef",
     {
         "DatasetImportJobArn": str,
     },
 )
 
@@ -852,22 +652,14 @@
 DescribeExplainabilityRequestRequestTypeDef = TypedDict(
     "DescribeExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityArn": str,
     },
 )
 
-ExplainabilityConfigOutputTypeDef = TypedDict(
-    "ExplainabilityConfigOutputTypeDef",
-    {
-        "TimeSeriesGranularity": TimeSeriesGranularityType,
-        "TimePointGranularity": TimePointGranularityType,
-    },
-)
-
 DescribeForecastExportJobRequestRequestTypeDef = TypedDict(
     "DescribeForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobArn": str,
     },
 )
 
@@ -895,23 +687,14 @@
 DescribePredictorRequestRequestTypeDef = TypedDict(
     "DescribePredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
-EvaluationParametersOutputTypeDef = TypedDict(
-    "EvaluationParametersOutputTypeDef",
-    {
-        "NumberOfBacktestWindows": int,
-        "BackTestWindowOffset": int,
-    },
-    total=False,
-)
-
 DescribeWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisArn": str,
     },
 )
 
@@ -925,21 +708,14 @@
 DescribeWhatIfForecastRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorMetricTypeDef = TypedDict(
     "ErrorMetricTypeDef",
     {
         "ForecastType": str,
         "WAPE": float,
         "RMSE": float,
         "MASE": float,
@@ -1018,53 +794,22 @@
 GetAccuracyMetricsRequestRequestTypeDef = TypedDict(
     "GetAccuracyMetricsRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
-SupplementaryFeatureOutputTypeDef = TypedDict(
-    "SupplementaryFeatureOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 SupplementaryFeatureTypeDef = TypedDict(
     "SupplementaryFeatureTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-_RequiredIntegerParameterRangeOutputTypeDef = TypedDict(
-    "_RequiredIntegerParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "MaxValue": int,
-        "MinValue": int,
-    },
-)
-_OptionalIntegerParameterRangeOutputTypeDef = TypedDict(
-    "_OptionalIntegerParameterRangeOutputTypeDef",
-    {
-        "ScalingType": ScalingTypeType,
-    },
-    total=False,
-)
-
-
-class IntegerParameterRangeOutputTypeDef(
-    _RequiredIntegerParameterRangeOutputTypeDef, _OptionalIntegerParameterRangeOutputTypeDef
-):
-    pass
-
-
 _RequiredIntegerParameterRangeTypeDef = TypedDict(
     "_RequiredIntegerParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": int,
         "MinValue": int,
     },
@@ -1080,39 +825,33 @@
 
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
 
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
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
 
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1134,22 +873,14 @@
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
 WhatIfAnalysisSummaryTypeDef = TypedDict(
     "WhatIfAnalysisSummaryTypeDef",
     {
         "WhatIfAnalysisArn": str,
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
         "Status": str,
@@ -1198,24 +929,14 @@
         "DatasetImportJobArn": str,
         "ForecastArn": str,
         "PredictorArn": str,
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
 PredictorEventTypeDef = TypedDict(
     "PredictorEventTypeDef",
     {
         "Detail": str,
         "Datetime": datetime,
     },
     total=False,
@@ -1228,41 +949,21 @@
         "TestWindowEnd": datetime,
         "Status": str,
         "Message": str,
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
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-SchemaAttributeOutputTypeDef = TypedDict(
-    "SchemaAttributeOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": AttributeTypeType,
-    },
-    total=False,
-)
-
 SchemaAttributeTypeDef = TypedDict(
     "SchemaAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeType": AttributeTypeType,
     },
     total=False,
@@ -1271,23 +972,14 @@
 StopResourceRequestRequestTypeDef = TypedDict(
     "StopResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TimeSeriesConditionOutputTypeDef = TypedDict(
-    "TimeSeriesConditionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeValue": str,
-        "Condition": ConditionType,
-    },
-)
-
 TimeSeriesConditionTypeDef = TypedDict(
     "TimeSeriesConditionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
         "Condition": ConditionType,
     },
@@ -1407,26 +1099,168 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DataDestinationOutputTypeDef = TypedDict(
-    "DataDestinationOutputTypeDef",
+CreateAutoPredictorResponseTypeDef = TypedDict(
+    "CreateAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
+    {
+        "DatasetImportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateExplainabilityExportResponseTypeDef = TypedDict(
+    "CreateExplainabilityExportResponseTypeDef",
+    {
+        "ExplainabilityExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateExplainabilityResponseTypeDef = TypedDict(
+    "CreateExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastExportJobResponseTypeDef = TypedDict(
+    "CreateForecastExportJobResponseTypeDef",
+    {
+        "ForecastExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastResponseTypeDef = TypedDict(
+    "CreateForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMonitorResponseTypeDef = TypedDict(
+    "CreateMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    {
+        "PredictorBacktestExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorResponseTypeDef = TypedDict(
+    "CreatePredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfAnalysisResponseTypeDef = TypedDict(
+    "CreateWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastExportResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastExportResponseTypeDef",
+    {
+        "WhatIfForecastExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupName": str,
+        "DatasetGroupArn": str,
+        "DatasetArns": List[str],
+        "Domain": DomainType,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
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
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+ExplainabilitySummaryTypeDef = TypedDict(
+    "ExplainabilitySummaryTypeDef",
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
     },
+    total=False,
 )
 
 DataDestinationTypeDef = TypedDict(
     "DataDestinationTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
@@ -1440,24 +1274,24 @@
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "DatasetGroups": List[DatasetGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorSummaryTypeDef = TypedDict(
     "PredictorSummaryTypeDef",
     {
         "PredictorArn": str,
@@ -1469,29 +1303,14 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
-ExplainabilitySummaryTypeDef = TypedDict(
-    "ExplainabilitySummaryTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredFeaturizationOutputTypeDef = TypedDict(
     "_RequiredFeaturizationOutputTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationOutputTypeDef = TypedDict(
@@ -1524,132 +1343,64 @@
 )
 
 
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
 
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExplainabilitiesRequestRequestTypeDef = TypedDict(
     "ListExplainabilitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
     "ListExplainabilityExportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListForecastExportJobsRequestRequestTypeDef = TypedDict(
     "ListForecastExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
-    "ListForecastsRequestListForecastsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListForecastsRequestRequestTypeDef = TypedDict(
     "ListForecastsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    {
-        "MonitorArn": str,
-    },
-)
-_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
-    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
 )
 _OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
@@ -1666,118 +1417,64 @@
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMonitorsRequestRequestTypeDef = TypedDict(
     "ListMonitorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPredictorsRequestRequestTypeDef = TypedDict(
     "ListPredictorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
     "ListWhatIfAnalysesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
     "ListWhatIfForecastExportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
     "ListWhatIfForecastsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1785,28 +1482,28 @@
 )
 
 ListForecastsResponseTypeDef = TypedDict(
     "ListForecastsResponseTypeDef",
     {
         "Forecasts": List[ForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredInputDataConfigOutputTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigOutputTypeDef = TypedDict(
     "_OptionalInputDataConfigOutputTypeDef",
     {
-        "SupplementaryFeatures": List[SupplementaryFeatureOutputTypeDef],
+        "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
 
 class InputDataConfigOutputTypeDef(
     _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
@@ -1833,62 +1530,192 @@
     pass
 
 
 ParameterRangesOutputTypeDef = TypedDict(
     "ParameterRangesOutputTypeDef",
     {
         "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
-        "ContinuousParameterRanges": List[ContinuousParameterRangeOutputTypeDef],
-        "IntegerParameterRanges": List[IntegerParameterRangeOutputTypeDef],
+        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMonitorsResponseTypeDef = TypedDict(
-    "ListMonitorsResponseTypeDef",
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
-        "Monitors": List[MonitorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
+    "ListForecastsRequestListForecastsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    {
+        "MonitorArn": str,
+    },
+)
+_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
+    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+):
+    pass
+
+
+ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMonitorsResponseTypeDef = TypedDict(
+    "ListMonitorsResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Monitors": List[MonitorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastsResponseTypeDef = TypedDict(
     "ListWhatIfForecastsResponseTypeDef",
     {
         "WhatIfForecasts": List[WhatIfForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsTypeDef = TypedDict(
     "MetricsTypeDef",
     {
         "RMSE": float,
@@ -1925,15 +1752,15 @@
     },
     total=False,
 )
 
 SchemaOutputTypeDef = TypedDict(
     "SchemaOutputTypeDef",
     {
-        "Attributes": List[SchemaAttributeOutputTypeDef],
+        "Attributes": List[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
@@ -1941,16 +1768,16 @@
     },
     total=False,
 )
 
 TimeSeriesTransformationOutputTypeDef = TypedDict(
     "TimeSeriesTransformationOutputTypeDef",
     {
-        "Action": ActionOutputTypeDef,
-        "TimeSeriesConditions": List[TimeSeriesConditionOutputTypeDef],
+        "Action": ActionTypeDef,
+        "TimeSeriesConditions": List[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
 TimeSeriesTransformationTypeDef = TypedDict(
     "TimeSeriesTransformationTypeDef",
     {
@@ -1967,26 +1794,26 @@
         "PredictorName": str,
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "ForecastFrequency": str,
         "ForecastDimensions": List[str],
         "DatasetImportJobArns": List[str],
         "DataConfig": DataConfigOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
         "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ExplainabilityInfo": ExplainabilityInfoTypeDef,
         "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
@@ -2023,320 +1850,320 @@
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
 
+ListExplainabilitiesResponseTypeDef = TypedDict(
+    "ListExplainabilitiesResponseTypeDef",
+    {
+        "Explainabilities": List[ExplainabilitySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "ExplainabilityExportName": str,
+        "ExplainabilityArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreateExplainabilityExportRequestRequestTypeDef(
+    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
+    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "ForecastExportJobName": str,
+        "ForecastArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreateForecastExportJobRequestRequestTypeDef(
+    _RequiredCreateForecastExportJobRequestRequestTypeDef,
+    _OptionalCreateForecastExportJobRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "PredictorBacktestExportJobName": str,
+        "PredictorArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreatePredictorBacktestExportJobRequestRequestTypeDef(
+    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
+    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "WhatIfForecastExportName": str,
+        "WhatIfForecastArns": Sequence[str],
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+
+class CreateWhatIfForecastExportRequestRequestTypeDef(
+    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
+    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
         "ForecastArn": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": List[str],
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 ForecastExportJobSummaryTypeDef = TypedDict(
     "ForecastExportJobSummaryTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 PredictorBacktestExportJobSummaryTypeDef = TypedDict(
     "PredictorBacktestExportJobSummaryTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 WhatIfForecastExportSummaryTypeDef = TypedDict(
     "WhatIfForecastExportSummaryTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastArns": List[str],
         "WhatIfForecastExportName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
-DatasetImportJobSummaryTypeDef = TypedDict(
-    "DatasetImportJobSummaryTypeDef",
+_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
     {
-        "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
-        "DataSource": DataSourceOutputTypeDef,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ImportMode": ImportModeType,
+        "DatasetArn": str,
+        "DataSource": DataSourceTypeDef,
     },
-    total=False,
 )
-
-DescribeDatasetImportJobResponseTypeDef = TypedDict(
-    "DescribeDatasetImportJobResponseTypeDef",
+_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
     {
-        "DatasetImportJobName": str,
-        "DatasetImportJobArn": str,
-        "DatasetArn": str,
         "TimestampFormat": str,
         "TimeZone": str,
         "UseGeolocationForTimeZone": bool,
         "GeolocationFormat": str,
-        "DataSource": DataSourceOutputTypeDef,
-        "EstimatedTimeRemainingInMinutes": int,
-        "FieldStatistics": Dict[str, StatisticsTypeDef],
-        "DataSize": float,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Format": str,
-        "ImportMode": ImportModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
-    {
-        "ExplainabilityExportName": str,
-        "ExplainabilityArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-
-class CreateExplainabilityExportRequestRequestTypeDef(
-    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
-    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "ForecastExportJobName": str,
-        "ForecastArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-
-class CreateForecastExportJobRequestRequestTypeDef(
-    _RequiredCreateForecastExportJobRequestRequestTypeDef,
-    _OptionalCreateForecastExportJobRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
-    {
-        "PredictorBacktestExportJobName": str,
-        "PredictorArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
-    {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
+        "ImportMode": ImportModeType,
     },
     total=False,
 )
 
 
-class CreatePredictorBacktestExportJobRequestRequestTypeDef(
-    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
-    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
+class CreateDatasetImportJobRequestRequestTypeDef(
+    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
+    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
-    {
-        "WhatIfForecastExportName": str,
-        "WhatIfForecastArns": Sequence[str],
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
+DatasetImportJobSummaryTypeDef = TypedDict(
+    "DatasetImportJobSummaryTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
+        "DatasetImportJobArn": str,
+        "DatasetImportJobName": str,
+        "DataSource": DataSourceTypeDef,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ImportMode": ImportModeType,
     },
     total=False,
 )
 
-
-class CreateWhatIfForecastExportRequestRequestTypeDef(
-    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
-    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
+DescribeDatasetImportJobResponseTypeDef = TypedDict(
+    "DescribeDatasetImportJobResponseTypeDef",
     {
         "DatasetImportJobName": str,
+        "DatasetImportJobArn": str,
         "DatasetArn": str,
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
-    {
         "TimestampFormat": str,
         "TimeZone": str,
         "UseGeolocationForTimeZone": bool,
         "GeolocationFormat": str,
-        "Tags": Sequence[TagTypeDef],
+        "DataSource": DataSourceTypeDef,
+        "EstimatedTimeRemainingInMinutes": int,
+        "FieldStatistics": Dict[str, StatisticsTypeDef],
+        "DataSize": float,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateDatasetImportJobRequestRequestTypeDef(
-    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
-    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
-):
-    pass
-
-
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListExplainabilitiesResponseTypeDef = TypedDict(
-    "ListExplainabilitiesResponseTypeDef",
-    {
-        "Explainabilities": List[ExplainabilitySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFeaturizationConfigOutputTypeDef = TypedDict(
     "_RequiredFeaturizationConfigOutputTypeDef",
     {
         "ForecastFrequency": str,
@@ -2409,15 +2236,15 @@
 )
 
 ListMonitorEvaluationsResponseTypeDef = TypedDict(
     "ListMonitorEvaluationsResponseTypeDef",
     {
         "NextToken": str,
         "PredictorMonitorEvaluations": List[PredictorMonitorEvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorExecutionDetailsTypeDef = TypedDict(
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
@@ -2430,57 +2257,57 @@
     {
         "DatasetArn": str,
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "DataFrequency": str,
         "Schema": SchemaOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExplainabilityResponseTypeDef = TypedDict(
     "DescribeExplainabilityResponseTypeDef",
     {
         "ExplainabilityArn": str,
         "ExplainabilityName": str,
         "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
         "EnableVisualization": bool,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Schema": SchemaOutputTypeDef,
         "StartDateTime": str,
         "EndDateTime": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesIdentifiersOutputTypeDef = TypedDict(
     "TimeSeriesIdentifiersOutputTypeDef",
     {
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Schema": SchemaOutputTypeDef,
         "Format": str,
     },
     total=False,
 )
 
 _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
     "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "S3Config": S3ConfigTypeDef,
         "Schema": SchemaOutputTypeDef,
     },
 )
 _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
     "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
     {
         "Format": str,
@@ -2596,60 +2423,60 @@
         "LastEvaluationTime": datetime,
         "LastEvaluationState": str,
         "Baseline": BaselineTypeDef,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "EstimatedEvaluationTimeRemainingInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExplainabilityExportsResponseTypeDef = TypedDict(
     "ListExplainabilityExportsResponseTypeDef",
     {
         "ExplainabilityExports": List[ExplainabilityExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListForecastExportJobsResponseTypeDef = TypedDict(
     "ListForecastExportJobsResponseTypeDef",
     {
         "ForecastExportJobs": List[ForecastExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPredictorBacktestExportJobsResponseTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsResponseTypeDef",
     {
         "PredictorBacktestExportJobs": List[PredictorBacktestExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastExportsResponseTypeDef = TypedDict(
     "ListWhatIfForecastExportsResponseTypeDef",
     {
         "WhatIfForecastExports": List[WhatIfForecastExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
@@ -2701,29 +2528,29 @@
         "AutoMLAlgorithmArns": List[str],
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
-        "EvaluationParameters": EvaluationParametersOutputTypeDef,
+        "EvaluationParameters": EvaluationParametersTypeDef,
         "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
         "InputDataConfig": InputDataConfigOutputTypeDef,
         "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesSelectorOutputTypeDef = TypedDict(
     "TimeSeriesSelectorOutputTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
@@ -2741,15 +2568,15 @@
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
         "ForecastTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
@@ -2785,15 +2612,15 @@
 GetAccuracyMetricsResponseTypeDef = TypedDict(
     "GetAccuracyMetricsResponseTypeDef",
     {
         "PredictorEvaluationResults": List[EvaluationResultTypeDef],
         "IsAutoPredictor": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeForecastResponseTypeDef = TypedDict(
     "DescribeForecastResponseTypeDef",
     {
         "ForecastArn": str,
@@ -2803,15 +2630,15 @@
         "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
     "DescribeWhatIfAnalysisResponseTypeDef",
     {
         "WhatIfAnalysisName": str,
@@ -2819,15 +2646,15 @@
         "ForecastArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
         "ForecastName": str,
```

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast/type_defs.pyi` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for forecast service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_forecast.type_defs import ActionOutputTypeDef
+    from mypy_boto3_forecast.type_defs import ActionTypeDef
 
-    data: ActionOutputTypeDef = {...}
+    data: ActionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -40,46 +40,30 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
     "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
     "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
-    "ContinuousParameterRangeOutputTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
-    "CreateAutoPredictorResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateExplainabilityExportResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ExplainabilityConfigTypeDef",
-    "CreateExplainabilityResponseTypeDef",
-    "CreateForecastExportJobResponseTypeDef",
-    "CreateForecastResponseTypeDef",
-    "CreateMonitorResponseTypeDef",
-    "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
-    "CreatePredictorResponseTypeDef",
-    "CreateWhatIfAnalysisResponseTypeDef",
-    "CreateWhatIfForecastExportResponseTypeDef",
-    "CreateWhatIfForecastResponseTypeDef",
-    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -90,147 +74,149 @@
     "DeletePredictorBacktestExportJobRequestRequestTypeDef",
     "DeletePredictorRequestRequestTypeDef",
     "DeleteResourceTreeRequestRequestTypeDef",
     "DeleteWhatIfAnalysisRequestRequestTypeDef",
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
-    "EncryptionConfigOutputTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
-    "TimeAlignmentBoundaryOutputTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
-    "ExplainabilityConfigOutputTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
-    "EvaluationParametersOutputTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
     "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
-    "SupplementaryFeatureOutputTypeDef",
     "SupplementaryFeatureTypeDef",
-    "IntegerParameterRangeOutputTypeDef",
     "IntegerParameterRangeTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
-    "SchemaAttributeOutputTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
-    "TimeSeriesConditionOutputTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
     "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "DataDestinationOutputTypeDef",
-    "DataSourceOutputTypeDef",
+    "CreateAutoPredictorResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateExplainabilityExportResponseTypeDef",
+    "CreateExplainabilityResponseTypeDef",
+    "CreateForecastExportJobResponseTypeDef",
+    "CreateForecastResponseTypeDef",
+    "CreateMonitorResponseTypeDef",
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    "CreatePredictorResponseTypeDef",
+    "CreateWhatIfAnalysisResponseTypeDef",
+    "CreateWhatIfForecastExportResponseTypeDef",
+    "CreateWhatIfForecastResponseTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
-    "ExplainabilitySummaryTypeDef",
     "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
-    "ListForecastsRequestListForecastsPaginateTypeDef",
     "ListForecastsRequestRequestTypeDef",
-    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     "ListMonitorsRequestRequestTypeDef",
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     "ListPredictorsRequestRequestTypeDef",
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
     "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+    "ListForecastsRequestListForecastsPaginateTypeDef",
+    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
     "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
     "CreateAutoPredictorRequestRequestTypeDef",
     "BaselineTypeDef",
+    "ListExplainabilitiesResponseTypeDef",
+    "CreateExplainabilityExportRequestRequestTypeDef",
+    "CreateForecastExportJobRequestRequestTypeDef",
+    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
+    "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
     "DescribeForecastExportJobResponseTypeDef",
     "DescribePredictorBacktestExportJobResponseTypeDef",
     "DescribeWhatIfForecastExportResponseTypeDef",
     "ExplainabilityExportSummaryTypeDef",
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
+    "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
-    "CreateExplainabilityExportRequestRequestTypeDef",
-    "CreateForecastExportJobRequestRequestTypeDef",
-    "CreatePredictorBacktestExportJobRequestRequestTypeDef",
-    "CreateWhatIfForecastExportRequestRequestTypeDef",
-    "CreateDatasetImportJobRequestRequestTypeDef",
     "ListPredictorsResponseTypeDef",
-    "ListExplainabilitiesResponseTypeDef",
     "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
     "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
@@ -258,23 +244,14 @@
     "GetAccuracyMetricsResponseTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
     "CreateForecastRequestRequestTypeDef",
     "CreateWhatIfAnalysisRequestRequestTypeDef",
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "Operation": OperationType,
-        "Value": float,
-    },
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
@@ -355,35 +332,14 @@
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
-_RequiredContinuousParameterRangeOutputTypeDef = TypedDict(
-    "_RequiredContinuousParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "MaxValue": float,
-        "MinValue": float,
-    },
-)
-_OptionalContinuousParameterRangeOutputTypeDef = TypedDict(
-    "_OptionalContinuousParameterRangeOutputTypeDef",
-    {
-        "ScalingType": ScalingTypeType,
-    },
-    total=False,
-)
-
-class ContinuousParameterRangeOutputTypeDef(
-    _RequiredContinuousParameterRangeOutputTypeDef, _OptionalContinuousParameterRangeOutputTypeDef
-):
-    pass
-
 _RequiredContinuousParameterRangeTypeDef = TypedDict(
     "_RequiredContinuousParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": float,
         "MinValue": float,
     },
@@ -431,161 +387,42 @@
         "DayOfMonth": int,
         "DayOfWeek": DayOfWeekType,
         "Hour": int,
     },
     total=False,
 )
 
-CreateAutoPredictorResponseTypeDef = TypedDict(
-    "CreateAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "DatasetImportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateExplainabilityExportResponseTypeDef = TypedDict(
-    "CreateExplainabilityExportResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ExplainabilityExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ExplainabilityConfigTypeDef = TypedDict(
     "ExplainabilityConfigTypeDef",
     {
         "TimeSeriesGranularity": TimeSeriesGranularityType,
         "TimePointGranularity": TimePointGranularityType,
     },
 )
 
-CreateExplainabilityResponseTypeDef = TypedDict(
-    "CreateExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastExportJobResponseTypeDef = TypedDict(
-    "CreateForecastExportJobResponseTypeDef",
-    {
-        "ForecastExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastResponseTypeDef = TypedDict(
-    "CreateForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMonitorResponseTypeDef = TypedDict(
-    "CreateMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    {
-        "PredictorBacktestExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluationParametersTypeDef = TypedDict(
     "EvaluationParametersTypeDef",
     {
         "NumberOfBacktestWindows": int,
         "BackTestWindowOffset": int,
     },
     total=False,
 )
 
-CreatePredictorResponseTypeDef = TypedDict(
-    "CreatePredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfAnalysisResponseTypeDef = TypedDict(
-    "CreateWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastExportResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastExportResponseTypeDef",
-    {
-        "WhatIfForecastExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredS3ConfigOutputTypeDef = TypedDict(
-    "_RequiredS3ConfigOutputTypeDef",
-    {
-        "Path": str,
-        "RoleArn": str,
-    },
-)
-_OptionalS3ConfigOutputTypeDef = TypedDict(
-    "_OptionalS3ConfigOutputTypeDef",
-    {
-        "KMSKeyArn": str,
-    },
-    total=False,
-)
-
-class S3ConfigOutputTypeDef(_RequiredS3ConfigOutputTypeDef, _OptionalS3ConfigOutputTypeDef):
-    pass
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -725,22 +562,14 @@
 DescribeAutoPredictorRequestRequestTypeDef = TypedDict(
     "DescribeAutoPredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
-EncryptionConfigOutputTypeDef = TypedDict(
-    "EncryptionConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "KMSKeyArn": str,
-    },
-)
-
 ExplainabilityInfoTypeDef = TypedDict(
     "ExplainabilityInfoTypeDef",
     {
         "ExplainabilityArn": str,
         "Status": str,
     },
     total=False,
@@ -760,46 +589,21 @@
     {
         "Arn": str,
         "State": StateType,
     },
     total=False,
 )
 
-TimeAlignmentBoundaryOutputTypeDef = TypedDict(
-    "TimeAlignmentBoundaryOutputTypeDef",
-    {
-        "Month": MonthType,
-        "DayOfMonth": int,
-        "DayOfWeek": DayOfWeekType,
-        "Hour": int,
-    },
-    total=False,
-)
-
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupName": str,
-        "DatasetGroupArn": str,
-        "DatasetArns": List[str],
-        "Domain": DomainType,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetImportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetImportJobRequestRequestTypeDef",
     {
         "DatasetImportJobArn": str,
     },
 )
 
@@ -839,22 +643,14 @@
 DescribeExplainabilityRequestRequestTypeDef = TypedDict(
     "DescribeExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityArn": str,
     },
 )
 
-ExplainabilityConfigOutputTypeDef = TypedDict(
-    "ExplainabilityConfigOutputTypeDef",
-    {
-        "TimeSeriesGranularity": TimeSeriesGranularityType,
-        "TimePointGranularity": TimePointGranularityType,
-    },
-)
-
 DescribeForecastExportJobRequestRequestTypeDef = TypedDict(
     "DescribeForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobArn": str,
     },
 )
 
@@ -882,23 +678,14 @@
 DescribePredictorRequestRequestTypeDef = TypedDict(
     "DescribePredictorRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
-EvaluationParametersOutputTypeDef = TypedDict(
-    "EvaluationParametersOutputTypeDef",
-    {
-        "NumberOfBacktestWindows": int,
-        "BackTestWindowOffset": int,
-    },
-    total=False,
-)
-
 DescribeWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisArn": str,
     },
 )
 
@@ -912,21 +699,14 @@
 DescribeWhatIfForecastRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorMetricTypeDef = TypedDict(
     "ErrorMetricTypeDef",
     {
         "ForecastType": str,
         "WAPE": float,
         "RMSE": float,
         "MASE": float,
@@ -1001,51 +781,22 @@
 GetAccuracyMetricsRequestRequestTypeDef = TypedDict(
     "GetAccuracyMetricsRequestRequestTypeDef",
     {
         "PredictorArn": str,
     },
 )
 
-SupplementaryFeatureOutputTypeDef = TypedDict(
-    "SupplementaryFeatureOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 SupplementaryFeatureTypeDef = TypedDict(
     "SupplementaryFeatureTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-_RequiredIntegerParameterRangeOutputTypeDef = TypedDict(
-    "_RequiredIntegerParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "MaxValue": int,
-        "MinValue": int,
-    },
-)
-_OptionalIntegerParameterRangeOutputTypeDef = TypedDict(
-    "_OptionalIntegerParameterRangeOutputTypeDef",
-    {
-        "ScalingType": ScalingTypeType,
-    },
-    total=False,
-)
-
-class IntegerParameterRangeOutputTypeDef(
-    _RequiredIntegerParameterRangeOutputTypeDef, _OptionalIntegerParameterRangeOutputTypeDef
-):
-    pass
-
 _RequiredIntegerParameterRangeTypeDef = TypedDict(
     "_RequiredIntegerParameterRangeTypeDef",
     {
         "Name": str,
         "MaxValue": int,
         "MinValue": int,
     },
@@ -1059,39 +810,33 @@
 )
 
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
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
 
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1113,22 +858,14 @@
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
 WhatIfAnalysisSummaryTypeDef = TypedDict(
     "WhatIfAnalysisSummaryTypeDef",
     {
         "WhatIfAnalysisArn": str,
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
         "Status": str,
@@ -1177,24 +914,14 @@
         "DatasetImportJobArn": str,
         "ForecastArn": str,
         "PredictorArn": str,
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
 PredictorEventTypeDef = TypedDict(
     "PredictorEventTypeDef",
     {
         "Detail": str,
         "Datetime": datetime,
     },
     total=False,
@@ -1207,41 +934,21 @@
         "TestWindowEnd": datetime,
         "Status": str,
         "Message": str,
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
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-SchemaAttributeOutputTypeDef = TypedDict(
-    "SchemaAttributeOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": AttributeTypeType,
-    },
-    total=False,
-)
-
 SchemaAttributeTypeDef = TypedDict(
     "SchemaAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeType": AttributeTypeType,
     },
     total=False,
@@ -1250,23 +957,14 @@
 StopResourceRequestRequestTypeDef = TypedDict(
     "StopResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TimeSeriesConditionOutputTypeDef = TypedDict(
-    "TimeSeriesConditionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeValue": str,
-        "Condition": ConditionType,
-    },
-)
-
 TimeSeriesConditionTypeDef = TypedDict(
     "TimeSeriesConditionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
         "Condition": ConditionType,
     },
@@ -1378,28 +1076,170 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DataDestinationOutputTypeDef = TypedDict(
-    "DataDestinationOutputTypeDef",
+CreateAutoPredictorResponseTypeDef = TypedDict(
+    "CreateAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "DatasetImportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateExplainabilityExportResponseTypeDef = TypedDict(
+    "CreateExplainabilityExportResponseTypeDef",
+    {
+        "ExplainabilityExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateExplainabilityResponseTypeDef = TypedDict(
+    "CreateExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastExportJobResponseTypeDef = TypedDict(
+    "CreateForecastExportJobResponseTypeDef",
+    {
+        "ForecastExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastResponseTypeDef = TypedDict(
+    "CreateForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMonitorResponseTypeDef = TypedDict(
+    "CreateMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    {
+        "PredictorBacktestExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorResponseTypeDef = TypedDict(
+    "CreatePredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfAnalysisResponseTypeDef = TypedDict(
+    "CreateWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastExportResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastExportResponseTypeDef",
+    {
+        "WhatIfForecastExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupName": str,
+        "DatasetGroupArn": str,
+        "DatasetArns": List[str],
+        "Domain": DomainType,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
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
+ExplainabilitySummaryTypeDef = TypedDict(
+    "ExplainabilitySummaryTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+    },
+    total=False,
+)
+
 DataDestinationTypeDef = TypedDict(
     "DataDestinationTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
 )
 
@@ -1411,24 +1251,24 @@
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "DatasetGroups": List[DatasetGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorSummaryTypeDef = TypedDict(
     "PredictorSummaryTypeDef",
     {
         "PredictorArn": str,
@@ -1440,29 +1280,14 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
-ExplainabilitySummaryTypeDef = TypedDict(
-    "ExplainabilitySummaryTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredFeaturizationOutputTypeDef = TypedDict(
     "_RequiredFeaturizationOutputTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationOutputTypeDef = TypedDict(
@@ -1491,130 +1316,64 @@
     },
     total=False,
 )
 
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExplainabilitiesRequestRequestTypeDef = TypedDict(
     "ListExplainabilitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
     "ListExplainabilityExportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListForecastExportJobsRequestRequestTypeDef = TypedDict(
     "ListForecastExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
-    "ListForecastsRequestListForecastsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListForecastsRequestRequestTypeDef = TypedDict(
     "ListForecastsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    {
-        "MonitorArn": str,
-    },
-)
-_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
-    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
 )
 _OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
@@ -1629,118 +1388,64 @@
 
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMonitorsRequestRequestTypeDef = TypedDict(
     "ListMonitorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPredictorsRequestRequestTypeDef = TypedDict(
     "ListPredictorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
     "ListWhatIfAnalysesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
     "ListWhatIfForecastExportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
     "ListWhatIfForecastsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1748,28 +1453,28 @@
 )
 
 ListForecastsResponseTypeDef = TypedDict(
     "ListForecastsResponseTypeDef",
     {
         "Forecasts": List[ForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInputDataConfigOutputTypeDef = TypedDict(
     "_RequiredInputDataConfigOutputTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigOutputTypeDef = TypedDict(
     "_OptionalInputDataConfigOutputTypeDef",
     {
-        "SupplementaryFeatures": List[SupplementaryFeatureOutputTypeDef],
+        "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
 class InputDataConfigOutputTypeDef(
     _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
 ):
@@ -1792,62 +1497,190 @@
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
 ParameterRangesOutputTypeDef = TypedDict(
     "ParameterRangesOutputTypeDef",
     {
         "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
-        "ContinuousParameterRanges": List[ContinuousParameterRangeOutputTypeDef],
-        "IntegerParameterRanges": List[IntegerParameterRangeOutputTypeDef],
+        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMonitorsResponseTypeDef = TypedDict(
-    "ListMonitorsResponseTypeDef",
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
-        "Monitors": List[MonitorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
+    "ListForecastsRequestListForecastsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    {
+        "MonitorArn": str,
+    },
+)
+_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
+    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+):
+    pass
+
+ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMonitorsResponseTypeDef = TypedDict(
+    "ListMonitorsResponseTypeDef",
+    {
+        "Monitors": List[MonitorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastsResponseTypeDef = TypedDict(
     "ListWhatIfForecastsResponseTypeDef",
     {
         "WhatIfForecasts": List[WhatIfForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsTypeDef = TypedDict(
     "MetricsTypeDef",
     {
         "RMSE": float,
@@ -1884,15 +1717,15 @@
     },
     total=False,
 )
 
 SchemaOutputTypeDef = TypedDict(
     "SchemaOutputTypeDef",
     {
-        "Attributes": List[SchemaAttributeOutputTypeDef],
+        "Attributes": List[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
@@ -1900,16 +1733,16 @@
     },
     total=False,
 )
 
 TimeSeriesTransformationOutputTypeDef = TypedDict(
     "TimeSeriesTransformationOutputTypeDef",
     {
-        "Action": ActionOutputTypeDef,
-        "TimeSeriesConditions": List[TimeSeriesConditionOutputTypeDef],
+        "Action": ActionTypeDef,
+        "TimeSeriesConditions": List[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
 TimeSeriesTransformationTypeDef = TypedDict(
     "TimeSeriesTransformationTypeDef",
     {
@@ -1926,26 +1759,26 @@
         "PredictorName": str,
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "ForecastFrequency": str,
         "ForecastDimensions": List[str],
         "DatasetImportJobArns": List[str],
         "DataConfig": DataConfigOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
         "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ExplainabilityInfo": ExplainabilityInfoTypeDef,
         "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
@@ -1980,142 +1813,271 @@
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
 
+ListExplainabilitiesResponseTypeDef = TypedDict(
+    "ListExplainabilitiesResponseTypeDef",
+    {
+        "Explainabilities": List[ExplainabilitySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "ExplainabilityExportName": str,
+        "ExplainabilityArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreateExplainabilityExportRequestRequestTypeDef(
+    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
+    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "ForecastExportJobName": str,
+        "ForecastArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreateForecastExportJobRequestRequestTypeDef(
+    _RequiredCreateForecastExportJobRequestRequestTypeDef,
+    _OptionalCreateForecastExportJobRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "PredictorBacktestExportJobName": str,
+        "PredictorArn": str,
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreatePredictorBacktestExportJobRequestRequestTypeDef(
+    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
+    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "WhatIfForecastExportName": str,
+        "WhatIfForecastArns": Sequence[str],
+        "Destination": DataDestinationTypeDef,
+    },
+)
+_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+    },
+    total=False,
+)
+
+class CreateWhatIfForecastExportRequestRequestTypeDef(
+    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
+    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
+):
+    pass
+
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
         "ForecastArn": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": List[str],
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 ForecastExportJobSummaryTypeDef = TypedDict(
     "ForecastExportJobSummaryTypeDef",
     {
         "ForecastExportJobArn": str,
         "ForecastExportJobName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 PredictorBacktestExportJobSummaryTypeDef = TypedDict(
     "PredictorBacktestExportJobSummaryTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
         "PredictorBacktestExportJobName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
 WhatIfForecastExportSummaryTypeDef = TypedDict(
     "WhatIfForecastExportSummaryTypeDef",
     {
         "WhatIfForecastExportArn": str,
         "WhatIfForecastArns": List[str],
         "WhatIfForecastExportName": str,
-        "Destination": DataDestinationOutputTypeDef,
+        "Destination": DataDestinationTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
+_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
+    {
+        "DatasetImportJobName": str,
+        "DatasetArn": str,
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
+    {
+        "TimestampFormat": str,
+        "TimeZone": str,
+        "UseGeolocationForTimeZone": bool,
+        "GeolocationFormat": str,
+        "Tags": Sequence[TagTypeDef],
+        "Format": str,
+        "ImportMode": ImportModeType,
+    },
+    total=False,
+)
+
+class CreateDatasetImportJobRequestRequestTypeDef(
+    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
+    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
+):
+    pass
+
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "ImportMode": ImportModeType,
     },
     total=False,
@@ -2127,163 +2089,34 @@
         "DatasetImportJobName": str,
         "DatasetImportJobArn": str,
         "DatasetArn": str,
         "TimestampFormat": str,
         "TimeZone": str,
         "UseGeolocationForTimeZone": bool,
         "GeolocationFormat": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "FieldStatistics": Dict[str, StatisticsTypeDef],
         "DataSize": float,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
-    {
-        "ExplainabilityExportName": str,
-        "ExplainabilityArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateExplainabilityExportRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-class CreateExplainabilityExportRequestRequestTypeDef(
-    _RequiredCreateExplainabilityExportRequestRequestTypeDef,
-    _OptionalCreateExplainabilityExportRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "ForecastExportJobName": str,
-        "ForecastArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateForecastExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateForecastExportJobRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-class CreateForecastExportJobRequestRequestTypeDef(
-    _RequiredCreateForecastExportJobRequestRequestTypeDef,
-    _OptionalCreateForecastExportJobRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
-    {
-        "PredictorBacktestExportJobName": str,
-        "PredictorArn": str,
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-class CreatePredictorBacktestExportJobRequestRequestTypeDef(
-    _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
-    _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
-    {
-        "WhatIfForecastExportName": str,
-        "WhatIfForecastArns": Sequence[str],
-        "Destination": DataDestinationTypeDef,
-    },
-)
-_OptionalCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWhatIfForecastExportRequestRequestTypeDef",
-    {
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-    },
-    total=False,
-)
-
-class CreateWhatIfForecastExportRequestRequestTypeDef(
-    _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
-    _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetImportJobRequestRequestTypeDef",
-    {
-        "DatasetImportJobName": str,
-        "DatasetArn": str,
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalCreateDatasetImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetImportJobRequestRequestTypeDef",
-    {
-        "TimestampFormat": str,
-        "TimeZone": str,
-        "UseGeolocationForTimeZone": bool,
-        "GeolocationFormat": str,
-        "Tags": Sequence[TagTypeDef],
-        "Format": str,
-        "ImportMode": ImportModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateDatasetImportJobRequestRequestTypeDef(
-    _RequiredCreateDatasetImportJobRequestRequestTypeDef,
-    _OptionalCreateDatasetImportJobRequestRequestTypeDef,
-):
-    pass
-
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListExplainabilitiesResponseTypeDef = TypedDict(
-    "ListExplainabilitiesResponseTypeDef",
-    {
-        "Explainabilities": List[ExplainabilitySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFeaturizationConfigOutputTypeDef = TypedDict(
     "_RequiredFeaturizationConfigOutputTypeDef",
     {
         "ForecastFrequency": str,
@@ -2352,15 +2185,15 @@
 )
 
 ListMonitorEvaluationsResponseTypeDef = TypedDict(
     "ListMonitorEvaluationsResponseTypeDef",
     {
         "NextToken": str,
         "PredictorMonitorEvaluations": List[PredictorMonitorEvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorExecutionDetailsTypeDef = TypedDict(
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
@@ -2373,57 +2206,57 @@
     {
         "DatasetArn": str,
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "DataFrequency": str,
         "Schema": SchemaOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExplainabilityResponseTypeDef = TypedDict(
     "DescribeExplainabilityResponseTypeDef",
     {
         "ExplainabilityArn": str,
         "ExplainabilityName": str,
         "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigOutputTypeDef,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
         "EnableVisualization": bool,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Schema": SchemaOutputTypeDef,
         "StartDateTime": str,
         "EndDateTime": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesIdentifiersOutputTypeDef = TypedDict(
     "TimeSeriesIdentifiersOutputTypeDef",
     {
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Schema": SchemaOutputTypeDef,
         "Format": str,
     },
     total=False,
 )
 
 _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
     "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "S3Config": S3ConfigTypeDef,
         "Schema": SchemaOutputTypeDef,
     },
 )
 _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
     "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
     {
         "Format": str,
@@ -2531,60 +2364,60 @@
         "LastEvaluationTime": datetime,
         "LastEvaluationState": str,
         "Baseline": BaselineTypeDef,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "EstimatedEvaluationTimeRemainingInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExplainabilityExportsResponseTypeDef = TypedDict(
     "ListExplainabilityExportsResponseTypeDef",
     {
         "ExplainabilityExports": List[ExplainabilityExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListForecastExportJobsResponseTypeDef = TypedDict(
     "ListForecastExportJobsResponseTypeDef",
     {
         "ForecastExportJobs": List[ForecastExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPredictorBacktestExportJobsResponseTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsResponseTypeDef",
     {
         "PredictorBacktestExportJobs": List[PredictorBacktestExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastExportsResponseTypeDef = TypedDict(
     "ListWhatIfForecastExportsResponseTypeDef",
     {
         "WhatIfForecastExports": List[WhatIfForecastExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
@@ -2634,29 +2467,29 @@
         "AutoMLAlgorithmArns": List[str],
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
-        "EvaluationParameters": EvaluationParametersOutputTypeDef,
+        "EvaluationParameters": EvaluationParametersTypeDef,
         "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
         "InputDataConfig": InputDataConfigOutputTypeDef,
         "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesSelectorOutputTypeDef = TypedDict(
     "TimeSeriesSelectorOutputTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
@@ -2674,15 +2507,15 @@
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
         "ForecastTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
@@ -2716,15 +2549,15 @@
 GetAccuracyMetricsResponseTypeDef = TypedDict(
     "GetAccuracyMetricsResponseTypeDef",
     {
         "PredictorEvaluationResults": List[EvaluationResultTypeDef],
         "IsAutoPredictor": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeForecastResponseTypeDef = TypedDict(
     "DescribeForecastResponseTypeDef",
     {
         "ForecastArn": str,
@@ -2734,15 +2567,15 @@
         "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
     "DescribeWhatIfAnalysisResponseTypeDef",
     {
         "WhatIfAnalysisName": str,
@@ -2750,15 +2583,15 @@
         "ForecastArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
         "ForecastName": str,
```

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/PKG-INFO` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.28.12
-Summary: Type annotations for boto3.ForecastService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,46 +396,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
-    ActionOutputTypeDef,
     ActionTypeDef,
     AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
     AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
     CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
-    ContinuousParameterRangeOutputTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
+    ResponseMetadataTypeDef,
     ExplainabilityConfigTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
-    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -446,147 +430,149 @@
     DeletePredictorBacktestExportJobRequestRequestTypeDef,
     DeletePredictorRequestRequestTypeDef,
     DeleteResourceTreeRequestRequestTypeDef,
     DeleteWhatIfAnalysisRequestRequestTypeDef,
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
-    EncryptionConfigOutputTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
-    TimeAlignmentBoundaryOutputTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
-    ExplainabilityConfigOutputTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
-    EvaluationParametersOutputTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
     FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
-    SupplementaryFeatureOutputTypeDef,
     SupplementaryFeatureTypeDef,
-    IntegerParameterRangeOutputTypeDef,
     IntegerParameterRangeTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
-    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
-    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
-    SchemaAttributeOutputTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
-    TimeSeriesConditionOutputTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
     DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    DataDestinationOutputTypeDef,
-    DataSourceOutputTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
-    ExplainabilitySummaryTypeDef,
     FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
     InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     CreateAutoPredictorRequestRequestTypeDef,
     BaselineTypeDef,
+    ListExplainabilitiesResponseTypeDef,
+    CreateExplainabilityExportRequestRequestTypeDef,
+    CreateForecastExportJobRequestRequestTypeDef,
+    CreatePredictorBacktestExportJobRequestRequestTypeDef,
+    CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
     DescribeForecastExportJobResponseTypeDef,
     DescribePredictorBacktestExportJobResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     ExplainabilityExportSummaryTypeDef,
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
+    CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
-    CreateExplainabilityExportRequestRequestTypeDef,
-    CreateForecastExportJobRequestRequestTypeDef,
-    CreatePredictorBacktestExportJobRequestRequestTypeDef,
-    CreateWhatIfForecastExportRequestRequestTypeDef,
-    CreateDatasetImportJobRequestRequestTypeDef,
     ListPredictorsResponseTypeDef,
-    ListExplainabilitiesResponseTypeDef,
     FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
     HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
@@ -615,15 +601,15 @@
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
     CreateForecastRequestRequestTypeDef,
     CreateWhatIfAnalysisRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionOutputTypeDef:
+def get_structure() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.12/mypy_boto3_forecast.egg-info/SOURCES.txt` & `mypy-boto3-forecast-1.28.15/mypy_boto3_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.12/setup.py` & `mypy-boto3-forecast-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-forecast",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ForecastService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ForecastService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

