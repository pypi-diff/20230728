# Comparing `tmp/mypy-boto3-xray-1.28.12.tar.gz` & `tmp/mypy-boto3-xray-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-xray-1.28.12.tar", last modified: Thu Jul 27 11:49:51 2023, max compression
+gzip compressed data, was "mypy-boto3-xray-1.28.15.tar", last modified: Fri Jul 28 20:43:58 2023, max compression
```

## Comparing `mypy-boto3-xray-1.28.12.tar` & `mypy-boto3-xray-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/mypy_boto3_xray/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-07-27 11:49:06.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44354 2023-07-27 11:49:05.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:51.000000 mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:51.225508 mypy-boto3-xray-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 11:49:04.000000 mypy-boto3-xray-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.378065 mypy-boto3-xray-1.28.15/mypy_boto3_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25897 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-28 20:41:50.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44015 2023-07-28 20:41:51.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43964 2023-07-28 20:41:50.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:58.000000 mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:58.386065 mypy-boto3-xray-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 20:41:49.000000 mypy-boto3-xray-1.28.15/setup.py
```

### Comparing `mypy-boto3-xray-1.28.12/LICENSE` & `mypy-boto3-xray-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/PKG-INFO` & `mypy-boto3-xray-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.12
-Summary: Type annotations for boto3.XRay 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,23 +399,21 @@
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
     GetServiceGraphRequestRequestTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
-    InsightsConfigurationOutputTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
     SamplingRuleOutputTypeDef,
@@ -431,52 +429,52 @@
     GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    GroupSummaryTypeDef,
+    GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
-    GroupSummaryTypeDef,
-    GroupTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     SamplingRuleRecordTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
     PutTelemetryRecordsRequestRequestTypeDef,
-    EdgeTypeDef,
-    TimeSeriesServiceStatisticsTypeDef,
-    ErrorRootCauseServiceTypeDef,
-    FaultRootCauseServiceTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
+    EdgeTypeDef,
+    TimeSeriesServiceStatisticsTypeDef,
+    ErrorRootCauseServiceTypeDef,
+    FaultRootCauseServiceTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
```

### Comparing `mypy-boto3-xray-1.28.12/README.md` & `mypy-boto3-xray-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,23 +367,21 @@
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
     GetServiceGraphRequestRequestTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
-    InsightsConfigurationOutputTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
     SamplingRuleOutputTypeDef,
@@ -399,52 +397,52 @@
     GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    GroupSummaryTypeDef,
+    GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
-    GroupSummaryTypeDef,
-    GroupTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     SamplingRuleRecordTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
     PutTelemetryRecordsRequestRequestTypeDef,
-    EdgeTypeDef,
-    TimeSeriesServiceStatisticsTypeDef,
-    ErrorRootCauseServiceTypeDef,
-    FaultRootCauseServiceTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
+    EdgeTypeDef,
+    TimeSeriesServiceStatisticsTypeDef,
+    ErrorRootCauseServiceTypeDef,
+    FaultRootCauseServiceTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
```

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.py` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/__init__.pyi` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/__main__.py` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.XRay 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.XRay 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
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

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.py` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/client.pyi` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.py` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/literals.pyi` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.py` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/paginator.pyi` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.py` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,23 +66,21 @@
     "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
     "GetServiceGraphRequestRequestTypeDef",
     "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
-    "InsightsConfigurationOutputTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
     "SamplingRuleOutputTypeDef",
@@ -98,52 +96,52 @@
     "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "GroupSummaryTypeDef",
+    "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
-    "GroupSummaryTypeDef",
-    "GroupTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
     "SamplingRuleRecordTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
     "PutTelemetryRecordsRequestRequestTypeDef",
-    "EdgeTypeDef",
-    "TimeSeriesServiceStatisticsTypeDef",
-    "ErrorRootCauseServiceTypeDef",
-    "FaultRootCauseServiceTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
+    "EdgeTypeDef",
+    "TimeSeriesServiceStatisticsTypeDef",
+    "ErrorRootCauseServiceTypeDef",
+    "FaultRootCauseServiceTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
     "CreateSamplingRuleResultTypeDef",
     "DeleteSamplingRuleResultTypeDef",
     "GetSamplingRulesResultTypeDef",
     "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
@@ -647,23 +645,14 @@
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
 )
 
-InsightsConfigurationOutputTypeDef = TypedDict(
-    "InsightsConfigurationOutputTypeDef",
-    {
-        "InsightsEnabled": bool,
-        "NotificationsEnabled": bool,
-    },
-    total=False,
-)
-
 HttpTypeDef = TypedDict(
     "HttpTypeDef",
     {
         "HttpURL": str,
         "HttpStatus": int,
         "HttpMethod": str,
         "UserAgent": str,
@@ -735,22 +724,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
 _OptionalPutEncryptionConfigRequestRequestTypeDef = TypedDict(
@@ -1091,14 +1072,36 @@
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
 
+GroupSummaryTypeDef = TypedDict(
+    "GroupSummaryTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationTypeDef,
+    },
+    total=False,
+)
+
+GroupTypeDef = TypedDict(
+    "GroupTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationTypeDef,
+    },
+    total=False,
+)
+
 UpdateGroupRequestRequestTypeDef = TypedDict(
     "UpdateGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -1125,14 +1128,23 @@
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1294,36 +1306,14 @@
 
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
 
-GroupSummaryTypeDef = TypedDict(
-    "GroupSummaryTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-GroupTypeDef = TypedDict(
-    "GroupTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1346,23 +1336,14 @@
     "PutResourcePolicyResultTypeDef",
     {
         "ResourcePolicy": ResourcePolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1479,14 +1460,47 @@
 class PutTelemetryRecordsRequestRequestTypeDef(
     _RequiredPutTelemetryRecordsRequestRequestTypeDef,
     _OptionalPutTelemetryRecordsRequestRequestTypeDef,
 ):
     pass
 
 
+GetGroupsResultTypeDef = TypedDict(
+    "GetGroupsResultTypeDef",
+    {
+        "Groups": List[GroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResultTypeDef = TypedDict(
+    "CreateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResultTypeDef = TypedDict(
+    "GetGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGroupResultTypeDef = TypedDict(
+    "UpdateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
         "StartTime": datetime,
         "EndTime": datetime,
         "SummaryStatistics": EdgeStatisticsTypeDef,
@@ -1532,47 +1546,14 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
-GetGroupsResultTypeDef = TypedDict(
-    "GetGroupsResultTypeDef",
-    {
-        "Groups": List[GroupSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupResultTypeDef = TypedDict(
-    "CreateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupResultTypeDef = TypedDict(
-    "GetGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGroupResultTypeDef = TypedDict(
-    "UpdateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
```

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray/type_defs.pyi` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,23 +65,21 @@
     "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
     "GetServiceGraphRequestRequestTypeDef",
     "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
-    "InsightsConfigurationOutputTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
     "SamplingRuleOutputTypeDef",
@@ -97,52 +95,52 @@
     "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "GroupSummaryTypeDef",
+    "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
-    "GroupSummaryTypeDef",
-    "GroupTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
     "SamplingRuleRecordTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
     "PutTelemetryRecordsRequestRequestTypeDef",
-    "EdgeTypeDef",
-    "TimeSeriesServiceStatisticsTypeDef",
-    "ErrorRootCauseServiceTypeDef",
-    "FaultRootCauseServiceTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
+    "EdgeTypeDef",
+    "TimeSeriesServiceStatisticsTypeDef",
+    "ErrorRootCauseServiceTypeDef",
+    "FaultRootCauseServiceTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
     "CreateSamplingRuleResultTypeDef",
     "DeleteSamplingRuleResultTypeDef",
     "GetSamplingRulesResultTypeDef",
     "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
@@ -626,23 +624,14 @@
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
 )
 
-InsightsConfigurationOutputTypeDef = TypedDict(
-    "InsightsConfigurationOutputTypeDef",
-    {
-        "InsightsEnabled": bool,
-        "NotificationsEnabled": bool,
-    },
-    total=False,
-)
-
 HttpTypeDef = TypedDict(
     "HttpTypeDef",
     {
         "HttpURL": str,
         "HttpStatus": int,
         "HttpMethod": str,
         "UserAgent": str,
@@ -712,22 +701,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
 _OptionalPutEncryptionConfigRequestRequestTypeDef = TypedDict(
@@ -1050,14 +1031,36 @@
 
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+GroupSummaryTypeDef = TypedDict(
+    "GroupSummaryTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationTypeDef,
+    },
+    total=False,
+)
+
+GroupTypeDef = TypedDict(
+    "GroupTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "FilterExpression": str,
+        "InsightsConfiguration": InsightsConfigurationTypeDef,
+    },
+    total=False,
+)
+
 UpdateGroupRequestRequestTypeDef = TypedDict(
     "UpdateGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -1082,14 +1085,23 @@
 )
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1245,36 +1257,14 @@
 )
 
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
-GroupSummaryTypeDef = TypedDict(
-    "GroupSummaryTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-GroupTypeDef = TypedDict(
-    "GroupTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "FilterExpression": str,
-        "InsightsConfiguration": InsightsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1297,23 +1287,14 @@
     "PutResourcePolicyResultTypeDef",
     {
         "ResourcePolicy": ResourcePolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1428,14 +1409,47 @@
 
 class PutTelemetryRecordsRequestRequestTypeDef(
     _RequiredPutTelemetryRecordsRequestRequestTypeDef,
     _OptionalPutTelemetryRecordsRequestRequestTypeDef,
 ):
     pass
 
+GetGroupsResultTypeDef = TypedDict(
+    "GetGroupsResultTypeDef",
+    {
+        "Groups": List[GroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResultTypeDef = TypedDict(
+    "CreateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResultTypeDef = TypedDict(
+    "GetGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGroupResultTypeDef = TypedDict(
+    "UpdateGroupResultTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
         "StartTime": datetime,
         "EndTime": datetime,
         "SummaryStatistics": EdgeStatisticsTypeDef,
@@ -1481,47 +1495,14 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
-GetGroupsResultTypeDef = TypedDict(
-    "GetGroupsResultTypeDef",
-    {
-        "Groups": List[GroupSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupResultTypeDef = TypedDict(
-    "CreateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupResultTypeDef = TypedDict(
-    "GetGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGroupResultTypeDef = TypedDict(
-    "UpdateGroupResultTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
```

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/PKG-INFO` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-xray
-Version: 1.28.12
-Summary: Type annotations for boto3.XRay 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-xray.svg?color=blue)](https://pypi.org/project/mypy-boto3-xray)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-xray)](https://pepy.tech/project/mypy-boto3-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.XRay 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[boto3.XRay 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [mypy-boto3-xray docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_xray/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,23 +399,21 @@
     SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
     GetServiceGraphRequestRequestTypeDef,
     GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
-    InsightsConfigurationOutputTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
     SamplingRuleOutputTypeDef,
@@ -431,52 +429,52 @@
     GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    GroupSummaryTypeDef,
+    GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
     GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
-    GroupSummaryTypeDef,
-    GroupTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
     SamplingRuleRecordTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
     PutTelemetryRecordsRequestRequestTypeDef,
-    EdgeTypeDef,
-    TimeSeriesServiceStatisticsTypeDef,
-    ErrorRootCauseServiceTypeDef,
-    FaultRootCauseServiceTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
+    EdgeTypeDef,
+    TimeSeriesServiceStatisticsTypeDef,
+    ErrorRootCauseServiceTypeDef,
+    FaultRootCauseServiceTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
     CreateSamplingRuleResultTypeDef,
     DeleteSamplingRuleResultTypeDef,
     GetSamplingRulesResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
```

### Comparing `mypy-boto3-xray-1.28.12/mypy_boto3_xray.egg-info/SOURCES.txt` & `mypy-boto3-xray-1.28.15/mypy_boto3_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-xray-1.28.12/setup.py` & `mypy-boto3-xray-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-xray",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.XRay 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.XRay 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

