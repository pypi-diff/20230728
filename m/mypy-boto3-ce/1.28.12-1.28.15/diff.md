# Comparing `tmp/mypy-boto3-ce-1.28.12.tar.gz` & `tmp/mypy-boto3-ce-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-ce-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
```

## Comparing `mypy-boto3-ce-1.28.12.tar` & `mypy-boto3-ce-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19628 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.796567 mypy-boto3-ce-1.28.12/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32603 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-27 05:18:06.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71661 2023-07-27 05:18:07.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71586 2023-07-27 05:18:06.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19628 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32603 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68658 2023-07-28 20:20:24.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68585 2023-07-28 20:20:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 20:42:22.000000 mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.344738 mypy-boto3-ce-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:20:21.000000 mypy-boto3-ce-1.28.15/setup.py
```

### Comparing `mypy-boto3-ce-1.28.12/LICENSE` & `mypy-boto3-ce-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.12/PKG-INFO` & `mypy-boto3-ce-1.28.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.12
-Summary: Type annotations for boto3.CostExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,126 +330,117 @@
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
-    AnomalyMonitorOutputTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
-    SubscriberOutputTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
-    CostCategoryInheritedValueDimensionOutputTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
     CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
     CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
-    DateIntervalOutputTypeDef,
+    DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagValuesOutputTypeDef,
-    DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
-    EC2SpecificationOutputTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
     TagValuesTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
-    GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
-    RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
     RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
-    CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
+    GetCostForecastRequestRequestTypeDef,
+    GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    GetCostForecastRequestRequestTypeDef,
-    GetUsageForecastRequestRequestTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
     ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
-    ServiceSpecificationOutputTypeDef,
     ServiceSpecificationTypeDef,
     ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
@@ -460,15 +451,14 @@
     GetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     GetSavingsPlansUtilizationRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GroupTypeDef,
     ReservationUtilizationGroupTypeDef,
     GetRightsizingRecommendationRequestRequestTypeDef,
     InstanceDetailsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RecommendationDetailDataTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.12/README.md` & `mypy-boto3-ce-1.28.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,126 +298,117 @@
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
-    AnomalyMonitorOutputTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
-    SubscriberOutputTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
-    CostCategoryInheritedValueDimensionOutputTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
     CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
     CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
-    DateIntervalOutputTypeDef,
+    DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagValuesOutputTypeDef,
-    DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
-    EC2SpecificationOutputTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
     TagValuesTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
-    GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
-    RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
     RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
-    CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
+    GetCostForecastRequestRequestTypeDef,
+    GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    GetCostForecastRequestRequestTypeDef,
-    GetUsageForecastRequestRequestTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
     ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
-    ServiceSpecificationOutputTypeDef,
     ServiceSpecificationTypeDef,
     ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
@@ -428,15 +419,14 @@
     GetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     GetSavingsPlansUtilizationRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GroupTypeDef,
     ReservationUtilizationGroupTypeDef,
     GetRightsizingRecommendationRequestRequestTypeDef,
     InstanceDetailsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RecommendationDetailDataTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.py` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.pyi` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.py` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.pyi` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.py` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,126 +56,117 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AnomalyDateIntervalTypeDef",
-    "AnomalyMonitorOutputTypeDef",
     "AnomalyMonitorTypeDef",
     "AnomalyScoreTypeDef",
-    "SubscriberOutputTypeDef",
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
-    "CostCategoryInheritedValueDimensionOutputTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
     "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
     "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
-    "DateIntervalOutputTypeDef",
+    "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagValuesOutputTypeDef",
-    "DateIntervalTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
     "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
-    "EC2SpecificationOutputTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
     "TagValuesTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
-    "GroupDefinitionOutputTypeDef",
     "SortDefinitionTypeDef",
-    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
-    "RightsizingRecommendationConfigurationOutputTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
-    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResourceTagOutputTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
     "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
     "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
-    "CostCategoryRuleOutputTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
     "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
+    "GetCostForecastRequestRequestTypeDef",
+    "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "GetCostForecastRequestRequestTypeDef",
-    "GetUsageForecastRequestRequestTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
+    "GetCostCategoriesResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
     "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
-    "ServiceSpecificationOutputTypeDef",
     "ServiceSpecificationTypeDef",
     "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
@@ -186,15 +177,14 @@
     "GetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     "GetSavingsPlansUtilizationRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GroupTypeDef",
     "ReservationUtilizationGroupTypeDef",
     "GetRightsizingRecommendationRequestRequestTypeDef",
     "InstanceDetailsTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RecommendationDetailDataTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
@@ -251,42 +241,14 @@
 
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
 
-_RequiredAnomalyMonitorOutputTypeDef = TypedDict(
-    "_RequiredAnomalyMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorType": MonitorTypeType,
-    },
-)
-_OptionalAnomalyMonitorOutputTypeDef = TypedDict(
-    "_OptionalAnomalyMonitorOutputTypeDef",
-    {
-        "MonitorArn": str,
-        "CreationDate": str,
-        "LastUpdatedDate": str,
-        "LastEvaluatedDate": str,
-        "MonitorDimension": Literal["SERVICE"],
-        "MonitorSpecification": "ExpressionOutputTypeDef",
-        "DimensionalValueCount": int,
-    },
-    total=False,
-)
-
-
-class AnomalyMonitorOutputTypeDef(
-    _RequiredAnomalyMonitorOutputTypeDef, _OptionalAnomalyMonitorOutputTypeDef
-):
-    pass
-
-
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
 )
@@ -313,24 +275,14 @@
     "AnomalyScoreTypeDef",
     {
         "MaxScore": float,
         "CurrentScore": float,
     },
 )
 
-SubscriberOutputTypeDef = TypedDict(
-    "SubscriberOutputTypeDef",
-    {
-        "Address": str,
-        "Type": SubscriberTypeType,
-        "Status": SubscriberStatusType,
-    },
-    total=False,
-)
-
 SubscriberTypeDef = TypedDict(
     "SubscriberTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
@@ -384,23 +336,14 @@
     {
         "TagKey": str,
         "Type": CostAllocationTagTypeType,
         "Status": CostAllocationTagStatusType,
     },
 )
 
-CostCategoryInheritedValueDimensionOutputTypeDef = TypedDict(
-    "CostCategoryInheritedValueDimensionOutputTypeDef",
-    {
-        "DimensionName": CostCategoryInheritedValueDimensionNameType,
-        "DimensionKey": str,
-    },
-    total=False,
-)
-
 CostCategoryInheritedValueDimensionTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
     },
     total=False,
@@ -447,16 +390,16 @@
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
-DateIntervalOutputTypeDef = TypedDict(
-    "DateIntervalOutputTypeDef",
+DateIntervalTypeDef = TypedDict(
+    "DateIntervalTypeDef",
     {
         "Start": str,
         "End": str,
     },
 )
 
 CoverageCostTypeDef = TypedDict(
@@ -493,57 +436,35 @@
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagValuesOutputTypeDef = TypedDict(
     "TagValuesOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
     total=False,
 )
 
-DateIntervalTypeDef = TypedDict(
-    "DateIntervalTypeDef",
-    {
-        "Start": str,
-        "End": str,
-    },
-)
-
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
 )
 
@@ -557,23 +478,14 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
@@ -681,22 +593,14 @@
         "NetworkOutBytesPerSecond": str,
         "NetworkPacketsInPerSecond": str,
         "NetworkPacketsOutPerSecond": str,
     },
     total=False,
 )
 
-EC2SpecificationOutputTypeDef = TypedDict(
-    "EC2SpecificationOutputTypeDef",
-    {
-        "OfferingClass": OfferingClassType,
-    },
-    total=False,
-)
-
 EC2SpecificationTypeDef = TypedDict(
     "EC2SpecificationTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
     total=False,
 )
@@ -796,23 +700,14 @@
     {
         "Type": GroupDefinitionTypeType,
         "Key": str,
     },
     total=False,
 )
 
-GroupDefinitionOutputTypeDef = TypedDict(
-    "GroupDefinitionOutputTypeDef",
-    {
-        "Type": GroupDefinitionTypeType,
-        "Key": str,
-    },
-    total=False,
-)
-
 _RequiredSortDefinitionTypeDef = TypedDict(
     "_RequiredSortDefinitionTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalSortDefinitionTypeDef = TypedDict(
@@ -824,26 +719,14 @@
 )
 
 
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
 
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
     total=False,
@@ -886,22 +769,14 @@
     "RightsizingRecommendationConfigurationTypeDef",
     {
         "RecommendationTarget": RecommendationTargetType,
         "BenefitsConsidered": bool,
     },
 )
 
-RightsizingRecommendationConfigurationOutputTypeDef = TypedDict(
-    "RightsizingRecommendationConfigurationOutputTypeDef",
-    {
-        "RecommendationTarget": RecommendationTargetType,
-        "BenefitsConsidered": bool,
-    },
-)
-
 RightsizingRecommendationMetadataTypeDef = TypedDict(
     "RightsizingRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "AdditionalMetadata": str,
@@ -961,25 +836,14 @@
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
     total=False,
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "DatabaseEngine": str,
@@ -1040,38 +904,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ResourceTagOutputTypeDef = TypedDict(
-    "ResourceTagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 ProvideAnomalyFeedbackRequestRequestTypeDef = TypedDict(
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationDetailHourlyMetricsTypeDef = TypedDict(
     "RecommendationDetailHourlyMetricsTypeDef",
     {
         "StartTime": str,
         "EstimatedOnDemandCost": str,
         "CurrentCoverage": str,
         "EstimatedCoverage": str,
@@ -1086,25 +934,14 @@
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
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
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
     total=False,
@@ -1175,24 +1012,14 @@
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
     total=False,
 )
 
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
     },
 )
@@ -1215,63 +1042,29 @@
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
-    {
-        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionOutputTypeDef",
     {
         "MonitorArnList": List[str],
-        "Subscribers": List[SubscriberOutputTypeDef],
+        "Subscribers": List[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
     },
 )
 _OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
     "_OptionalAnomalySubscriptionOutputTypeDef",
     {
@@ -1373,34 +1166,14 @@
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CostCategoryRuleOutputTypeDef = TypedDict(
-    "CostCategoryRuleOutputTypeDef",
-    {
-        "Value": str,
-        "Rule": "ExpressionOutputTypeDef",
-        "InheritedValue": CostCategoryInheritedValueDimensionOutputTypeDef,
-        "Type": CostCategoryRuleTypeType,
-    },
-    total=False,
-)
-
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionTypeDef,
         "Type": CostCategoryRuleTypeType,
@@ -1469,22 +1242,70 @@
 ):
     pass
 
 
 ForecastResultTypeDef = TypedDict(
     "ForecastResultTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
     },
     total=False,
 )
 
+_RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
+    "_RequiredGetCostForecastRequestRequestTypeDef",
+    {
+        "TimePeriod": DateIntervalTypeDef,
+        "Metric": MetricType,
+        "Granularity": GranularityType,
+    },
+)
+_OptionalGetCostForecastRequestRequestTypeDef = TypedDict(
+    "_OptionalGetCostForecastRequestRequestTypeDef",
+    {
+        "Filter": "ExpressionTypeDef",
+        "PredictionIntervalLevel": int,
+    },
+    total=False,
+)
+
+
+class GetCostForecastRequestRequestTypeDef(
+    _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
+    "_RequiredGetUsageForecastRequestRequestTypeDef",
+    {
+        "TimePeriod": DateIntervalTypeDef,
+        "Metric": MetricType,
+        "Granularity": GranularityType,
+    },
+)
+_OptionalGetUsageForecastRequestRequestTypeDef = TypedDict(
+    "_OptionalGetUsageForecastRequestRequestTypeDef",
+    {
+        "Filter": "ExpressionTypeDef",
+        "PredictionIntervalLevel": int,
+    },
+    total=False,
+)
+
+
+class GetUsageForecastRequestRequestTypeDef(
+    _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
+):
+    pass
+
+
 CoverageTypeDef = TypedDict(
     "CoverageTypeDef",
     {
         "CoverageHours": CoverageHoursTypeDef,
         "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
         "CoverageCost": CoverageCostTypeDef,
     },
@@ -1517,61 +1338,139 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 
-_RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
-    "_RequiredGetCostForecastRequestRequestTypeDef",
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
-        "Metric": MetricType,
-        "Granularity": GranularityType,
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGetCostForecastRequestRequestTypeDef = TypedDict(
-    "_OptionalGetCostForecastRequestRequestTypeDef",
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
     {
-        "Filter": "ExpressionTypeDef",
-        "PredictionIntervalLevel": int,
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class GetCostForecastRequestRequestTypeDef(
-    _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
-):
-    pass
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
-    "_RequiredGetUsageForecastRequestRequestTypeDef",
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
-        "Metric": MetricType,
-        "Granularity": GranularityType,
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGetUsageForecastRequestRequestTypeDef = TypedDict(
-    "_OptionalGetUsageForecastRequestRequestTypeDef",
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
     {
-        "Filter": "ExpressionTypeDef",
-        "PredictionIntervalLevel": int,
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class GetUsageForecastRequestRequestTypeDef(
-    _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
-):
-    pass
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ExpressionOutputTypeDef = TypedDict(
     "ExpressionOutputTypeDef",
     {
         "Or": List[Dict[str, Any]],
         "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
@@ -1585,15 +1484,15 @@
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
@@ -1610,22 +1509,14 @@
         "EBSResourceUtilization": EBSResourceUtilizationTypeDef,
         "DiskResourceUtilization": DiskResourceUtilizationTypeDef,
         "NetworkResourceUtilization": NetworkResourceUtilizationTypeDef,
     },
     total=False,
 )
 
-ServiceSpecificationOutputTypeDef = TypedDict(
-    "ServiceSpecificationOutputTypeDef",
-    {
-        "EC2Specification": EC2SpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 ServiceSpecificationTypeDef = TypedDict(
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
@@ -1644,15 +1535,15 @@
 )
 
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1994,22 +1885,14 @@
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceTags": List[ResourceTagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationDetailDataTypeDef = TypedDict(
     "RecommendationDetailDataTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
@@ -2043,15 +1926,15 @@
 )
 
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
     },
     total=False,
 )
 
 SavingsPlansPurchaseRecommendationDetailTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     {
@@ -2098,15 +1981,15 @@
 ):
     pass
 
 
 _RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
     "_RequiredSavingsPlansUtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
     },
 )
 _OptionalSavingsPlansUtilizationByTimeTypeDef = TypedDict(
     "_OptionalSavingsPlansUtilizationByTimeTypeDef",
     {
         "Savings": SavingsPlansSavingsTypeDef,
@@ -2134,24 +2017,24 @@
     total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnomalySubscriptionsResponseTypeDef = TypedDict(
     "GetAnomalySubscriptionsResponseTypeDef",
     {
         "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -2174,35 +2057,35 @@
 
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCostCategoryTypeDef = TypedDict(
     "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": List[CostCategoryRuleOutputTypeDef],
+        "Rules": List[CostCategoryRuleTypeDef],
     },
 )
 _OptionalCostCategoryTypeDef = TypedDict(
     "_OptionalCostCategoryTypeDef",
     {
         "EffectiveEnd": str,
         "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
@@ -2271,24 +2154,24 @@
 
 
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
@@ -2334,26 +2217,26 @@
 ):
     pass
 
 
 ResultByTimeTypeDef = TypedDict(
     "ResultByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
     },
     total=False,
 )
 
 UtilizationByTimeTypeDef = TypedDict(
     "UtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationUtilizationGroupTypeDef],
         "Total": ReservationAggregatesTypeDef,
     },
     total=False,
 )
 
 ReservationPurchaseRecommendationDetailTypeDef = TypedDict(
@@ -2383,24 +2266,24 @@
 )
 
 GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     {
         "RecommendationDetailId": str,
         "RecommendationDetailData": RecommendationDetailDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2419,41 +2302,41 @@
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
     total=False,
 )
 
 CurrentInstanceTypeDef = TypedDict(
@@ -2488,73 +2371,73 @@
     total=False,
 )
 
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
+        "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
+        "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
-        "ServiceSpecification": ServiceSpecificationOutputTypeDef,
+        "ServiceSpecification": ServiceSpecificationTypeDef,
         "RecommendationDetails": List[ReservationPurchaseRecommendationDetailTypeDef],
         "RecommendationSummary": ReservationPurchaseRecommendationSummaryTypeDef,
     },
     total=False,
 )
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
@@ -2564,15 +2447,15 @@
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
@@ -2588,11 +2471,11 @@
 GetRightsizingRecommendationResponseTypeDef = TypedDict(
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
-        "Configuration": RightsizingRecommendationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Configuration": RightsizingRecommendationConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.pyi` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,126 +55,117 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AnomalyDateIntervalTypeDef",
-    "AnomalyMonitorOutputTypeDef",
     "AnomalyMonitorTypeDef",
     "AnomalyScoreTypeDef",
-    "SubscriberOutputTypeDef",
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
-    "CostCategoryInheritedValueDimensionOutputTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
     "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
     "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
-    "DateIntervalOutputTypeDef",
+    "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagValuesOutputTypeDef",
-    "DateIntervalTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
     "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
-    "EC2SpecificationOutputTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
     "TagValuesTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
-    "GroupDefinitionOutputTypeDef",
     "SortDefinitionTypeDef",
-    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
-    "RightsizingRecommendationConfigurationOutputTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
-    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResourceTagOutputTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
     "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
     "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
-    "CostCategoryRuleOutputTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
     "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
+    "GetCostForecastRequestRequestTypeDef",
+    "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "GetCostForecastRequestRequestTypeDef",
-    "GetUsageForecastRequestRequestTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
+    "GetCostCategoriesResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
     "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
-    "ServiceSpecificationOutputTypeDef",
     "ServiceSpecificationTypeDef",
     "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
@@ -185,15 +176,14 @@
     "GetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     "GetSavingsPlansUtilizationRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GroupTypeDef",
     "ReservationUtilizationGroupTypeDef",
     "GetRightsizingRecommendationRequestRequestTypeDef",
     "InstanceDetailsTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RecommendationDetailDataTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
@@ -248,40 +238,14 @@
 )
 
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
-_RequiredAnomalyMonitorOutputTypeDef = TypedDict(
-    "_RequiredAnomalyMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorType": MonitorTypeType,
-    },
-)
-_OptionalAnomalyMonitorOutputTypeDef = TypedDict(
-    "_OptionalAnomalyMonitorOutputTypeDef",
-    {
-        "MonitorArn": str,
-        "CreationDate": str,
-        "LastUpdatedDate": str,
-        "LastEvaluatedDate": str,
-        "MonitorDimension": Literal["SERVICE"],
-        "MonitorSpecification": "ExpressionOutputTypeDef",
-        "DimensionalValueCount": int,
-    },
-    total=False,
-)
-
-class AnomalyMonitorOutputTypeDef(
-    _RequiredAnomalyMonitorOutputTypeDef, _OptionalAnomalyMonitorOutputTypeDef
-):
-    pass
-
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
 )
@@ -306,24 +270,14 @@
     "AnomalyScoreTypeDef",
     {
         "MaxScore": float,
         "CurrentScore": float,
     },
 )
 
-SubscriberOutputTypeDef = TypedDict(
-    "SubscriberOutputTypeDef",
-    {
-        "Address": str,
-        "Type": SubscriberTypeType,
-        "Status": SubscriberStatusType,
-    },
-    total=False,
-)
-
 SubscriberTypeDef = TypedDict(
     "SubscriberTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
@@ -375,23 +329,14 @@
     {
         "TagKey": str,
         "Type": CostAllocationTagTypeType,
         "Status": CostAllocationTagStatusType,
     },
 )
 
-CostCategoryInheritedValueDimensionOutputTypeDef = TypedDict(
-    "CostCategoryInheritedValueDimensionOutputTypeDef",
-    {
-        "DimensionName": CostCategoryInheritedValueDimensionNameType,
-        "DimensionKey": str,
-    },
-    total=False,
-)
-
 CostCategoryInheritedValueDimensionTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
     },
     total=False,
@@ -438,16 +383,16 @@
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
-DateIntervalOutputTypeDef = TypedDict(
-    "DateIntervalOutputTypeDef",
+DateIntervalTypeDef = TypedDict(
+    "DateIntervalTypeDef",
     {
         "Start": str,
         "End": str,
     },
 )
 
 CoverageCostTypeDef = TypedDict(
@@ -484,57 +429,35 @@
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagValuesOutputTypeDef = TypedDict(
     "TagValuesOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
     total=False,
 )
 
-DateIntervalTypeDef = TypedDict(
-    "DateIntervalTypeDef",
-    {
-        "Start": str,
-        "End": str,
-    },
-)
-
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorArn": str,
     },
 )
 
@@ -548,23 +471,14 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
@@ -670,22 +584,14 @@
         "NetworkOutBytesPerSecond": str,
         "NetworkPacketsInPerSecond": str,
         "NetworkPacketsOutPerSecond": str,
     },
     total=False,
 )
 
-EC2SpecificationOutputTypeDef = TypedDict(
-    "EC2SpecificationOutputTypeDef",
-    {
-        "OfferingClass": OfferingClassType,
-    },
-    total=False,
-)
-
 EC2SpecificationTypeDef = TypedDict(
     "EC2SpecificationTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
     total=False,
 )
@@ -783,23 +689,14 @@
     {
         "Type": GroupDefinitionTypeType,
         "Key": str,
     },
     total=False,
 )
 
-GroupDefinitionOutputTypeDef = TypedDict(
-    "GroupDefinitionOutputTypeDef",
-    {
-        "Type": GroupDefinitionTypeType,
-        "Key": str,
-    },
-    total=False,
-)
-
 _RequiredSortDefinitionTypeDef = TypedDict(
     "_RequiredSortDefinitionTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalSortDefinitionTypeDef = TypedDict(
@@ -809,26 +706,14 @@
     },
     total=False,
 )
 
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
     total=False,
@@ -871,22 +756,14 @@
     "RightsizingRecommendationConfigurationTypeDef",
     {
         "RecommendationTarget": RecommendationTargetType,
         "BenefitsConsidered": bool,
     },
 )
 
-RightsizingRecommendationConfigurationOutputTypeDef = TypedDict(
-    "RightsizingRecommendationConfigurationOutputTypeDef",
-    {
-        "RecommendationTarget": RecommendationTargetType,
-        "BenefitsConsidered": bool,
-    },
-)
-
 RightsizingRecommendationMetadataTypeDef = TypedDict(
     "RightsizingRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "AdditionalMetadata": str,
@@ -944,25 +821,14 @@
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
     total=False,
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "DatabaseEngine": str,
@@ -1023,38 +889,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ResourceTagOutputTypeDef = TypedDict(
-    "ResourceTagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 ProvideAnomalyFeedbackRequestRequestTypeDef = TypedDict(
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationDetailHourlyMetricsTypeDef = TypedDict(
     "RecommendationDetailHourlyMetricsTypeDef",
     {
         "StartTime": str,
         "EstimatedOnDemandCost": str,
         "CurrentCoverage": str,
         "EstimatedCoverage": str,
@@ -1069,25 +919,14 @@
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
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
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
     total=False,
@@ -1158,24 +997,14 @@
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
     total=False,
 )
 
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
     },
 )
@@ -1196,63 +1025,29 @@
 
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
-    {
-        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionOutputTypeDef",
     {
         "MonitorArnList": List[str],
-        "Subscribers": List[SubscriberOutputTypeDef],
+        "Subscribers": List[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
     },
 )
 _OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
     "_OptionalAnomalySubscriptionOutputTypeDef",
     {
@@ -1346,34 +1141,14 @@
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CostCategoryRuleOutputTypeDef = TypedDict(
-    "CostCategoryRuleOutputTypeDef",
-    {
-        "Value": str,
-        "Rule": "ExpressionOutputTypeDef",
-        "InheritedValue": CostCategoryInheritedValueDimensionOutputTypeDef,
-        "Type": CostCategoryRuleTypeType,
-    },
-    total=False,
-)
-
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionTypeDef,
         "Type": CostCategoryRuleTypeType,
@@ -1438,22 +1213,66 @@
     _RequiredCostCategorySplitChargeRuleTypeDef, _OptionalCostCategorySplitChargeRuleTypeDef
 ):
     pass
 
 ForecastResultTypeDef = TypedDict(
     "ForecastResultTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
     },
     total=False,
 )
 
+_RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
+    "_RequiredGetCostForecastRequestRequestTypeDef",
+    {
+        "TimePeriod": DateIntervalTypeDef,
+        "Metric": MetricType,
+        "Granularity": GranularityType,
+    },
+)
+_OptionalGetCostForecastRequestRequestTypeDef = TypedDict(
+    "_OptionalGetCostForecastRequestRequestTypeDef",
+    {
+        "Filter": "ExpressionTypeDef",
+        "PredictionIntervalLevel": int,
+    },
+    total=False,
+)
+
+class GetCostForecastRequestRequestTypeDef(
+    _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
+    "_RequiredGetUsageForecastRequestRequestTypeDef",
+    {
+        "TimePeriod": DateIntervalTypeDef,
+        "Metric": MetricType,
+        "Granularity": GranularityType,
+    },
+)
+_OptionalGetUsageForecastRequestRequestTypeDef = TypedDict(
+    "_OptionalGetUsageForecastRequestRequestTypeDef",
+    {
+        "Filter": "ExpressionTypeDef",
+        "PredictionIntervalLevel": int,
+    },
+    total=False,
+)
+
+class GetUsageForecastRequestRequestTypeDef(
+    _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
+):
+    pass
+
 CoverageTypeDef = TypedDict(
     "CoverageTypeDef",
     {
         "CoverageHours": CoverageHoursTypeDef,
         "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
         "CoverageCost": CoverageCostTypeDef,
     },
@@ -1484,57 +1303,139 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 
-_RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
-    "_RequiredGetCostForecastRequestRequestTypeDef",
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
-        "Metric": MetricType,
-        "Granularity": GranularityType,
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGetCostForecastRequestRequestTypeDef = TypedDict(
-    "_OptionalGetCostForecastRequestRequestTypeDef",
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
     {
-        "Filter": "ExpressionTypeDef",
-        "PredictionIntervalLevel": int,
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class GetCostForecastRequestRequestTypeDef(
-    _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
-):
-    pass
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
-    "_RequiredGetUsageForecastRequestRequestTypeDef",
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
     {
-        "TimePeriod": DateIntervalTypeDef,
-        "Metric": MetricType,
-        "Granularity": GranularityType,
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGetUsageForecastRequestRequestTypeDef = TypedDict(
-    "_OptionalGetUsageForecastRequestRequestTypeDef",
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
     {
-        "Filter": "ExpressionTypeDef",
-        "PredictionIntervalLevel": int,
+        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class GetUsageForecastRequestRequestTypeDef(
-    _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
-):
-    pass
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ExpressionOutputTypeDef = TypedDict(
     "ExpressionOutputTypeDef",
     {
         "Or": List[Dict[str, Any]],
         "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
@@ -1548,15 +1449,15 @@
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
@@ -1573,22 +1474,14 @@
         "EBSResourceUtilization": EBSResourceUtilizationTypeDef,
         "DiskResourceUtilization": DiskResourceUtilizationTypeDef,
         "NetworkResourceUtilization": NetworkResourceUtilizationTypeDef,
     },
     total=False,
 )
 
-ServiceSpecificationOutputTypeDef = TypedDict(
-    "ServiceSpecificationOutputTypeDef",
-    {
-        "EC2Specification": EC2SpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 ServiceSpecificationTypeDef = TypedDict(
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
@@ -1607,15 +1500,15 @@
 )
 
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1933,22 +1826,14 @@
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceTags": List[ResourceTagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationDetailDataTypeDef = TypedDict(
     "RecommendationDetailDataTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
@@ -1982,15 +1867,15 @@
 )
 
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
     },
     total=False,
 )
 
 SavingsPlansPurchaseRecommendationDetailTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     {
@@ -2035,15 +1920,15 @@
     _OptionalSavingsPlansUtilizationAggregatesTypeDef,
 ):
     pass
 
 _RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
     "_RequiredSavingsPlansUtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
     },
 )
 _OptionalSavingsPlansUtilizationByTimeTypeDef = TypedDict(
     "_OptionalSavingsPlansUtilizationByTimeTypeDef",
     {
         "Savings": SavingsPlansSavingsTypeDef,
@@ -2069,24 +1954,24 @@
     total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnomalySubscriptionsResponseTypeDef = TypedDict(
     "GetAnomalySubscriptionsResponseTypeDef",
     {
         "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -2107,35 +1992,35 @@
     pass
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCostCategoryTypeDef = TypedDict(
     "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": List[CostCategoryRuleOutputTypeDef],
+        "Rules": List[CostCategoryRuleTypeDef],
     },
 )
 _OptionalCostCategoryTypeDef = TypedDict(
     "_OptionalCostCategoryTypeDef",
     {
         "EffectiveEnd": str,
         "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
@@ -2198,24 +2083,24 @@
     pass
 
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
@@ -2259,26 +2144,26 @@
     _OptionalGetReservationPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
 ResultByTimeTypeDef = TypedDict(
     "ResultByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
     },
     total=False,
 )
 
 UtilizationByTimeTypeDef = TypedDict(
     "UtilizationByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationUtilizationGroupTypeDef],
         "Total": ReservationAggregatesTypeDef,
     },
     total=False,
 )
 
 ReservationPurchaseRecommendationDetailTypeDef = TypedDict(
@@ -2308,24 +2193,24 @@
 )
 
 GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     {
         "RecommendationDetailId": str,
         "RecommendationDetailData": RecommendationDetailDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2344,41 +2229,41 @@
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
-        "TimePeriod": DateIntervalOutputTypeDef,
+        "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
     total=False,
 )
 
 CurrentInstanceTypeDef = TypedDict(
@@ -2413,73 +2298,73 @@
     total=False,
 )
 
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
+        "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
-        "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
+        "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
-        "ServiceSpecification": ServiceSpecificationOutputTypeDef,
+        "ServiceSpecification": ServiceSpecificationTypeDef,
         "RecommendationDetails": List[ReservationPurchaseRecommendationDetailTypeDef],
         "RecommendationSummary": ReservationPurchaseRecommendationSummaryTypeDef,
     },
     total=False,
 )
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
@@ -2489,15 +2374,15 @@
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
@@ -2513,11 +2398,11 @@
 GetRightsizingRecommendationResponseTypeDef = TypedDict(
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
-        "Configuration": RightsizingRecommendationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Configuration": RightsizingRecommendationConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.12
-Summary: Type annotations for boto3.CostExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,126 +330,117 @@
 
 `mypy_boto3_ce.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
-    AnomalyMonitorOutputTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
-    SubscriberOutputTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
-    CostCategoryInheritedValueDimensionOutputTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
     CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
     CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
-    DateIntervalOutputTypeDef,
+    DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagValuesOutputTypeDef,
-    DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
-    EC2SpecificationOutputTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
     TagValuesTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
-    GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
-    RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
     RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
-    CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
+    GetCostForecastRequestRequestTypeDef,
+    GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    GetCostForecastRequestRequestTypeDef,
-    GetUsageForecastRequestRequestTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
     ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
-    ServiceSpecificationOutputTypeDef,
     ServiceSpecificationTypeDef,
     ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
@@ -460,15 +451,14 @@
     GetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     GetSavingsPlansUtilizationRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GroupTypeDef,
     ReservationUtilizationGroupTypeDef,
     GetRightsizingRecommendationRequestRequestTypeDef,
     InstanceDetailsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RecommendationDetailDataTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy-boto3-ce-1.28.15/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.12/setup.py` & `mypy-boto3-ce-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostExplorer 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CostExplorer 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

