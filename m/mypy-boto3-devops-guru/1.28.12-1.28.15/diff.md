# Comparing `tmp/mypy-boto3-devops-guru-1.28.12.tar.gz` & `tmp/mypy-boto3-devops-guru-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devops-guru-1.28.12.tar", last modified: Thu Jul 27 05:34:34 2023, max compression
+gzip compressed data, was "mypy-boto3-devops-guru-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
```

## Comparing `mypy-boto3-devops-guru-1.28.12.tar` & `mypy-boto3-devops-guru-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.056535 mypy-boto3-devops-guru-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23524 2023-07-27 05:34:34.052535 mypy-boto3-devops-guru-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22022 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.052535 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65792 2023-07-27 05:20:13.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65725 2023-07-27 05:20:12.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:11.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.052535 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23524 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:33.000000 mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:34.056535 mypy-boto3-devops-guru-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-27 05:20:10.000000 mypy-boto3-devops-guru-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.976961 mypy-boto3-devops-guru-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23366 2023-07-28 20:42:37.972960 mypy-boto3-devops-guru-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.968960 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-07-28 20:22:53.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64825 2023-07-28 20:22:55.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64758 2023-07-28 20:22:54.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.972960 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23366 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.976961 mypy-boto3-devops-guru-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/setup.py
```

### Comparing `mypy-boto3-devops-guru-1.28.12/LICENSE` & `mypy-boto3-devops-guru-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/PKG-INFO` & `mypy-boto3-devops-guru-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.12
-Summary: Type annotations for boto3.DevOpsGuru 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,16 +407,15 @@
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
-    AmazonCodeGuruProfilerIntegrationOutputTypeDef,
+    ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
     CloudFormationCollectionOutputTypeDef,
@@ -426,88 +425,85 @@
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
-    InsightFeedbackOutputTypeDef,
+    InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
     EndTimeRangeTypeDef,
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
-    InsightFeedbackTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
     NotificationFilterConfigOutputTypeDef,
-    SnsChannelConfigOutputTypeDef,
-    NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
+    NotificationFilterConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
-    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
     ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
     TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
-    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
-    EventSourcesConfigOutputTypeDef,
+    AddNotificationChannelResponseTypeDef,
+    DescribeAccountHealthResponseTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
     PutFeedbackRequestRequestTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
```

### Comparing `mypy-boto3-devops-guru-1.28.12/README.md` & `mypy-boto3-devops-guru-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,16 +375,15 @@
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
-    AmazonCodeGuruProfilerIntegrationOutputTypeDef,
+    ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
     CloudFormationCollectionOutputTypeDef,
@@ -394,88 +393,85 @@
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
-    InsightFeedbackOutputTypeDef,
+    InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
     EndTimeRangeTypeDef,
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
-    InsightFeedbackTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
     NotificationFilterConfigOutputTypeDef,
-    SnsChannelConfigOutputTypeDef,
-    NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
+    NotificationFilterConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
-    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
     ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
     TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
-    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
-    EventSourcesConfigOutputTypeDef,
+    AddNotificationChannelResponseTypeDef,
+    DescribeAccountHealthResponseTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
     PutFeedbackRequestRequestTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
```

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.py` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__init__.pyi` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/__main__.py` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DevOpsGuru 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.DevOpsGuru 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
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

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.py` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/client.pyi` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.py` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/literals.pyi` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.py` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
 
@@ -135,30 +135,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
 
 class GetCostEstimationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCostEstimationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
         """
 
 
@@ -168,15 +168,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
 
@@ -189,30 +189,30 @@
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
 
 class ListAnomalousLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
     """
 
     def paginate(
-        self, *, InsightId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnomalousLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
         """
 
 
@@ -223,15 +223,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listeventspaginator)
         """
 
 
@@ -241,15 +241,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
         """
 
 
@@ -259,30 +259,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
 
 class ListNotificationChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotificationChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
         """
 
 
@@ -294,15 +294,15 @@
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
 
@@ -314,15 +314,15 @@
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listrecommendationspaginator)
         """
 
 
@@ -334,15 +334,15 @@
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchinsightspaginator)
         """
 
 
@@ -355,13 +355,13 @@
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/paginator.pyi` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
 class DescribeResourceCollectionHealthPaginator(Paginator):
@@ -131,29 +131,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
 class GetCostEstimationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCostEstimationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getcostestimationpaginator)
         """
 
 class GetResourceCollectionPaginator(Paginator):
@@ -162,15 +162,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
 class ListAnomaliesForInsightPaginator(Paginator):
@@ -182,29 +182,29 @@
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
 class ListAnomalousLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
     """
 
     def paginate(
-        self, *, InsightId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnomalousLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listanomalousloggroupspaginator)
         """
 
 class ListEventsPaginator(Paginator):
@@ -214,15 +214,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listeventspaginator)
         """
 
 class ListInsightsPaginator(Paginator):
@@ -231,15 +231,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listinsightspaginator)
         """
 
 class ListMonitoredResourcesPaginator(Paginator):
@@ -248,29 +248,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
 class ListNotificationChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotificationChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listnotificationchannelspaginator)
         """
 
 class ListOrganizationInsightsPaginator(Paginator):
@@ -281,15 +281,15 @@
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
 class ListRecommendationsPaginator(Paginator):
@@ -300,15 +300,15 @@
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#listrecommendationspaginator)
         """
 
 class SearchInsightsPaginator(Paginator):
@@ -319,15 +319,15 @@
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchinsightspaginator)
         """
 
 class SearchOrganizationInsightsPaginator(Paginator):
@@ -339,13 +339,13 @@
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.py` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountInsightHealthTypeDef",
-    "AddNotificationChannelResponseTypeDef",
-    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
     "CloudFormationCollectionOutputTypeDef",
@@ -66,88 +65,85 @@
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
     "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
-    "DescribeAccountOverviewResponseTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
-    "InsightFeedbackOutputTypeDef",
+    "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
-    "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
-    "DescribeOrganizationOverviewResponseTypeDef",
-    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
-    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
     "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
     "EventTimeRangeTypeDef",
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
-    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
-    "InsightFeedbackTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
     "StartTimeRangeTypeDef",
-    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
-    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
     "NotificationFilterConfigOutputTypeDef",
-    "SnsChannelConfigOutputTypeDef",
-    "NotificationFilterConfigTypeDef",
     "SnsChannelConfigTypeDef",
+    "NotificationFilterConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
-    "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
     "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
     "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
-    "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
-    "EventSourcesConfigOutputTypeDef",
+    "AddNotificationChannelResponseTypeDef",
+    "DescribeAccountHealthResponseTypeDef",
+    "DescribeAccountOverviewResponseTypeDef",
+    "DescribeOrganizationHealthResponseTypeDef",
+    "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
     "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeFeedbackResponseTypeDef",
-    "ListInsightsClosedStatusFilterTypeDef",
     "PutFeedbackRequestRequestTypeDef",
+    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    "ListInsightsClosedStatusFilterTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
     "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
@@ -229,28 +225,23 @@
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
 )
 
-AddNotificationChannelResponseTypeDef = TypedDict(
-    "AddNotificationChannelResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AmazonCodeGuruProfilerIntegrationOutputTypeDef = TypedDict(
-    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": EventSourceOptInStatusType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
     },
@@ -412,26 +403,14 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DescribeAccountHealthResponseTypeDef = TypedDict(
-    "DescribeAccountHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "AnalyzedResourceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
@@ -446,24 +425,14 @@
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAccountOverviewResponseTypeDef = TypedDict(
-    "DescribeAccountOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "MeanTimeToRecoverInMilliseconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribeAnomalyRequestRequestTypeDef = TypedDict(
@@ -485,16 +454,16 @@
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
 
-InsightFeedbackOutputTypeDef = TypedDict(
-    "InsightFeedbackOutputTypeDef",
+InsightFeedbackTypeDef = TypedDict(
+    "InsightFeedbackTypeDef",
     {
         "Id": str,
         "Feedback": InsightFeedbackOptionType,
     },
     total=False,
 )
 
@@ -524,25 +493,14 @@
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationHealthResponseTypeDef = TypedDict(
-    "DescribeOrganizationHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
@@ -559,48 +517,24 @@
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeOrganizationOverviewResponseTypeDef = TypedDict(
-    "DescribeOrganizationOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "MaxResults": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -618,36 +552,14 @@
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -689,22 +601,14 @@
     "EventTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
 )
 
-GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -717,36 +621,14 @@
         "Count": int,
         "UnitCost": float,
         "Cost": float,
     },
     total=False,
 )
 
-_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
-    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
@@ -761,23 +643,14 @@
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
 
-InsightFeedbackTypeDef = TypedDict(
-    "InsightFeedbackTypeDef",
-    {
-        "Id": str,
-        "Feedback": InsightFeedbackOptionType,
-    },
-    total=False,
-)
-
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
 _OptionalInsightTimeRangeTypeDef = TypedDict(
@@ -826,36 +699,14 @@
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
-    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -886,54 +737,22 @@
     "ListMonitoredResourcesFiltersTypeDef",
     {
         "ResourcePermission": ResourcePermissionType,
         "ResourceTypeFilters": Sequence[ResourceTypeFilterType],
     },
 )
 
-ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNotificationChannelsRequestRequestTypeDef = TypedDict(
     "ListNotificationChannelsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "Locale": LocaleType,
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
-    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -989,16 +808,16 @@
     {
         "Severities": List[InsightSeverityType],
         "MessageTypes": List[NotificationMessageTypeType],
     },
     total=False,
 )
 
-SnsChannelConfigOutputTypeDef = TypedDict(
-    "SnsChannelConfigOutputTypeDef",
+SnsChannelConfigTypeDef = TypedDict(
+    "SnsChannelConfigTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
 NotificationFilterConfigTypeDef = TypedDict(
@@ -1006,22 +825,14 @@
     {
         "Severities": Sequence[InsightSeverityType],
         "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
 )
 
-SnsChannelConfigTypeDef = TypedDict(
-    "SnsChannelConfigTypeDef",
-    {
-        "TopicArn": str,
-    },
-    total=False,
-)
-
 OpsCenterIntegrationConfigTypeDef = TypedDict(
     "OpsCenterIntegrationConfigTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
@@ -1030,24 +841,14 @@
     "OpsCenterIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
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
 PerformanceInsightsMetricDimensionGroupTypeDef = TypedDict(
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     {
         "Group": str,
         "Dimensions": List[str],
         "Limit": int,
     },
@@ -1154,25 +955,14 @@
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": Sequence[str],
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
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
@@ -1199,20 +989,62 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
-EventSourcesConfigOutputTypeDef = TypedDict(
-    "EventSourcesConfigOutputTypeDef",
+AddNotificationChannelResponseTypeDef = TypedDict(
+    "AddNotificationChannelResponseTypeDef",
     {
-        "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationOutputTypeDef,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountHealthResponseTypeDef = TypedDict(
+    "DescribeAccountHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "AnalyzedResourceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountOverviewResponseTypeDef = TypedDict(
+    "DescribeAccountOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "MeanTimeToRecoverInMilliseconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationHealthResponseTypeDef = TypedDict(
+    "DescribeOrganizationHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationOverviewResponseTypeDef = TypedDict(
+    "DescribeOrganizationOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
@@ -1266,35 +1098,166 @@
     },
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
-        "InsightFeedback": InsightFeedbackOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InsightFeedback": InsightFeedbackTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListInsightsClosedStatusFilterTypeDef = TypedDict(
-    "ListInsightsClosedStatusFilterTypeDef",
+PutFeedbackRequestRequestTypeDef = TypedDict(
+    "PutFeedbackRequestRequestTypeDef",
     {
-        "Type": InsightTypeType,
-        "EndTimeRange": EndTimeRangeTypeDef,
+        "InsightFeedback": InsightFeedbackTypeDef,
     },
+    total=False,
 )
 
-PutFeedbackRequestRequestTypeDef = TypedDict(
-    "PutFeedbackRequestRequestTypeDef",
+_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     {
-        "InsightFeedback": InsightFeedbackTypeDef,
+        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+
+GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
+    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
+    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+):
+    pass
+
+
+ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "Locale": LocaleType,
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
+    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
+):
+    pass
+
+
+ListInsightsClosedStatusFilterTypeDef = TypedDict(
+    "ListInsightsClosedStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "EndTimeRange": EndTimeRangeTypeDef,
+    },
+)
+
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
@@ -1307,15 +1270,15 @@
     },
 )
 
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitoredResourcesRequestRequestTypeDef = TypedDict(
     "ListMonitoredResourcesRequestRequestTypeDef",
     {
@@ -1333,15 +1296,15 @@
     },
     total=False,
 )
 
 _RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigOutputTypeDef",
     {
-        "Sns": SnsChannelConfigOutputTypeDef,
+        "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
     "_OptionalNotificationChannelConfigOutputTypeDef",
     {
         "Filters": NotificationFilterConfigOutputTypeDef,
     },
@@ -1468,16 +1431,16 @@
     },
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
-        "EventSources": EventSourcesConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EventSources": EventSourcesConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
@@ -1504,15 +1467,15 @@
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
@@ -1542,15 +1505,15 @@
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
@@ -1630,15 +1593,15 @@
     },
 )
 
 DescribeServiceIntegrationResponseTypeDef = TypedDict(
     "DescribeServiceIntegrationResponseTypeDef",
     {
         "ServiceIntegration": ServiceIntegrationConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceMetricTypeDef = TypedDict(
     "PerformanceInsightsReferenceMetricTypeDef",
     {
         "MetricQuery": PerformanceInsightsMetricQueryTypeDef,
@@ -1657,15 +1620,15 @@
 )
 
 GetResourceCollectionResponseTypeDef = TypedDict(
     "GetResourceCollectionResponseTypeDef",
     {
         "ResourceCollection": ResourceCollectionFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "ResourceCollection": ResourceCollectionOutputTypeDef,
@@ -1826,26 +1789,26 @@
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "Account": List[AccountHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceCollectionHealthResponseTypeDef = TypedDict(
     "DescribeResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceCollectionRequestRequestTypeDef = TypedDict(
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
@@ -1858,15 +1821,15 @@
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
@@ -1904,15 +1867,15 @@
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
@@ -1948,24 +1911,24 @@
 
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationChannelsResponseTypeDef = TypedDict(
     "ListNotificationChannelsResponseTypeDef",
     {
         "Channels": List[NotificationChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceComparisonValuesTypeDef = TypedDict(
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     {
         "ReferenceScalar": PerformanceInsightsReferenceScalarTypeDef,
@@ -1989,87 +1952,87 @@
 )
 
 ListEventsResponseTypeDef = TypedDict(
     "ListEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInsightsResponseTypeDef = TypedDict(
     "ListInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchInsightsResponseTypeDef = TypedDict(
     "SearchInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchOrganizationInsightsResponseTypeDef = TypedDict(
     "SearchOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInsightResponseTypeDef = TypedDict(
     "DescribeInsightResponseTypeDef",
     {
         "ProactiveInsight": ProactiveInsightTypeDef,
         "ReactiveInsight": ReactiveInsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrganizationInsightsResponseTypeDef = TypedDict(
     "ListOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_RequiredListEventsRequestListEventsPaginateTypeDef",
     {
         "Filters": ListEventsFiltersTypeDef,
     },
 )
 _OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_OptionalListEventsRequestListEventsPaginateTypeDef",
     {
         "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListEventsRequestListEventsPaginateTypeDef(
     _RequiredListEventsRequestListEventsPaginateTypeDef,
@@ -2132,15 +2095,15 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "Filters": SearchInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
@@ -2183,15 +2146,15 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
@@ -2210,15 +2173,15 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsMetricsDetailTypeDef = TypedDict(
     "PerformanceInsightsMetricsDetailTypeDef",
     {
         "MetricDisplayName": str,
@@ -2324,19 +2287,19 @@
 
 ListAnomaliesForInsightResponseTypeDef = TypedDict(
     "ListAnomaliesForInsightResponseTypeDef",
     {
         "ProactiveAnomalies": List[ProactiveAnomalySummaryTypeDef],
         "ReactiveAnomalies": List[ReactiveAnomalySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnomalyResponseTypeDef = TypedDict(
     "DescribeAnomalyResponseTypeDef",
     {
         "ProactiveAnomaly": ProactiveAnomalyTypeDef,
         "ReactiveAnomaly": ReactiveAnomalyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru/type_defs.pyi` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountInsightHealthTypeDef",
-    "AddNotificationChannelResponseTypeDef",
-    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
     "CloudFormationCollectionOutputTypeDef",
@@ -65,88 +64,85 @@
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
     "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
-    "DescribeAccountOverviewResponseTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
-    "InsightFeedbackOutputTypeDef",
+    "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
-    "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
-    "DescribeOrganizationOverviewResponseTypeDef",
-    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
-    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
     "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
     "EventTimeRangeTypeDef",
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
-    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
-    "InsightFeedbackTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
     "StartTimeRangeTypeDef",
-    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
-    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
     "NotificationFilterConfigOutputTypeDef",
-    "SnsChannelConfigOutputTypeDef",
-    "NotificationFilterConfigTypeDef",
     "SnsChannelConfigTypeDef",
+    "NotificationFilterConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
-    "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
     "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
     "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
-    "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
-    "EventSourcesConfigOutputTypeDef",
+    "AddNotificationChannelResponseTypeDef",
+    "DescribeAccountHealthResponseTypeDef",
+    "DescribeAccountOverviewResponseTypeDef",
+    "DescribeOrganizationHealthResponseTypeDef",
+    "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
     "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeFeedbackResponseTypeDef",
-    "ListInsightsClosedStatusFilterTypeDef",
     "PutFeedbackRequestRequestTypeDef",
+    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    "ListInsightsClosedStatusFilterTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
     "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
@@ -228,28 +224,23 @@
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
 )
 
-AddNotificationChannelResponseTypeDef = TypedDict(
-    "AddNotificationChannelResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AmazonCodeGuruProfilerIntegrationOutputTypeDef = TypedDict(
-    "AmazonCodeGuruProfilerIntegrationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": EventSourceOptInStatusType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
     },
@@ -407,26 +398,14 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DescribeAccountHealthResponseTypeDef = TypedDict(
-    "DescribeAccountHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "AnalyzedResourceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
@@ -439,24 +418,14 @@
 
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
-DescribeAccountOverviewResponseTypeDef = TypedDict(
-    "DescribeAccountOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "MeanTimeToRecoverInMilliseconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribeAnomalyRequestRequestTypeDef = TypedDict(
@@ -476,16 +445,16 @@
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
 
-InsightFeedbackOutputTypeDef = TypedDict(
-    "InsightFeedbackOutputTypeDef",
+InsightFeedbackTypeDef = TypedDict(
+    "InsightFeedbackTypeDef",
     {
         "Id": str,
         "Feedback": InsightFeedbackOptionType,
     },
     total=False,
 )
 
@@ -513,25 +482,14 @@
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationHealthResponseTypeDef = TypedDict(
-    "DescribeOrganizationHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
     {
         "FromTime": Union[datetime, str],
     },
 )
 _OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
@@ -546,46 +504,24 @@
 
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
-DescribeOrganizationOverviewResponseTypeDef = TypedDict(
-    "DescribeOrganizationOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "MaxResults": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -601,34 +537,14 @@
 
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -668,22 +584,14 @@
     "EventTimeRangeTypeDef",
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
 )
 
-GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -696,34 +604,14 @@
         "Count": int,
         "UnitCost": float,
         "Cost": float,
     },
     total=False,
 )
 
-_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
-    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-):
-    pass
-
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
@@ -736,23 +624,14 @@
 
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
-InsightFeedbackTypeDef = TypedDict(
-    "InsightFeedbackTypeDef",
-    {
-        "Id": str,
-        "Feedback": InsightFeedbackOptionType,
-    },
-    total=False,
-)
-
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
 _OptionalInsightTimeRangeTypeDef = TypedDict(
@@ -799,34 +678,14 @@
     {
         "FromTime": Union[datetime, str],
         "ToTime": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
-    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -855,52 +714,22 @@
     "ListMonitoredResourcesFiltersTypeDef",
     {
         "ResourcePermission": ResourcePermissionType,
         "ResourceTypeFilters": Sequence[ResourceTypeFilterType],
     },
 )
 
-ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNotificationChannelsRequestRequestTypeDef = TypedDict(
     "ListNotificationChannelsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "Locale": LocaleType,
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
-    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -954,16 +783,16 @@
     {
         "Severities": List[InsightSeverityType],
         "MessageTypes": List[NotificationMessageTypeType],
     },
     total=False,
 )
 
-SnsChannelConfigOutputTypeDef = TypedDict(
-    "SnsChannelConfigOutputTypeDef",
+SnsChannelConfigTypeDef = TypedDict(
+    "SnsChannelConfigTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
 NotificationFilterConfigTypeDef = TypedDict(
@@ -971,22 +800,14 @@
     {
         "Severities": Sequence[InsightSeverityType],
         "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
 )
 
-SnsChannelConfigTypeDef = TypedDict(
-    "SnsChannelConfigTypeDef",
-    {
-        "TopicArn": str,
-    },
-    total=False,
-)
-
 OpsCenterIntegrationConfigTypeDef = TypedDict(
     "OpsCenterIntegrationConfigTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
@@ -995,24 +816,14 @@
     "OpsCenterIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
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
 PerformanceInsightsMetricDimensionGroupTypeDef = TypedDict(
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     {
         "Group": str,
         "Dimensions": List[str],
         "Limit": int,
     },
@@ -1117,25 +928,14 @@
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": Sequence[str],
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
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
@@ -1162,20 +962,62 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
-EventSourcesConfigOutputTypeDef = TypedDict(
-    "EventSourcesConfigOutputTypeDef",
+AddNotificationChannelResponseTypeDef = TypedDict(
+    "AddNotificationChannelResponseTypeDef",
     {
-        "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationOutputTypeDef,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountHealthResponseTypeDef = TypedDict(
+    "DescribeAccountHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "AnalyzedResourceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountOverviewResponseTypeDef = TypedDict(
+    "DescribeAccountOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "MeanTimeToRecoverInMilliseconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationHealthResponseTypeDef = TypedDict(
+    "DescribeOrganizationHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationOverviewResponseTypeDef = TypedDict(
+    "DescribeOrganizationOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
@@ -1229,35 +1071,156 @@
     },
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
-        "InsightFeedback": InsightFeedbackOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InsightFeedback": InsightFeedbackTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListInsightsClosedStatusFilterTypeDef = TypedDict(
-    "ListInsightsClosedStatusFilterTypeDef",
+PutFeedbackRequestRequestTypeDef = TypedDict(
+    "PutFeedbackRequestRequestTypeDef",
     {
-        "Type": InsightTypeType,
-        "EndTimeRange": EndTimeRangeTypeDef,
+        "InsightFeedback": InsightFeedbackTypeDef,
     },
+    total=False,
 )
 
-PutFeedbackRequestRequestTypeDef = TypedDict(
-    "PutFeedbackRequestRequestTypeDef",
+_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     {
-        "InsightFeedback": InsightFeedbackTypeDef,
+        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
+    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+):
+    pass
+
+_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
+    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+):
+    pass
+
+ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "Locale": LocaleType,
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
+    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
+):
+    pass
+
+ListInsightsClosedStatusFilterTypeDef = TypedDict(
+    "ListInsightsClosedStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "EndTimeRange": EndTimeRangeTypeDef,
+    },
+)
+
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
@@ -1270,15 +1233,15 @@
     },
 )
 
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitoredResourcesRequestRequestTypeDef = TypedDict(
     "ListMonitoredResourcesRequestRequestTypeDef",
     {
@@ -1296,15 +1259,15 @@
     },
     total=False,
 )
 
 _RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigOutputTypeDef",
     {
-        "Sns": SnsChannelConfigOutputTypeDef,
+        "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
     "_OptionalNotificationChannelConfigOutputTypeDef",
     {
         "Filters": NotificationFilterConfigOutputTypeDef,
     },
@@ -1427,16 +1390,16 @@
     },
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
-        "EventSources": EventSourcesConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EventSources": EventSourcesConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
@@ -1463,15 +1426,15 @@
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
@@ -1499,15 +1462,15 @@
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
@@ -1583,15 +1546,15 @@
     },
 )
 
 DescribeServiceIntegrationResponseTypeDef = TypedDict(
     "DescribeServiceIntegrationResponseTypeDef",
     {
         "ServiceIntegration": ServiceIntegrationConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceMetricTypeDef = TypedDict(
     "PerformanceInsightsReferenceMetricTypeDef",
     {
         "MetricQuery": PerformanceInsightsMetricQueryTypeDef,
@@ -1610,15 +1573,15 @@
 )
 
 GetResourceCollectionResponseTypeDef = TypedDict(
     "GetResourceCollectionResponseTypeDef",
     {
         "ResourceCollection": ResourceCollectionFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "ResourceCollection": ResourceCollectionOutputTypeDef,
@@ -1779,26 +1742,26 @@
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "Account": List[AccountHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceCollectionHealthResponseTypeDef = TypedDict(
     "DescribeResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceCollectionRequestRequestTypeDef = TypedDict(
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
@@ -1811,15 +1774,15 @@
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
     _OptionalListInsightsRequestListInsightsPaginateTypeDef,
@@ -1853,15 +1816,15 @@
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
@@ -1893,24 +1856,24 @@
 
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationChannelsResponseTypeDef = TypedDict(
     "ListNotificationChannelsResponseTypeDef",
     {
         "Channels": List[NotificationChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceComparisonValuesTypeDef = TypedDict(
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     {
         "ReferenceScalar": PerformanceInsightsReferenceScalarTypeDef,
@@ -1934,87 +1897,87 @@
 )
 
 ListEventsResponseTypeDef = TypedDict(
     "ListEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInsightsResponseTypeDef = TypedDict(
     "ListInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchInsightsResponseTypeDef = TypedDict(
     "SearchInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchOrganizationInsightsResponseTypeDef = TypedDict(
     "SearchOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInsightResponseTypeDef = TypedDict(
     "DescribeInsightResponseTypeDef",
     {
         "ProactiveInsight": ProactiveInsightTypeDef,
         "ReactiveInsight": ReactiveInsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrganizationInsightsResponseTypeDef = TypedDict(
     "ListOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_RequiredListEventsRequestListEventsPaginateTypeDef",
     {
         "Filters": ListEventsFiltersTypeDef,
     },
 )
 _OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
     "_OptionalListEventsRequestListEventsPaginateTypeDef",
     {
         "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListEventsRequestListEventsPaginateTypeDef(
     _RequiredListEventsRequestListEventsPaginateTypeDef,
     _OptionalListEventsRequestListEventsPaginateTypeDef,
@@ -2071,15 +2034,15 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "Filters": SearchInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
@@ -2118,15 +2081,15 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
@@ -2143,15 +2106,15 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsMetricsDetailTypeDef = TypedDict(
     "PerformanceInsightsMetricsDetailTypeDef",
     {
         "MetricDisplayName": str,
@@ -2257,19 +2220,19 @@
 
 ListAnomaliesForInsightResponseTypeDef = TypedDict(
     "ListAnomaliesForInsightResponseTypeDef",
     {
         "ProactiveAnomalies": List[ProactiveAnomalySummaryTypeDef],
         "ReactiveAnomalies": List[ReactiveAnomalySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnomalyResponseTypeDef = TypedDict(
     "DescribeAnomalyResponseTypeDef",
     {
         "ProactiveAnomaly": ProactiveAnomalyTypeDef,
         "ReactiveAnomaly": ReactiveAnomalyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/PKG-INFO` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.12
-Summary: Type annotations for boto3.DevOpsGuru 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devops-guru)](https://pepy.tech/project/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,16 +407,15 @@
 
 `mypy_boto3_devops_guru.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
-    AmazonCodeGuruProfilerIntegrationOutputTypeDef,
+    ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
     CloudFormationCollectionOutputTypeDef,
@@ -426,88 +425,85 @@
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
     TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewRequestRequestTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
-    InsightFeedbackOutputTypeDef,
+    InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
     DescribeOrganizationOverviewRequestRequestTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
     EndTimeRangeTypeDef,
     EventResourceTypeDef,
     EventTimeRangeTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
-    InsightFeedbackTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
     StartTimeRangeTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
     NotificationFilterConfigOutputTypeDef,
-    SnsChannelConfigOutputTypeDef,
-    NotificationFilterConfigTypeDef,
     SnsChannelConfigTypeDef,
+    NotificationFilterConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
-    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
     ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
     TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
-    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
-    EventSourcesConfigOutputTypeDef,
+    AddNotificationChannelResponseTypeDef,
+    DescribeAccountHealthResponseTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
     CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeFeedbackResponseTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
     PutFeedbackRequestRequestTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
     ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
     NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
```

### Comparing `mypy-boto3-devops-guru-1.28.12/mypy_boto3_devops_guru.egg-info/SOURCES.txt` & `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.12/setup.py` & `mypy-boto3-devops-guru-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devops-guru",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DevOpsGuru 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

