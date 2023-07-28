# Comparing `tmp/mypy-boto3-lookoutmetrics-1.28.12.tar.gz` & `tmp/mypy-boto3-lookoutmetrics-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
```

## Comparing `mypy-boto3-lookoutmetrics-1.28.12.tar` & `mypy-boto3-lookoutmetrics-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.888453 mypy-boto3-lookoutmetrics-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-27 05:34:57.884453 mypy-boto3-lookoutmetrics-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.884453 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42825 2023-07-27 05:25:38.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42788 2023-07-27 05:25:38.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.884453 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:57.000000 mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.888453 mypy-boto3-lookoutmetrics-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:25:37.000000 mypy-boto3-lookoutmetrics-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.773426 mypy-boto3-lookoutmetrics-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-07-28 20:43:11.769426 mypy-boto3-lookoutmetrics-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.765426 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39698 2023-07-28 20:30:36.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39665 2023-07-28 20:30:35.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.765426 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:11.000000 mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.773426 mypy-boto3-lookoutmetrics-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:30:34.000000 mypy-boto3-lookoutmetrics-1.28.15/setup.py
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/LICENSE` & `mypy-boto3-lookoutmetrics-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.28.12
-Summary: Type annotations for boto3.LookoutMetrics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,100 +311,89 @@
 ### Typed dictionaries
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
-    LambdaConfigurationOutputTypeDef,
-    SNSConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
     DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
-    AppFlowConfigOutputTypeDef,
     AppFlowConfigTypeDef,
-    BackTestConfigurationOutputTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
-    CreateMetricSetResponseTypeDef,
     CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     ExecutionStatusTypeDef,
     DescribeAnomalyDetectorRequestRequestTypeDef,
     DescribeMetricSetRequestRequestTypeDef,
-    MetricOutputTypeDef,
-    TimestampColumnOutputTypeDef,
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
-    JsonFormatDescriptorOutputTypeDef,
     JsonFormatDescriptorTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
-    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
     AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
-    ListAlertsResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
-    AthenaSourceConfigOutputTypeDef,
-    CloudWatchConfigOutputTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
+    CreateMetricSetResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
+    GetSampleDataResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
     FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
     MetricSetDimensionFilterOutputTypeDef,
@@ -444,15 +433,15 @@
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationOutputTypeDef:
+def get_structure() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/README.md` & `mypy-boto3-lookoutmetrics-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,100 +279,89 @@
 ### Typed dictionaries
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
-    LambdaConfigurationOutputTypeDef,
-    SNSConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
     DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
-    AppFlowConfigOutputTypeDef,
     AppFlowConfigTypeDef,
-    BackTestConfigurationOutputTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
-    CreateMetricSetResponseTypeDef,
     CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     ExecutionStatusTypeDef,
     DescribeAnomalyDetectorRequestRequestTypeDef,
     DescribeMetricSetRequestRequestTypeDef,
-    MetricOutputTypeDef,
-    TimestampColumnOutputTypeDef,
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
-    JsonFormatDescriptorOutputTypeDef,
     JsonFormatDescriptorTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
-    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
     AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
-    ListAlertsResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
-    AthenaSourceConfigOutputTypeDef,
-    CloudWatchConfigOutputTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
+    CreateMetricSetResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
+    GetSampleDataResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
     FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
     MetricSetDimensionFilterOutputTypeDef,
@@ -412,15 +401,15 @@
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationOutputTypeDef:
+def get_structure() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/__main__.py` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutMetrics 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LookoutMetrics 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.py` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/client.pyi` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.py` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/literals.pyi` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.py` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lookoutmetrics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationOutputTypeDef
+    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
-    data: LambdaConfigurationOutputTypeDef = {...}
+    data: LambdaConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,102 +36,90 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "LambdaConfigurationOutputTypeDef",
-    "SNSConfigurationOutputTypeDef",
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
-    "AppFlowConfigOutputTypeDef",
     "AppFlowConfigTypeDef",
-    "BackTestConfigurationOutputTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
-    "CreateAlertResponseTypeDef",
-    "CreateAnomalyDetectorResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
-    "CreateMetricSetResponseTypeDef",
     "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
     "ExecutionStatusTypeDef",
     "DescribeAnomalyDetectorRequestRequestTypeDef",
     "DescribeMetricSetRequestRequestTypeDef",
-    "MetricOutputTypeDef",
-    "TimestampColumnOutputTypeDef",
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
-    "JsonFormatDescriptorOutputTypeDef",
     "JsonFormatDescriptorTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
-    "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlertResponseTypeDef",
-    "UpdateAnomalyDetectorResponseTypeDef",
-    "UpdateMetricSetResponseTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
-    "ListAlertsResponseTypeDef",
-    "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
-    "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
-    "AthenaSourceConfigOutputTypeDef",
-    "CloudWatchConfigOutputTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
+    "CreateAlertResponseTypeDef",
+    "CreateAnomalyDetectorResponseTypeDef",
+    "CreateMetricSetResponseTypeDef",
+    "DescribeAnomalyDetectorResponseTypeDef",
+    "GetSampleDataResponseTypeDef",
+    "ListAlertsResponseTypeDef",
+    "ListAnomalyDetectorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateAlertResponseTypeDef",
+    "UpdateAnomalyDetectorResponseTypeDef",
+    "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
     "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
     "MetricSetDimensionFilterOutputTypeDef",
@@ -170,44 +158,14 @@
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
-LambdaConfigurationOutputTypeDef = TypedDict(
-    "LambdaConfigurationOutputTypeDef",
-    {
-        "RoleArn": str,
-        "LambdaArn": str,
-    },
-)
-
-_RequiredSNSConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSNSConfigurationOutputTypeDef",
-    {
-        "RoleArn": str,
-        "SnsTopicArn": str,
-    },
-)
-_OptionalSNSConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSNSConfigurationOutputTypeDef",
-    {
-        "SnsFormat": SnsFormatType,
-    },
-    total=False,
-)
-
-
-class SNSConfigurationOutputTypeDef(
-    _RequiredSNSConfigurationOutputTypeDef, _OptionalSNSConfigurationOutputTypeDef
-):
-    pass
-
-
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "RoleArn": str,
         "LambdaArn": str,
     },
 )
@@ -223,19 +181,17 @@
     "_OptionalSNSConfigurationTypeDef",
     {
         "SnsFormat": SnsFormatType,
     },
     total=False,
 )
 
-
 class SNSConfigurationTypeDef(_RequiredSNSConfigurationTypeDef, _OptionalSNSConfigurationTypeDef):
     pass
 
-
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
@@ -343,46 +299,28 @@
     "_OptionalAnomalyGroupTimeSeriesTypeDef",
     {
         "TimeSeriesId": str,
     },
     total=False,
 )
 
-
 class AnomalyGroupTimeSeriesTypeDef(
     _RequiredAnomalyGroupTimeSeriesTypeDef, _OptionalAnomalyGroupTimeSeriesTypeDef
 ):
     pass
 
-
-AppFlowConfigOutputTypeDef = TypedDict(
-    "AppFlowConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "FlowName": str,
-    },
-    total=False,
-)
-
 AppFlowConfigTypeDef = TypedDict(
     "AppFlowConfigTypeDef",
     {
         "RoleArn": str,
         "FlowName": str,
     },
     total=False,
 )
 
-BackTestConfigurationOutputTypeDef = TypedDict(
-    "BackTestConfigurationOutputTypeDef",
-    {
-        "RunBackTestMode": bool,
-    },
-)
-
 BackTestConfigurationTypeDef = TypedDict(
     "BackTestConfigurationTypeDef",
     {
         "RunBackTestMode": bool,
     },
 )
 
@@ -411,27 +349,22 @@
 BackTestAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-CreateAlertResponseTypeDef = TypedDict(
-    "CreateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalyDetectorResponseTypeDef = TypedDict(
-    "CreateAnomalyDetectorResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "MetricName": str,
@@ -442,36 +375,26 @@
     "_OptionalMetricTypeDef",
     {
         "Namespace": str,
     },
     total=False,
 )
 
-
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
-
 TimestampColumnTypeDef = TypedDict(
     "TimestampColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
-CreateMetricSetResponseTypeDef = TypedDict(
-    "CreateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CsvFormatDescriptorOutputTypeDef = TypedDict(
     "CsvFormatDescriptorOutputTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -545,22 +468,20 @@
         "Timestamp": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAnomalyDetectionExecutionsRequestRequestTypeDef(
     _RequiredDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     _OptionalDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 ExecutionStatusTypeDef = TypedDict(
     "ExecutionStatusTypeDef",
     {
         "Timestamp": str,
         "Status": AnomalyDetectionTaskStatusType,
         "FailureReason": str,
     },
@@ -577,43 +498,14 @@
 DescribeMetricSetRequestRequestTypeDef = TypedDict(
     "DescribeMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 
-_RequiredMetricOutputTypeDef = TypedDict(
-    "_RequiredMetricOutputTypeDef",
-    {
-        "MetricName": str,
-        "AggregationFunction": AggregationFunctionType,
-    },
-)
-_OptionalMetricOutputTypeDef = TypedDict(
-    "_OptionalMetricOutputTypeDef",
-    {
-        "Namespace": str,
-    },
-    total=False,
-)
-
-
-class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
-    pass
-
-
-TimestampColumnOutputTypeDef = TypedDict(
-    "TimestampColumnOutputTypeDef",
-    {
-        "ColumnName": str,
-        "ColumnFormat": str,
-    },
-    total=False,
-)
-
 DimensionValueContributionTypeDef = TypedDict(
     "DimensionValueContributionTypeDef",
     {
         "DimensionValue": str,
         "ContributionScore": float,
     },
     total=False,
@@ -623,41 +515,23 @@
     "DimensionNameValueTypeDef",
     {
         "DimensionName": str,
         "DimensionValue": str,
     },
 )
 
-JsonFormatDescriptorOutputTypeDef = TypedDict(
-    "JsonFormatDescriptorOutputTypeDef",
-    {
-        "FileCompression": JsonFileCompressionType,
-        "Charset": str,
-    },
-    total=False,
-)
-
 JsonFormatDescriptorTypeDef = TypedDict(
     "JsonFormatDescriptorTypeDef",
     {
         "FileCompression": JsonFileCompressionType,
         "Charset": str,
     },
     total=False,
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "DimensionValue": str,
-        "FilterOperation": Literal["EQUALS"],
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "DimensionValue": str,
         "FilterOperation": Literal["EQUALS"],
     },
     total=False,
@@ -681,40 +555,29 @@
     "_OptionalGetDataQualityMetricsRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
     total=False,
 )
 
-
 class GetDataQualityMetricsRequestRequestTypeDef(
     _RequiredGetDataQualityMetricsRequestRequestTypeDef,
     _OptionalGetDataQualityMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 TimeSeriesFeedbackTypeDef = TypedDict(
     "TimeSeriesFeedbackTypeDef",
     {
         "TimeSeriesId": str,
         "IsAnomaly": bool,
     },
     total=False,
 )
 
-GetSampleDataResponseTypeDef = TypedDict(
-    "GetSampleDataResponseTypeDef",
-    {
-        "HeaderValues": List[str],
-        "SampleRows": List[List[str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InterMetricImpactDetailsTypeDef = TypedDict(
     "InterMetricImpactDetailsTypeDef",
     {
         "MetricName": str,
         "AnomalyGroupId": str,
         "RelationshipType": RelationshipTypeType,
         "ContributionPercentage": float,
@@ -754,22 +617,20 @@
         "RelationshipTypeFilter": RelationshipTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalyGroupRelatedMetricsRequestRequestTypeDef(
     _RequiredListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     _OptionalListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAnomalyGroupSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupSummariesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "SensitivityThreshold": int,
     },
 )
@@ -778,22 +639,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalyGroupSummariesRequestRequestTypeDef(
     _RequiredListAnomalyGroupSummariesRequestRequestTypeDef,
     _OptionalListAnomalyGroupSummariesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "AnomalyGroupId": str,
         "MetricName": str,
     },
@@ -803,22 +662,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalyGroupTimeSeriesRequestRequestTypeDef(
     _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     _OptionalListAnomalyGroupTimeSeriesRequestRequestTypeDef,
 ):
     pass
 
-
 ListMetricSetsRequestRequestTypeDef = TypedDict(
     "ListMetricSetsRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -842,22 +699,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 VpcConfigurationOutputTypeDef = TypedDict(
     "VpcConfigurationOutputTypeDef",
     {
         "SubnetIdList": List[str],
         "SecurityGroupIdList": List[str],
     },
 )
@@ -866,25 +715,14 @@
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -893,47 +731,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAlertResponseTypeDef = TypedDict(
-    "UpdateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalyDetectorResponseTypeDef = TypedDict(
-    "UpdateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMetricSetResponseTypeDef = TypedDict(
-    "UpdateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "SNSConfiguration": SNSConfigurationOutputTypeDef,
-        "LambdaConfiguration": LambdaConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
@@ -953,40 +758,14 @@
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
 )
 
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "AlertSummaryList": List[AlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAnomalyDetectorResponseTypeDef = TypedDict(
-    "DescribeAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "AnomalyDetectorName": str,
-        "AnomalyDetectorDescription": str,
-        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Status": AnomalyDetectorStatusType,
-        "FailureReason": str,
-        "KmsKeyArn": str,
-        "FailureType": AnomalyDetectorFailureTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorName": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
 )
@@ -996,22 +775,20 @@
         "AnomalyDetectorDescription": str,
         "KmsKeyArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAnomalyDetectorRequestRequestTypeDef(
     _RequiredCreateAnomalyDetectorRequestRequestTypeDef,
     _OptionalCreateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 _OptionalUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
@@ -1020,31 +797,20 @@
         "KmsKeyArn": str,
         "AnomalyDetectorDescription": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAnomalyDetectorRequestRequestTypeDef(
     _RequiredUpdateAnomalyDetectorRequestRequestTypeDef,
     _OptionalUpdateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
-
-ListAnomalyDetectorsResponseTypeDef = TypedDict(
-    "ListAnomalyDetectorsResponseTypeDef",
-    {
-        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnomalyGroupStatisticsTypeDef = TypedDict(
     "AnomalyGroupStatisticsTypeDef",
     {
         "EvaluationStartDate": str,
         "TotalCount": int,
         "ItemizedMetricStatsList": List[ItemizedMetricStatsTypeDef],
     },
@@ -1071,44 +837,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetFeedbackRequestRequestTypeDef(
     _RequiredGetFeedbackRequestRequestTypeDef, _OptionalGetFeedbackRequestRequestTypeDef
 ):
     pass
 
-
-AthenaSourceConfigOutputTypeDef = TypedDict(
-    "AthenaSourceConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "DatabaseName": str,
-        "DataCatalog": str,
-        "TableName": str,
-        "WorkGroupName": str,
-        "S3ResultsPath": str,
-        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-CloudWatchConfigOutputTypeDef = TypedDict(
-    "CloudWatchConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 AthenaSourceConfigTypeDef = TypedDict(
     "AthenaSourceConfigTypeDef",
     {
         "RoleArn": str,
         "DatabaseName": str,
         "DataCatalog": str,
         "TableName": str,
@@ -1142,29 +883,129 @@
     "AutoDetectionMetricSourceTypeDef",
     {
         "S3SourceConfig": AutoDetectionS3SourceConfigTypeDef,
     },
     total=False,
 )
 
+CreateAlertResponseTypeDef = TypedDict(
+    "CreateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalyDetectorResponseTypeDef = TypedDict(
+    "CreateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMetricSetResponseTypeDef = TypedDict(
+    "CreateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAnomalyDetectorResponseTypeDef = TypedDict(
+    "DescribeAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "AnomalyDetectorName": str,
+        "AnomalyDetectorDescription": str,
+        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Status": AnomalyDetectorStatusType,
+        "FailureReason": str,
+        "KmsKeyArn": str,
+        "FailureType": AnomalyDetectorFailureTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSampleDataResponseTypeDef = TypedDict(
+    "GetSampleDataResponseTypeDef",
+    {
+        "HeaderValues": List[str],
+        "SampleRows": List[List[str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "AlertSummaryList": List[AlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAnomalyDetectorsResponseTypeDef = TypedDict(
+    "ListAnomalyDetectorsResponseTypeDef",
+    {
+        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlertResponseTypeDef = TypedDict(
+    "UpdateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyDetectorResponseTypeDef = TypedDict(
+    "UpdateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMetricSetResponseTypeDef = TypedDict(
+    "UpdateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MetricSetDataQualityMetricTypeDef = TypedDict(
     "MetricSetDataQualityMetricTypeDef",
     {
         "MetricSetArn": str,
         "DataQualityMetricList": List[DataQualityMetricTypeDef],
     },
     total=False,
 )
 
 DescribeAnomalyDetectionExecutionsResponseTypeDef = TypedDict(
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     {
         "ExecutionList": List[ExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DimensionContributionTypeDef = TypedDict(
     "DimensionContributionTypeDef",
     {
         "DimensionName": str,
@@ -1182,15 +1023,15 @@
     },
 )
 
 FileFormatDescriptorOutputTypeDef = TypedDict(
     "FileFormatDescriptorOutputTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
-        "JsonFormatDescriptor": JsonFormatDescriptorOutputTypeDef,
+        "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
@@ -1200,15 +1041,15 @@
     total=False,
 )
 
 MetricSetDimensionFilterOutputTypeDef = TypedDict(
     "MetricSetDimensionFilterOutputTypeDef",
     {
         "Name": str,
-        "FilterList": List[FilterOutputTypeDef],
+        "FilterList": List[FilterTypeDef],
     },
     total=False,
 )
 
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
@@ -1219,33 +1060,33 @@
 )
 
 GetFeedbackResponseTypeDef = TypedDict(
     "GetFeedbackResponseTypeDef",
     {
         "AnomalyGroupTimeSeriesFeedback": List[TimeSeriesFeedbackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnomalyGroupRelatedMetricsResponseTypeDef = TypedDict(
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     {
         "InterMetricImpactList": List[InterMetricImpactDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricSetsResponseTypeDef = TypedDict(
     "ListMetricSetsResponseTypeDef",
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RDSSourceConfigOutputTypeDef = TypedDict(
     "RDSSourceConfigOutputTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -1304,15 +1145,15 @@
     },
     total=False,
 )
 
 AlertTypeDef = TypedDict(
     "AlertTypeDef",
     {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "AlertDescription": str,
         "AlertArn": str,
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
@@ -1338,21 +1179,19 @@
         "AlertDescription": str,
         "Tags": Mapping[str, str],
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
-
 class CreateAlertRequestRequestTypeDef(
     _RequiredCreateAlertRequestRequestTypeDef, _OptionalCreateAlertRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlertRequestRequestTypeDef",
     {
         "AlertArn": str,
     },
 )
 _OptionalUpdateAlertRequestRequestTypeDef = TypedDict(
@@ -1362,28 +1201,26 @@
         "AlertSensitivityThreshold": int,
         "Action": ActionTypeDef,
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAlertRequestRequestTypeDef(
     _RequiredUpdateAlertRequestRequestTypeDef, _OptionalUpdateAlertRequestRequestTypeDef
 ):
     pass
 
-
 ListAnomalyGroupSummariesResponseTypeDef = TypedDict(
     "ListAnomalyGroupSummariesResponseTypeDef",
     {
         "AnomalyGroupSummaryList": List[AnomalyGroupSummaryTypeDef],
         "AnomalyGroupStatistics": AnomalyGroupStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedCsvFormatDescriptorTypeDef = TypedDict(
     "DetectedCsvFormatDescriptorTypeDef",
     {
         "FileCompression": DetectedFieldTypeDef,
@@ -1434,15 +1271,15 @@
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     {
         "AnomalyGroupId": str,
         "MetricName": str,
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3SourceConfigOutputTypeDef = TypedDict(
     "S3SourceConfigOutputTypeDef",
     {
         "RoleArn": str,
@@ -1476,26 +1313,24 @@
     {
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
     },
     total=False,
 )
 
-
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
-
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedFileFormatDescriptorTypeDef = TypedDict(
     "DetectedFileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": DetectedCsvFormatDescriptorTypeDef,
@@ -1504,15 +1339,15 @@
     total=False,
 )
 
 GetDataQualityMetricsResponseTypeDef = TypedDict(
     "GetDataQualityMetricsResponseTypeDef",
     {
         "AnomalyDetectorDataQualityMetricList": List[AnomalyDetectorDataQualityMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricLevelImpactTypeDef = TypedDict(
     "MetricLevelImpactTypeDef",
     {
         "MetricName": str,
@@ -1522,19 +1357,19 @@
     total=False,
 )
 
 MetricSourceOutputTypeDef = TypedDict(
     "MetricSourceOutputTypeDef",
     {
         "S3SourceConfig": S3SourceConfigOutputTypeDef,
-        "AppFlowConfig": AppFlowConfigOutputTypeDef,
-        "CloudWatchConfig": CloudWatchConfigOutputTypeDef,
+        "AppFlowConfig": AppFlowConfigTypeDef,
+        "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
         "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
-        "AthenaSourceConfig": AthenaSourceConfigOutputTypeDef,
+        "AthenaSourceConfig": AthenaSourceConfigTypeDef,
     },
     total=False,
 )
 
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
@@ -1583,22 +1418,22 @@
         "MetricSetArn": str,
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricSetDescription": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Offset": int,
-        "MetricList": List[MetricOutputTypeDef],
-        "TimestampColumn": TimestampColumnOutputTypeDef,
+        "MetricList": List[MetricTypeDef],
+        "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": List[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "MetricSource": MetricSourceOutputTypeDef,
         "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
@@ -1618,21 +1453,19 @@
         "Timezone": str,
         "Tags": Mapping[str, str],
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
-
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1646,34 +1479,32 @@
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
-
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
     pass
 
-
 DetectedMetricSourceTypeDef = TypedDict(
     "DetectedMetricSourceTypeDef",
     {
         "S3SourceConfig": DetectedS3SourceConfigTypeDef,
     },
     total=False,
 )
 
 GetAnomalyGroupResponseTypeDef = TypedDict(
     "GetAnomalyGroupResponseTypeDef",
     {
         "AnomalyGroup": AnomalyGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedMetricSetConfigTypeDef = TypedDict(
     "DetectedMetricSetConfigTypeDef",
     {
         "Offset": DetectedFieldTypeDef,
@@ -1683,10 +1514,10 @@
     total=False,
 )
 
 DetectMetricSetConfigResponseTypeDef = TypedDict(
     "DetectMetricSetConfigResponseTypeDef",
     {
         "DetectedMetricSetConfig": DetectedMetricSetConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics/type_defs.pyi` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lookoutmetrics service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationOutputTypeDef
+    from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
-    data: LambdaConfigurationOutputTypeDef = {...}
+    data: LambdaConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,101 +36,91 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "LambdaConfigurationOutputTypeDef",
-    "SNSConfigurationOutputTypeDef",
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
-    "AppFlowConfigOutputTypeDef",
     "AppFlowConfigTypeDef",
-    "BackTestConfigurationOutputTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
-    "CreateAlertResponseTypeDef",
-    "CreateAnomalyDetectorResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
-    "CreateMetricSetResponseTypeDef",
     "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
     "ExecutionStatusTypeDef",
     "DescribeAnomalyDetectorRequestRequestTypeDef",
     "DescribeMetricSetRequestRequestTypeDef",
-    "MetricOutputTypeDef",
-    "TimestampColumnOutputTypeDef",
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
-    "JsonFormatDescriptorOutputTypeDef",
     "JsonFormatDescriptorTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
-    "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlertResponseTypeDef",
-    "UpdateAnomalyDetectorResponseTypeDef",
-    "UpdateMetricSetResponseTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
-    "ListAlertsResponseTypeDef",
-    "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
-    "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
-    "AthenaSourceConfigOutputTypeDef",
-    "CloudWatchConfigOutputTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
+    "CreateAlertResponseTypeDef",
+    "CreateAnomalyDetectorResponseTypeDef",
+    "CreateMetricSetResponseTypeDef",
+    "DescribeAnomalyDetectorResponseTypeDef",
+    "GetSampleDataResponseTypeDef",
+    "ListAlertsResponseTypeDef",
+    "ListAnomalyDetectorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateAlertResponseTypeDef",
+    "UpdateAnomalyDetectorResponseTypeDef",
+    "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
     "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
     "MetricSetDimensionFilterOutputTypeDef",
@@ -169,42 +159,14 @@
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
-LambdaConfigurationOutputTypeDef = TypedDict(
-    "LambdaConfigurationOutputTypeDef",
-    {
-        "RoleArn": str,
-        "LambdaArn": str,
-    },
-)
-
-_RequiredSNSConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSNSConfigurationOutputTypeDef",
-    {
-        "RoleArn": str,
-        "SnsTopicArn": str,
-    },
-)
-_OptionalSNSConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSNSConfigurationOutputTypeDef",
-    {
-        "SnsFormat": SnsFormatType,
-    },
-    total=False,
-)
-
-class SNSConfigurationOutputTypeDef(
-    _RequiredSNSConfigurationOutputTypeDef, _OptionalSNSConfigurationOutputTypeDef
-):
-    pass
-
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "RoleArn": str,
         "LambdaArn": str,
     },
 )
@@ -220,17 +182,19 @@
     "_OptionalSNSConfigurationTypeDef",
     {
         "SnsFormat": SnsFormatType,
     },
     total=False,
 )
 
+
 class SNSConfigurationTypeDef(_RequiredSNSConfigurationTypeDef, _OptionalSNSConfigurationTypeDef):
     pass
 
+
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
@@ -338,44 +302,30 @@
     "_OptionalAnomalyGroupTimeSeriesTypeDef",
     {
         "TimeSeriesId": str,
     },
     total=False,
 )
 
+
 class AnomalyGroupTimeSeriesTypeDef(
     _RequiredAnomalyGroupTimeSeriesTypeDef, _OptionalAnomalyGroupTimeSeriesTypeDef
 ):
     pass
 
-AppFlowConfigOutputTypeDef = TypedDict(
-    "AppFlowConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "FlowName": str,
-    },
-    total=False,
-)
 
 AppFlowConfigTypeDef = TypedDict(
     "AppFlowConfigTypeDef",
     {
         "RoleArn": str,
         "FlowName": str,
     },
     total=False,
 )
 
-BackTestConfigurationOutputTypeDef = TypedDict(
-    "BackTestConfigurationOutputTypeDef",
-    {
-        "RunBackTestMode": bool,
-    },
-)
-
 BackTestConfigurationTypeDef = TypedDict(
     "BackTestConfigurationTypeDef",
     {
         "RunBackTestMode": bool,
     },
 )
 
@@ -404,27 +354,22 @@
 BackTestAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-CreateAlertResponseTypeDef = TypedDict(
-    "CreateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalyDetectorResponseTypeDef = TypedDict(
-    "CreateAnomalyDetectorResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "MetricName": str,
@@ -435,34 +380,28 @@
     "_OptionalMetricTypeDef",
     {
         "Namespace": str,
     },
     total=False,
 )
 
+
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
+
 TimestampColumnTypeDef = TypedDict(
     "TimestampColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
-CreateMetricSetResponseTypeDef = TypedDict(
-    "CreateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CsvFormatDescriptorOutputTypeDef = TypedDict(
     "CsvFormatDescriptorOutputTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -536,20 +475,22 @@
         "Timestamp": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAnomalyDetectionExecutionsRequestRequestTypeDef(
     _RequiredDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     _OptionalDescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 ExecutionStatusTypeDef = TypedDict(
     "ExecutionStatusTypeDef",
     {
         "Timestamp": str,
         "Status": AnomalyDetectionTaskStatusType,
         "FailureReason": str,
     },
@@ -566,41 +507,14 @@
 DescribeMetricSetRequestRequestTypeDef = TypedDict(
     "DescribeMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 
-_RequiredMetricOutputTypeDef = TypedDict(
-    "_RequiredMetricOutputTypeDef",
-    {
-        "MetricName": str,
-        "AggregationFunction": AggregationFunctionType,
-    },
-)
-_OptionalMetricOutputTypeDef = TypedDict(
-    "_OptionalMetricOutputTypeDef",
-    {
-        "Namespace": str,
-    },
-    total=False,
-)
-
-class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
-    pass
-
-TimestampColumnOutputTypeDef = TypedDict(
-    "TimestampColumnOutputTypeDef",
-    {
-        "ColumnName": str,
-        "ColumnFormat": str,
-    },
-    total=False,
-)
-
 DimensionValueContributionTypeDef = TypedDict(
     "DimensionValueContributionTypeDef",
     {
         "DimensionValue": str,
         "ContributionScore": float,
     },
     total=False,
@@ -610,41 +524,23 @@
     "DimensionNameValueTypeDef",
     {
         "DimensionName": str,
         "DimensionValue": str,
     },
 )
 
-JsonFormatDescriptorOutputTypeDef = TypedDict(
-    "JsonFormatDescriptorOutputTypeDef",
-    {
-        "FileCompression": JsonFileCompressionType,
-        "Charset": str,
-    },
-    total=False,
-)
-
 JsonFormatDescriptorTypeDef = TypedDict(
     "JsonFormatDescriptorTypeDef",
     {
         "FileCompression": JsonFileCompressionType,
         "Charset": str,
     },
     total=False,
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "DimensionValue": str,
-        "FilterOperation": Literal["EQUALS"],
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "DimensionValue": str,
         "FilterOperation": Literal["EQUALS"],
     },
     total=False,
@@ -668,38 +564,31 @@
     "_OptionalGetDataQualityMetricsRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
     total=False,
 )
 
+
 class GetDataQualityMetricsRequestRequestTypeDef(
     _RequiredGetDataQualityMetricsRequestRequestTypeDef,
     _OptionalGetDataQualityMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 TimeSeriesFeedbackTypeDef = TypedDict(
     "TimeSeriesFeedbackTypeDef",
     {
         "TimeSeriesId": str,
         "IsAnomaly": bool,
     },
     total=False,
 )
 
-GetSampleDataResponseTypeDef = TypedDict(
-    "GetSampleDataResponseTypeDef",
-    {
-        "HeaderValues": List[str],
-        "SampleRows": List[List[str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InterMetricImpactDetailsTypeDef = TypedDict(
     "InterMetricImpactDetailsTypeDef",
     {
         "MetricName": str,
         "AnomalyGroupId": str,
         "RelationshipType": RelationshipTypeType,
         "ContributionPercentage": float,
@@ -739,20 +628,22 @@
         "RelationshipTypeFilter": RelationshipTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalyGroupRelatedMetricsRequestRequestTypeDef(
     _RequiredListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     _OptionalListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAnomalyGroupSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupSummariesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "SensitivityThreshold": int,
     },
 )
@@ -761,20 +652,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalyGroupSummariesRequestRequestTypeDef(
     _RequiredListAnomalyGroupSummariesRequestRequestTypeDef,
     _OptionalListAnomalyGroupSummariesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "AnomalyGroupId": str,
         "MetricName": str,
     },
@@ -784,20 +677,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalyGroupTimeSeriesRequestRequestTypeDef(
     _RequiredListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     _OptionalListAnomalyGroupTimeSeriesRequestRequestTypeDef,
 ):
     pass
 
+
 ListMetricSetsRequestRequestTypeDef = TypedDict(
     "ListMetricSetsRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -821,22 +716,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 VpcConfigurationOutputTypeDef = TypedDict(
     "VpcConfigurationOutputTypeDef",
     {
         "SubnetIdList": List[str],
         "SecurityGroupIdList": List[str],
     },
 )
@@ -845,25 +732,14 @@
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -872,47 +748,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAlertResponseTypeDef = TypedDict(
-    "UpdateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalyDetectorResponseTypeDef = TypedDict(
-    "UpdateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMetricSetResponseTypeDef = TypedDict(
-    "UpdateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "SNSConfiguration": SNSConfigurationOutputTypeDef,
-        "LambdaConfiguration": LambdaConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
@@ -932,40 +775,14 @@
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
 )
 
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "AlertSummaryList": List[AlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAnomalyDetectorResponseTypeDef = TypedDict(
-    "DescribeAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "AnomalyDetectorName": str,
-        "AnomalyDetectorDescription": str,
-        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Status": AnomalyDetectorStatusType,
-        "FailureReason": str,
-        "KmsKeyArn": str,
-        "FailureType": AnomalyDetectorFailureTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorName": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
 )
@@ -975,20 +792,22 @@
         "AnomalyDetectorDescription": str,
         "KmsKeyArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAnomalyDetectorRequestRequestTypeDef(
     _RequiredCreateAnomalyDetectorRequestRequestTypeDef,
     _OptionalCreateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 _OptionalUpdateAnomalyDetectorRequestRequestTypeDef = TypedDict(
@@ -997,28 +816,21 @@
         "KmsKeyArn": str,
         "AnomalyDetectorDescription": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAnomalyDetectorRequestRequestTypeDef(
     _RequiredUpdateAnomalyDetectorRequestRequestTypeDef,
     _OptionalUpdateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
-ListAnomalyDetectorsResponseTypeDef = TypedDict(
-    "ListAnomalyDetectorsResponseTypeDef",
-    {
-        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 AnomalyGroupStatisticsTypeDef = TypedDict(
     "AnomalyGroupStatisticsTypeDef",
     {
         "EvaluationStartDate": str,
         "TotalCount": int,
         "ItemizedMetricStatsList": List[ItemizedMetricStatsTypeDef],
@@ -1046,41 +858,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetFeedbackRequestRequestTypeDef(
     _RequiredGetFeedbackRequestRequestTypeDef, _OptionalGetFeedbackRequestRequestTypeDef
 ):
     pass
 
-AthenaSourceConfigOutputTypeDef = TypedDict(
-    "AthenaSourceConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "DatabaseName": str,
-        "DataCatalog": str,
-        "TableName": str,
-        "WorkGroupName": str,
-        "S3ResultsPath": str,
-        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-CloudWatchConfigOutputTypeDef = TypedDict(
-    "CloudWatchConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "BackTestConfiguration": BackTestConfigurationOutputTypeDef,
-    },
-    total=False,
-)
 
 AthenaSourceConfigTypeDef = TypedDict(
     "AthenaSourceConfigTypeDef",
     {
         "RoleArn": str,
         "DatabaseName": str,
         "DataCatalog": str,
@@ -1115,29 +906,129 @@
     "AutoDetectionMetricSourceTypeDef",
     {
         "S3SourceConfig": AutoDetectionS3SourceConfigTypeDef,
     },
     total=False,
 )
 
+CreateAlertResponseTypeDef = TypedDict(
+    "CreateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalyDetectorResponseTypeDef = TypedDict(
+    "CreateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMetricSetResponseTypeDef = TypedDict(
+    "CreateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAnomalyDetectorResponseTypeDef = TypedDict(
+    "DescribeAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "AnomalyDetectorName": str,
+        "AnomalyDetectorDescription": str,
+        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Status": AnomalyDetectorStatusType,
+        "FailureReason": str,
+        "KmsKeyArn": str,
+        "FailureType": AnomalyDetectorFailureTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSampleDataResponseTypeDef = TypedDict(
+    "GetSampleDataResponseTypeDef",
+    {
+        "HeaderValues": List[str],
+        "SampleRows": List[List[str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "AlertSummaryList": List[AlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAnomalyDetectorsResponseTypeDef = TypedDict(
+    "ListAnomalyDetectorsResponseTypeDef",
+    {
+        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlertResponseTypeDef = TypedDict(
+    "UpdateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyDetectorResponseTypeDef = TypedDict(
+    "UpdateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMetricSetResponseTypeDef = TypedDict(
+    "UpdateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MetricSetDataQualityMetricTypeDef = TypedDict(
     "MetricSetDataQualityMetricTypeDef",
     {
         "MetricSetArn": str,
         "DataQualityMetricList": List[DataQualityMetricTypeDef],
     },
     total=False,
 )
 
 DescribeAnomalyDetectionExecutionsResponseTypeDef = TypedDict(
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     {
         "ExecutionList": List[ExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DimensionContributionTypeDef = TypedDict(
     "DimensionContributionTypeDef",
     {
         "DimensionName": str,
@@ -1155,15 +1046,15 @@
     },
 )
 
 FileFormatDescriptorOutputTypeDef = TypedDict(
     "FileFormatDescriptorOutputTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
-        "JsonFormatDescriptor": JsonFormatDescriptorOutputTypeDef,
+        "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
@@ -1173,15 +1064,15 @@
     total=False,
 )
 
 MetricSetDimensionFilterOutputTypeDef = TypedDict(
     "MetricSetDimensionFilterOutputTypeDef",
     {
         "Name": str,
-        "FilterList": List[FilterOutputTypeDef],
+        "FilterList": List[FilterTypeDef],
     },
     total=False,
 )
 
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
@@ -1192,33 +1083,33 @@
 )
 
 GetFeedbackResponseTypeDef = TypedDict(
     "GetFeedbackResponseTypeDef",
     {
         "AnomalyGroupTimeSeriesFeedback": List[TimeSeriesFeedbackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnomalyGroupRelatedMetricsResponseTypeDef = TypedDict(
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     {
         "InterMetricImpactList": List[InterMetricImpactDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricSetsResponseTypeDef = TypedDict(
     "ListMetricSetsResponseTypeDef",
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RDSSourceConfigOutputTypeDef = TypedDict(
     "RDSSourceConfigOutputTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -1277,15 +1168,15 @@
     },
     total=False,
 )
 
 AlertTypeDef = TypedDict(
     "AlertTypeDef",
     {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "AlertDescription": str,
         "AlertArn": str,
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
@@ -1311,19 +1202,21 @@
         "AlertDescription": str,
         "Tags": Mapping[str, str],
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
+
 class CreateAlertRequestRequestTypeDef(
     _RequiredCreateAlertRequestRequestTypeDef, _OptionalCreateAlertRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlertRequestRequestTypeDef",
     {
         "AlertArn": str,
     },
 )
 _OptionalUpdateAlertRequestRequestTypeDef = TypedDict(
@@ -1333,26 +1226,28 @@
         "AlertSensitivityThreshold": int,
         "Action": ActionTypeDef,
         "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAlertRequestRequestTypeDef(
     _RequiredUpdateAlertRequestRequestTypeDef, _OptionalUpdateAlertRequestRequestTypeDef
 ):
     pass
 
+
 ListAnomalyGroupSummariesResponseTypeDef = TypedDict(
     "ListAnomalyGroupSummariesResponseTypeDef",
     {
         "AnomalyGroupSummaryList": List[AnomalyGroupSummaryTypeDef],
         "AnomalyGroupStatistics": AnomalyGroupStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedCsvFormatDescriptorTypeDef = TypedDict(
     "DetectedCsvFormatDescriptorTypeDef",
     {
         "FileCompression": DetectedFieldTypeDef,
@@ -1403,15 +1298,15 @@
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     {
         "AnomalyGroupId": str,
         "MetricName": str,
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3SourceConfigOutputTypeDef = TypedDict(
     "S3SourceConfigOutputTypeDef",
     {
         "RoleArn": str,
@@ -1445,24 +1340,26 @@
     {
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
     },
     total=False,
 )
 
+
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
+
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedFileFormatDescriptorTypeDef = TypedDict(
     "DetectedFileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": DetectedCsvFormatDescriptorTypeDef,
@@ -1471,15 +1368,15 @@
     total=False,
 )
 
 GetDataQualityMetricsResponseTypeDef = TypedDict(
     "GetDataQualityMetricsResponseTypeDef",
     {
         "AnomalyDetectorDataQualityMetricList": List[AnomalyDetectorDataQualityMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricLevelImpactTypeDef = TypedDict(
     "MetricLevelImpactTypeDef",
     {
         "MetricName": str,
@@ -1489,19 +1386,19 @@
     total=False,
 )
 
 MetricSourceOutputTypeDef = TypedDict(
     "MetricSourceOutputTypeDef",
     {
         "S3SourceConfig": S3SourceConfigOutputTypeDef,
-        "AppFlowConfig": AppFlowConfigOutputTypeDef,
-        "CloudWatchConfig": CloudWatchConfigOutputTypeDef,
+        "AppFlowConfig": AppFlowConfigTypeDef,
+        "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
         "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
-        "AthenaSourceConfig": AthenaSourceConfigOutputTypeDef,
+        "AthenaSourceConfig": AthenaSourceConfigTypeDef,
     },
     total=False,
 )
 
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
@@ -1550,22 +1447,22 @@
         "MetricSetArn": str,
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricSetDescription": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Offset": int,
-        "MetricList": List[MetricOutputTypeDef],
-        "TimestampColumn": TimestampColumnOutputTypeDef,
+        "MetricList": List[MetricTypeDef],
+        "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": List[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "MetricSource": MetricSourceOutputTypeDef,
         "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
@@ -1585,19 +1482,21 @@
         "Timezone": str,
         "Tags": Mapping[str, str],
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
+
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1611,32 +1510,34 @@
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
         "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
+
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
     pass
 
+
 DetectedMetricSourceTypeDef = TypedDict(
     "DetectedMetricSourceTypeDef",
     {
         "S3SourceConfig": DetectedS3SourceConfigTypeDef,
     },
     total=False,
 )
 
 GetAnomalyGroupResponseTypeDef = TypedDict(
     "GetAnomalyGroupResponseTypeDef",
     {
         "AnomalyGroup": AnomalyGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedMetricSetConfigTypeDef = TypedDict(
     "DetectedMetricSetConfigTypeDef",
     {
         "Offset": DetectedFieldTypeDef,
@@ -1646,10 +1547,10 @@
     total=False,
 )
 
 DetectMetricSetConfigResponseTypeDef = TypedDict(
     "DetectMetricSetConfigResponseTypeDef",
     {
         "DetectedMetricSetConfig": DetectedMetricSetConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.28.12
-Summary: Type annotations for boto3.LookoutMetrics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,100 +311,89 @@
 ### Typed dictionaries
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
-    LambdaConfigurationOutputTypeDef,
-    SNSConfigurationOutputTypeDef,
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
     DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
-    AppFlowConfigOutputTypeDef,
     AppFlowConfigTypeDef,
-    BackTestConfigurationOutputTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
-    CreateMetricSetResponseTypeDef,
     CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
     ExecutionStatusTypeDef,
     DescribeAnomalyDetectorRequestRequestTypeDef,
     DescribeMetricSetRequestRequestTypeDef,
-    MetricOutputTypeDef,
-    TimestampColumnOutputTypeDef,
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
-    JsonFormatDescriptorOutputTypeDef,
     JsonFormatDescriptorTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
-    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
     AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
-    ListAlertsResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
-    AthenaSourceConfigOutputTypeDef,
-    CloudWatchConfigOutputTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
+    CreateMetricSetResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
+    GetSampleDataResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
     FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
     MetricSetDimensionFilterOutputTypeDef,
@@ -444,15 +433,15 @@
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationOutputTypeDef:
+def get_structure() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt` & `mypy-boto3-lookoutmetrics-1.28.15/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.12/setup.py` & `mypy-boto3-lookoutmetrics-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutmetrics",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutMetrics 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LookoutMetrics 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

