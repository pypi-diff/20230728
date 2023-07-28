# Comparing `tmp/mypy-boto3-resiliencehub-1.28.12.tar.gz` & `tmp/mypy-boto3-resiliencehub-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resiliencehub-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-resiliencehub-1.28.15.tar", last modified: Fri Jul 28 20:43:33 2023, max compression
```

## Comparing `mypy-boto3-resiliencehub-1.28.12.tar` & `mypy-boto3-resiliencehub-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.265213 mypy-boto3-resiliencehub-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-27 11:49:30.261213 mypy-boto3-resiliencehub-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.257213 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-27 11:44:36.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-27 11:44:36.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63431 2023-07-27 11:44:38.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63320 2023-07-27 11:44:37.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.261213 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.265213 mypy-boto3-resiliencehub-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.853729 mypy-boto3-resiliencehub-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-07-28 20:43:33.849729 mypy-boto3-resiliencehub-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.841729 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-28 20:36:52.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-07-28 20:36:52.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-28 20:36:52.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-28 20:36:52.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60960 2023-07-28 20:36:54.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60855 2023-07-28 20:36:53.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.849729 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-07-28 20:43:33.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:43:33.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:33.000000 mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.853729 mypy-boto3-resiliencehub-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:36:51.000000 mypy-boto3-resiliencehub-1.28.15/setup.py
```

### Comparing `mypy-boto3-resiliencehub-1.28.12/LICENSE` & `mypy-boto3-resiliencehub-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.12/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.12
-Summary: Type annotations for boto3.ResilienceHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResilienceHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,43 +329,40 @@
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
-    EksSourceClusterNamespaceOutputTypeDef,
-    TerraformSourceOutputTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    TerraformSourceTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    EksSourceClusterNamespaceTypeDef,
-    TerraformSourceTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceOutputTypeDef,
     EksSourceTypeDef,
-    FailurePolicyOutputTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -375,16 +372,14 @@
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
-    LogicalResourceIdOutputTypeDef,
-    PhysicalResourceIdOutputTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
     ResourceErrorTypeDef,
@@ -415,34 +410,33 @@
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
+    DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
+    ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    DeleteAppInputSourceRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    ResiliencyPolicyTypeDef,
     PhysicalResourceTypeDef,
-    ResourceMappingOutputTypeDef,
-    UnsupportedResourceTypeDef,
     ResourceMappingTypeDef,
+    UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
@@ -455,18 +449,18 @@
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
+    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
-    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     ListRecommendationTemplatesResponseTypeDef,
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
```

### Comparing `mypy-boto3-resiliencehub-1.28.12/README.md` & `mypy-boto3-resiliencehub-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,43 +297,40 @@
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
-    EksSourceClusterNamespaceOutputTypeDef,
-    TerraformSourceOutputTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    TerraformSourceTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    EksSourceClusterNamespaceTypeDef,
-    TerraformSourceTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceOutputTypeDef,
     EksSourceTypeDef,
-    FailurePolicyOutputTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -343,16 +340,14 @@
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
-    LogicalResourceIdOutputTypeDef,
-    PhysicalResourceIdOutputTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
     ResourceErrorTypeDef,
@@ -383,34 +378,33 @@
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
+    DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
+    ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    DeleteAppInputSourceRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    ResiliencyPolicyTypeDef,
     PhysicalResourceTypeDef,
-    ResourceMappingOutputTypeDef,
-    UnsupportedResourceTypeDef,
     ResourceMappingTypeDef,
+    UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
@@ -423,18 +417,18 @@
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
+    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
-    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     ListRecommendationTemplatesResponseTypeDef,
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
```

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__main__.py` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResilienceHub 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ResilienceHub 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.py` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.pyi` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.py` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.pyi` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.py` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,43 +57,40 @@
 __all__ = (
     "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
-    "EksSourceClusterNamespaceOutputTypeDef",
-    "TerraformSourceOutputTypeDef",
+    "EksSourceClusterNamespaceTypeDef",
+    "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
     "AppTypeDef",
     "AppVersionSummaryTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
-    "EksSourceClusterNamespaceTypeDef",
-    "TerraformSourceTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
-    "FailurePolicyOutputTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
@@ -103,16 +100,14 @@
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
-    "LogicalResourceIdOutputTypeDef",
-    "PhysicalResourceIdOutputTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
@@ -143,34 +138,33 @@
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
+    "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
+    "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "DeleteAppInputSourceRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    "ResiliencyPolicyTypeDef",
     "PhysicalResourceTypeDef",
-    "ResourceMappingOutputTypeDef",
-    "UnsupportedResourceTypeDef",
     "ResourceMappingTypeDef",
+    "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
@@ -183,18 +177,18 @@
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     "ListAppVersionResourceMappingsResponseTypeDef",
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "CreateRecommendationTemplateResponseTypeDef",
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
 )
@@ -284,24 +278,24 @@
 )
 
 
 class AppComponentTypeDef(_RequiredAppComponentTypeDef, _OptionalAppComponentTypeDef):
     pass
 
 
-EksSourceClusterNamespaceOutputTypeDef = TypedDict(
-    "EksSourceClusterNamespaceOutputTypeDef",
+EksSourceClusterNamespaceTypeDef = TypedDict(
+    "EksSourceClusterNamespaceTypeDef",
     {
         "eksClusterArn": str,
         "namespace": str,
     },
 )
 
-TerraformSourceOutputTypeDef = TypedDict(
-    "TerraformSourceOutputTypeDef",
+TerraformSourceTypeDef = TypedDict(
+    "TerraformSourceTypeDef",
     {
         "s3StateFileUrl": str,
     },
 )
 
 _RequiredAppSummaryTypeDef = TypedDict(
     "_RequiredAppSummaryTypeDef",
@@ -518,29 +512,14 @@
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
 
-EksSourceClusterNamespaceTypeDef = TypedDict(
-    "EksSourceClusterNamespaceTypeDef",
-    {
-        "eksClusterArn": str,
-        "namespace": str,
-    },
-)
-
-TerraformSourceTypeDef = TypedDict(
-    "TerraformSourceTypeDef",
-    {
-        "s3StateFileUrl": str,
-    },
-)
-
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalDeleteAppRequestRequestTypeDef = TypedDict(
@@ -714,22 +693,14 @@
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
 
-FailurePolicyOutputTypeDef = TypedDict(
-    "FailurePolicyOutputTypeDef",
-    {
-        "rpoInSecs": int,
-        "rtoInSecs": int,
-    },
-)
-
 _RequiredListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlarmRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1060,61 +1031,14 @@
 class ListUnsupportedAppVersionResourcesRequestRequestTypeDef(
     _RequiredListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     _OptionalListUnsupportedAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredLogicalResourceIdOutputTypeDef = TypedDict(
-    "_RequiredLogicalResourceIdOutputTypeDef",
-    {
-        "identifier": str,
-    },
-)
-_OptionalLogicalResourceIdOutputTypeDef = TypedDict(
-    "_OptionalLogicalResourceIdOutputTypeDef",
-    {
-        "eksSourceName": str,
-        "logicalStackName": str,
-        "resourceGroupName": str,
-        "terraformSourceName": str,
-    },
-    total=False,
-)
-
-
-class LogicalResourceIdOutputTypeDef(
-    _RequiredLogicalResourceIdOutputTypeDef, _OptionalLogicalResourceIdOutputTypeDef
-):
-    pass
-
-
-_RequiredPhysicalResourceIdOutputTypeDef = TypedDict(
-    "_RequiredPhysicalResourceIdOutputTypeDef",
-    {
-        "identifier": str,
-        "type": PhysicalIdentifierTypeType,
-    },
-)
-_OptionalPhysicalResourceIdOutputTypeDef = TypedDict(
-    "_OptionalPhysicalResourceIdOutputTypeDef",
-    {
-        "awsAccountId": str,
-        "awsRegion": str,
-    },
-    total=False,
-)
-
-
-class PhysicalResourceIdOutputTypeDef(
-    _RequiredPhysicalResourceIdOutputTypeDef, _OptionalPhysicalResourceIdOutputTypeDef
-):
-    pass
-
-
 _RequiredPhysicalResourceIdTypeDef = TypedDict(
     "_RequiredPhysicalResourceIdTypeDef",
     {
         "identifier": str,
         "type": PhysicalIdentifierTypeType,
     },
 )
@@ -1632,28 +1556,53 @@
     {
         "importType": ResourceMappingTypeType,
     },
 )
 _OptionalAppInputSourceTypeDef = TypedDict(
     "_OptionalAppInputSourceTypeDef",
     {
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceOutputTypeDef,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
         "resourceCount": int,
         "sourceArn": str,
         "sourceName": str,
-        "terraformSource": TerraformSourceOutputTypeDef,
+        "terraformSource": TerraformSourceTypeDef,
     },
     total=False,
 )
 
 
 class AppInputSourceTypeDef(_RequiredAppInputSourceTypeDef, _OptionalAppInputSourceTypeDef):
     pass
 
 
+_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
+        "sourceArn": str,
+        "terraformSource": TerraformSourceTypeDef,
+    },
+    total=False,
+)
+
+
+class DeleteAppInputSourceRequestRequestTypeDef(
+    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
+    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
+):
+    pass
+
+
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1860,14 +1809,30 @@
 class CreateResiliencyPolicyRequestRequestTypeDef(
     _RequiredCreateResiliencyPolicyRequestRequestTypeDef,
     _OptionalCreateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+ResiliencyPolicyTypeDef = TypedDict(
+    "ResiliencyPolicyTypeDef",
+    {
+        "creationTime": datetime,
+        "dataLocationConstraint": DataLocationConstraintType,
+        "estimatedCostTier": EstimatedCostTierType,
+        "policy": Dict[DisruptionTypeType, FailurePolicyTypeDef],
+        "policyArn": str,
+        "policyDescription": str,
+        "policyName": str,
+        "tags": Dict[str, str],
+        "tier": ResiliencyPolicyTierType,
+    },
+    total=False,
+)
+
 _RequiredUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -1886,48 +1851,23 @@
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
-        "sourceArn": str,
-        "terraformSource": TerraformSourceTypeDef,
-    },
-    total=False,
-)
-
-
-class DeleteAppInputSourceRequestRequestTypeDef(
-    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
-    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
-):
-    pass
-
-
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "eksSources": List[EksSourceOutputTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
-        "terraformSources": List[TerraformSourceOutputTypeDef],
+        "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
     "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
     {
@@ -1949,35 +1889,19 @@
 class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
     _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
     _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
 ):
     pass
 
 
-ResiliencyPolicyTypeDef = TypedDict(
-    "ResiliencyPolicyTypeDef",
-    {
-        "creationTime": datetime,
-        "dataLocationConstraint": DataLocationConstraintType,
-        "estimatedCostTier": EstimatedCostTierType,
-        "policy": Dict[DisruptionTypeType, FailurePolicyOutputTypeDef],
-        "policyArn": str,
-        "policyDescription": str,
-        "policyName": str,
-        "tags": Dict[str, str],
-        "tier": ResiliencyPolicyTierType,
-    },
-    total=False,
-)
-
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdOutputTypeDef,
-        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
+        "logicalResourceId": LogicalResourceIdTypeDef,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
 )
 _OptionalPhysicalResourceTypeDef = TypedDict(
     "_OptionalPhysicalResourceTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
@@ -1991,46 +1915,44 @@
 )
 
 
 class PhysicalResourceTypeDef(_RequiredPhysicalResourceTypeDef, _OptionalPhysicalResourceTypeDef):
     pass
 
 
-_RequiredResourceMappingOutputTypeDef = TypedDict(
-    "_RequiredResourceMappingOutputTypeDef",
+_RequiredResourceMappingTypeDef = TypedDict(
+    "_RequiredResourceMappingTypeDef",
     {
         "mappingType": ResourceMappingTypeType,
-        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
     },
 )
-_OptionalResourceMappingOutputTypeDef = TypedDict(
-    "_OptionalResourceMappingOutputTypeDef",
+_OptionalResourceMappingTypeDef = TypedDict(
+    "_OptionalResourceMappingTypeDef",
     {
         "appRegistryAppName": str,
         "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "resourceName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
 
-class ResourceMappingOutputTypeDef(
-    _RequiredResourceMappingOutputTypeDef, _OptionalResourceMappingOutputTypeDef
-):
+class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
     pass
 
 
 _RequiredUnsupportedResourceTypeDef = TypedDict(
     "_RequiredUnsupportedResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdOutputTypeDef,
-        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
+        "logicalResourceId": LogicalResourceIdTypeDef,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
 )
 _OptionalUnsupportedResourceTypeDef = TypedDict(
     "_OptionalUnsupportedResourceTypeDef",
     {
         "unsupportedResourceStatus": str,
@@ -2041,39 +1963,14 @@
 
 class UnsupportedResourceTypeDef(
     _RequiredUnsupportedResourceTypeDef, _OptionalUnsupportedResourceTypeDef
 ):
     pass
 
 
-_RequiredResourceMappingTypeDef = TypedDict(
-    "_RequiredResourceMappingTypeDef",
-    {
-        "mappingType": ResourceMappingTypeType,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
-    },
-)
-_OptionalResourceMappingTypeDef = TypedDict(
-    "_OptionalResourceMappingTypeDef",
-    {
-        "appRegistryAppName": str,
-        "eksSourceName": str,
-        "logicalStackName": str,
-        "resourceGroupName": str,
-        "resourceName": str,
-        "terraformSourceName": str,
-    },
-    total=False,
-)
-
-
-class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
-    pass
-
-
 _RequiredRecommendationTemplateTypeDef = TypedDict(
     "_RequiredRecommendationTemplateTypeDef",
     {
         "assessmentArn": str,
         "format": TemplateFormatType,
         "name": str,
         "recommendationTemplateArn": str,
@@ -2272,51 +2169,51 @@
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "resourceMappings": Sequence[ResourceMappingTypeDef],
+    },
+)
+
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "resourceMappings": List[ResourceMappingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
-        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "resourceMappings": List[ResourceMappingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "resourceMappings": Sequence[ResourceMappingTypeDef],
-    },
-)
-
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.pyi` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,43 +56,40 @@
 __all__ = (
     "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
-    "EksSourceClusterNamespaceOutputTypeDef",
-    "TerraformSourceOutputTypeDef",
+    "EksSourceClusterNamespaceTypeDef",
+    "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
     "AppTypeDef",
     "AppVersionSummaryTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
-    "EksSourceClusterNamespaceTypeDef",
-    "TerraformSourceTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
-    "FailurePolicyOutputTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
@@ -102,16 +99,14 @@
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
-    "LogicalResourceIdOutputTypeDef",
-    "PhysicalResourceIdOutputTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
@@ -142,34 +137,33 @@
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
+    "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
+    "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "DeleteAppInputSourceRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    "ResiliencyPolicyTypeDef",
     "PhysicalResourceTypeDef",
-    "ResourceMappingOutputTypeDef",
-    "UnsupportedResourceTypeDef",
     "ResourceMappingTypeDef",
+    "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
@@ -182,18 +176,18 @@
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     "ListAppVersionResourceMappingsResponseTypeDef",
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "CreateRecommendationTemplateResponseTypeDef",
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
 )
@@ -279,24 +273,24 @@
     },
     total=False,
 )
 
 class AppComponentTypeDef(_RequiredAppComponentTypeDef, _OptionalAppComponentTypeDef):
     pass
 
-EksSourceClusterNamespaceOutputTypeDef = TypedDict(
-    "EksSourceClusterNamespaceOutputTypeDef",
+EksSourceClusterNamespaceTypeDef = TypedDict(
+    "EksSourceClusterNamespaceTypeDef",
     {
         "eksClusterArn": str,
         "namespace": str,
     },
 )
 
-TerraformSourceOutputTypeDef = TypedDict(
-    "TerraformSourceOutputTypeDef",
+TerraformSourceTypeDef = TypedDict(
+    "TerraformSourceTypeDef",
     {
         "s3StateFileUrl": str,
     },
 )
 
 _RequiredAppSummaryTypeDef = TypedDict(
     "_RequiredAppSummaryTypeDef",
@@ -497,29 +491,14 @@
 
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
-EksSourceClusterNamespaceTypeDef = TypedDict(
-    "EksSourceClusterNamespaceTypeDef",
-    {
-        "eksClusterArn": str,
-        "namespace": str,
-    },
-)
-
-TerraformSourceTypeDef = TypedDict(
-    "TerraformSourceTypeDef",
-    {
-        "s3StateFileUrl": str,
-    },
-)
-
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalDeleteAppRequestRequestTypeDef = TypedDict(
@@ -683,22 +662,14 @@
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
 
-FailurePolicyOutputTypeDef = TypedDict(
-    "FailurePolicyOutputTypeDef",
-    {
-        "rpoInSecs": int,
-        "rtoInSecs": int,
-    },
-)
-
 _RequiredListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlarmRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1005,57 +976,14 @@
 
 class ListUnsupportedAppVersionResourcesRequestRequestTypeDef(
     _RequiredListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     _OptionalListUnsupportedAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLogicalResourceIdOutputTypeDef = TypedDict(
-    "_RequiredLogicalResourceIdOutputTypeDef",
-    {
-        "identifier": str,
-    },
-)
-_OptionalLogicalResourceIdOutputTypeDef = TypedDict(
-    "_OptionalLogicalResourceIdOutputTypeDef",
-    {
-        "eksSourceName": str,
-        "logicalStackName": str,
-        "resourceGroupName": str,
-        "terraformSourceName": str,
-    },
-    total=False,
-)
-
-class LogicalResourceIdOutputTypeDef(
-    _RequiredLogicalResourceIdOutputTypeDef, _OptionalLogicalResourceIdOutputTypeDef
-):
-    pass
-
-_RequiredPhysicalResourceIdOutputTypeDef = TypedDict(
-    "_RequiredPhysicalResourceIdOutputTypeDef",
-    {
-        "identifier": str,
-        "type": PhysicalIdentifierTypeType,
-    },
-)
-_OptionalPhysicalResourceIdOutputTypeDef = TypedDict(
-    "_OptionalPhysicalResourceIdOutputTypeDef",
-    {
-        "awsAccountId": str,
-        "awsRegion": str,
-    },
-    total=False,
-)
-
-class PhysicalResourceIdOutputTypeDef(
-    _RequiredPhysicalResourceIdOutputTypeDef, _OptionalPhysicalResourceIdOutputTypeDef
-):
-    pass
-
 _RequiredPhysicalResourceIdTypeDef = TypedDict(
     "_RequiredPhysicalResourceIdTypeDef",
     {
         "identifier": str,
         "type": PhysicalIdentifierTypeType,
     },
 )
@@ -1553,26 +1481,49 @@
     {
         "importType": ResourceMappingTypeType,
     },
 )
 _OptionalAppInputSourceTypeDef = TypedDict(
     "_OptionalAppInputSourceTypeDef",
     {
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceOutputTypeDef,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
         "resourceCount": int,
         "sourceArn": str,
         "sourceName": str,
-        "terraformSource": TerraformSourceOutputTypeDef,
+        "terraformSource": TerraformSourceTypeDef,
     },
     total=False,
 )
 
 class AppInputSourceTypeDef(_RequiredAppInputSourceTypeDef, _OptionalAppInputSourceTypeDef):
     pass
 
+_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
+        "sourceArn": str,
+        "terraformSource": TerraformSourceTypeDef,
+    },
+    total=False,
+)
+
+class DeleteAppInputSourceRequestRequestTypeDef(
+    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
+    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
+):
+    pass
+
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1767,14 +1718,30 @@
 
 class CreateResiliencyPolicyRequestRequestTypeDef(
     _RequiredCreateResiliencyPolicyRequestRequestTypeDef,
     _OptionalCreateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
+ResiliencyPolicyTypeDef = TypedDict(
+    "ResiliencyPolicyTypeDef",
+    {
+        "creationTime": datetime,
+        "dataLocationConstraint": DataLocationConstraintType,
+        "estimatedCostTier": EstimatedCostTierType,
+        "policy": Dict[DisruptionTypeType, FailurePolicyTypeDef],
+        "policyArn": str,
+        "policyDescription": str,
+        "policyName": str,
+        "tags": Dict[str, str],
+        "tier": ResiliencyPolicyTierType,
+    },
+    total=False,
+)
+
 _RequiredUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -1791,46 +1758,23 @@
 
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
-        "sourceArn": str,
-        "terraformSource": TerraformSourceTypeDef,
-    },
-    total=False,
-)
-
-class DeleteAppInputSourceRequestRequestTypeDef(
-    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
-    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
-):
-    pass
-
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "eksSources": List[EksSourceOutputTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
-        "terraformSources": List[TerraformSourceOutputTypeDef],
+        "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
     "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
     {
@@ -1850,35 +1794,19 @@
 
 class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
     _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
     _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
 ):
     pass
 
-ResiliencyPolicyTypeDef = TypedDict(
-    "ResiliencyPolicyTypeDef",
-    {
-        "creationTime": datetime,
-        "dataLocationConstraint": DataLocationConstraintType,
-        "estimatedCostTier": EstimatedCostTierType,
-        "policy": Dict[DisruptionTypeType, FailurePolicyOutputTypeDef],
-        "policyArn": str,
-        "policyDescription": str,
-        "policyName": str,
-        "tags": Dict[str, str],
-        "tier": ResiliencyPolicyTierType,
-    },
-    total=False,
-)
-
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdOutputTypeDef,
-        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
+        "logicalResourceId": LogicalResourceIdTypeDef,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
 )
 _OptionalPhysicalResourceTypeDef = TypedDict(
     "_OptionalPhysicalResourceTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
@@ -1890,44 +1818,42 @@
     },
     total=False,
 )
 
 class PhysicalResourceTypeDef(_RequiredPhysicalResourceTypeDef, _OptionalPhysicalResourceTypeDef):
     pass
 
-_RequiredResourceMappingOutputTypeDef = TypedDict(
-    "_RequiredResourceMappingOutputTypeDef",
+_RequiredResourceMappingTypeDef = TypedDict(
+    "_RequiredResourceMappingTypeDef",
     {
         "mappingType": ResourceMappingTypeType,
-        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
     },
 )
-_OptionalResourceMappingOutputTypeDef = TypedDict(
-    "_OptionalResourceMappingOutputTypeDef",
+_OptionalResourceMappingTypeDef = TypedDict(
+    "_OptionalResourceMappingTypeDef",
     {
         "appRegistryAppName": str,
         "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "resourceName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
-class ResourceMappingOutputTypeDef(
-    _RequiredResourceMappingOutputTypeDef, _OptionalResourceMappingOutputTypeDef
-):
+class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
     pass
 
 _RequiredUnsupportedResourceTypeDef = TypedDict(
     "_RequiredUnsupportedResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdOutputTypeDef,
-        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
+        "logicalResourceId": LogicalResourceIdTypeDef,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
 )
 _OptionalUnsupportedResourceTypeDef = TypedDict(
     "_OptionalUnsupportedResourceTypeDef",
     {
         "unsupportedResourceStatus": str,
@@ -1936,37 +1862,14 @@
 )
 
 class UnsupportedResourceTypeDef(
     _RequiredUnsupportedResourceTypeDef, _OptionalUnsupportedResourceTypeDef
 ):
     pass
 
-_RequiredResourceMappingTypeDef = TypedDict(
-    "_RequiredResourceMappingTypeDef",
-    {
-        "mappingType": ResourceMappingTypeType,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
-    },
-)
-_OptionalResourceMappingTypeDef = TypedDict(
-    "_OptionalResourceMappingTypeDef",
-    {
-        "appRegistryAppName": str,
-        "eksSourceName": str,
-        "logicalStackName": str,
-        "resourceGroupName": str,
-        "resourceName": str,
-        "terraformSourceName": str,
-    },
-    total=False,
-)
-
-class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
-    pass
-
 _RequiredRecommendationTemplateTypeDef = TypedDict(
     "_RequiredRecommendationTemplateTypeDef",
     {
         "assessmentArn": str,
         "format": TemplateFormatType,
         "name": str,
         "recommendationTemplateArn": str,
@@ -2163,51 +2066,51 @@
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "resourceMappings": Sequence[ResourceMappingTypeDef],
+    },
+)
+
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "resourceMappings": List[ResourceMappingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
-        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "resourceMappings": List[ResourceMappingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "resourceMappings": Sequence[ResourceMappingTypeDef],
-    },
-)
-
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.12
-Summary: Type annotations for boto3.ResilienceHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResilienceHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,43 +329,40 @@
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
-    EksSourceClusterNamespaceOutputTypeDef,
-    TerraformSourceOutputTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    TerraformSourceTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    EksSourceClusterNamespaceTypeDef,
-    TerraformSourceTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceOutputTypeDef,
     EksSourceTypeDef,
-    FailurePolicyOutputTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -375,16 +372,14 @@
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
-    LogicalResourceIdOutputTypeDef,
-    PhysicalResourceIdOutputTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
     ResourceErrorTypeDef,
@@ -415,34 +410,33 @@
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
+    DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
+    ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    DeleteAppInputSourceRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    ResiliencyPolicyTypeDef,
     PhysicalResourceTypeDef,
-    ResourceMappingOutputTypeDef,
-    UnsupportedResourceTypeDef,
     ResourceMappingTypeDef,
+    UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
@@ -455,18 +449,18 @@
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
+    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
-    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     ListRecommendationTemplatesResponseTypeDef,
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
```

### Comparing `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/SOURCES.txt` & `mypy-boto3-resiliencehub-1.28.15/mypy_boto3_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.12/setup.py` & `mypy-boto3-resiliencehub-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resiliencehub",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResilienceHub 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ResilienceHub 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

