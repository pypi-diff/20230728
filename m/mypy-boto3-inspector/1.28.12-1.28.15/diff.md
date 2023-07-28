# Comparing `tmp/mypy-boto3-inspector-1.28.12.tar.gz` & `tmp/mypy-boto3-inspector-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-inspector-1.28.12.tar` & `mypy-boto3-inspector-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.296490 mypy-boto3-inspector-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-07-27 05:34:47.292490 mypy-boto3-inspector-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.284490 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31933 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41766 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.292490 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.296490 mypy-boto3-inspector-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.345214 mypy-boto3-inspector-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18832 2023-07-28 20:42:56.345214 mypy-boto3-inspector-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.325214 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31933 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40434 2023-07-28 20:27:45.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-07-28 20:27:43.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:42.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.345214 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18832 2023-07-28 20:42:56.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:56.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:56.000000 mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.345214 mypy-boto3-inspector-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:27:41.000000 mypy-boto3-inspector-1.28.15/setup.py
```

### Comparing `mypy-boto3-inspector-1.28.12/LICENSE` & `mypy-boto3-inspector-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/PKG-INFO` & `mypy-boto3-inspector-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.28.12
-Summary: Type annotations for boto3.Inspector 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Inspector 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,121 +373,118 @@
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
+    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
-    AttributeOutputTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
-    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
-    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
-    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
-    ResourceGroupTagOutputTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
-    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
+    AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
+    CreateResourceGroupResponseTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssessmentReportResponseTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
-    AssessmentTemplateTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
+    ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
-    ResourceGroupTypeDef,
-    SetTagsForResourceRequestRequestTypeDef,
+    DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
-    DescribeAssessmentTemplatesResponseTypeDef,
+    DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
-    DescribeResourceGroupsResponseTypeDef,
     FindingTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-inspector-1.28.12/README.md` & `mypy-boto3-inspector-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,121 +341,118 @@
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
+    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
-    AttributeOutputTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
-    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
-    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
-    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
-    ResourceGroupTagOutputTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
-    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
+    AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
+    CreateResourceGroupResponseTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssessmentReportResponseTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
-    AssessmentTemplateTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
+    ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
-    ResourceGroupTypeDef,
-    SetTagsForResourceRequestRequestTypeDef,
+    DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
-    DescribeAssessmentTemplatesResponseTypeDef,
+    DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
-    DescribeResourceGroupsResponseTypeDef,
     FindingTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.py` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.pyi` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__main__.py` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Inspector 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector\nOther"
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

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.py` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.pyi` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.py` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.pyi` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.py` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -65,170 +65,159 @@
     "ListEventSubscriptionsPaginator",
     "ListExclusionsPaginator",
     "ListFindingsPaginator",
     "ListRulesPackagesPaginator",
     "PreviewAgentsPaginator",
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
 class ListAssessmentRunAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
-
 class ListAssessmentRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
         """
 
-
 class ListAssessmentTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
         """
 
-
 class ListAssessmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
-
 class ListEventSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
         """
 
-
 class ListExclusionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
     """
 
     def paginate(
-        self, *, assessmentRunArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assessmentRunArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExclusionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
         """
 
-
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
         """
 
-
 class ListRulesPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
         """
 
-
 class PreviewAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
     """
 
     def paginate(
-        self, *, previewAgentsArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, previewAgentsArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PreviewAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
         """
```

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.pyi` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,159 +65,170 @@
     "ListEventSubscriptionsPaginator",
     "ListExclusionsPaginator",
     "ListFindingsPaginator",
     "ListRulesPackagesPaginator",
     "PreviewAgentsPaginator",
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
 class ListAssessmentRunAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
+
 class ListAssessmentRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
         """
 
+
 class ListAssessmentTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
         """
 
+
 class ListAssessmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
+
 class ListEventSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
         """
 
+
 class ListExclusionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
     """
 
     def paginate(
-        self, *, assessmentRunArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assessmentRunArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExclusionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
         """
 
+
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
         """
 
+
 class ListRulesPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
         """
 
+
 class PreviewAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
     """
 
     def paginate(
-        self, *, previewAgentsArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, previewAgentsArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PreviewAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
         """
```

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.py` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -36,125 +36,121 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
     "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
-    "AttributeOutputTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
-    "CreateAssessmentTargetResponseTypeDef",
-    "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
-    "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
-    "CreateResourceGroupResponseTypeDef",
     "DeleteAssessmentRunRequestRequestTypeDef",
     "DeleteAssessmentTargetRequestRequestTypeDef",
     "DeleteAssessmentTemplateRequestRequestTypeDef",
     "DescribeAssessmentRunsRequestRequestTypeDef",
     "DescribeAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
     "DescribeExclusionsRequestRequestTypeDef",
     "DescribeFindingsRequestRequestTypeDef",
     "DescribeResourceGroupsRequestRequestTypeDef",
     "DescribeRulesPackagesRequestRequestTypeDef",
     "RulesPackageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionTypeDef",
     "ScopeTypeDef",
     "InspectorServiceAttributesTypeDef",
     "GetAssessmentReportRequestRequestTypeDef",
-    "GetAssessmentReportResponseTypeDef",
     "GetExclusionsPreviewRequestRequestTypeDef",
     "GetTelemetryMetadataRequestRequestTypeDef",
-    "ListAssessmentRunsResponseTypeDef",
-    "ListAssessmentTargetsResponseTypeDef",
-    "ListAssessmentTemplatesResponseTypeDef",
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventSubscriptionsRequestRequestTypeDef",
-    "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListExclusionsRequestRequestTypeDef",
-    "ListExclusionsResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "ListRulesPackagesRequestRequestTypeDef",
-    "ListRulesPackagesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
-    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
-    "ResourceGroupTagOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "TagTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
-    "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
+    "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
+    "CreateAssessmentTargetResponseTypeDef",
+    "CreateAssessmentTemplateResponseTypeDef",
+    "CreateExclusionsPreviewResponseTypeDef",
+    "CreateResourceGroupResponseTypeDef",
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAssessmentReportResponseTypeDef",
+    "ListAssessmentRunsResponseTypeDef",
+    "ListAssessmentTargetsResponseTypeDef",
+    "ListAssessmentTemplatesResponseTypeDef",
+    "ListExclusionsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListRulesPackagesResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
-    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "StartAssessmentRunResponseTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
     "AssessmentRunFilterTypeDef",
     "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
-    "AssessmentTemplateTypeDef",
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
+    "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
+    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "ListExclusionsRequestListExclusionsPaginateTypeDef",
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
-    "ResourceGroupTypeDef",
-    "SetTagsForResourceRequestRequestTypeDef",
+    "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     "ListAssessmentRunsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
-    "DescribeAssessmentTemplatesResponseTypeDef",
+    "DescribeResourceGroupsResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
-    "DescribeResourceGroupsResponseTypeDef",
     "FindingTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -165,27 +161,36 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 FailedItemDetailsTypeDef = TypedDict(
     "FailedItemDetailsTypeDef",
     {
         "failureCode": FailedItemErrorCodeType,
         "retryable": bool,
     },
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
 AgentFilterTypeDef = TypedDict(
     "AgentFilterTypeDef",
     {
         "agentHealths": Sequence[AgentHealthType],
         "agentHealthCodes": Sequence[AgentHealthCodeType],
     },
 )
@@ -206,19 +211,17 @@
         "operatingSystem": str,
         "kernelVersion": str,
         "ipv4Address": str,
     },
     total=False,
 )
 
-
 class AgentPreviewTypeDef(_RequiredAgentPreviewTypeDef, _OptionalAgentPreviewTypeDef):
     pass
 
-
 _RequiredTelemetryMetadataTypeDef = TypedDict(
     "_RequiredTelemetryMetadataTypeDef",
     {
         "messageType": str,
         "count": int,
     },
 )
@@ -226,21 +229,19 @@
     "_OptionalTelemetryMetadataTypeDef",
     {
         "dataSize": int,
     },
     total=False,
 )
 
-
 class TelemetryMetadataTypeDef(
     _RequiredTelemetryMetadataTypeDef, _OptionalTelemetryMetadataTypeDef
 ):
     pass
 
-
 DurationRangeTypeDef = TypedDict(
     "DurationRangeTypeDef",
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
@@ -269,48 +270,27 @@
         "message": str,
         "snsTopicArn": str,
         "snsPublishStatusCode": AssessmentRunNotificationSnsStatusCodeType,
     },
     total=False,
 )
 
-
 class AssessmentRunNotificationTypeDef(
     _RequiredAssessmentRunNotificationTypeDef, _OptionalAssessmentRunNotificationTypeDef
 ):
     pass
 
-
 AssessmentRunStateChangeTypeDef = TypedDict(
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
 
-_RequiredAttributeOutputTypeDef = TypedDict(
-    "_RequiredAttributeOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalAttributeOutputTypeDef = TypedDict(
-    "_OptionalAttributeOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
-    pass
-
-
 AssessmentTargetFilterTypeDef = TypedDict(
     "AssessmentTargetFilterTypeDef",
     {
         "assessmentTargetNamePattern": str,
     },
     total=False,
 )
@@ -328,118 +308,78 @@
     "_OptionalAssessmentTargetTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
-
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
+_RequiredTagTypeDef = TypedDict(
+    "_RequiredTagTypeDef",
     {
         "key": str,
     },
 )
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
+_OptionalTagTypeDef = TypedDict(
+    "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
     },
 )
 _OptionalCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class CreateAssessmentTargetRequestRequestTypeDef(
     _RequiredCreateAssessmentTargetRequestRequestTypeDef,
     _OptionalCreateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
-
-CreateAssessmentTargetResponseTypeDef = TypedDict(
-    "CreateAssessmentTargetResponseTypeDef",
-    {
-        "assessmentTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssessmentTemplateResponseTypeDef = TypedDict(
-    "CreateAssessmentTemplateResponseTypeDef",
-    {
-        "assessmentTemplateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "CreateExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 
-CreateExclusionsPreviewResponseTypeDef = TypedDict(
-    "CreateExclusionsPreviewResponseTypeDef",
-    {
-        "previewToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredResourceGroupTagTypeDef = TypedDict(
     "_RequiredResourceGroupTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalResourceGroupTagTypeDef = TypedDict(
     "_OptionalResourceGroupTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class ResourceGroupTagTypeDef(_RequiredResourceGroupTagTypeDef, _OptionalResourceGroupTagTypeDef):
     pass
 
-
-CreateResourceGroupResponseTypeDef = TypedDict(
-    "CreateResourceGroupResponseTypeDef",
-    {
-        "resourceGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAssessmentRunRequestRequestTypeDef = TypedDict(
     "DeleteAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
@@ -474,67 +414,53 @@
 DescribeAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
     },
 )
 
-DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    {
-        "roleArn": str,
-        "valid": bool,
-        "registeredAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeExclusionsRequestRequestTypeDef",
     {
         "exclusionArns": Sequence[str],
     },
 )
 _OptionalDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeExclusionsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeExclusionsRequestRequestTypeDef(
     _RequiredDescribeExclusionsRequestRequestTypeDef,
     _OptionalDescribeExclusionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
     },
 )
 _OptionalDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFindingsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeFindingsRequestRequestTypeDef(
     _RequiredDescribeFindingsRequestRequestTypeDef, _OptionalDescribeFindingsRequestRequestTypeDef
 ):
     pass
 
-
 DescribeResourceGroupsRequestRequestTypeDef = TypedDict(
     "DescribeResourceGroupsRequestRequestTypeDef",
     {
         "resourceGroupArns": Sequence[str],
     },
 )
 
@@ -548,22 +474,20 @@
     "_OptionalDescribeRulesPackagesRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeRulesPackagesRequestRequestTypeDef(
     _RequiredDescribeRulesPackagesRequestRequestTypeDef,
     _OptionalDescribeRulesPackagesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRulesPackageTypeDef = TypedDict(
     "_RequiredRulesPackageTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "provider": str,
@@ -573,26 +497,17 @@
     "_OptionalRulesPackageTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class RulesPackageTypeDef(_RequiredRulesPackageTypeDef, _OptionalRulesPackageTypeDef):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "event": InspectorEventType,
         "subscribedAt": datetime,
     },
 )
@@ -617,39 +532,28 @@
     {
         "assessmentRunArn": str,
         "rulesPackageArn": str,
     },
     total=False,
 )
 
-
 class InspectorServiceAttributesTypeDef(
     _RequiredInspectorServiceAttributesTypeDef, _OptionalInspectorServiceAttributesTypeDef
 ):
     pass
 
-
 GetAssessmentReportRequestRequestTypeDef = TypedDict(
     "GetAssessmentReportRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
         "reportFileFormat": ReportFileFormatType,
         "reportType": ReportTypeType,
     },
 )
 
-GetAssessmentReportResponseTypeDef = TypedDict(
-    "GetAssessmentReportResponseTypeDef",
-    {
-        "status": ReportStatusType,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
         "previewToken": str,
     },
 )
@@ -659,97 +563,47 @@
         "nextToken": str,
         "maxResults": int,
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class GetExclusionsPreviewRequestRequestTypeDef(
     _RequiredGetExclusionsPreviewRequestRequestTypeDef,
     _OptionalGetExclusionsPreviewRequestRequestTypeDef,
 ):
     pass
 
-
 GetTelemetryMetadataRequestRequestTypeDef = TypedDict(
     "GetTelemetryMetadataRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
-ListAssessmentRunsResponseTypeDef = TypedDict(
-    "ListAssessmentRunsResponseTypeDef",
-    {
-        "assessmentRunArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTargetsResponseTypeDef = TypedDict(
-    "ListAssessmentTargetsResponseTypeDef",
-    {
-        "assessmentTargetArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTemplatesResponseTypeDef = TypedDict(
-    "ListAssessmentTemplatesResponseTypeDef",
-    {
-        "assessmentTemplateArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "resourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEventSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListEventSubscriptionsRequestRequestTypeDef",
     {
         "resourceArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExclusionsRequestListExclusionsPaginateTypeDef(
-    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
-    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExclusionsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalListExclusionsRequestRequestTypeDef = TypedDict(
@@ -757,65 +611,28 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListExclusionsRequestRequestTypeDef(
     _RequiredListExclusionsRequestRequestTypeDef, _OptionalListExclusionsRequestRequestTypeDef
 ):
     pass
 
-
-ListExclusionsResponseTypeDef = TypedDict(
-    "ListExclusionsResponseTypeDef",
-    {
-        "exclusionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesPackagesRequestRequestTypeDef = TypedDict(
     "ListRulesPackagesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListRulesPackagesResponseTypeDef = TypedDict(
-    "ListRulesPackagesResponseTypeDef",
-    {
-        "rulesPackageArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -833,46 +650,14 @@
     {
         "groupName": str,
         "groupId": str,
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
-_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "previewAgentsArn": str,
-    },
-)
-_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
-    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredPreviewAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredPreviewAgentsRequestRequestTypeDef",
     {
         "previewAgentsArn": str,
     },
 )
 _OptionalPreviewAgentsRequestRequestTypeDef = TypedDict(
@@ -880,21 +665,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class PreviewAgentsRequestRequestTypeDef(
     _RequiredPreviewAgentsRequestRequestTypeDef, _OptionalPreviewAgentsRequestRequestTypeDef
 ):
     pass
 
-
 RegisterCrossAccountAccessRoleRequestRequestTypeDef = TypedDict(
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -902,116 +685,53 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
     },
 )
 
-_RequiredResourceGroupTagOutputTypeDef = TypedDict(
-    "_RequiredResourceGroupTagOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalResourceGroupTagOutputTypeDef = TypedDict(
-    "_OptionalResourceGroupTagOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class ResourceGroupTagOutputTypeDef(
-    _RequiredResourceGroupTagOutputTypeDef, _OptionalResourceGroupTagOutputTypeDef
-):
-    pass
-
-
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
-_RequiredTagTypeDef = TypedDict(
-    "_RequiredTagTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalTagTypeDef = TypedDict(
-    "_OptionalTagTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
-    pass
-
-
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunName": str,
     },
     total=False,
 )
 
-
 class StartAssessmentRunRequestRequestTypeDef(
     _RequiredStartAssessmentRunRequestRequestTypeDef,
     _OptionalStartAssessmentRunRequestRequestTypeDef,
 ):
     pass
 
-
-StartAssessmentRunResponseTypeDef = TypedDict(
-    "StartAssessmentRunResponseTypeDef",
-    {
-        "assessmentRunArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStopAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStopAssessmentRunRequestRequestTypeDef",
     {
         "stopAction": StopActionType,
     },
     total=False,
 )
 
-
 class StopAssessmentRunRequestRequestTypeDef(
     _RequiredStopAssessmentRunRequestRequestTypeDef, _OptionalStopAssessmentRunRequestRequestTypeDef
 ):
     pass
 
-
 SubscribeToEventRequestRequestTypeDef = TypedDict(
     "SubscribeToEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -1037,30 +757,54 @@
     "_OptionalUpdateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class UpdateAssessmentTargetRequestRequestTypeDef(
     _RequiredUpdateAssessmentTargetRequestRequestTypeDef,
     _OptionalUpdateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
-
 AddAttributesToFindingsRequestRequestTypeDef = TypedDict(
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
+_RequiredAssessmentTemplateTypeDef = TypedDict(
+    "_RequiredAssessmentTemplateTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "assessmentTargetArn": str,
+        "durationInSeconds": int,
+        "rulesPackageArns": List[str],
+        "userAttributesForFindings": List[AttributeTypeDef],
+        "assessmentRunCount": int,
+        "createdAt": datetime,
+    },
+)
+_OptionalAssessmentTemplateTypeDef = TypedDict(
+    "_OptionalAssessmentTemplateTypeDef",
+    {
+        "lastAssessmentRunArn": str,
+    },
+    total=False,
+)
+
+class AssessmentTemplateTypeDef(
+    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
+):
+    pass
+
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -1070,60 +814,155 @@
     "_OptionalCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "userAttributesForFindings": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class CreateAssessmentTemplateRequestRequestTypeDef(
     _RequiredCreateAssessmentTemplateRequestRequestTypeDef,
     _OptionalCreateAssessmentTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 AddAttributesToFindingsResponseTypeDef = TypedDict(
     "AddAttributesToFindingsResponseTypeDef",
     {
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
-    "RemoveAttributesFromFindingsResponseTypeDef",
+CreateAssessmentTargetResponseTypeDef = TypedDict(
+    "CreateAssessmentTargetResponseTypeDef",
     {
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+CreateAssessmentTemplateResponseTypeDef = TypedDict(
+    "CreateAssessmentTemplateResponseTypeDef",
     {
-        "assessmentRunArn": str,
+        "assessmentTemplateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+
+CreateExclusionsPreviewResponseTypeDef = TypedDict(
+    "CreateExclusionsPreviewResponseTypeDef",
     {
-        "filter": AgentFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "previewToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateResourceGroupResponseTypeDef = TypedDict(
+    "CreateResourceGroupResponseTypeDef",
+    {
+        "resourceGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
-    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-):
-    pass
+DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    {
+        "roleArn": str,
+        "valid": bool,
+        "registeredAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAssessmentReportResponseTypeDef = TypedDict(
+    "GetAssessmentReportResponseTypeDef",
+    {
+        "status": ReportStatusType,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentRunsResponseTypeDef = TypedDict(
+    "ListAssessmentRunsResponseTypeDef",
+    {
+        "assessmentRunArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTargetsResponseTypeDef = TypedDict(
+    "ListAssessmentTargetsResponseTypeDef",
+    {
+        "assessmentTargetArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTemplatesResponseTypeDef = TypedDict(
+    "ListAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplateArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListExclusionsResponseTypeDef = TypedDict(
+    "ListExclusionsResponseTypeDef",
+    {
+        "exclusionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRulesPackagesResponseTypeDef = TypedDict(
+    "ListRulesPackagesResponseTypeDef",
+    {
+        "rulesPackageArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
+    "RemoveAttributesFromFindingsResponseTypeDef",
+    {
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAssessmentRunResponseTypeDef = TypedDict(
+    "StartAssessmentRunResponseTypeDef",
+    {
+        "assessmentRunArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredListAssessmentRunAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentRunAgentsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -1133,28 +972,26 @@
         "filter": AgentFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssessmentRunAgentsRequestRequestTypeDef(
     _RequiredListAssessmentRunAgentsRequestRequestTypeDef,
     _OptionalListAssessmentRunAgentsRequestRequestTypeDef,
 ):
     pass
 
-
 PreviewAgentsResponseTypeDef = TypedDict(
     "PreviewAgentsResponseTypeDef",
     {
         "agentPreviews": List[AgentPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssessmentRunAgentTypeDef = TypedDict(
     "_RequiredAssessmentRunAgentTypeDef",
     {
         "agentId": str,
@@ -1169,26 +1006,24 @@
     {
         "agentHealthDetails": str,
         "autoScalingGroup": str,
     },
     total=False,
 )
 
-
 class AssessmentRunAgentTypeDef(
     _RequiredAssessmentRunAgentTypeDef, _OptionalAssessmentRunAgentTypeDef
 ):
     pass
 
-
 GetTelemetryMetadataResponseTypeDef = TypedDict(
     "GetTelemetryMetadataResponseTypeDef",
     {
         "telemetryMetadata": List[TelemetryMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTemplateFilterTypeDef = TypedDict(
     "AssessmentTemplateFilterTypeDef",
     {
         "namePattern": str,
@@ -1232,15 +1067,15 @@
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
         "durationInSeconds": int,
         "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeOutputTypeDef],
+        "userAttributesForFindings": List[AttributeTypeDef],
         "createdAt": datetime,
         "stateChangedAt": datetime,
         "dataCollected": bool,
         "stateChanges": List[AssessmentRunStateChangeTypeDef],
         "notifications": List[AssessmentRunNotificationTypeDef],
         "findingCounts": Dict[SeverityType, int],
     },
@@ -1250,56 +1085,17 @@
     {
         "startedAt": datetime,
         "completedAt": datetime,
     },
     total=False,
 )
 
-
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
-
-_RequiredAssessmentTemplateTypeDef = TypedDict(
-    "_RequiredAssessmentTemplateTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "assessmentTargetArn": str,
-        "durationInSeconds": int,
-        "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeOutputTypeDef],
-        "assessmentRunCount": int,
-        "createdAt": datetime,
-    },
-)
-_OptionalAssessmentTemplateTypeDef = TypedDict(
-    "_OptionalAssessmentTemplateTypeDef",
-    {
-        "lastAssessmentRunArn": str,
-    },
-    total=False,
-)
-
-
-class AssessmentTemplateTypeDef(
-    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
-):
-    pass
-
-
-ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    {
-        "filter": AssessmentTargetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssessmentTargetsRequestRequestTypeDef = TypedDict(
     "ListAssessmentTargetsRequestRequestTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1307,39 +1103,68 @@
 )
 
 DescribeAssessmentTargetsResponseTypeDef = TypedDict(
     "DescribeAssessmentTargetsResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredSetTagsForResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalSetTagsForResourceRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class SetTagsForResourceRequestRequestTypeDef(
+    _RequiredSetTagsForResourceRequestRequestTypeDef,
+    _OptionalSetTagsForResourceRequestRequestTypeDef,
+):
+    pass
+
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
+ResourceGroupTypeDef = TypedDict(
+    "ResourceGroupTypeDef",
+    {
+        "arn": str,
+        "tags": List[ResourceGroupTagTypeDef],
+        "createdAt": datetime,
+    },
+)
+
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "resourceArn": str,
@@ -1356,110 +1181,171 @@
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionPreviewTypeDef = TypedDict(
     "_OptionalExclusionPreviewTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
 
-
 _RequiredExclusionTypeDef = TypedDict(
     "_RequiredExclusionTypeDef",
     {
         "arn": str,
         "title": str,
         "description": str,
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionTypeDef = TypedDict(
     "_OptionalExclusionTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
 
-
-NetworkInterfaceTypeDef = TypedDict(
-    "NetworkInterfaceTypeDef",
+_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     {
-        "networkInterfaceId": str,
-        "subnetId": str,
-        "vpcId": str,
-        "privateDnsName": str,
-        "privateIpAddress": str,
-        "privateIpAddresses": List[PrivateIpTypeDef],
-        "publicDnsName": str,
-        "publicIp": str,
-        "ipv6Addresses": List[str],
-        "securityGroups": List[SecurityGroupTypeDef],
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    {
+        "filter": AgentFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResourceGroupTypeDef = TypedDict(
-    "ResourceGroupTypeDef",
+class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
+    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+):
+    pass
+
+ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     {
-        "arn": str,
-        "tags": List[ResourceGroupTagOutputTypeDef],
-        "createdAt": datetime,
+        "filter": AssessmentTargetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredSetTagsForResourceRequestRequestTypeDef",
+ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
     {
         "resourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "assessmentRunArn": str,
     },
 )
-_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalSetTagsForResourceRequestRequestTypeDef",
+_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListExclusionsRequestListExclusionsPaginateTypeDef(
+    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
+    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
+):
+    pass
 
-class SetTagsForResourceRequestRequestTypeDef(
-    _RequiredSetTagsForResourceRequestRequestTypeDef,
-    _OptionalSetTagsForResourceRequestRequestTypeDef,
+ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "previewAgentsArn": str,
+    },
+)
+_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
+    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
 ):
     pass
 
+NetworkInterfaceTypeDef = TypedDict(
+    "NetworkInterfaceTypeDef",
+    {
+        "networkInterfaceId": str,
+        "subnetId": str,
+        "vpcId": str,
+        "privateDnsName": str,
+        "privateIpAddress": str,
+        "privateIpAddresses": List[PrivateIpTypeDef],
+        "publicDnsName": str,
+        "publicIp": str,
+        "ipv6Addresses": List[str],
+        "securityGroups": List[SecurityGroupTypeDef],
+    },
+    total=False,
+)
+
+DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
+    "DescribeAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplates": List[AssessmentTemplateTypeDef],
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     {
         "assessmentTargetArns": Sequence[str],
         "filter": AssessmentTemplateFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestRequestTypeDef",
     {
@@ -1472,15 +1358,15 @@
 )
 
 ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
         "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAssessmentRunsRequestRequestTypeDef = TypedDict(
     "ListAssessmentRunsRequestRequestTypeDef",
     {
@@ -1493,15 +1379,15 @@
 )
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "assessmentRunArns": Sequence[str],
         "filter": FindingFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -1514,52 +1400,52 @@
 )
 
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
-    "DescribeAssessmentTemplatesResponseTypeDef",
+DescribeResourceGroupsResponseTypeDef = TypedDict(
+    "DescribeResourceGroupsResponseTypeDef",
     {
-        "assessmentTemplates": List[AssessmentTemplateTypeDef],
+        "resourceGroups": List[ResourceGroupTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
     {
         "subscriptions": List[SubscriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExclusionsPreviewResponseTypeDef = TypedDict(
     "GetExclusionsPreviewResponseTypeDef",
     {
         "previewStatus": PreviewStatusType,
         "exclusionPreviews": List[ExclusionPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExclusionsResponseTypeDef = TypedDict(
     "DescribeExclusionsResponseTypeDef",
     {
         "exclusions": Dict[str, ExclusionTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetAttributesTypeDef = TypedDict(
     "_RequiredAssetAttributesTypeDef",
     {
         "schemaVersion": int,
@@ -1569,40 +1455,29 @@
     "_OptionalAssetAttributesTypeDef",
     {
         "agentId": str,
         "autoScalingGroup": str,
         "amiId": str,
         "hostname": str,
         "ipv4Addresses": List[str],
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
-
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
-
-DescribeResourceGroupsResponseTypeDef = TypedDict(
-    "DescribeResourceGroupsResponseTypeDef",
-    {
-        "resourceGroups": List[ResourceGroupTypeDef],
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
-        "attributes": List[AttributeOutputTypeDef],
-        "userAttributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "userAttributes": List[AttributeTypeDef],
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalFindingTypeDef = TypedDict(
     "_OptionalFindingTypeDef",
     {
@@ -1619,20 +1494,18 @@
         "numericSeverity": float,
         "confidence": int,
         "indicatorOfCompromise": bool,
     },
     total=False,
 )
 
-
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
-
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.pyi` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,124 +36,122 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
     "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
-    "AttributeOutputTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
-    "CreateAssessmentTargetResponseTypeDef",
-    "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
-    "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
-    "CreateResourceGroupResponseTypeDef",
     "DeleteAssessmentRunRequestRequestTypeDef",
     "DeleteAssessmentTargetRequestRequestTypeDef",
     "DeleteAssessmentTemplateRequestRequestTypeDef",
     "DescribeAssessmentRunsRequestRequestTypeDef",
     "DescribeAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
     "DescribeExclusionsRequestRequestTypeDef",
     "DescribeFindingsRequestRequestTypeDef",
     "DescribeResourceGroupsRequestRequestTypeDef",
     "DescribeRulesPackagesRequestRequestTypeDef",
     "RulesPackageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionTypeDef",
     "ScopeTypeDef",
     "InspectorServiceAttributesTypeDef",
     "GetAssessmentReportRequestRequestTypeDef",
-    "GetAssessmentReportResponseTypeDef",
     "GetExclusionsPreviewRequestRequestTypeDef",
     "GetTelemetryMetadataRequestRequestTypeDef",
-    "ListAssessmentRunsResponseTypeDef",
-    "ListAssessmentTargetsResponseTypeDef",
-    "ListAssessmentTemplatesResponseTypeDef",
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventSubscriptionsRequestRequestTypeDef",
-    "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListExclusionsRequestRequestTypeDef",
-    "ListExclusionsResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "ListRulesPackagesRequestRequestTypeDef",
-    "ListRulesPackagesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
-    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
-    "ResourceGroupTagOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "TagTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
-    "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
+    "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
+    "CreateAssessmentTargetResponseTypeDef",
+    "CreateAssessmentTemplateResponseTypeDef",
+    "CreateExclusionsPreviewResponseTypeDef",
+    "CreateResourceGroupResponseTypeDef",
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAssessmentReportResponseTypeDef",
+    "ListAssessmentRunsResponseTypeDef",
+    "ListAssessmentTargetsResponseTypeDef",
+    "ListAssessmentTemplatesResponseTypeDef",
+    "ListExclusionsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListRulesPackagesResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
-    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "StartAssessmentRunResponseTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
     "AssessmentRunFilterTypeDef",
     "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
-    "AssessmentTemplateTypeDef",
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
+    "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
+    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "ListExclusionsRequestListExclusionsPaginateTypeDef",
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
-    "ResourceGroupTypeDef",
-    "SetTagsForResourceRequestRequestTypeDef",
+    "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     "ListAssessmentRunsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
-    "DescribeAssessmentTemplatesResponseTypeDef",
+    "DescribeResourceGroupsResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
-    "DescribeResourceGroupsResponseTypeDef",
     "FindingTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -164,25 +162,38 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 FailedItemDetailsTypeDef = TypedDict(
     "FailedItemDetailsTypeDef",
     {
         "failureCode": FailedItemErrorCodeType,
         "retryable": bool,
     },
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
 AgentFilterTypeDef = TypedDict(
     "AgentFilterTypeDef",
     {
         "agentHealths": Sequence[AgentHealthType],
         "agentHealthCodes": Sequence[AgentHealthCodeType],
     },
 )
@@ -203,17 +214,19 @@
         "operatingSystem": str,
         "kernelVersion": str,
         "ipv4Address": str,
     },
     total=False,
 )
 
+
 class AgentPreviewTypeDef(_RequiredAgentPreviewTypeDef, _OptionalAgentPreviewTypeDef):
     pass
 
+
 _RequiredTelemetryMetadataTypeDef = TypedDict(
     "_RequiredTelemetryMetadataTypeDef",
     {
         "messageType": str,
         "count": int,
     },
 )
@@ -221,19 +234,21 @@
     "_OptionalTelemetryMetadataTypeDef",
     {
         "dataSize": int,
     },
     total=False,
 )
 
+
 class TelemetryMetadataTypeDef(
     _RequiredTelemetryMetadataTypeDef, _OptionalTelemetryMetadataTypeDef
 ):
     pass
 
+
 DurationRangeTypeDef = TypedDict(
     "DurationRangeTypeDef",
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
@@ -262,44 +277,29 @@
         "message": str,
         "snsTopicArn": str,
         "snsPublishStatusCode": AssessmentRunNotificationSnsStatusCodeType,
     },
     total=False,
 )
 
+
 class AssessmentRunNotificationTypeDef(
     _RequiredAssessmentRunNotificationTypeDef, _OptionalAssessmentRunNotificationTypeDef
 ):
     pass
 
+
 AssessmentRunStateChangeTypeDef = TypedDict(
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
 
-_RequiredAttributeOutputTypeDef = TypedDict(
-    "_RequiredAttributeOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalAttributeOutputTypeDef = TypedDict(
-    "_OptionalAttributeOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
-    pass
-
 AssessmentTargetFilterTypeDef = TypedDict(
     "AssessmentTargetFilterTypeDef",
     {
         "assessmentTargetNamePattern": str,
     },
     total=False,
 )
@@ -317,109 +317,85 @@
     "_OptionalAssessmentTargetTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
+
+_RequiredTagTypeDef = TypedDict(
+    "_RequiredTagTypeDef",
     {
         "key": str,
     },
 )
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
+_OptionalTagTypeDef = TypedDict(
+    "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+
+class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
     },
 )
 _OptionalCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class CreateAssessmentTargetRequestRequestTypeDef(
     _RequiredCreateAssessmentTargetRequestRequestTypeDef,
     _OptionalCreateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
-CreateAssessmentTargetResponseTypeDef = TypedDict(
-    "CreateAssessmentTargetResponseTypeDef",
-    {
-        "assessmentTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssessmentTemplateResponseTypeDef = TypedDict(
-    "CreateAssessmentTemplateResponseTypeDef",
-    {
-        "assessmentTemplateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "CreateExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 
-CreateExclusionsPreviewResponseTypeDef = TypedDict(
-    "CreateExclusionsPreviewResponseTypeDef",
-    {
-        "previewToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredResourceGroupTagTypeDef = TypedDict(
     "_RequiredResourceGroupTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalResourceGroupTagTypeDef = TypedDict(
     "_OptionalResourceGroupTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class ResourceGroupTagTypeDef(_RequiredResourceGroupTagTypeDef, _OptionalResourceGroupTagTypeDef):
     pass
 
-CreateResourceGroupResponseTypeDef = TypedDict(
-    "CreateResourceGroupResponseTypeDef",
-    {
-        "resourceGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteAssessmentRunRequestRequestTypeDef = TypedDict(
     "DeleteAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -455,63 +431,57 @@
 DescribeAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
     },
 )
 
-DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    {
-        "roleArn": str,
-        "valid": bool,
-        "registeredAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeExclusionsRequestRequestTypeDef",
     {
         "exclusionArns": Sequence[str],
     },
 )
 _OptionalDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeExclusionsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeExclusionsRequestRequestTypeDef(
     _RequiredDescribeExclusionsRequestRequestTypeDef,
     _OptionalDescribeExclusionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
     },
 )
 _OptionalDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFindingsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeFindingsRequestRequestTypeDef(
     _RequiredDescribeFindingsRequestRequestTypeDef, _OptionalDescribeFindingsRequestRequestTypeDef
 ):
     pass
 
+
 DescribeResourceGroupsRequestRequestTypeDef = TypedDict(
     "DescribeResourceGroupsRequestRequestTypeDef",
     {
         "resourceGroupArns": Sequence[str],
     },
 )
 
@@ -525,20 +495,22 @@
     "_OptionalDescribeRulesPackagesRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeRulesPackagesRequestRequestTypeDef(
     _RequiredDescribeRulesPackagesRequestRequestTypeDef,
     _OptionalDescribeRulesPackagesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRulesPackageTypeDef = TypedDict(
     "_RequiredRulesPackageTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "provider": str,
@@ -548,23 +520,18 @@
     "_OptionalRulesPackageTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class RulesPackageTypeDef(_RequiredRulesPackageTypeDef, _OptionalRulesPackageTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "event": InspectorEventType,
         "subscribedAt": datetime,
     },
@@ -590,37 +557,30 @@
     {
         "assessmentRunArn": str,
         "rulesPackageArn": str,
     },
     total=False,
 )
 
+
 class InspectorServiceAttributesTypeDef(
     _RequiredInspectorServiceAttributesTypeDef, _OptionalInspectorServiceAttributesTypeDef
 ):
     pass
 
+
 GetAssessmentReportRequestRequestTypeDef = TypedDict(
     "GetAssessmentReportRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
         "reportFileFormat": ReportFileFormatType,
         "reportType": ReportTypeType,
     },
 )
 
-GetAssessmentReportResponseTypeDef = TypedDict(
-    "GetAssessmentReportResponseTypeDef",
-    {
-        "status": ReportStatusType,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
         "previewToken": str,
     },
 )
@@ -630,93 +590,49 @@
         "nextToken": str,
         "maxResults": int,
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class GetExclusionsPreviewRequestRequestTypeDef(
     _RequiredGetExclusionsPreviewRequestRequestTypeDef,
     _OptionalGetExclusionsPreviewRequestRequestTypeDef,
 ):
     pass
 
+
 GetTelemetryMetadataRequestRequestTypeDef = TypedDict(
     "GetTelemetryMetadataRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
-ListAssessmentRunsResponseTypeDef = TypedDict(
-    "ListAssessmentRunsResponseTypeDef",
-    {
-        "assessmentRunArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTargetsResponseTypeDef = TypedDict(
-    "ListAssessmentTargetsResponseTypeDef",
-    {
-        "assessmentTargetArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTemplatesResponseTypeDef = TypedDict(
-    "ListAssessmentTemplatesResponseTypeDef",
-    {
-        "assessmentTemplateArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "resourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEventSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListEventSubscriptionsRequestRequestTypeDef",
     {
         "resourceArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExclusionsRequestListExclusionsPaginateTypeDef(
-    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
-    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExclusionsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalListExclusionsRequestRequestTypeDef = TypedDict(
@@ -724,63 +640,30 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListExclusionsRequestRequestTypeDef(
     _RequiredListExclusionsRequestRequestTypeDef, _OptionalListExclusionsRequestRequestTypeDef
 ):
     pass
 
-ListExclusionsResponseTypeDef = TypedDict(
-    "ListExclusionsResponseTypeDef",
-    {
-        "exclusionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListRulesPackagesRequestRequestTypeDef = TypedDict(
     "ListRulesPackagesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListRulesPackagesResponseTypeDef = TypedDict(
-    "ListRulesPackagesResponseTypeDef",
-    {
-        "rulesPackageArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -798,44 +681,14 @@
     {
         "groupName": str,
         "groupId": str,
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
-_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "previewAgentsArn": str,
-    },
-)
-_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
-    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-):
-    pass
-
 _RequiredPreviewAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredPreviewAgentsRequestRequestTypeDef",
     {
         "previewAgentsArn": str,
     },
 )
 _OptionalPreviewAgentsRequestRequestTypeDef = TypedDict(
@@ -843,19 +696,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class PreviewAgentsRequestRequestTypeDef(
     _RequiredPreviewAgentsRequestRequestTypeDef, _OptionalPreviewAgentsRequestRequestTypeDef
 ):
     pass
 
+
 RegisterCrossAccountAccessRoleRequestRequestTypeDef = TypedDict(
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -863,88 +718,35 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
     },
 )
 
-_RequiredResourceGroupTagOutputTypeDef = TypedDict(
-    "_RequiredResourceGroupTagOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalResourceGroupTagOutputTypeDef = TypedDict(
-    "_OptionalResourceGroupTagOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class ResourceGroupTagOutputTypeDef(
-    _RequiredResourceGroupTagOutputTypeDef, _OptionalResourceGroupTagOutputTypeDef
-):
-    pass
-
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
-_RequiredTagTypeDef = TypedDict(
-    "_RequiredTagTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalTagTypeDef = TypedDict(
-    "_OptionalTagTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
-    pass
-
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunName": str,
     },
     total=False,
 )
 
+
 class StartAssessmentRunRequestRequestTypeDef(
     _RequiredStartAssessmentRunRequestRequestTypeDef,
     _OptionalStartAssessmentRunRequestRequestTypeDef,
 ):
     pass
 
-StartAssessmentRunResponseTypeDef = TypedDict(
-    "StartAssessmentRunResponseTypeDef",
-    {
-        "assessmentRunArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStopAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -952,19 +754,21 @@
     "_OptionalStopAssessmentRunRequestRequestTypeDef",
     {
         "stopAction": StopActionType,
     },
     total=False,
 )
 
+
 class StopAssessmentRunRequestRequestTypeDef(
     _RequiredStopAssessmentRunRequestRequestTypeDef, _OptionalStopAssessmentRunRequestRequestTypeDef
 ):
     pass
 
+
 SubscribeToEventRequestRequestTypeDef = TypedDict(
     "SubscribeToEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -990,28 +794,58 @@
     "_OptionalUpdateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class UpdateAssessmentTargetRequestRequestTypeDef(
     _RequiredUpdateAssessmentTargetRequestRequestTypeDef,
     _OptionalUpdateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
+
 AddAttributesToFindingsRequestRequestTypeDef = TypedDict(
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
+_RequiredAssessmentTemplateTypeDef = TypedDict(
+    "_RequiredAssessmentTemplateTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "assessmentTargetArn": str,
+        "durationInSeconds": int,
+        "rulesPackageArns": List[str],
+        "userAttributesForFindings": List[AttributeTypeDef],
+        "assessmentRunCount": int,
+        "createdAt": datetime,
+    },
+)
+_OptionalAssessmentTemplateTypeDef = TypedDict(
+    "_OptionalAssessmentTemplateTypeDef",
+    {
+        "lastAssessmentRunArn": str,
+    },
+    total=False,
+)
+
+
+class AssessmentTemplateTypeDef(
+    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
+):
+    pass
+
+
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -1021,56 +855,157 @@
     "_OptionalCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "userAttributesForFindings": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class CreateAssessmentTemplateRequestRequestTypeDef(
     _RequiredCreateAssessmentTemplateRequestRequestTypeDef,
     _OptionalCreateAssessmentTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 AddAttributesToFindingsResponseTypeDef = TypedDict(
     "AddAttributesToFindingsResponseTypeDef",
     {
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
-    "RemoveAttributesFromFindingsResponseTypeDef",
+CreateAssessmentTargetResponseTypeDef = TypedDict(
+    "CreateAssessmentTargetResponseTypeDef",
     {
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+CreateAssessmentTemplateResponseTypeDef = TypedDict(
+    "CreateAssessmentTemplateResponseTypeDef",
     {
-        "assessmentRunArn": str,
+        "assessmentTemplateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+
+CreateExclusionsPreviewResponseTypeDef = TypedDict(
+    "CreateExclusionsPreviewResponseTypeDef",
     {
-        "filter": AgentFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "previewToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
-    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-):
-    pass
+CreateResourceGroupResponseTypeDef = TypedDict(
+    "CreateResourceGroupResponseTypeDef",
+    {
+        "resourceGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    {
+        "roleArn": str,
+        "valid": bool,
+        "registeredAt": datetime,
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
+GetAssessmentReportResponseTypeDef = TypedDict(
+    "GetAssessmentReportResponseTypeDef",
+    {
+        "status": ReportStatusType,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentRunsResponseTypeDef = TypedDict(
+    "ListAssessmentRunsResponseTypeDef",
+    {
+        "assessmentRunArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTargetsResponseTypeDef = TypedDict(
+    "ListAssessmentTargetsResponseTypeDef",
+    {
+        "assessmentTargetArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTemplatesResponseTypeDef = TypedDict(
+    "ListAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplateArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListExclusionsResponseTypeDef = TypedDict(
+    "ListExclusionsResponseTypeDef",
+    {
+        "exclusionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRulesPackagesResponseTypeDef = TypedDict(
+    "ListRulesPackagesResponseTypeDef",
+    {
+        "rulesPackageArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
+    "RemoveAttributesFromFindingsResponseTypeDef",
+    {
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAssessmentRunResponseTypeDef = TypedDict(
+    "StartAssessmentRunResponseTypeDef",
+    {
+        "assessmentRunArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredListAssessmentRunAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentRunAgentsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -1080,26 +1015,28 @@
         "filter": AgentFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssessmentRunAgentsRequestRequestTypeDef(
     _RequiredListAssessmentRunAgentsRequestRequestTypeDef,
     _OptionalListAssessmentRunAgentsRequestRequestTypeDef,
 ):
     pass
 
+
 PreviewAgentsResponseTypeDef = TypedDict(
     "PreviewAgentsResponseTypeDef",
     {
         "agentPreviews": List[AgentPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssessmentRunAgentTypeDef = TypedDict(
     "_RequiredAssessmentRunAgentTypeDef",
     {
         "agentId": str,
@@ -1114,24 +1051,26 @@
     {
         "agentHealthDetails": str,
         "autoScalingGroup": str,
     },
     total=False,
 )
 
+
 class AssessmentRunAgentTypeDef(
     _RequiredAssessmentRunAgentTypeDef, _OptionalAssessmentRunAgentTypeDef
 ):
     pass
 
+
 GetTelemetryMetadataResponseTypeDef = TypedDict(
     "GetTelemetryMetadataResponseTypeDef",
     {
         "telemetryMetadata": List[TelemetryMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTemplateFilterTypeDef = TypedDict(
     "AssessmentTemplateFilterTypeDef",
     {
         "namePattern": str,
@@ -1175,15 +1114,15 @@
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
         "durationInSeconds": int,
         "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeOutputTypeDef],
+        "userAttributesForFindings": List[AttributeTypeDef],
         "createdAt": datetime,
         "stateChangedAt": datetime,
         "dataCollected": bool,
         "stateChanges": List[AssessmentRunStateChangeTypeDef],
         "notifications": List[AssessmentRunNotificationTypeDef],
         "findingCounts": Dict[SeverityType, int],
     },
@@ -1193,51 +1132,18 @@
     {
         "startedAt": datetime,
         "completedAt": datetime,
     },
     total=False,
 )
 
+
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
-_RequiredAssessmentTemplateTypeDef = TypedDict(
-    "_RequiredAssessmentTemplateTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "assessmentTargetArn": str,
-        "durationInSeconds": int,
-        "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeOutputTypeDef],
-        "assessmentRunCount": int,
-        "createdAt": datetime,
-    },
-)
-_OptionalAssessmentTemplateTypeDef = TypedDict(
-    "_OptionalAssessmentTemplateTypeDef",
-    {
-        "lastAssessmentRunArn": str,
-    },
-    total=False,
-)
-
-class AssessmentTemplateTypeDef(
-    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
-):
-    pass
-
-ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    {
-        "filter": AssessmentTargetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListAssessmentTargetsRequestRequestTypeDef = TypedDict(
     "ListAssessmentTargetsRequestRequestTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
@@ -1246,39 +1152,70 @@
 )
 
 DescribeAssessmentTargetsResponseTypeDef = TypedDict(
     "DescribeAssessmentTargetsResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredSetTagsForResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalSetTagsForResourceRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class SetTagsForResourceRequestRequestTypeDef(
+    _RequiredSetTagsForResourceRequestRequestTypeDef,
+    _OptionalSetTagsForResourceRequestRequestTypeDef,
+):
+    pass
+
+
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
+ResourceGroupTypeDef = TypedDict(
+    "ResourceGroupTypeDef",
+    {
+        "arn": str,
+        "tags": List[ResourceGroupTagTypeDef],
+        "createdAt": datetime,
+    },
+)
+
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "resourceArn": str,
@@ -1295,104 +1232,181 @@
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionPreviewTypeDef = TypedDict(
     "_OptionalExclusionPreviewTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
 
+
 _RequiredExclusionTypeDef = TypedDict(
     "_RequiredExclusionTypeDef",
     {
         "arn": str,
         "title": str,
         "description": str,
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionTypeDef = TypedDict(
     "_OptionalExclusionTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
 
-NetworkInterfaceTypeDef = TypedDict(
-    "NetworkInterfaceTypeDef",
+
+_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     {
-        "networkInterfaceId": str,
-        "subnetId": str,
-        "vpcId": str,
-        "privateDnsName": str,
-        "privateIpAddress": str,
-        "privateIpAddresses": List[PrivateIpTypeDef],
-        "publicDnsName": str,
-        "publicIp": str,
-        "ipv6Addresses": List[str],
-        "securityGroups": List[SecurityGroupTypeDef],
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    {
+        "filter": AgentFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResourceGroupTypeDef = TypedDict(
-    "ResourceGroupTypeDef",
+
+class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
+    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+):
+    pass
+
+
+ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     {
-        "arn": str,
-        "tags": List[ResourceGroupTagOutputTypeDef],
-        "createdAt": datetime,
+        "filter": AssessmentTargetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredSetTagsForResourceRequestRequestTypeDef",
+ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
     {
         "resourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalSetTagsForResourceRequestRequestTypeDef",
+
+_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class SetTagsForResourceRequestRequestTypeDef(
-    _RequiredSetTagsForResourceRequestRequestTypeDef,
-    _OptionalSetTagsForResourceRequestRequestTypeDef,
+
+class ListExclusionsRequestListExclusionsPaginateTypeDef(
+    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
+    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
+):
+    pass
+
+
+ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "previewAgentsArn": str,
+    },
+)
+_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
+    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
 ):
     pass
 
+
+NetworkInterfaceTypeDef = TypedDict(
+    "NetworkInterfaceTypeDef",
+    {
+        "networkInterfaceId": str,
+        "subnetId": str,
+        "vpcId": str,
+        "privateDnsName": str,
+        "privateIpAddress": str,
+        "privateIpAddresses": List[PrivateIpTypeDef],
+        "publicDnsName": str,
+        "publicIp": str,
+        "ipv6Addresses": List[str],
+        "securityGroups": List[SecurityGroupTypeDef],
+    },
+    total=False,
+)
+
+DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
+    "DescribeAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplates": List[AssessmentTemplateTypeDef],
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     {
         "assessmentTargetArns": Sequence[str],
         "filter": AssessmentTemplateFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestRequestTypeDef",
     {
@@ -1405,15 +1419,15 @@
 )
 
 ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
         "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAssessmentRunsRequestRequestTypeDef = TypedDict(
     "ListAssessmentRunsRequestRequestTypeDef",
     {
@@ -1426,15 +1440,15 @@
 )
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "assessmentRunArns": Sequence[str],
         "filter": FindingFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -1447,52 +1461,52 @@
 )
 
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
-    "DescribeAssessmentTemplatesResponseTypeDef",
+DescribeResourceGroupsResponseTypeDef = TypedDict(
+    "DescribeResourceGroupsResponseTypeDef",
     {
-        "assessmentTemplates": List[AssessmentTemplateTypeDef],
+        "resourceGroups": List[ResourceGroupTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
     {
         "subscriptions": List[SubscriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExclusionsPreviewResponseTypeDef = TypedDict(
     "GetExclusionsPreviewResponseTypeDef",
     {
         "previewStatus": PreviewStatusType,
         "exclusionPreviews": List[ExclusionPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExclusionsResponseTypeDef = TypedDict(
     "DescribeExclusionsResponseTypeDef",
     {
         "exclusions": Dict[str, ExclusionTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetAttributesTypeDef = TypedDict(
     "_RequiredAssetAttributesTypeDef",
     {
         "schemaVersion": int,
@@ -1502,38 +1516,31 @@
     "_OptionalAssetAttributesTypeDef",
     {
         "agentId": str,
         "autoScalingGroup": str,
         "amiId": str,
         "hostname": str,
         "ipv4Addresses": List[str],
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
+
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
-DescribeResourceGroupsResponseTypeDef = TypedDict(
-    "DescribeResourceGroupsResponseTypeDef",
-    {
-        "resourceGroups": List[ResourceGroupTypeDef],
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
-        "attributes": List[AttributeOutputTypeDef],
-        "userAttributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "userAttributes": List[AttributeTypeDef],
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalFindingTypeDef = TypedDict(
     "_OptionalFindingTypeDef",
     {
@@ -1550,18 +1557,20 @@
         "numericSeverity": float,
         "confidence": int,
         "indicatorOfCompromise": bool,
     },
     total=False,
 )
 
+
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
+
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/PKG-INFO` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.28.12
-Summary: Type annotations for boto3.Inspector 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Inspector 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,121 +373,118 @@
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
+    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
-    AttributeOutputTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
-    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
-    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
-    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
-    ResourceGroupTagOutputTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
-    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
+    AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
+    CreateResourceGroupResponseTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssessmentReportResponseTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
-    AssessmentTemplateTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
+    ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
-    ResourceGroupTypeDef,
-    SetTagsForResourceRequestRequestTypeDef,
+    DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
-    DescribeAssessmentTemplatesResponseTypeDef,
+    DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
-    DescribeResourceGroupsResponseTypeDef,
     FindingTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/SOURCES.txt` & `mypy-boto3-inspector-1.28.15/mypy_boto3_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.12/setup.py` & `mypy-boto3-inspector-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_inspector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Inspector 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

