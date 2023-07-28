# Comparing `tmp/mypy-boto3-application-insights-1.28.12.tar.gz` & `tmp/mypy-boto3-application-insights-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-insights-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-application-insights-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
```

## Comparing `mypy-boto3-application-insights-1.28.12.tar` & `mypy-boto3-application-insights-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.472577 mypy-boto3-application-insights-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-27 05:34:18.464577 mypy-boto3-application-insights-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.464577 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20900 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19938 2023-07-27 05:17:26.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19923 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.464577 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.472577 mypy-boto3-application-insights-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.688180 mypy-boto3-application-insights-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15502 2023-07-28 19:47:31.688180 mypy-boto3-application-insights-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.684180 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25242 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27974 2023-07-28 19:46:49.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:46:48.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.684180 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15502 2023-07-28 19:47:31.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-28 19:47:31.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 19:47:31.000000 mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.688180 mypy-boto3-application-insights-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-28 19:46:47.000000 mypy-boto3-application-insights-1.28.15/setup.py
```

### Comparing `mypy-boto3-application-insights-1.28.12/LICENSE` & `mypy-boto3-application-insights-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.12/PKG-INFO` & `mypy-boto3-application-insights-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationInsights 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationInsights 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,17 +286,21 @@
     ConfigurationEventStatusType,
     DiscoveryTypeType,
     FeedbackKeyType,
     FeedbackValueType,
     GroupingTypeType,
     LogFilterType,
     OsTypeType,
+    RecommendationTypeType,
+    ResolutionMethodType,
     SeverityLevelType,
     StatusType,
     TierType,
+    UpdateStatusType,
+    VisibilityType,
     ApplicationInsightsServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -309,74 +313,85 @@
 ### Typed dictionaries
 
 `mypy_boto3_application_insights.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
+    WorkloadConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
+    DescribeWorkloadRequestRequestTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
-    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ResponseMetadataTypeDef,
+    ListWorkloadsRequestRequestTypeDef,
+    WorkloadTypeDef,
+    RemoveWorkloadRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
+    UpdateProblemRequestRequestTypeDef,
+    AddWorkloadRequestRequestTypeDef,
+    UpdateWorkloadRequestRequestTypeDef,
+    AddWorkloadResponseTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
+    DescribeWorkloadResponseTypeDef,
+    ListLogPatternSetsResponseTypeDef,
+    UpdateWorkloadResponseTypeDef,
     DescribeComponentResponseTypeDef,
     ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListWorkloadsResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationComponentTypeDef:
+def get_structure() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-insights-1.28.12/README.md` & `mypy-boto3-application-insights-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -254,17 +254,21 @@
     ConfigurationEventStatusType,
     DiscoveryTypeType,
     FeedbackKeyType,
     FeedbackValueType,
     GroupingTypeType,
     LogFilterType,
     OsTypeType,
+    RecommendationTypeType,
+    ResolutionMethodType,
     SeverityLevelType,
     StatusType,
     TierType,
+    UpdateStatusType,
+    VisibilityType,
     ApplicationInsightsServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -277,74 +281,85 @@
 ### Typed dictionaries
 
 `mypy_boto3_application_insights.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
+    WorkloadConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
+    DescribeWorkloadRequestRequestTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
-    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ResponseMetadataTypeDef,
+    ListWorkloadsRequestRequestTypeDef,
+    WorkloadTypeDef,
+    RemoveWorkloadRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
+    UpdateProblemRequestRequestTypeDef,
+    AddWorkloadRequestRequestTypeDef,
+    UpdateWorkloadRequestRequestTypeDef,
+    AddWorkloadResponseTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
+    DescribeWorkloadResponseTypeDef,
+    ListLogPatternSetsResponseTypeDef,
+    UpdateWorkloadResponseTypeDef,
     DescribeComponentResponseTypeDef,
     ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListWorkloadsResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationComponentTypeDef:
+def get_structure() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__main__.py` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationInsights 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ApplicationInsights 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.py` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,36 +15,41 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ConfigurationEventStatusType, TierType
+from .literals import ConfigurationEventStatusType, RecommendationTypeType, TierType, VisibilityType
 from .type_defs import (
+    AddWorkloadResponseTypeDef,
     CreateApplicationResponseTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
     DescribeProblemResponseTypeDef,
+    DescribeWorkloadResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListWorkloadsResponseTypeDef,
     TagTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
+    UpdateWorkloadResponseTypeDef,
+    WorkloadConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -85,14 +90,28 @@
         """
         ApplicationInsightsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#exceptions)
         """
 
+    def add_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef
+    ) -> AddWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.add_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#add_workload)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#can_paginate)
         """
@@ -172,89 +191,110 @@
         """
         Removes the specified log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#delete_log_pattern)
         """
 
-    def describe_application(self, *, ResourceGroupName: str) -> DescribeApplicationResponseTypeDef:
+    def describe_application(
+        self, *, ResourceGroupName: str, AccountId: str = ...
+    ) -> DescribeApplicationResponseTypeDef:
         """
         Describes the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_application)
         """
 
     def describe_component(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentResponseTypeDef:
         """
         Describes a component and lists the resources that are grouped together in a
         component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component)
         """
 
     def describe_component_configuration(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentConfigurationResponseTypeDef:
         """
         Describes the monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component_configuration)
         """
 
     def describe_component_configuration_recommendation(
-        self, *, ResourceGroupName: str, ComponentName: str, Tier: TierType
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        Tier: TierType,
+        RecommendationType: RecommendationTypeType = ...
     ) -> DescribeComponentConfigurationRecommendationResponseTypeDef:
         """
         Describes the recommended monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component_configuration_recommendation)
         """
 
     def describe_log_pattern(
-        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
+        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str, AccountId: str = ...
     ) -> DescribeLogPatternResponseTypeDef:
         """
         Describe a specific log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_log_pattern)
         """
 
-    def describe_observation(self, *, ObservationId: str) -> DescribeObservationResponseTypeDef:
+    def describe_observation(
+        self, *, ObservationId: str, AccountId: str = ...
+    ) -> DescribeObservationResponseTypeDef:
         """
         Describes an anomaly or error with the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_observation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_observation)
         """
 
-    def describe_problem(self, *, ProblemId: str) -> DescribeProblemResponseTypeDef:
+    def describe_problem(
+        self, *, ProblemId: str, AccountId: str = ...
+    ) -> DescribeProblemResponseTypeDef:
         """
         Describes an application problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_problem)
         """
 
     def describe_problem_observations(
-        self, *, ProblemId: str
+        self, *, ProblemId: str, AccountId: str = ...
     ) -> DescribeProblemObservationsResponseTypeDef:
         """
         Describes the anomalies or errors associated with the problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem_observations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_problem_observations)
         """
 
+    def describe_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str, AccountId: str = ...
+    ) -> DescribeWorkloadResponseTypeDef:
+        """
+        Describes a workload and its configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_workload)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -262,25 +302,30 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#generate_presigned_url)
         """
 
     def list_applications(
-        self, *, MaxResults: int = ..., NextToken: str = ...
+        self, *, MaxResults: int = ..., NextToken: str = ..., AccountId: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the IDs of the applications that you are monitoring.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_applications)
         """
 
     def list_components(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListComponentsResponseTypeDef:
         """
         Lists the auto-grouped, standalone, and custom components of the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_components)
         """
@@ -289,58 +334,67 @@
         self,
         *,
         ResourceGroupName: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_configuration_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_configuration_history)
         """
 
     def list_log_pattern_sets(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternSetsResponseTypeDef:
         """
         Lists the log pattern sets in the specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_pattern_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_log_pattern_sets)
         """
 
     def list_log_patterns(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternsResponseTypeDef:
         """
         Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_log_patterns)
         """
 
     def list_problems(
         self,
         *,
+        AccountId: str = ...,
         ResourceGroupName: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ComponentName: str = ...
+        ComponentName: str = ...,
+        Visibility: VisibilityType = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_problems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_problems)
         """
@@ -350,14 +404,40 @@
         Retrieve a list of the tags (keys and values) that are associated with a
         specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_tags_for_resource)
         """
 
+    def list_workloads(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
+    ) -> ListWorkloadsResponseTypeDef:
+        """
+        Lists the workloads that are configured on a given component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_workloads)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_workloads)
+        """
+
+    def remove_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str
+    ) -> Dict[str, Any]:
+        """
+        Remove workload from a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.remove_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#remove_workload)
+        """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Add one or more tags (keys and values) to a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#tag_resource)
         """
@@ -431,7 +511,36 @@
     ) -> UpdateLogPatternResponseTypeDef:
         """
         Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_log_pattern)
         """
+
+    def update_problem(
+        self,
+        *,
+        ProblemId: str,
+        UpdateStatus: Literal["RESOLVED"] = ...,
+        Visibility: VisibilityType = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the visibility of the problem or specifies the problem as `RESOLVED`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_problem)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_problem)
+        """
+
+    def update_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef,
+        WorkloadId: str = ...
+    ) -> UpdateWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_workload)
+        """
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.pyi` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -15,36 +15,41 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ConfigurationEventStatusType, TierType
+from .literals import ConfigurationEventStatusType, RecommendationTypeType, TierType, VisibilityType
 from .type_defs import (
+    AddWorkloadResponseTypeDef,
     CreateApplicationResponseTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
     DescribeProblemResponseTypeDef,
+    DescribeWorkloadResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListWorkloadsResponseTypeDef,
     TagTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
+    UpdateWorkloadResponseTypeDef,
+    WorkloadConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -80,14 +85,27 @@
     def exceptions(self) -> Exceptions:
         """
         ApplicationInsightsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#exceptions)
         """
+    def add_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef
+    ) -> AddWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.add_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#add_workload)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#can_paginate)
         """
@@ -159,105 +177,130 @@
     ) -> Dict[str, Any]:
         """
         Removes the specified log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#delete_log_pattern)
         """
-    def describe_application(self, *, ResourceGroupName: str) -> DescribeApplicationResponseTypeDef:
+    def describe_application(
+        self, *, ResourceGroupName: str, AccountId: str = ...
+    ) -> DescribeApplicationResponseTypeDef:
         """
         Describes the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_application)
         """
     def describe_component(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentResponseTypeDef:
         """
         Describes a component and lists the resources that are grouped together in a
         component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component)
         """
     def describe_component_configuration(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentConfigurationResponseTypeDef:
         """
         Describes the monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component_configuration)
         """
     def describe_component_configuration_recommendation(
-        self, *, ResourceGroupName: str, ComponentName: str, Tier: TierType
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        Tier: TierType,
+        RecommendationType: RecommendationTypeType = ...
     ) -> DescribeComponentConfigurationRecommendationResponseTypeDef:
         """
         Describes the recommended monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component_configuration_recommendation)
         """
     def describe_log_pattern(
-        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
+        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str, AccountId: str = ...
     ) -> DescribeLogPatternResponseTypeDef:
         """
         Describe a specific log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_log_pattern)
         """
-    def describe_observation(self, *, ObservationId: str) -> DescribeObservationResponseTypeDef:
+    def describe_observation(
+        self, *, ObservationId: str, AccountId: str = ...
+    ) -> DescribeObservationResponseTypeDef:
         """
         Describes an anomaly or error with the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_observation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_observation)
         """
-    def describe_problem(self, *, ProblemId: str) -> DescribeProblemResponseTypeDef:
+    def describe_problem(
+        self, *, ProblemId: str, AccountId: str = ...
+    ) -> DescribeProblemResponseTypeDef:
         """
         Describes an application problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_problem)
         """
     def describe_problem_observations(
-        self, *, ProblemId: str
+        self, *, ProblemId: str, AccountId: str = ...
     ) -> DescribeProblemObservationsResponseTypeDef:
         """
         Describes the anomalies or errors associated with the problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem_observations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_problem_observations)
         """
+    def describe_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str, AccountId: str = ...
+    ) -> DescribeWorkloadResponseTypeDef:
+        """
+        Describes a workload and its configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_workload)
+        """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#generate_presigned_url)
         """
     def list_applications(
-        self, *, MaxResults: int = ..., NextToken: str = ...
+        self, *, MaxResults: int = ..., NextToken: str = ..., AccountId: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the IDs of the applications that you are monitoring.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_applications)
         """
     def list_components(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListComponentsResponseTypeDef:
         """
         Lists the auto-grouped, standalone, and custom components of the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_components)
         """
@@ -265,55 +308,64 @@
         self,
         *,
         ResourceGroupName: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_configuration_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_configuration_history)
         """
     def list_log_pattern_sets(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternSetsResponseTypeDef:
         """
         Lists the log pattern sets in the specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_pattern_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_log_pattern_sets)
         """
     def list_log_patterns(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternsResponseTypeDef:
         """
         Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_log_patterns)
         """
     def list_problems(
         self,
         *,
+        AccountId: str = ...,
         ResourceGroupName: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ComponentName: str = ...
+        ComponentName: str = ...,
+        Visibility: VisibilityType = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_problems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_problems)
         """
@@ -321,14 +373,38 @@
         """
         Retrieve a list of the tags (keys and values) that are associated with a
         specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_tags_for_resource)
         """
+    def list_workloads(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
+    ) -> ListWorkloadsResponseTypeDef:
+        """
+        Lists the workloads that are configured on a given component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_workloads)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_workloads)
+        """
+    def remove_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str
+    ) -> Dict[str, Any]:
+        """
+        Remove workload from a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.remove_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#remove_workload)
+        """
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Add one or more tags (keys and values) to a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#tag_resource)
         """
@@ -397,7 +473,34 @@
     ) -> UpdateLogPatternResponseTypeDef:
         """
         Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_log_pattern)
         """
+    def update_problem(
+        self,
+        *,
+        ProblemId: str,
+        UpdateStatus: Literal["RESOLVED"] = ...,
+        Visibility: VisibilityType = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the visibility of the problem or specifies the problem as `RESOLVED`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_problem)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_problem)
+        """
+    def update_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef,
+        WorkloadId: str = ...
+    ) -> UpdateWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_workload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_workload)
+        """
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.py` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,21 @@
     "ConfigurationEventStatusType",
     "DiscoveryTypeType",
     "FeedbackKeyType",
     "FeedbackValueType",
     "GroupingTypeType",
     "LogFilterType",
     "OsTypeType",
+    "RecommendationTypeType",
+    "ResolutionMethodType",
     "SeverityLevelType",
     "StatusType",
     "TierType",
+    "UpdateStatusType",
+    "VisibilityType",
     "ApplicationInsightsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
@@ -46,16 +50,18 @@
 ConfigurationEventStatusType = Literal["ERROR", "INFO", "WARN"]
 DiscoveryTypeType = Literal["ACCOUNT_BASED", "RESOURCE_GROUP_BASED"]
 FeedbackKeyType = Literal["INSIGHTS_FEEDBACK"]
 FeedbackValueType = Literal["NOT_SPECIFIED", "NOT_USEFUL", "USEFUL"]
 GroupingTypeType = Literal["ACCOUNT_BASED"]
 LogFilterType = Literal["ERROR", "INFO", "WARN"]
 OsTypeType = Literal["LINUX", "WINDOWS"]
+RecommendationTypeType = Literal["ALL", "INFRA_ONLY", "WORKLOAD_ONLY"]
+ResolutionMethodType = Literal["AUTOMATIC", "MANUAL", "UNRESOLVED"]
 SeverityLevelType = Literal["High", "Informative", "Low", "Medium"]
-StatusType = Literal["IGNORE", "PENDING", "RECURRING", "RESOLVED"]
+StatusType = Literal["IGNORE", "PENDING", "RECOVERING", "RECURRING", "RESOLVED"]
 TierType = Literal[
     "ACTIVE_DIRECTORY",
     "CUSTOM",
     "DEFAULT",
     "DOT_NET_CORE",
     "DOT_NET_WEB",
     "DOT_NET_WEB_TIER",
@@ -63,19 +69,24 @@
     "JAVA_JMX",
     "MYSQL",
     "ORACLE",
     "POSTGRESQL",
     "SAP_HANA_HIGH_AVAILABILITY",
     "SAP_HANA_MULTI_NODE",
     "SAP_HANA_SINGLE_NODE",
+    "SAP_NETWEAVER_DISTRIBUTED",
+    "SAP_NETWEAVER_HIGH_AVAILABILITY",
+    "SAP_NETWEAVER_STANDARD",
     "SHAREPOINT",
     "SQL_SERVER",
     "SQL_SERVER_ALWAYSON_AVAILABILITY_GROUP",
     "SQL_SERVER_FAILOVER_CLUSTER_INSTANCE",
 ]
+UpdateStatusType = Literal["RESOLVED"]
+VisibilityType = Literal["IGNORED", "VISIBLE"]
 ApplicationInsightsServiceName = Literal["application-insights"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.pyi` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,21 @@
     "ConfigurationEventStatusType",
     "DiscoveryTypeType",
     "FeedbackKeyType",
     "FeedbackValueType",
     "GroupingTypeType",
     "LogFilterType",
     "OsTypeType",
+    "RecommendationTypeType",
+    "ResolutionMethodType",
     "SeverityLevelType",
     "StatusType",
     "TierType",
+    "UpdateStatusType",
+    "VisibilityType",
     "ApplicationInsightsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 CloudWatchEventSourceType = Literal["CODE_DEPLOY", "EC2", "HEALTH", "RDS"]
@@ -44,16 +48,18 @@
 ConfigurationEventStatusType = Literal["ERROR", "INFO", "WARN"]
 DiscoveryTypeType = Literal["ACCOUNT_BASED", "RESOURCE_GROUP_BASED"]
 FeedbackKeyType = Literal["INSIGHTS_FEEDBACK"]
 FeedbackValueType = Literal["NOT_SPECIFIED", "NOT_USEFUL", "USEFUL"]
 GroupingTypeType = Literal["ACCOUNT_BASED"]
 LogFilterType = Literal["ERROR", "INFO", "WARN"]
 OsTypeType = Literal["LINUX", "WINDOWS"]
+RecommendationTypeType = Literal["ALL", "INFRA_ONLY", "WORKLOAD_ONLY"]
+ResolutionMethodType = Literal["AUTOMATIC", "MANUAL", "UNRESOLVED"]
 SeverityLevelType = Literal["High", "Informative", "Low", "Medium"]
-StatusType = Literal["IGNORE", "PENDING", "RECURRING", "RESOLVED"]
+StatusType = Literal["IGNORE", "PENDING", "RECOVERING", "RECURRING", "RESOLVED"]
 TierType = Literal[
     "ACTIVE_DIRECTORY",
     "CUSTOM",
     "DEFAULT",
     "DOT_NET_CORE",
     "DOT_NET_WEB",
     "DOT_NET_WEB_TIER",
@@ -61,19 +67,24 @@
     "JAVA_JMX",
     "MYSQL",
     "ORACLE",
     "POSTGRESQL",
     "SAP_HANA_HIGH_AVAILABILITY",
     "SAP_HANA_MULTI_NODE",
     "SAP_HANA_SINGLE_NODE",
+    "SAP_NETWEAVER_DISTRIBUTED",
+    "SAP_NETWEAVER_HIGH_AVAILABILITY",
+    "SAP_NETWEAVER_STANDARD",
     "SHAREPOINT",
     "SQL_SERVER",
     "SQL_SERVER_ALWAYSON_AVAILABILITY_GROUP",
     "SQL_SERVER_FAILOVER_CLUSTER_INSTANCE",
 ]
+UpdateStatusType = Literal["RESOLVED"]
+VisibilityType = Literal["IGNORED", "VISIBLE"]
 ApplicationInsightsServiceName = Literal["application-insights"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.py` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,105 +2,140 @@
 Type annotations for application-insights service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_application_insights.type_defs import ApplicationComponentTypeDef
+    from mypy_boto3_application_insights.type_defs import WorkloadConfigurationTypeDef
 
-    data: ApplicationComponentTypeDef = {...}
+    data: WorkloadConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CloudWatchEventSourceType,
     ConfigurationEventResourceTypeType,
     ConfigurationEventStatusType,
     DiscoveryTypeType,
     FeedbackValueType,
     LogFilterType,
     OsTypeType,
+    RecommendationTypeType,
+    ResolutionMethodType,
     SeverityLevelType,
     StatusType,
     TierType,
+    VisibilityType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "WorkloadConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationRequestRequestTypeDef",
-    "DescribeComponentConfigurationResponseTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
+    "DescribeWorkloadRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListWorkloadsRequestRequestTypeDef",
+    "WorkloadTypeDef",
+    "RemoveWorkloadRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
+    "UpdateProblemRequestRequestTypeDef",
+    "AddWorkloadRequestRequestTypeDef",
+    "UpdateWorkloadRequestRequestTypeDef",
+    "AddWorkloadResponseTypeDef",
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    "DescribeComponentConfigurationResponseTypeDef",
+    "DescribeWorkloadResponseTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
+    "UpdateWorkloadResponseTypeDef",
     "DescribeComponentResponseTypeDef",
     "ListComponentsResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListWorkloadsResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
+WorkloadConfigurationTypeDef = TypedDict(
+    "WorkloadConfigurationTypeDef",
+    {
+        "WorkloadName": str,
+        "Tier": TierType,
+        "Configuration": str,
+    },
+    total=False,
+)
+
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
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
         "ComponentRemarks": str,
         "ResourceType": str,
         "OsType": OsTypeType,
@@ -110,14 +145,15 @@
     },
     total=False,
 )
 
 ApplicationInfoTypeDef = TypedDict(
     "ApplicationInfoTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "LifeCycle": str,
         "OpsItemSNSTopicArn": str,
         "OpsCenterEnabled": bool,
         "CWEMonitorEnabled": bool,
         "Remarks": str,
         "AutoConfigEnabled": bool,
@@ -125,14 +161,16 @@
     },
     total=False,
 )
 
 ConfigurationEventTypeDef = TypedDict(
     "ConfigurationEventTypeDef",
     {
+        "ResourceGroupName": str,
+        "AccountId": str,
         "MonitoredResourceARN": str,
         "EventStatus": ConfigurationEventStatusType,
         "EventResourceType": ConfigurationEventResourceTypeType,
         "EventTime": datetime,
         "EventDetail": str,
         "EventResourceName": str,
     },
@@ -198,79 +236,150 @@
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
 
-DescribeApplicationRequestRequestTypeDef = TypedDict(
-    "DescribeApplicationRequestRequestTypeDef",
+_RequiredDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
+_OptionalDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeApplicationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+
+class DescribeApplicationRequestRequestTypeDef(
+    _RequiredDescribeApplicationRequestRequestTypeDef,
+    _OptionalDescribeApplicationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
-
-DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
     {
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RecommendationType": RecommendationTypeType,
     },
+    total=False,
 )
 
-DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRequestRequestTypeDef",
+
+class DescribeComponentConfigurationRecommendationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
-
-DescribeComponentConfigurationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationResponseTypeDef",
+_OptionalDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRequestRequestTypeDef",
     {
-        "Monitor": bool,
-        "Tier": TierType,
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
     },
+    total=False,
 )
 
-DescribeComponentRequestRequestTypeDef = TypedDict(
-    "DescribeComponentRequestRequestTypeDef",
+
+class DescribeComponentConfigurationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
+_OptionalDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeLogPatternRequestRequestTypeDef = TypedDict(
-    "DescribeLogPatternRequestRequestTypeDef",
+
+class DescribeComponentRequestRequestTypeDef(
+    _RequiredDescribeComponentRequestRequestTypeDef, _OptionalDescribeComponentRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeLogPatternRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
+_OptionalDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeLogPatternRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeObservationRequestRequestTypeDef = TypedDict(
-    "DescribeObservationRequestRequestTypeDef",
+
+class DescribeLogPatternRequestRequestTypeDef(
+    _RequiredDescribeLogPatternRequestRequestTypeDef,
+    _OptionalDescribeLogPatternRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeObservationRequestRequestTypeDef",
     {
         "ObservationId": str,
     },
 )
+_OptionalDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeObservationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class DescribeObservationRequestRequestTypeDef(
+    _RequiredDescribeObservationRequestRequestTypeDef,
+    _OptionalDescribeObservationRequestRequestTypeDef,
+):
+    pass
+
 
 ObservationTypeDef = TypedDict(
     "ObservationTypeDef",
     {
         "Id": str,
         "StartTime": datetime,
         "EndTime": datetime,
@@ -316,52 +425,108 @@
         "XRayRequestAverageLatency": int,
         "XRayNodeName": str,
         "XRayNodeType": str,
     },
     total=False,
 )
 
-DescribeProblemObservationsRequestRequestTypeDef = TypedDict(
-    "DescribeProblemObservationsRequestRequestTypeDef",
+_RequiredDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemObservationsRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemObservationsRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeProblemRequestRequestTypeDef = TypedDict(
-    "DescribeProblemRequestRequestTypeDef",
+
+class DescribeProblemObservationsRequestRequestTypeDef(
+    _RequiredDescribeProblemObservationsRequestRequestTypeDef,
+    _OptionalDescribeProblemObservationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class DescribeProblemRequestRequestTypeDef(
+    _RequiredDescribeProblemRequestRequestTypeDef, _OptionalDescribeProblemRequestRequestTypeDef
+):
+    pass
+
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "Id": str,
         "Title": str,
         "Insights": str,
         "Status": StatusType,
         "AffectedResource": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "SeverityLevel": SeverityLevelType,
+        "AccountId": str,
         "ResourceGroupName": str,
         "Feedback": Dict[Literal["INSIGHTS_FEEDBACK"], FeedbackValueType],
         "RecurringCount": int,
         "LastRecurrenceTime": datetime,
+        "Visibility": VisibilityType,
+        "ResolutionMethod": ResolutionMethodType,
     },
     total=False,
 )
 
+_RequiredDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
+    },
+)
+_OptionalDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeWorkloadRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class DescribeWorkloadRequestRequestTypeDef(
+    _RequiredDescribeWorkloadRequestRequestTypeDef, _OptionalDescribeWorkloadRequestRequestTypeDef
+):
+    pass
+
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 _RequiredListComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentsRequestRequestTypeDef",
     {
@@ -369,14 +534,15 @@
     },
 )
 _OptionalListComponentsRequestRequestTypeDef = TypedDict(
     "_OptionalListComponentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
@@ -389,14 +555,15 @@
     {
         "ResourceGroupName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "EventStatus": ConfigurationEventStatusType,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 _RequiredListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternSetsRequestRequestTypeDef",
     {
@@ -404,95 +571,115 @@
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
     _OptionalListLogPatternSetsRequestRequestTypeDef,
 ):
     pass
 
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
-    {
-        "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListLogPatternsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternsRequestRequestTypeDef",
     {
         "PatternSetName": str,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
 ):
     pass
 
 
 ListProblemsRequestRequestTypeDef = TypedDict(
     "ListProblemsRequestRequestTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "MaxResults": int,
         "NextToken": str,
         "ComponentName": str,
+        "Visibility": VisibilityType,
     },
     total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+_RequiredListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_RequiredListWorkloadsRequestRequestTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "ResourceGroupName": str,
+        "ComponentName": str,
     },
 )
+_OptionalListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_OptionalListWorkloadsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class ListWorkloadsRequestRequestTypeDef(
+    _RequiredListWorkloadsRequestRequestTypeDef, _OptionalListWorkloadsRequestRequestTypeDef
+):
+    pass
+
+
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "WorkloadId": str,
+        "ComponentName": str,
+        "WorkloadName": str,
+        "Tier": TierType,
+        "WorkloadRemarks": str,
+    },
+    total=False,
+)
+
+RemoveWorkloadRequestRequestTypeDef = TypedDict(
+    "RemoveWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -594,71 +781,182 @@
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProblemRequestRequestTypeDef",
+    {
+        "ProblemId": str,
+    },
+)
+_OptionalUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProblemRequestRequestTypeDef",
+    {
+        "UpdateStatus": Literal["RESOLVED"],
+        "Visibility": VisibilityType,
+    },
+    total=False,
+)
+
+
+class UpdateProblemRequestRequestTypeDef(
+    _RequiredUpdateProblemRequestRequestTypeDef, _OptionalUpdateProblemRequestRequestTypeDef
+):
+    pass
+
+
+AddWorkloadRequestRequestTypeDef = TypedDict(
+    "AddWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+    },
+)
+
+_RequiredUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+    },
+)
+_OptionalUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkloadRequestRequestTypeDef",
+    {
+        "WorkloadId": str,
+    },
+    total=False,
+)
+
+
+class UpdateWorkloadRequestRequestTypeDef(
+    _RequiredUpdateWorkloadRequestRequestTypeDef, _OptionalUpdateWorkloadRequestRequestTypeDef
+):
+    pass
+
+
+AddWorkloadResponseTypeDef = TypedDict(
+    "AddWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    {
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationResponseTypeDef",
+    {
+        "Monitor": bool,
+        "Tier": TierType,
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkloadResponseTypeDef = TypedDict(
+    "DescribeWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadRemarks": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
+    {
+        "ResourceGroupName": str,
+        "AccountId": str,
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkloadResponseTypeDef = TypedDict(
+    "UpdateWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "ApplicationComponent": ApplicationComponentTypeDef,
         "ResourceList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "ApplicationComponentList": List[ApplicationComponentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationRequestRequestTypeDef = TypedDict(
     "CreateApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
@@ -669,64 +967,74 @@
         "AutoConfigEnabled": bool,
         "AutoCreate": bool,
         "GroupingType": Literal["ACCOUNT_BASED"],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
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
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
     "UpdateLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObservationResponseTypeDef = TypedDict(
     "DescribeObservationResponseTypeDef",
     {
         "Observation": ObservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedObservationsTypeDef = TypedDict(
     "RelatedObservationsTypeDef",
     {
         "ObservationList": List[ObservationTypeDef],
@@ -734,36 +1042,38 @@
     total=False,
 )
 
 DescribeProblemResponseTypeDef = TypedDict(
     "DescribeProblemResponseTypeDef",
     {
         "Problem": ProblemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListWorkloadsResponseTypeDef = TypedDict(
+    "ListWorkloadsResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WorkloadList": List[WorkloadTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.pyi` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights/type_defs.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -2,104 +2,139 @@
 Type annotations for application-insights service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_application_insights.type_defs import ApplicationComponentTypeDef
+    from mypy_boto3_application_insights.type_defs import WorkloadConfigurationTypeDef
 
-    data: ApplicationComponentTypeDef = {...}
+    data: WorkloadConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CloudWatchEventSourceType,
     ConfigurationEventResourceTypeType,
     ConfigurationEventStatusType,
     DiscoveryTypeType,
     FeedbackValueType,
     LogFilterType,
     OsTypeType,
+    RecommendationTypeType,
+    ResolutionMethodType,
     SeverityLevelType,
     StatusType,
     TierType,
+    VisibilityType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "WorkloadConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationRequestRequestTypeDef",
-    "DescribeComponentConfigurationResponseTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
+    "DescribeWorkloadRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListWorkloadsRequestRequestTypeDef",
+    "WorkloadTypeDef",
+    "RemoveWorkloadRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
+    "UpdateProblemRequestRequestTypeDef",
+    "AddWorkloadRequestRequestTypeDef",
+    "UpdateWorkloadRequestRequestTypeDef",
+    "AddWorkloadResponseTypeDef",
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    "DescribeComponentConfigurationResponseTypeDef",
+    "DescribeWorkloadResponseTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
+    "UpdateWorkloadResponseTypeDef",
     "DescribeComponentResponseTypeDef",
     "ListComponentsResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListWorkloadsResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
+WorkloadConfigurationTypeDef = TypedDict(
+    "WorkloadConfigurationTypeDef",
+    {
+        "WorkloadName": str,
+        "Tier": TierType,
+        "Configuration": str,
+    },
+    total=False,
+)
+
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
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
         "ComponentRemarks": str,
         "ResourceType": str,
         "OsType": OsTypeType,
@@ -109,14 +144,15 @@
     },
     total=False,
 )
 
 ApplicationInfoTypeDef = TypedDict(
     "ApplicationInfoTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "LifeCycle": str,
         "OpsItemSNSTopicArn": str,
         "OpsCenterEnabled": bool,
         "CWEMonitorEnabled": bool,
         "Remarks": str,
         "AutoConfigEnabled": bool,
@@ -124,14 +160,16 @@
     },
     total=False,
 )
 
 ConfigurationEventTypeDef = TypedDict(
     "ConfigurationEventTypeDef",
     {
+        "ResourceGroupName": str,
+        "AccountId": str,
         "MonitoredResourceARN": str,
         "EventStatus": ConfigurationEventStatusType,
         "EventResourceType": ConfigurationEventResourceTypeType,
         "EventTime": datetime,
         "EventDetail": str,
         "EventResourceName": str,
     },
@@ -197,79 +235,138 @@
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
 
-DescribeApplicationRequestRequestTypeDef = TypedDict(
-    "DescribeApplicationRequestRequestTypeDef",
+_RequiredDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
+_OptionalDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeApplicationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+class DescribeApplicationRequestRequestTypeDef(
+    _RequiredDescribeApplicationRequestRequestTypeDef,
+    _OptionalDescribeApplicationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
-
-DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
     {
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RecommendationType": RecommendationTypeType,
     },
+    total=False,
 )
 
-DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRequestRequestTypeDef",
+class DescribeComponentConfigurationRecommendationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
-
-DescribeComponentConfigurationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationResponseTypeDef",
+_OptionalDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRequestRequestTypeDef",
     {
-        "Monitor": bool,
-        "Tier": TierType,
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
     },
+    total=False,
 )
 
-DescribeComponentRequestRequestTypeDef = TypedDict(
-    "DescribeComponentRequestRequestTypeDef",
+class DescribeComponentConfigurationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
+_OptionalDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeLogPatternRequestRequestTypeDef = TypedDict(
-    "DescribeLogPatternRequestRequestTypeDef",
+class DescribeComponentRequestRequestTypeDef(
+    _RequiredDescribeComponentRequestRequestTypeDef, _OptionalDescribeComponentRequestRequestTypeDef
+):
+    pass
+
+_RequiredDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeLogPatternRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
+_OptionalDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeLogPatternRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeObservationRequestRequestTypeDef = TypedDict(
-    "DescribeObservationRequestRequestTypeDef",
+class DescribeLogPatternRequestRequestTypeDef(
+    _RequiredDescribeLogPatternRequestRequestTypeDef,
+    _OptionalDescribeLogPatternRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeObservationRequestRequestTypeDef",
     {
         "ObservationId": str,
     },
 )
+_OptionalDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeObservationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class DescribeObservationRequestRequestTypeDef(
+    _RequiredDescribeObservationRequestRequestTypeDef,
+    _OptionalDescribeObservationRequestRequestTypeDef,
+):
+    pass
 
 ObservationTypeDef = TypedDict(
     "ObservationTypeDef",
     {
         "Id": str,
         "StartTime": datetime,
         "EndTime": datetime,
@@ -315,52 +412,102 @@
         "XRayRequestAverageLatency": int,
         "XRayNodeName": str,
         "XRayNodeType": str,
     },
     total=False,
 )
 
-DescribeProblemObservationsRequestRequestTypeDef = TypedDict(
-    "DescribeProblemObservationsRequestRequestTypeDef",
+_RequiredDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemObservationsRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemObservationsRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeProblemRequestRequestTypeDef = TypedDict(
-    "DescribeProblemRequestRequestTypeDef",
+class DescribeProblemObservationsRequestRequestTypeDef(
+    _RequiredDescribeProblemObservationsRequestRequestTypeDef,
+    _OptionalDescribeProblemObservationsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class DescribeProblemRequestRequestTypeDef(
+    _RequiredDescribeProblemRequestRequestTypeDef, _OptionalDescribeProblemRequestRequestTypeDef
+):
+    pass
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "Id": str,
         "Title": str,
         "Insights": str,
         "Status": StatusType,
         "AffectedResource": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "SeverityLevel": SeverityLevelType,
+        "AccountId": str,
         "ResourceGroupName": str,
         "Feedback": Dict[Literal["INSIGHTS_FEEDBACK"], FeedbackValueType],
         "RecurringCount": int,
         "LastRecurrenceTime": datetime,
+        "Visibility": VisibilityType,
+        "ResolutionMethod": ResolutionMethodType,
+    },
+    total=False,
+)
+
+_RequiredDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
+    },
+)
+_OptionalDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeWorkloadRequestRequestTypeDef",
+    {
+        "AccountId": str,
     },
     total=False,
 )
 
+class DescribeWorkloadRequestRequestTypeDef(
+    _RequiredDescribeWorkloadRequestRequestTypeDef, _OptionalDescribeWorkloadRequestRequestTypeDef
+):
+    pass
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 _RequiredListComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentsRequestRequestTypeDef",
     {
@@ -368,14 +515,15 @@
     },
 )
 _OptionalListComponentsRequestRequestTypeDef = TypedDict(
     "_OptionalListComponentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
 ):
@@ -386,14 +534,15 @@
     {
         "ResourceGroupName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "EventStatus": ConfigurationEventStatusType,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 _RequiredListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternSetsRequestRequestTypeDef",
     {
@@ -401,91 +550,109 @@
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
     _OptionalListLogPatternSetsRequestRequestTypeDef,
 ):
     pass
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
-    {
-        "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListLogPatternsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternsRequestRequestTypeDef",
     {
         "PatternSetName": str,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
 ):
     pass
 
 ListProblemsRequestRequestTypeDef = TypedDict(
     "ListProblemsRequestRequestTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "MaxResults": int,
         "NextToken": str,
         "ComponentName": str,
+        "Visibility": VisibilityType,
     },
     total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+_RequiredListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_RequiredListWorkloadsRequestRequestTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "ResourceGroupName": str,
+        "ComponentName": str,
+    },
+)
+_OptionalListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_OptionalListWorkloadsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class ListWorkloadsRequestRequestTypeDef(
+    _RequiredListWorkloadsRequestRequestTypeDef, _OptionalListWorkloadsRequestRequestTypeDef
+):
+    pass
+
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "WorkloadId": str,
+        "ComponentName": str,
+        "WorkloadName": str,
+        "Tier": TierType,
+        "WorkloadRemarks": str,
+    },
+    total=False,
+)
+
+RemoveWorkloadRequestRequestTypeDef = TypedDict(
+    "RemoveWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -579,71 +746,178 @@
 )
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
+_RequiredUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProblemRequestRequestTypeDef",
+    {
+        "ProblemId": str,
+    },
+)
+_OptionalUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProblemRequestRequestTypeDef",
+    {
+        "UpdateStatus": Literal["RESOLVED"],
+        "Visibility": VisibilityType,
+    },
+    total=False,
+)
+
+class UpdateProblemRequestRequestTypeDef(
+    _RequiredUpdateProblemRequestRequestTypeDef, _OptionalUpdateProblemRequestRequestTypeDef
+):
+    pass
+
+AddWorkloadRequestRequestTypeDef = TypedDict(
+    "AddWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+    },
+)
+
+_RequiredUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+    },
+)
+_OptionalUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkloadRequestRequestTypeDef",
+    {
+        "WorkloadId": str,
+    },
+    total=False,
+)
+
+class UpdateWorkloadRequestRequestTypeDef(
+    _RequiredUpdateWorkloadRequestRequestTypeDef, _OptionalUpdateWorkloadRequestRequestTypeDef
+):
+    pass
+
+AddWorkloadResponseTypeDef = TypedDict(
+    "AddWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    {
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationResponseTypeDef",
+    {
+        "Monitor": bool,
+        "Tier": TierType,
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkloadResponseTypeDef = TypedDict(
+    "DescribeWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadRemarks": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
+    {
+        "ResourceGroupName": str,
+        "AccountId": str,
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkloadResponseTypeDef = TypedDict(
+    "UpdateWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "ApplicationComponent": ApplicationComponentTypeDef,
         "ResourceList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "ApplicationComponentList": List[ApplicationComponentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationRequestRequestTypeDef = TypedDict(
     "CreateApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
@@ -654,64 +928,74 @@
         "AutoConfigEnabled": bool,
         "AutoCreate": bool,
         "GroupingType": Literal["ACCOUNT_BASED"],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
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
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
     "UpdateLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObservationResponseTypeDef = TypedDict(
     "DescribeObservationResponseTypeDef",
     {
         "Observation": ObservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedObservationsTypeDef = TypedDict(
     "RelatedObservationsTypeDef",
     {
         "ObservationList": List[ObservationTypeDef],
@@ -719,36 +1003,38 @@
     total=False,
 )
 
 DescribeProblemResponseTypeDef = TypedDict(
     "DescribeProblemResponseTypeDef",
     {
         "Problem": ProblemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListWorkloadsResponseTypeDef = TypedDict(
+    "ListWorkloadsResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WorkloadList": List[WorkloadTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/PKG-INFO` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationInsights 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationInsights 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,17 +286,21 @@
     ConfigurationEventStatusType,
     DiscoveryTypeType,
     FeedbackKeyType,
     FeedbackValueType,
     GroupingTypeType,
     LogFilterType,
     OsTypeType,
+    RecommendationTypeType,
+    ResolutionMethodType,
     SeverityLevelType,
     StatusType,
     TierType,
+    UpdateStatusType,
+    VisibilityType,
     ApplicationInsightsServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -309,74 +313,85 @@
 ### Typed dictionaries
 
 `mypy_boto3_application_insights.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
+    WorkloadConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
+    DescribeWorkloadRequestRequestTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
-    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ResponseMetadataTypeDef,
+    ListWorkloadsRequestRequestTypeDef,
+    WorkloadTypeDef,
+    RemoveWorkloadRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
+    UpdateProblemRequestRequestTypeDef,
+    AddWorkloadRequestRequestTypeDef,
+    UpdateWorkloadRequestRequestTypeDef,
+    AddWorkloadResponseTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
+    DescribeWorkloadResponseTypeDef,
+    ListLogPatternSetsResponseTypeDef,
+    UpdateWorkloadResponseTypeDef,
     DescribeComponentResponseTypeDef,
     ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListWorkloadsResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationComponentTypeDef:
+def get_structure() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/SOURCES.txt` & `mypy-boto3-application-insights-1.28.15/mypy_boto3_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.12/setup.py` & `mypy-boto3-application-insights-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-insights",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationInsights 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ApplicationInsights 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

