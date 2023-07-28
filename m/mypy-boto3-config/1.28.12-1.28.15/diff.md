# Comparing `tmp/mypy-boto3-config-1.28.12.tar.gz` & `tmp/mypy-boto3-config-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-config-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
+gzip compressed data, was "mypy-boto3-config-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-config-1.28.12.tar` & `mypy-boto3-config-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.368543 mypy-boto3-config-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37783 2023-07-27 05:34:31.360543 mypy-boto3-config-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36293 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.356543 mypy-boto3-config-1.28.12/mypy_boto3_config/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88855 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88725 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42993 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    42960 2023-07-27 05:19:33.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   141473 2023-07-27 05:19:36.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   141296 2023-07-27 05:19:35.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/mypy_boto3_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.360543 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37783 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:31.000000 mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.368543 mypy-boto3-config-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:19:32.000000 mypy-boto3-config-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.600911 mypy-boto3-config-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37108 2023-07-28 20:42:34.596912 mypy-boto3-config-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.596912 mypy-boto3-config-1.28.15/mypy_boto3_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88855 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88725 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-07-28 20:22:11.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-28 20:22:11.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42907 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-07-28 20:22:10.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   135358 2023-07-28 20:22:15.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135191 2023-07-28 20:22:13.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/mypy_boto3_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.596912 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37108 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:34.000000 mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.600911 mypy-boto3-config-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:22:09.000000 mypy-boto3-config-1.28.15/setup.py
```

### Comparing `mypy-boto3-config-1.28.12/LICENSE` & `mypy-boto3-config-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/PKG-INFO` & `mypy-boto3-config-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-config
-Version: 1.28.12
-Summary: Type annotations for boto3.ConfigService 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 config type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-config"></a>
 
 # mypy-boto3-config
 
 [![PyPI - mypy-boto3-config](https://img.shields.io/pypi/v/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -512,47 +480,42 @@
 from mypy_boto3_config.type_defs import (
     AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
-    AggregateResourceIdentifierOutputTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
+    ResponseMetadataTypeDef,
     ResourceKeyTypeDef,
-    ResourceKeyOutputTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
-    EvaluationModeConfigurationOutputTypeDef,
-    ScopeOutputTypeDef,
     EvaluationModeConfigurationTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
-    ConfigSnapshotDeliveryPropertiesOutputTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
     OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
-    ConformancePackInputParameterOutputTypeDef,
-    TemplateSSMDocumentDetailsOutputTypeDef,
-    ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
+    TemplateSSMDocumentDetailsTypeDef,
+    ConformancePackEvaluationFiltersTypeDef,
     ConformancePackRuleComplianceTypeDef,
     ConformancePackStatusDetailTypeDef,
-    CustomPolicyDetailsOutputTypeDef,
     CustomPolicyDetailsTypeDef,
     DeleteAggregationAuthorizationRequestRequestTypeDef,
     DeleteConfigRuleRequestRequestTypeDef,
     DeleteConfigurationAggregatorRequestRequestTypeDef,
     DeleteConfigurationRecorderRequestRequestTypeDef,
     DeleteConformancePackRequestRequestTypeDef,
     DeleteDeliveryChannelRequestRequestTypeDef,
@@ -562,233 +525,220 @@
     DeletePendingAggregationRequestRequestRequestTypeDef,
     DeleteRemediationConfigurationRequestRequestTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     DeleteResourceConfigRequestRequestTypeDef,
     DeleteRetentionConfigurationRequestRequestTypeDef,
     DeleteStoredQueryRequestRequestTypeDef,
     DeliverConfigSnapshotRequestRequestTypeDef,
-    DeliverConfigSnapshotResponseTypeDef,
-    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAggregationAuthorizationsRequestRequestTypeDef,
-    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByConfigRuleRequestRequestTypeDef,
-    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeComplianceByResourceRequestRequestTypeDef,
-    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestRequestTypeDef,
     DescribeConfigRulesFiltersTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
-    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
     DescribeConfigurationAggregatorsRequestRequestTypeDef,
     DescribeConfigurationRecorderStatusRequestRequestTypeDef,
     DescribeConfigurationRecordersRequestRequestTypeDef,
-    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
     DescribeConformancePackStatusRequestRequestTypeDef,
-    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
     DescribeConformancePacksRequestRequestTypeDef,
     DescribeDeliveryChannelStatusRequestRequestTypeDef,
     DescribeDeliveryChannelsRequestRequestTypeDef,
-    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
     DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef,
     OrganizationConfigRuleStatusTypeDef,
-    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
     DescribeOrganizationConfigRulesRequestRequestTypeDef,
-    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
     DescribeOrganizationConformancePackStatusesRequestRequestTypeDef,
     OrganizationConformancePackStatusTypeDef,
-    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
     DescribeOrganizationConformancePacksRequestRequestTypeDef,
-    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribePendingAggregationRequestsRequestRequestTypeDef,
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
-    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluationContextOutputTypeDef,
     EvaluationContextTypeDef,
     EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
     EvaluationTypeDef,
     ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
-    SsmControlsOutputTypeDef,
     SsmControlsTypeDef,
     ExternalEvaluationTypeDef,
-    RemediationExceptionResourceKeyOutputTypeDef,
     FieldInfoTypeDef,
-    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
-    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
-    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
-    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     GetConformancePackComplianceSummaryRequestRequestTypeDef,
     GetCustomRulePolicyRequestRequestTypeDef,
-    GetCustomRulePolicyResponseTypeDef,
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetOrganizationCustomRulePolicyResponseTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
-    ResourceDetailsOutputTypeDef,
+    ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
-    StoredQueryOutputTypeDef,
+    StoredQueryTypeDef,
     ResourceFiltersTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     OrganizationCustomRuleMetadataOutputTypeDef,
     OrganizationManagedRuleMetadataOutputTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    TagTypeDef,
-    TemplateSSMDocumentDetailsTypeDef,
-    PutConformancePackResponseTypeDef,
-    PutOrganizationConfigRuleResponseTypeDef,
-    PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
-    StoredQueryTypeDef,
-    PutStoredQueryResponseTypeDef,
-    RecordingStrategyOutputTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
-    ResourceValueOutputTypeDef,
-    StaticValueOutputTypeDef,
     ResourceValueTypeDef,
+    StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    ResourceDetailsTypeDef,
     TimeWindowTypeDef,
-    ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
-    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
-    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-    SourceDetailOutputTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
-    StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
-    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    BatchGetAggregateResourceConfigResponseTypeDef,
+    DeliverConfigSnapshotResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCustomRulePolicyResponseTypeDef,
+    GetOrganizationCustomRulePolicyResponseTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
-    BatchGetAggregateResourceConfigResponseTypeDef,
+    PutConformancePackResponseTypeDef,
+    PutOrganizationConfigRuleResponseTypeDef,
+    PutOrganizationConformancePackResponseTypeDef,
+    PutStoredQueryResponseTypeDef,
+    StartResourceEvaluationResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
-    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    BatchGetResourceConfigResponseTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
-    BatchGetResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
-    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
-    DeliveryChannelOutputTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
     DescribeConfigurationRecorderStatusResponseTypeDef,
     DescribeConformancePackComplianceRequestRequestTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListConformancePackComplianceScoresRequestRequestTypeDef,
     GetConformancePackComplianceSummaryResponseTypeDef,
     OrganizationConformancePackTypeDef,
+    PutOrganizationConformancePackRequestRequestTypeDef,
     ConformancePackDetailTypeDef,
+    PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
-    PutOrganizationConformancePackRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
+    FailedDeleteRemediationExceptionsBatchTypeDef,
     PutRemediationExceptionsRequestRequestTypeDef,
+    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
+    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
+    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
+    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
+    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
+    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
+    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
+    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
+    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
+    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
+    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
+    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
+    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
     PutEvaluationsRequestRequestTypeDef,
-    ExecutionControlsOutputTypeDef,
     ExecutionControlsTypeDef,
     PutExternalEvaluationRequestRequestTypeDef,
-    FailedDeleteRemediationExceptionsBatchTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     GetOrganizationConformancePackDetailedStatusResponseTypeDef,
     GetResourceEvaluationSummaryResponseTypeDef,
+    StartResourceEvaluationRequestRequestTypeDef,
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationConfigRuleTypeDef,
-    PutOrganizationConfigRuleRequestRequestTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    PutConformancePackRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
+    OrganizationConfigRuleTypeDef,
+    PutOrganizationConfigRuleRequestRequestTypeDef,
     RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
     RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    StartResourceEvaluationRequestRequestTypeDef,
     ResourceEvaluationFiltersTypeDef,
     SourceOutputTypeDef,
     SourceTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
@@ -801,19 +751,19 @@
     DescribeDeliveryChannelStatusResponseTypeDef,
     DescribeConfigurationAggregatorsResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetResourceConfigHistoryResponseTypeDef,
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
+    DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
-    DeleteRemediationExceptionsResponseTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
     ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     RemediationConfigurationOutputTypeDef,
```

### Comparing `mypy-boto3-config-1.28.12/README.md` & `mypy-boto3-config-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-config
+Version: 1.28.15
+Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 config type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-config"></a>
 
 # mypy-boto3-config
 
 [![PyPI - mypy-boto3-config](https://img.shields.io/pypi/v/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -480,47 +512,42 @@
 from mypy_boto3_config.type_defs import (
     AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
-    AggregateResourceIdentifierOutputTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
+    ResponseMetadataTypeDef,
     ResourceKeyTypeDef,
-    ResourceKeyOutputTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
-    EvaluationModeConfigurationOutputTypeDef,
-    ScopeOutputTypeDef,
     EvaluationModeConfigurationTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
-    ConfigSnapshotDeliveryPropertiesOutputTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
     OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
-    ConformancePackInputParameterOutputTypeDef,
-    TemplateSSMDocumentDetailsOutputTypeDef,
-    ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
+    TemplateSSMDocumentDetailsTypeDef,
+    ConformancePackEvaluationFiltersTypeDef,
     ConformancePackRuleComplianceTypeDef,
     ConformancePackStatusDetailTypeDef,
-    CustomPolicyDetailsOutputTypeDef,
     CustomPolicyDetailsTypeDef,
     DeleteAggregationAuthorizationRequestRequestTypeDef,
     DeleteConfigRuleRequestRequestTypeDef,
     DeleteConfigurationAggregatorRequestRequestTypeDef,
     DeleteConfigurationRecorderRequestRequestTypeDef,
     DeleteConformancePackRequestRequestTypeDef,
     DeleteDeliveryChannelRequestRequestTypeDef,
@@ -530,233 +557,220 @@
     DeletePendingAggregationRequestRequestRequestTypeDef,
     DeleteRemediationConfigurationRequestRequestTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     DeleteResourceConfigRequestRequestTypeDef,
     DeleteRetentionConfigurationRequestRequestTypeDef,
     DeleteStoredQueryRequestRequestTypeDef,
     DeliverConfigSnapshotRequestRequestTypeDef,
-    DeliverConfigSnapshotResponseTypeDef,
-    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAggregationAuthorizationsRequestRequestTypeDef,
-    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByConfigRuleRequestRequestTypeDef,
-    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeComplianceByResourceRequestRequestTypeDef,
-    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestRequestTypeDef,
     DescribeConfigRulesFiltersTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
-    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
     DescribeConfigurationAggregatorsRequestRequestTypeDef,
     DescribeConfigurationRecorderStatusRequestRequestTypeDef,
     DescribeConfigurationRecordersRequestRequestTypeDef,
-    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
     DescribeConformancePackStatusRequestRequestTypeDef,
-    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
     DescribeConformancePacksRequestRequestTypeDef,
     DescribeDeliveryChannelStatusRequestRequestTypeDef,
     DescribeDeliveryChannelsRequestRequestTypeDef,
-    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
     DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef,
     OrganizationConfigRuleStatusTypeDef,
-    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
     DescribeOrganizationConfigRulesRequestRequestTypeDef,
-    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
     DescribeOrganizationConformancePackStatusesRequestRequestTypeDef,
     OrganizationConformancePackStatusTypeDef,
-    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
     DescribeOrganizationConformancePacksRequestRequestTypeDef,
-    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribePendingAggregationRequestsRequestRequestTypeDef,
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
-    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluationContextOutputTypeDef,
     EvaluationContextTypeDef,
     EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
     EvaluationTypeDef,
     ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
-    SsmControlsOutputTypeDef,
     SsmControlsTypeDef,
     ExternalEvaluationTypeDef,
-    RemediationExceptionResourceKeyOutputTypeDef,
     FieldInfoTypeDef,
-    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
-    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
-    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
-    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     GetConformancePackComplianceSummaryRequestRequestTypeDef,
     GetCustomRulePolicyRequestRequestTypeDef,
-    GetCustomRulePolicyResponseTypeDef,
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetOrganizationCustomRulePolicyResponseTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
-    ResourceDetailsOutputTypeDef,
+    ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
-    StoredQueryOutputTypeDef,
+    StoredQueryTypeDef,
     ResourceFiltersTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     OrganizationCustomRuleMetadataOutputTypeDef,
     OrganizationManagedRuleMetadataOutputTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    TagTypeDef,
-    TemplateSSMDocumentDetailsTypeDef,
-    PutConformancePackResponseTypeDef,
-    PutOrganizationConfigRuleResponseTypeDef,
-    PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
-    StoredQueryTypeDef,
-    PutStoredQueryResponseTypeDef,
-    RecordingStrategyOutputTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
-    ResourceValueOutputTypeDef,
-    StaticValueOutputTypeDef,
     ResourceValueTypeDef,
+    StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    ResourceDetailsTypeDef,
     TimeWindowTypeDef,
-    ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
-    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
-    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-    SourceDetailOutputTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
-    StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
-    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    BatchGetAggregateResourceConfigResponseTypeDef,
+    DeliverConfigSnapshotResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCustomRulePolicyResponseTypeDef,
+    GetOrganizationCustomRulePolicyResponseTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
-    BatchGetAggregateResourceConfigResponseTypeDef,
+    PutConformancePackResponseTypeDef,
+    PutOrganizationConfigRuleResponseTypeDef,
+    PutOrganizationConformancePackResponseTypeDef,
+    PutStoredQueryResponseTypeDef,
+    StartResourceEvaluationResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
-    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    BatchGetResourceConfigResponseTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
-    BatchGetResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
-    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
-    DeliveryChannelOutputTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
     DescribeConfigurationRecorderStatusResponseTypeDef,
     DescribeConformancePackComplianceRequestRequestTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListConformancePackComplianceScoresRequestRequestTypeDef,
     GetConformancePackComplianceSummaryResponseTypeDef,
     OrganizationConformancePackTypeDef,
+    PutOrganizationConformancePackRequestRequestTypeDef,
     ConformancePackDetailTypeDef,
+    PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
-    PutOrganizationConformancePackRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
+    FailedDeleteRemediationExceptionsBatchTypeDef,
     PutRemediationExceptionsRequestRequestTypeDef,
+    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
+    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
+    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
+    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
+    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
+    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
+    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
+    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
+    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
+    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
+    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
+    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
+    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
     PutEvaluationsRequestRequestTypeDef,
-    ExecutionControlsOutputTypeDef,
     ExecutionControlsTypeDef,
     PutExternalEvaluationRequestRequestTypeDef,
-    FailedDeleteRemediationExceptionsBatchTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     GetOrganizationConformancePackDetailedStatusResponseTypeDef,
     GetResourceEvaluationSummaryResponseTypeDef,
+    StartResourceEvaluationRequestRequestTypeDef,
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationConfigRuleTypeDef,
-    PutOrganizationConfigRuleRequestRequestTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    PutConformancePackRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
+    OrganizationConfigRuleTypeDef,
+    PutOrganizationConfigRuleRequestRequestTypeDef,
     RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
     RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    StartResourceEvaluationRequestRequestTypeDef,
     ResourceEvaluationFiltersTypeDef,
     SourceOutputTypeDef,
     SourceTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
@@ -769,19 +783,19 @@
     DescribeDeliveryChannelStatusResponseTypeDef,
     DescribeConfigurationAggregatorsResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetResourceConfigHistoryResponseTypeDef,
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
+    DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
-    DeleteRemediationExceptionsResponseTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
     ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     RemediationConfigurationOutputTypeDef,
```

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.py` & `mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/__init__.pyi` & `mypy-boto3-config-1.28.15/mypy_boto3_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/__main__.py` & `mypy-boto3-config-1.28.15/mypy_boto3_config/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConfigService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ConfigService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/client.py` & `mypy-boto3-config-1.28.15/mypy_boto3_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/client.pyi` & `mypy-boto3-config-1.28.15/mypy_boto3_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/literals.py` & `mypy-boto3-config-1.28.15/mypy_boto3_config/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/literals.pyi` & `mypy-boto3-config-1.28.15/mypy_boto3_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.py` & `mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregatecompliancebyconfigrulespaginator)
         """
 
 
@@ -204,30 +204,30 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregatecompliancebyconformancepackspaginator)
         """
 
 
 class DescribeAggregationAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregationauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAggregationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregationauthorizationspaginator)
         """
 
 
@@ -238,15 +238,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeComplianceByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByConfigRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describecompliancebyconfigrulepaginator)
         """
 
 
@@ -258,15 +258,15 @@
 
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeComplianceByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describecompliancebyresourcepaginator)
         """
 
 
@@ -276,15 +276,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigruleevaluationstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigruleevaluationstatuspaginator)
         """
 
 
@@ -295,15 +295,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         Filters: DescribeConfigRulesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigrulespaginator)
         """
 
 
@@ -314,15 +314,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigurationaggregatorsourcesstatuspaginator)
         """
 
 
@@ -332,15 +332,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigurationaggregatorspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigurationAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigurationaggregatorspaginator)
         """
 
 
@@ -350,15 +350,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConformancePackStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePackStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackstatuspaginator)
         """
 
 
@@ -368,15 +368,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackspaginator)
         """
 
 
@@ -386,15 +386,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulestatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulestatusespaginator)
         """
 
 
@@ -404,15 +404,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulespaginator)
         """
 
 
@@ -422,15 +422,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackstatusespaginator)
         """
 
 
@@ -440,30 +440,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackspaginator)
         """
 
 
 class DescribePendingAggregationRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describependingaggregationrequestspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePendingAggregationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describependingaggregationrequestspaginator)
         """
 
 
@@ -474,15 +474,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRemediationExecutionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRemediationExecutionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeremediationexecutionstatuspaginator)
         """
 
 
@@ -492,15 +492,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeretentionconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         RetentionConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRetentionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRetentionConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeretentionconfigurationspaginator)
         """
 
 
@@ -514,15 +514,15 @@
         self,
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getaggregatecompliancedetailsbyconfigrulepaginator)
         """
 
 
@@ -533,15 +533,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getcompliancedetailsbyconfigrulepaginator)
         """
 
 
@@ -554,33 +554,30 @@
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         ResourceEvaluationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetComplianceDetailsByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getcompliancedetailsbyresourcepaginator)
         """
 
 
 class GetConformancePackComplianceSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getconformancepackcompliancesummarypaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ConformancePackNames: Sequence[str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ConformancePackNames: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetConformancePackComplianceSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getconformancepackcompliancesummarypaginator)
         """
 
 
@@ -591,15 +588,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getorganizationconfigruledetailedstatuspaginator)
         """
 
 
@@ -610,15 +607,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getorganizationconformancepackdetailedstatuspaginator)
         """
 
 
@@ -632,15 +629,15 @@
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
         laterTime: Union[datetime, str] = ...,
         earlierTime: Union[datetime, str] = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getresourceconfighistorypaginator)
         """
 
 
@@ -652,15 +649,15 @@
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListAggregateDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listaggregatediscoveredresourcespaginator)
         """
 
 
@@ -673,15 +670,15 @@
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         includeDeletedResources: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listdiscoveredresourcespaginator)
         """
 
 
@@ -691,30 +688,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listresourceevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListResourceEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listresourceevaluationspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listtagsforresourcepaginator)
         """
 
 
@@ -726,28 +723,28 @@
 
     def paginate(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SelectAggregateResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectAggregateResourceConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#selectaggregateresourceconfigpaginator)
         """
 
 
 class SelectResourceConfigPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#selectresourceconfigpaginator)
     """
 
     def paginate(
-        self, *, Expression: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Expression: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SelectResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#selectresourceconfigpaginator)
         """
```

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/paginator.pyi` & `mypy-boto3-config-1.28.15/mypy_boto3_config/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregatecompliancebyconfigrulespaginator)
         """
 
 class DescribeAggregateComplianceByConformancePacksPaginator(Paginator):
@@ -200,29 +200,29 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregatecompliancebyconformancepackspaginator)
         """
 
 class DescribeAggregationAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregationauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAggregationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeaggregationauthorizationspaginator)
         """
 
 class DescribeComplianceByConfigRulePaginator(Paginator):
@@ -232,15 +232,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeComplianceByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByConfigRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describecompliancebyconfigrulepaginator)
         """
 
 class DescribeComplianceByResourcePaginator(Paginator):
@@ -251,15 +251,15 @@
 
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeComplianceByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describecompliancebyresourcepaginator)
         """
 
 class DescribeConfigRuleEvaluationStatusPaginator(Paginator):
@@ -268,15 +268,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigruleevaluationstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigruleevaluationstatuspaginator)
         """
 
 class DescribeConfigRulesPaginator(Paginator):
@@ -286,15 +286,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         Filters: DescribeConfigRulesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigrulespaginator)
         """
 
 class DescribeConfigurationAggregatorSourcesStatusPaginator(Paginator):
@@ -304,15 +304,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigurationaggregatorsourcesstatuspaginator)
         """
 
 class DescribeConfigurationAggregatorsPaginator(Paginator):
@@ -321,15 +321,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigurationaggregatorspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConfigurationAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconfigurationaggregatorspaginator)
         """
 
 class DescribeConformancePackStatusPaginator(Paginator):
@@ -338,15 +338,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConformancePackStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePackStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackstatuspaginator)
         """
 
 class DescribeConformancePacksPaginator(Paginator):
@@ -355,15 +355,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeconformancepackspaginator)
         """
 
 class DescribeOrganizationConfigRuleStatusesPaginator(Paginator):
@@ -372,15 +372,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulestatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulestatusespaginator)
         """
 
 class DescribeOrganizationConfigRulesPaginator(Paginator):
@@ -389,15 +389,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconfigrulespaginator)
         """
 
 class DescribeOrganizationConformancePackStatusesPaginator(Paginator):
@@ -406,15 +406,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackstatusespaginator)
         """
 
 class DescribeOrganizationConformancePacksPaginator(Paginator):
@@ -423,29 +423,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeOrganizationConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeorganizationconformancepackspaginator)
         """
 
 class DescribePendingAggregationRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describependingaggregationrequestspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePendingAggregationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describependingaggregationrequestspaginator)
         """
 
 class DescribeRemediationExecutionStatusPaginator(Paginator):
@@ -455,15 +455,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRemediationExecutionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRemediationExecutionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeremediationexecutionstatuspaginator)
         """
 
 class DescribeRetentionConfigurationsPaginator(Paginator):
@@ -472,15 +472,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeretentionconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         RetentionConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRetentionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRetentionConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#describeretentionconfigurationspaginator)
         """
 
 class GetAggregateComplianceDetailsByConfigRulePaginator(Paginator):
@@ -493,15 +493,15 @@
         self,
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getaggregatecompliancedetailsbyconfigrulepaginator)
         """
 
 class GetComplianceDetailsByConfigRulePaginator(Paginator):
@@ -511,15 +511,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getcompliancedetailsbyconfigrulepaginator)
         """
 
 class GetComplianceDetailsByResourcePaginator(Paginator):
@@ -531,32 +531,29 @@
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         ResourceEvaluationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetComplianceDetailsByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getcompliancedetailsbyresourcepaginator)
         """
 
 class GetConformancePackComplianceSummaryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getconformancepackcompliancesummarypaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ConformancePackNames: Sequence[str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ConformancePackNames: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetConformancePackComplianceSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getconformancepackcompliancesummarypaginator)
         """
 
 class GetOrganizationConfigRuleDetailedStatusPaginator(Paginator):
@@ -566,15 +563,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getorganizationconfigruledetailedstatuspaginator)
         """
 
 class GetOrganizationConformancePackDetailedStatusPaginator(Paginator):
@@ -584,15 +581,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getorganizationconformancepackdetailedstatuspaginator)
         """
 
 class GetResourceConfigHistoryPaginator(Paginator):
@@ -605,15 +602,15 @@
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
         laterTime: Union[datetime, str] = ...,
         earlierTime: Union[datetime, str] = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#getresourceconfighistorypaginator)
         """
 
 class ListAggregateDiscoveredResourcesPaginator(Paginator):
@@ -624,15 +621,15 @@
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListAggregateDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listaggregatediscoveredresourcespaginator)
         """
 
 class ListDiscoveredResourcesPaginator(Paginator):
@@ -644,15 +641,15 @@
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         includeDeletedResources: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listdiscoveredresourcespaginator)
         """
 
 class ListResourceEvaluationsPaginator(Paginator):
@@ -661,29 +658,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listresourceevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListResourceEvaluations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listresourceevaluationspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#listtagsforresourcepaginator)
         """
 
 class SelectAggregateResourceConfigPaginator(Paginator):
@@ -694,27 +691,27 @@
 
     def paginate(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SelectAggregateResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectAggregateResourceConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#selectaggregateresourceconfigpaginator)
         """
 
 class SelectResourceConfigPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#selectresourceconfigpaginator)
     """
 
     def paginate(
-        self, *, Expression: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Expression: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SelectResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/paginators/#selectresourceconfigpaginator)
         """
```

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.py` & `mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,47 +60,42 @@
 __all__ = (
     "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
-    "AggregateResourceIdentifierOutputTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
     "AggregationAuthorizationTypeDef",
     "BaseConfigurationItemTypeDef",
+    "ResponseMetadataTypeDef",
     "ResourceKeyTypeDef",
-    "ResourceKeyOutputTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
-    "EvaluationModeConfigurationOutputTypeDef",
-    "ScopeOutputTypeDef",
     "EvaluationModeConfigurationTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
-    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
     "OrganizationAggregationSourceOutputTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
-    "ConformancePackInputParameterOutputTypeDef",
-    "TemplateSSMDocumentDetailsOutputTypeDef",
-    "ConformancePackEvaluationFiltersTypeDef",
     "ConformancePackInputParameterTypeDef",
+    "TemplateSSMDocumentDetailsTypeDef",
+    "ConformancePackEvaluationFiltersTypeDef",
     "ConformancePackRuleComplianceTypeDef",
     "ConformancePackStatusDetailTypeDef",
-    "CustomPolicyDetailsOutputTypeDef",
     "CustomPolicyDetailsTypeDef",
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     "DeleteConfigRuleRequestRequestTypeDef",
     "DeleteConfigurationAggregatorRequestRequestTypeDef",
     "DeleteConfigurationRecorderRequestRequestTypeDef",
     "DeleteConformancePackRequestRequestTypeDef",
     "DeleteDeliveryChannelRequestRequestTypeDef",
@@ -110,233 +105,220 @@
     "DeletePendingAggregationRequestRequestRequestTypeDef",
     "DeleteRemediationConfigurationRequestRequestTypeDef",
     "RemediationExceptionResourceKeyTypeDef",
     "DeleteResourceConfigRequestRequestTypeDef",
     "DeleteRetentionConfigurationRequestRequestTypeDef",
     "DeleteStoredQueryRequestRequestTypeDef",
     "DeliverConfigSnapshotRequestRequestTypeDef",
-    "DeliverConfigSnapshotResponseTypeDef",
-    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
     "DescribeComplianceByResourceRequestRequestTypeDef",
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     "DescribeConfigRulesFiltersTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     "DescribeConfigurationRecorderStatusRequestRequestTypeDef",
     "DescribeConfigurationRecordersRequestRequestTypeDef",
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
     "DescribeConformancePackStatusRequestRequestTypeDef",
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
     "DescribeConformancePacksRequestRequestTypeDef",
     "DescribeDeliveryChannelStatusRequestRequestTypeDef",
     "DescribeDeliveryChannelsRequestRequestTypeDef",
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     "OrganizationConfigRuleStatusTypeDef",
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     "OrganizationConformancePackStatusTypeDef",
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EvaluationContextOutputTypeDef",
     "EvaluationContextTypeDef",
     "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
     "EvaluationTypeDef",
     "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
-    "SsmControlsOutputTypeDef",
     "SsmControlsTypeDef",
     "ExternalEvaluationTypeDef",
-    "RemediationExceptionResourceKeyOutputTypeDef",
     "FieldInfoTypeDef",
-    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
-    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
-    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     "GetConformancePackComplianceSummaryRequestRequestTypeDef",
     "GetCustomRulePolicyRequestRequestTypeDef",
-    "GetCustomRulePolicyResponseTypeDef",
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     "ResourceCountTypeDef",
     "StatusDetailFiltersTypeDef",
     "MemberAccountStatusTypeDef",
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
-    "ResourceDetailsOutputTypeDef",
+    "ResourceDetailsTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
-    "StoredQueryOutputTypeDef",
+    "StoredQueryTypeDef",
     "ResourceFiltersTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     "OrganizationCustomRuleMetadataOutputTypeDef",
     "OrganizationManagedRuleMetadataOutputTypeDef",
     "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
-    "PaginatorConfigTypeDef",
-    "TagTypeDef",
-    "TemplateSSMDocumentDetailsTypeDef",
-    "PutConformancePackResponseTypeDef",
-    "PutOrganizationConfigRuleResponseTypeDef",
-    "PutOrganizationConformancePackResponseTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
-    "StoredQueryTypeDef",
-    "PutStoredQueryResponseTypeDef",
-    "RecordingStrategyOutputTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
-    "ResourceValueOutputTypeDef",
-    "StaticValueOutputTypeDef",
     "ResourceValueTypeDef",
+    "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
-    "ResourceDetailsTypeDef",
     "TimeWindowTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
-    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
-    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    "SourceDetailOutputTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
-    "StartResourceEvaluationResponseTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
-    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "DeliverConfigSnapshotResponseTypeDef",
     "DescribeAggregationAuthorizationsResponseTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCustomRulePolicyResponseTypeDef",
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "PutAggregationAuthorizationResponseTypeDef",
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "PutConformancePackResponseTypeDef",
+    "PutOrganizationConfigRuleResponseTypeDef",
+    "PutOrganizationConformancePackResponseTypeDef",
+    "PutStoredQueryResponseTypeDef",
+    "StartResourceEvaluationResponseTypeDef",
     "BatchGetResourceConfigRequestRequestTypeDef",
-    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    "BatchGetResourceConfigResponseTypeDef",
     "DescribeRemediationExecutionStatusRequestRequestTypeDef",
     "StartRemediationExecutionRequestRequestTypeDef",
-    "BatchGetResourceConfigResponseTypeDef",
     "StartRemediationExecutionResponseTypeDef",
     "ComplianceSummaryTypeDef",
     "ComplianceTypeDef",
-    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     "GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
-    "DeliveryChannelOutputTypeDef",
     "DeliveryChannelTypeDef",
     "DeliveryChannelStatusTypeDef",
     "ConfigurationAggregatorTypeDef",
     "ConfigurationItemTypeDef",
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     "DescribeConformancePackComplianceRequestRequestTypeDef",
     "ListConformancePackComplianceScoresResponseTypeDef",
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     "GetConformancePackComplianceSummaryResponseTypeDef",
     "OrganizationConformancePackTypeDef",
+    "PutOrganizationConformancePackRequestRequestTypeDef",
     "ConformancePackDetailTypeDef",
+    "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
-    "PutOrganizationConformancePackRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "PutRemediationExceptionsRequestRequestTypeDef",
+    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
     "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
     "PutEvaluationsRequestRequestTypeDef",
-    "ExecutionControlsOutputTypeDef",
     "ExecutionControlsTypeDef",
     "PutExternalEvaluationRequestRequestTypeDef",
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     "GetResourceEvaluationSummaryResponseTypeDef",
+    "StartResourceEvaluationRequestRequestTypeDef",
     "GetStoredQueryResponseTypeDef",
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "OrganizationConfigRuleTypeDef",
-    "PutOrganizationConfigRuleRequestRequestTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "PutConformancePackRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
+    "OrganizationConfigRuleTypeDef",
+    "PutOrganizationConfigRuleRequestRequestTypeDef",
     "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
     "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "StartResourceEvaluationRequestRequestTypeDef",
     "ResourceEvaluationFiltersTypeDef",
     "SourceOutputTypeDef",
     "SourceTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
@@ -349,19 +331,19 @@
     "DescribeDeliveryChannelStatusResponseTypeDef",
     "DescribeConfigurationAggregatorsResponseTypeDef",
     "PutConfigurationAggregatorResponseTypeDef",
     "GetAggregateResourceConfigResponseTypeDef",
     "GetResourceConfigHistoryResponseTypeDef",
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
+    "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
-    "DeleteRemediationExceptionsResponseTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
     "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
     "RemediationConfigurationOutputTypeDef",
@@ -469,39 +451,14 @@
     {
         "AccountId": str,
         "AwsRegion": str,
     },
     total=False,
 )
 
-_RequiredAggregateResourceIdentifierOutputTypeDef = TypedDict(
-    "_RequiredAggregateResourceIdentifierOutputTypeDef",
-    {
-        "SourceAccountId": str,
-        "SourceRegion": str,
-        "ResourceId": str,
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalAggregateResourceIdentifierOutputTypeDef = TypedDict(
-    "_OptionalAggregateResourceIdentifierOutputTypeDef",
-    {
-        "ResourceName": str,
-    },
-    total=False,
-)
-
-
-class AggregateResourceIdentifierOutputTypeDef(
-    _RequiredAggregateResourceIdentifierOutputTypeDef,
-    _OptionalAggregateResourceIdentifierOutputTypeDef,
-):
-    pass
-
-
 _RequiredAggregateResourceIdentifierTypeDef = TypedDict(
     "_RequiredAggregateResourceIdentifierTypeDef",
     {
         "SourceAccountId": str,
         "SourceRegion": str,
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
@@ -564,24 +521,27 @@
         "resourceCreationTime": datetime,
         "configuration": str,
         "supplementaryConfiguration": Dict[str, str],
     },
     total=False,
 )
 
-ResourceKeyTypeDef = TypedDict(
-    "ResourceKeyTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ResourceKeyOutputTypeDef = TypedDict(
-    "ResourceKeyOutputTypeDef",
+ResourceKeyTypeDef = TypedDict(
+    "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
 
 ComplianceContributorCountTypeDef = TypedDict(
@@ -644,16 +604,16 @@
         "LastDebugLogDeliveryStatus": str,
         "LastDebugLogDeliveryStatusReason": str,
         "LastDebugLogDeliveryTime": datetime,
     },
     total=False,
 )
 
-EvaluationModeConfigurationOutputTypeDef = TypedDict(
-    "EvaluationModeConfigurationOutputTypeDef",
+EvaluationModeConfigurationTypeDef = TypedDict(
+    "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
 ScopeOutputTypeDef = TypedDict(
@@ -663,41 +623,25 @@
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
-EvaluationModeConfigurationTypeDef = TypedDict(
-    "EvaluationModeConfigurationTypeDef",
-    {
-        "Mode": EvaluationModeType,
-    },
-    total=False,
-)
-
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "ComplianceResourceTypes": Sequence[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
-ConfigSnapshotDeliveryPropertiesOutputTypeDef = TypedDict(
-    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
-    {
-        "deliveryFrequency": MaximumExecutionFrequencyType,
-    },
-    total=False,
-)
-
 ConfigSnapshotDeliveryPropertiesTypeDef = TypedDict(
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     {
         "deliveryFrequency": MaximumExecutionFrequencyType,
     },
     total=False,
 )
@@ -792,40 +736,39 @@
     "ConformancePackComplianceSummaryTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackComplianceStatus": ConformancePackComplianceTypeType,
     },
 )
 
-ConformancePackInputParameterOutputTypeDef = TypedDict(
-    "ConformancePackInputParameterOutputTypeDef",
+ConformancePackInputParameterTypeDef = TypedDict(
+    "ConformancePackInputParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
 )
 
-_RequiredTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
-    "_RequiredTemplateSSMDocumentDetailsOutputTypeDef",
+_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_RequiredTemplateSSMDocumentDetailsTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
-    "_OptionalTemplateSSMDocumentDetailsOutputTypeDef",
+_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_OptionalTemplateSSMDocumentDetailsTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
 
-class TemplateSSMDocumentDetailsOutputTypeDef(
-    _RequiredTemplateSSMDocumentDetailsOutputTypeDef,
-    _OptionalTemplateSSMDocumentDetailsOutputTypeDef,
+class TemplateSSMDocumentDetailsTypeDef(
+    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
 ):
     pass
 
 
 ConformancePackEvaluationFiltersTypeDef = TypedDict(
     "ConformancePackEvaluationFiltersTypeDef",
     {
@@ -833,22 +776,14 @@
         "ComplianceType": ConformancePackComplianceTypeType,
         "ResourceType": str,
         "ResourceIds": Sequence[str],
     },
     total=False,
 )
 
-ConformancePackInputParameterTypeDef = TypedDict(
-    "ConformancePackInputParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-    },
-)
-
 ConformancePackRuleComplianceTypeDef = TypedDict(
     "ConformancePackRuleComplianceTypeDef",
     {
         "ConfigRuleName": str,
         "ComplianceType": ConformancePackComplianceTypeType,
         "Controls": List[str],
     },
@@ -878,36 +813,14 @@
 
 class ConformancePackStatusDetailTypeDef(
     _RequiredConformancePackStatusDetailTypeDef, _OptionalConformancePackStatusDetailTypeDef
 ):
     pass
 
 
-_RequiredCustomPolicyDetailsOutputTypeDef = TypedDict(
-    "_RequiredCustomPolicyDetailsOutputTypeDef",
-    {
-        "PolicyRuntime": str,
-        "PolicyText": str,
-    },
-)
-_OptionalCustomPolicyDetailsOutputTypeDef = TypedDict(
-    "_OptionalCustomPolicyDetailsOutputTypeDef",
-    {
-        "EnableDebugLogDelivery": bool,
-    },
-    total=False,
-)
-
-
-class CustomPolicyDetailsOutputTypeDef(
-    _RequiredCustomPolicyDetailsOutputTypeDef, _OptionalCustomPolicyDetailsOutputTypeDef
-):
-    pass
-
-
 _RequiredCustomPolicyDetailsTypeDef = TypedDict(
     "_RequiredCustomPolicyDetailsTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -1054,93 +967,55 @@
 DeliverConfigSnapshotRequestRequestTypeDef = TypedDict(
     "DeliverConfigSnapshotRequestRequestTypeDef",
     {
         "deliveryChannelName": str,
     },
 )
 
-DeliverConfigSnapshotResponseTypeDef = TypedDict(
-    "DeliverConfigSnapshotResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configSnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
-)
-
-DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
-    TypedDict(
-        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+    total=False,
 )
 
 DescribeAggregationAuthorizationsRequestRequestTypeDef = TypedDict(
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByConfigRuleRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByResourceRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigRuleEvaluationStatusRequestRequestTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1151,37 +1026,14 @@
     "DescribeConfigRulesFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
     },
     total=False,
 )
 
-_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
-    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
@@ -1198,23 +1050,14 @@
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
-    {
-        "ConfigurationAggregatorNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigurationAggregatorsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1233,42 +1076,24 @@
     "DescribeConfigurationRecordersRequestRequestTypeDef",
     {
         "ConfigurationRecorderNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePackStatusRequestRequestTypeDef = TypedDict(
     "DescribeConformancePackStatusRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeConformancePacksRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1287,23 +1112,14 @@
     "DescribeDeliveryChannelsRequestRequestTypeDef",
     {
         "DeliveryChannelNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1330,42 +1146,24 @@
 
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
 
-DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePackStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1393,41 +1191,24 @@
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
 
-DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePendingAggregationRequestsRequestRequestTypeDef = TypedDict(
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1469,23 +1250,14 @@
 
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
 
-DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
-    {
-        "RetentionConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRetentionConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -1495,29 +1267,14 @@
     "RetentionConfigurationTypeDef",
     {
         "Name": str,
         "RetentionPeriodInDays": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EvaluationContextOutputTypeDef = TypedDict(
-    "EvaluationContextOutputTypeDef",
-    {
-        "EvaluationContextIdentifier": str,
-    },
-    total=False,
-)
-
 EvaluationContextTypeDef = TypedDict(
     "EvaluationContextTypeDef",
     {
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
@@ -1608,23 +1365,14 @@
     "ExclusionByResourceTypesTypeDef",
     {
         "resourceTypes": Sequence[ResourceTypeType],
     },
     total=False,
 )
 
-SsmControlsOutputTypeDef = TypedDict(
-    "SsmControlsOutputTypeDef",
-    {
-        "ConcurrentExecutionRatePercentage": int,
-        "ErrorPercentage": int,
-    },
-    total=False,
-)
-
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
         "ConcurrentExecutionRatePercentage": int,
         "ErrorPercentage": int,
     },
     total=False,
@@ -1650,57 +1398,22 @@
 
 class ExternalEvaluationTypeDef(
     _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
 
-RemediationExceptionResourceKeyOutputTypeDef = TypedDict(
-    "RemediationExceptionResourceKeyOutputTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-    },
-    total=False,
-)
-
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-        "ConfigRuleName": str,
-        "AccountId": str,
-        "AwsRegion": str,
-    },
-)
-_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceType": ComplianceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigRuleName": str,
         "AccountId": str,
         "AwsRegion": str,
@@ -1738,37 +1451,14 @@
     "GroupedResourceCountTypeDef",
     {
         "GroupName": str,
         "ResourceCount": int,
     },
 )
 
-_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleName": str,
-    },
-)
-_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
@@ -1785,26 +1475,14 @@
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
 
-GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "ResourceEvaluationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetComplianceDetailsByResourceRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
@@ -1817,36 +1495,14 @@
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
     {
         "ResourceTypes": Sequence[str],
     },
     total=False,
 )
 
-_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-    },
-)
-_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
-    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
     },
 )
 _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -1870,22 +1526,14 @@
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
 
-GetCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredResourceCountsRequestRequestTypeDef = TypedDict(
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[str],
         "limit": int,
         "nextToken": str,
     },
@@ -1973,48 +1621,14 @@
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
-GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
-    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
@@ -2041,104 +1655,75 @@
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
-_RequiredResourceDetailsOutputTypeDef = TypedDict(
-    "_RequiredResourceDetailsOutputTypeDef",
+_RequiredResourceDetailsTypeDef = TypedDict(
+    "_RequiredResourceDetailsTypeDef",
     {
         "ResourceId": str,
         "ResourceType": str,
         "ResourceConfiguration": str,
     },
 )
-_OptionalResourceDetailsOutputTypeDef = TypedDict(
-    "_OptionalResourceDetailsOutputTypeDef",
+_OptionalResourceDetailsTypeDef = TypedDict(
+    "_OptionalResourceDetailsTypeDef",
     {
         "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
     },
     total=False,
 )
 
 
-class ResourceDetailsOutputTypeDef(
-    _RequiredResourceDetailsOutputTypeDef, _OptionalResourceDetailsOutputTypeDef
-):
+class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
     pass
 
 
 GetStoredQueryRequestRequestTypeDef = TypedDict(
     "GetStoredQueryRequestRequestTypeDef",
     {
         "QueryName": str,
     },
 )
 
-_RequiredStoredQueryOutputTypeDef = TypedDict(
-    "_RequiredStoredQueryOutputTypeDef",
+_RequiredStoredQueryTypeDef = TypedDict(
+    "_RequiredStoredQueryTypeDef",
     {
         "QueryName": str,
     },
 )
-_OptionalStoredQueryOutputTypeDef = TypedDict(
-    "_OptionalStoredQueryOutputTypeDef",
+_OptionalStoredQueryTypeDef = TypedDict(
+    "_OptionalStoredQueryTypeDef",
     {
         "QueryId": str,
         "QueryArn": str,
         "Description": str,
         "Expression": str,
     },
     total=False,
 )
 
 
-class StoredQueryOutputTypeDef(
-    _RequiredStoredQueryOutputTypeDef, _OptionalStoredQueryOutputTypeDef
-):
+class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
     pass
 
 
 ResourceFiltersTypeDef = TypedDict(
     "ResourceFiltersTypeDef",
     {
         "AccountId": str,
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
     },
     total=False,
 )
 
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceIds": Sequence[str],
-        "resourceName": str,
-        "includeDeletedResources": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
@@ -2210,36 +1795,14 @@
 
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -2255,16 +1818,16 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -2446,78 +2009,14 @@
 
 class OrganizationManagedRuleMetadataTypeDef(
     _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
 ):
     pass
 
 
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
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_RequiredTemplateSSMDocumentDetailsTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_OptionalTemplateSSMDocumentDetailsTypeDef",
-    {
-        "DocumentVersion": str,
-    },
-    total=False,
-)
-
-
-class TemplateSSMDocumentDetailsTypeDef(
-    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
-):
-    pass
-
-
-PutConformancePackResponseTypeDef = TypedDict(
-    "PutConformancePackResponseTypeDef",
-    {
-        "ConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutOrganizationConfigRuleResponseTypeDef = TypedDict(
-    "PutOrganizationConfigRuleResponseTypeDef",
-    {
-        "OrganizationConfigRuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutOrganizationConformancePackResponseTypeDef = TypedDict(
-    "PutOrganizationConformancePackResponseTypeDef",
-    {
-        "OrganizationConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -2542,52 +2041,14 @@
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
-_RequiredStoredQueryTypeDef = TypedDict(
-    "_RequiredStoredQueryTypeDef",
-    {
-        "QueryName": str,
-    },
-)
-_OptionalStoredQueryTypeDef = TypedDict(
-    "_OptionalStoredQueryTypeDef",
-    {
-        "QueryId": str,
-        "QueryArn": str,
-        "Description": str,
-        "Expression": str,
-    },
-    total=False,
-)
-
-
-class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
-    pass
-
-
-PutStoredQueryResponseTypeDef = TypedDict(
-    "PutStoredQueryResponseTypeDef",
-    {
-        "QueryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RecordingStrategyOutputTypeDef = TypedDict(
-    "RecordingStrategyOutputTypeDef",
-    {
-        "useOnly": RecordingStrategyTypeType,
-    },
-    total=False,
-)
-
 RecordingStrategyTypeDef = TypedDict(
     "RecordingStrategyTypeDef",
     {
         "useOnly": RecordingStrategyTypeType,
     },
     total=False,
 )
@@ -2600,83 +2061,44 @@
         "ErrorMessage": str,
         "StartTime": datetime,
         "StopTime": datetime,
     },
     total=False,
 )
 
-ResourceValueOutputTypeDef = TypedDict(
-    "ResourceValueOutputTypeDef",
+ResourceValueTypeDef = TypedDict(
+    "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
 StaticValueOutputTypeDef = TypedDict(
     "StaticValueOutputTypeDef",
     {
         "Values": List[str],
     },
 )
 
-ResourceValueTypeDef = TypedDict(
-    "ResourceValueTypeDef",
-    {
-        "Value": Literal["RESOURCE_ID"],
-    },
-)
-
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-_RequiredResourceDetailsTypeDef = TypedDict(
-    "_RequiredResourceDetailsTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ResourceConfiguration": str,
-    },
-)
-_OptionalResourceDetailsTypeDef = TypedDict(
-    "_OptionalResourceDetailsTypeDef",
-    {
-        "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
-    },
-    total=False,
-)
-
-
-class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
-    pass
-
-
 TimeWindowTypeDef = TypedDict(
     "TimeWindowTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
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
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
         "ConfigurationAggregatorName": str,
     },
 )
@@ -2694,42 +2116,14 @@
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "Expression": str,
-            "ConfigurationAggregatorName": str,
-        },
-    )
-)
-_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "MaxResults": int,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
-    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-):
-    pass
-
-
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2745,46 +2139,14 @@
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
-    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-):
-    pass
-
-
-SourceDetailOutputTypeDef = TypedDict(
-    "SourceDetailOutputTypeDef",
-    {
-        "EventSource": Literal["aws.config"],
-        "MessageType": MessageTypeType,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-    },
-    total=False,
-)
-
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
     },
@@ -2802,22 +2164,14 @@
 StartConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StartConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
-StartResourceEvaluationResponseTypeDef = TypedDict(
-    "StartResourceEvaluationResponseTypeDef",
-    {
-        "ResourceEvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StopConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
@@ -2845,37 +2199,14 @@
     {
         "ComplianceSummary": AggregateConformancePackComplianceCountTypeDef,
         "GroupName": str,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
@@ -2917,23 +2248,14 @@
 class GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
 
-ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
-    {
-        "ResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchGetAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifiers": Sequence[AggregateResourceIdentifierTypeDef],
     },
 )
@@ -2942,78 +2264,144 @@
     "GetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifier": AggregateResourceIdentifierTypeDef,
     },
 )
 
+BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetAggregateResourceConfigResponseTypeDef",
+    {
+        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeliverConfigSnapshotResponseTypeDef = TypedDict(
+    "DeliverConfigSnapshotResponseTypeDef",
+    {
+        "configSnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
+    "DescribeAggregationAuthorizationsResponseTypeDef",
+    {
+        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeConfigurationAggregatorSourcesStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     {
         "AggregatedSourceStatusList": List[AggregatedSourceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
-    "DescribeAggregationAuthorizationsResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
+    {
+        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAggregationAuthorizationResponseTypeDef = TypedDict(
     "PutAggregationAuthorizationResponseTypeDef",
     {
         "AggregationAuthorization": AggregationAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+PutConformancePackResponseTypeDef = TypedDict(
+    "PutConformancePackResponseTypeDef",
     {
-        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
-    "BatchGetResourceConfigRequestRequestTypeDef",
+PutOrganizationConfigRuleResponseTypeDef = TypedDict(
+    "PutOrganizationConfigRuleResponseTypeDef",
     {
-        "resourceKeys": Sequence[ResourceKeyTypeDef],
+        "OrganizationConfigRuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+PutOrganizationConformancePackResponseTypeDef = TypedDict(
+    "PutOrganizationConformancePackResponseTypeDef",
     {
-        "ConfigRuleName": str,
+        "OrganizationConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+
+PutStoredQueryResponseTypeDef = TypedDict(
+    "PutStoredQueryResponseTypeDef",
     {
-        "ResourceKeys": Sequence[ResourceKeyTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "QueryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+StartResourceEvaluationResponseTypeDef = TypedDict(
+    "StartResourceEvaluationResponseTypeDef",
+    {
+        "ResourceEvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
-    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-):
-    pass
+BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
+    "BatchGetResourceConfigRequestRequestTypeDef",
+    {
+        "resourceKeys": Sequence[ResourceKeyTypeDef],
+    },
+)
 
+BatchGetResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetResourceConfigResponseTypeDef",
+    {
+        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
@@ -3039,29 +2427,20 @@
     "StartRemediationExecutionRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
 
-BatchGetResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetResourceConfigResponseTypeDef",
-    {
-        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "unprocessedResourceKeys": List[ResourceKeyOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartRemediationExecutionResponseTypeDef = TypedDict(
     "StartRemediationExecutionResponseTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[ResourceKeyOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FailedItems": List[ResourceKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryTypeDef = TypedDict(
     "ComplianceSummaryTypeDef",
     {
         "CompliantResourceCount": ComplianceContributorCountTypeDef,
@@ -3076,37 +2455,14 @@
     {
         "ComplianceType": ComplianceTypeType,
         "ComplianceContributorCount": ComplianceContributorCountTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "Filters": ConfigRuleComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
@@ -3153,31 +2509,18 @@
 
 
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeliveryChannelOutputTypeDef = TypedDict(
-    "DeliveryChannelOutputTypeDef",
-    {
-        "name": str,
-        "s3BucketName": str,
-        "s3KeyPrefix": str,
-        "s3KmsKeyArn": str,
-        "snsTopicARN": str,
-        "configSnapshotDeliveryProperties": ConfigSnapshotDeliveryPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 DeliveryChannelTypeDef = TypedDict(
     "DeliveryChannelTypeDef",
     {
         "name": str,
         "s3BucketName": str,
         "s3KeyPrefix": str,
         "s3KmsKeyArn": str,
@@ -3237,15 +2580,15 @@
     total=False,
 )
 
 DescribeConfigurationRecorderStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     {
         "ConfigurationRecordersStatus": List[ConfigurationRecorderStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeConformancePackComplianceRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConformancePackComplianceRequestRequestTypeDef",
     {
         "ConformancePackName": str,
@@ -3270,15 +2613,15 @@
 
 
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConformancePackComplianceScoresRequestRequestTypeDef = TypedDict(
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     {
         "Filters": ConformancePackComplianceScoresFiltersTypeDef,
@@ -3291,15 +2634,15 @@
 )
 
 GetConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetConformancePackComplianceSummaryResponseTypeDef",
     {
         "ConformancePackComplianceSummaryList": List[ConformancePackComplianceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOrganizationConformancePackTypeDef = TypedDict(
     "_RequiredOrganizationConformancePackTypeDef",
     {
         "OrganizationConformancePackName": str,
@@ -3308,122 +2651,149 @@
     },
 )
 _OptionalOrganizationConformancePackTypeDef = TypedDict(
     "_OptionalOrganizationConformancePackTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
         "ExcludedAccounts": List[str],
     },
     total=False,
 )
 
 
 class OrganizationConformancePackTypeDef(
     _RequiredOrganizationConformancePackTypeDef, _OptionalOrganizationConformancePackTypeDef
 ):
     pass
 
 
+_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "OrganizationConformancePackName": str,
+    },
+)
+_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "ExcludedAccounts": Sequence[str],
+    },
+    total=False,
+)
+
+
+class PutOrganizationConformancePackRequestRequestTypeDef(
+    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
+    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredConformancePackDetailTypeDef = TypedDict(
     "_RequiredConformancePackDetailTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackArn": str,
         "ConformancePackId": str,
     },
 )
 _OptionalConformancePackDetailTypeDef = TypedDict(
     "_OptionalConformancePackDetailTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
         "LastUpdateRequestedTime": datetime,
         "CreatedBy": str,
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsOutputTypeDef,
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
 
 class ConformancePackDetailTypeDef(
     _RequiredConformancePackDetailTypeDef, _OptionalConformancePackDetailTypeDef
 ):
     pass
 
 
-_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
+_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConformancePackRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
-_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef",
+_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConformancePackRequestRequestTypeDef",
     {
-        "Filters": ConformancePackEvaluationFiltersTypeDef,
-        "Limit": int,
-        "NextToken": str,
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
 
-class GetConformancePackComplianceDetailsRequestRequestTypeDef(
-    _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
-    _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
+class PutConformancePackRequestRequestTypeDef(
+    _RequiredPutConformancePackRequestRequestTypeDef,
+    _OptionalPutConformancePackRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
+_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
-        "OrganizationConformancePackName": str,
+        "ConformancePackName": str,
     },
 )
-_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
+_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "ExcludedAccounts": Sequence[str],
+        "Filters": ConformancePackEvaluationFiltersTypeDef,
+        "Limit": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 
-class PutOrganizationConformancePackRequestRequestTypeDef(
-    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
-    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
+class GetConformancePackComplianceDetailsRequestRequestTypeDef(
+    _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
+    _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
 ):
     pass
 
 
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePackStatusResponseTypeDef = TypedDict(
     "DescribeConformancePackStatusResponseTypeDef",
     {
         "ConformancePackStatusDetails": List[ConformancePackStatusDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
@@ -3451,14 +2821,23 @@
 class DescribeRemediationExceptionsRequestRequestTypeDef(
     _RequiredDescribeRemediationExceptionsRequestRequestTypeDef,
     _OptionalDescribeRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
 
+FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
+    {
+        "FailureMessage": str,
+        "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
+    },
+    total=False,
+)
+
 _RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
 )
@@ -3475,20 +2854,438 @@
 class PutRemediationExceptionsRequestRequestTypeDef(
     _RequiredPutRemediationExceptionsRequestRequestTypeDef,
     _OptionalPutRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "Filters": ConfigRuleComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+):
+    pass
+
+
+DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
+    TypedDict(
+        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
+    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+):
+    pass
+
+
+DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    {
+        "ConfigurationAggregatorNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    {
+        "ConfigRuleName": str,
+    },
+)
+_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    {
+        "ResourceKeys": Sequence[ResourceKeyTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
+    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+):
+    pass
+
+
+DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    {
+        "RetentionConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+        "ConfigRuleName": str,
+        "AccountId": str,
+        "AwsRegion": str,
+    },
+)
+_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceType": ComplianceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleName": str,
+    },
+)
+_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+
+GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "ResourceEvaluationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+    },
+)
+_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
+    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "laterTime": Union[datetime, str],
+        "earlierTime": Union[datetime, str],
+        "chronologicalOrder": ChronologicalOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
+    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceIds": Sequence[str],
+        "resourceName": str,
+        "includeDeletedResources": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "Expression": str,
+            "ConfigurationAggregatorName": str,
+        },
+    )
+)
+_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "MaxResults": int,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
+    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "Expression": str,
+    },
+)
+_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
+    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+):
+    pass
+
+
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeConfigRulesRequestRequestTypeDef",
     {
@@ -3500,42 +3297,42 @@
 )
 
 DescribeOrganizationConfigRuleStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     {
         "OrganizationConfigRuleStatuses": List[OrganizationConfigRuleStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePackStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     {
         "OrganizationConformancePackStatuses": List[OrganizationConformancePackStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePendingAggregationRequestsResponseTypeDef = TypedDict(
     "DescribePendingAggregationRequestsResponseTypeDef",
     {
         "PendingAggregationRequests": List[PendingAggregationRequestTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRemediationExceptionsResponseTypeDef = TypedDict(
     "DescribeRemediationExceptionsResponseTypeDef",
     {
         "RemediationExceptions": List[RemediationExceptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationExceptionBatchTypeDef = TypedDict(
     "FailedRemediationExceptionBatchTypeDef",
     {
         "FailureMessage": str,
@@ -3545,31 +3342,31 @@
 )
 
 DescribeRetentionConfigurationsResponseTypeDef = TypedDict(
     "DescribeRetentionConfigurationsResponseTypeDef",
     {
         "RetentionConfigurations": List[RetentionConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRetentionConfigurationResponseTypeDef = TypedDict(
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEvaluationsResponseTypeDef = TypedDict(
     "PutEvaluationsResponseTypeDef",
     {
         "FailedEvaluations": List[EvaluationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
@@ -3597,22 +3394,14 @@
 
 class PutEvaluationsRequestRequestTypeDef(
     _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
 ):
     pass
 
 
-ExecutionControlsOutputTypeDef = TypedDict(
-    "ExecutionControlsOutputTypeDef",
-    {
-        "SsmControls": SsmControlsOutputTypeDef,
-    },
-    total=False,
-)
-
 ExecutionControlsTypeDef = TypedDict(
     "ExecutionControlsTypeDef",
     {
         "SsmControls": SsmControlsTypeDef,
     },
     total=False,
 )
@@ -3621,23 +3410,14 @@
     "PutExternalEvaluationRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ExternalEvaluation": ExternalEvaluationTypeDef,
     },
 )
 
-FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
-    {
-        "FailureMessage": str,
-        "FailedItems": List[RemediationExceptionResourceKeyOutputTypeDef],
-    },
-    total=False,
-)
-
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
     total=False,
 )
@@ -3670,39 +3450,39 @@
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetDiscoveredResourceCountsResponseTypeDef",
     {
         "totalDiscoveredResources": int,
         "resourceCounts": List[ResourceCountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "Filters": StatusDetailFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
@@ -3736,29 +3516,29 @@
 
 
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
@@ -3794,52 +3574,77 @@
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceEvaluationSummaryResponseTypeDef = TypedDict(
     "GetResourceEvaluationSummaryResponseTypeDef",
     {
         "ResourceEvaluationId": str,
         "EvaluationMode": EvaluationModeType,
         "EvaluationStatus": EvaluationStatusTypeDef,
         "EvaluationStartTimestamp": datetime,
         "Compliance": ComplianceTypeType,
-        "EvaluationContext": EvaluationContextOutputTypeDef,
-        "ResourceDetails": ResourceDetailsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EvaluationContext": EvaluationContextTypeDef,
+        "ResourceDetails": ResourceDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "ResourceDetails": ResourceDetailsTypeDef,
+        "EvaluationMode": EvaluationModeType,
+    },
+)
+_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "EvaluationContext": EvaluationContextTypeDef,
+        "EvaluationTimeout": int,
+        "ClientToken": str,
     },
+    total=False,
 )
 
+
+class StartResourceEvaluationRequestRequestTypeDef(
+    _RequiredStartResourceEvaluationRequestRequestTypeDef,
+    _OptionalStartResourceEvaluationRequestRequestTypeDef,
+):
+    pass
+
+
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
-        "StoredQuery": StoredQueryOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StoredQuery": StoredQueryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "Filters": ResourceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
@@ -3874,119 +3679,97 @@
 
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceEvaluationsResponseTypeDef = TypedDict(
     "ListResourceEvaluationsResponseTypeDef",
     {
         "ResourceEvaluations": List[ResourceEvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStoredQueriesResponseTypeDef = TypedDict(
     "ListStoredQueriesResponseTypeDef",
     {
         "StoredQueryMetadata": List[StoredQueryMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredOrganizationConfigRuleTypeDef = TypedDict(
-    "_RequiredOrganizationConfigRuleTypeDef",
+_RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
-        "OrganizationConfigRuleArn": str,
+        "AuthorizedAccountId": str,
+        "AuthorizedAwsRegion": str,
     },
 )
-_OptionalOrganizationConfigRuleTypeDef = TypedDict(
-    "_OptionalOrganizationConfigRuleTypeDef",
+_OptionalPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
-        "ExcludedAccounts": List[str],
-        "LastUpdateTime": datetime,
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class OrganizationConfigRuleTypeDef(
-    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
+class PutAggregationAuthorizationRequestRequestTypeDef(
+    _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
+    _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
+_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
+        "StoredQuery": StoredQueryTypeDef,
     },
 )
-_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
+_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
-        "ExcludedAccounts": Sequence[str],
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class PutOrganizationConfigRuleRequestRequestTypeDef(
-    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
-    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
+class PutStoredQueryRequestRequestTypeDef(
+    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
-    {
-        "AuthorizedAccountId": str,
-        "AuthorizedAwsRegion": str,
-    },
-)
-_OptionalPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
+        "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-
-class PutAggregationAuthorizationRequestRequestTypeDef(
-    _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
-    _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
@@ -4003,78 +3786,73 @@
 class PutConfigurationAggregatorRequestRequestTypeDef(
     _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
     _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConformancePackRequestRequestTypeDef",
+_RequiredOrganizationConfigRuleTypeDef = TypedDict(
+    "_RequiredOrganizationConfigRuleTypeDef",
     {
-        "ConformancePackName": str,
+        "OrganizationConfigRuleName": str,
+        "OrganizationConfigRuleArn": str,
     },
 )
-_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConformancePackRequestRequestTypeDef",
+_OptionalOrganizationConfigRuleTypeDef = TypedDict(
+    "_OptionalOrganizationConfigRuleTypeDef",
     {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
+        "ExcludedAccounts": List[str],
+        "LastUpdateTime": datetime,
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
 
-class PutConformancePackRequestRequestTypeDef(
-    _RequiredPutConformancePackRequestRequestTypeDef,
-    _OptionalPutConformancePackRequestRequestTypeDef,
+class OrganizationConfigRuleTypeDef(
+    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
 
-_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredPutStoredQueryRequestRequestTypeDef",
+_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
-        "StoredQuery": StoredQueryTypeDef,
+        "OrganizationConfigRuleName": str,
     },
 )
-_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalPutStoredQueryRequestRequestTypeDef",
+_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
+        "ExcludedAccounts": Sequence[str],
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
     },
     total=False,
 )
 
 
-class PutStoredQueryRequestRequestTypeDef(
-    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
+class PutOrganizationConfigRuleRequestRequestTypeDef(
+    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
+    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
 
 RecordingGroupOutputTypeDef = TypedDict(
     "RecordingGroupOutputTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
         "resourceTypes": List[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
-        "recordingStrategy": RecordingStrategyOutputTypeDef,
+        "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
@@ -4086,66 +3864,41 @@
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
     "RemediationExecutionStatusTypeDef",
     {
-        "ResourceKey": ResourceKeyOutputTypeDef,
+        "ResourceKey": ResourceKeyTypeDef,
         "State": RemediationExecutionStateType,
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
 RemediationParameterValueOutputTypeDef = TypedDict(
     "RemediationParameterValueOutputTypeDef",
     {
-        "ResourceValue": ResourceValueOutputTypeDef,
+        "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueOutputTypeDef,
     },
     total=False,
 )
 
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "ResourceDetails": ResourceDetailsTypeDef,
-        "EvaluationMode": EvaluationModeType,
-    },
-)
-_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "EvaluationContext": EvaluationContextTypeDef,
-        "EvaluationTimeout": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class StartResourceEvaluationRequestRequestTypeDef(
-    _RequiredStartResourceEvaluationRequestRequestTypeDef,
-    _OptionalStartResourceEvaluationRequestRequestTypeDef,
-):
-    pass
-
-
 ResourceEvaluationFiltersTypeDef = TypedDict(
     "ResourceEvaluationFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
         "TimeWindow": TimeWindowTypeDef,
         "EvaluationContextIdentifier": str,
     },
@@ -4158,16 +3911,16 @@
         "Owner": OwnerType,
     },
 )
 _OptionalSourceOutputTypeDef = TypedDict(
     "_OptionalSourceOutputTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailOutputTypeDef],
-        "CustomPolicyDetails": CustomPolicyDetailsOutputTypeDef,
+        "SourceDetails": List[SourceDetailTypeDef],
+        "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
 
 class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
     pass
@@ -4195,27 +3948,27 @@
 
 
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     {
         "AggregateConformancePackComplianceSummaries": List[
             AggregateConformancePackComplianceSummaryTypeDef
         ],
         "GroupByKey": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceCountTypeDef = TypedDict(
     "AggregateComplianceCountTypeDef",
     {
         "GroupName": str,
@@ -4233,15 +3986,15 @@
     total=False,
 )
 
 GetComplianceSummaryByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     {
         "ComplianceSummary": ComplianceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceByConfigRuleTypeDef = TypedDict(
     "AggregateComplianceByConfigRuleTypeDef",
     {
         "ConfigRuleName": str,
@@ -4270,91 +4023,99 @@
     },
     total=False,
 )
 
 DescribeDeliveryChannelsResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelsResponseTypeDef",
     {
-        "DeliveryChannels": List[DeliveryChannelOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeliveryChannels": List[DeliveryChannelTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDeliveryChannelRequestRequestTypeDef = TypedDict(
     "PutDeliveryChannelRequestRequestTypeDef",
     {
         "DeliveryChannel": DeliveryChannelTypeDef,
     },
 )
 
 DescribeDeliveryChannelStatusResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelStatusResponseTypeDef",
     {
         "DeliveryChannelsStatus": List[DeliveryChannelStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationAggregatorsResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsResponseTypeDef",
     {
         "ConfigurationAggregators": List[ConfigurationAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationAggregatorResponseTypeDef = TypedDict(
     "PutConfigurationAggregatorResponseTypeDef",
     {
         "ConfigurationAggregator": ConfigurationAggregatorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateResourceConfigResponseTypeDef = TypedDict(
     "GetAggregateResourceConfigResponseTypeDef",
     {
         "ConfigurationItem": ConfigurationItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceConfigHistoryResponseTypeDef = TypedDict(
     "GetResourceConfigHistoryResponseTypeDef",
     {
         "configurationItems": List[ConfigurationItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePacksResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksResponseTypeDef",
     {
         "OrganizationConformancePacks": List[OrganizationConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePacksResponseTypeDef = TypedDict(
     "DescribeConformancePacksResponseTypeDef",
     {
         "ConformancePackDetails": List[ConformancePackDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRemediationExceptionsResponseTypeDef = TypedDict(
+    "DeleteRemediationExceptionsResponseTypeDef",
+    {
+        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRemediationExceptionsResponseTypeDef = TypedDict(
     "PutRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationExceptionBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateEvaluationResultTypeDef = TypedDict(
     "AggregateEvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
@@ -4401,48 +4162,40 @@
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
-DeleteRemediationExceptionsResponseTypeDef = TypedDict(
-    "DeleteRemediationExceptionsResponseTypeDef",
-    {
-        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectResourceConfigResponseTypeDef = TypedDict(
     "SelectResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigRulesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesResponseTypeDef",
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationRecorderOutputTypeDef = TypedDict(
     "ConfigurationRecorderOutputTypeDef",
     {
         "name": str,
@@ -4463,15 +4216,15 @@
 )
 
 DescribeRemediationExecutionStatusResponseTypeDef = TypedDict(
     "DescribeRemediationExecutionStatusResponseTypeDef",
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRemediationConfigurationOutputTypeDef = TypedDict(
     "_RequiredRemediationConfigurationOutputTypeDef",
     {
         "ConfigRuleName": str,
@@ -4482,15 +4235,15 @@
 _OptionalRemediationConfigurationOutputTypeDef = TypedDict(
     "_OptionalRemediationConfigurationOutputTypeDef",
     {
         "TargetVersion": str,
         "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
         "ResourceType": str,
         "Automatic": bool,
-        "ExecutionControls": ExecutionControlsOutputTypeDef,
+        "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
@@ -4533,15 +4286,15 @@
     pass
 
 
 ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     {
         "Filters": ResourceEvaluationFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
     "ListResourceEvaluationsRequestRequestTypeDef",
     {
@@ -4566,15 +4319,15 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeOutputTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationOutputTypeDef],
+        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
 
 class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
     pass
@@ -4610,110 +4363,110 @@
 
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceSummaryByResourceTypeResponseTypeDef = TypedDict(
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     {
         "ComplianceSummariesByResourceType": List[ComplianceSummaryByResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAggregateComplianceByConfigRulesResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     {
         "AggregateComplianceByConfigRules": List[AggregateComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByConfigRuleResponseTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleResponseTypeDef",
     {
         "ComplianceByConfigRules": List[ComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByResourceResponseTypeDef = TypedDict(
     "DescribeComplianceByResourceResponseTypeDef",
     {
         "ComplianceByResources": List[ComplianceByResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "AggregateEvaluationResults": List[AggregateEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConformancePackComplianceDetailsResponseTypeDef = TypedDict(
     "GetConformancePackComplianceDetailsResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleEvaluationResults": List[ConformancePackEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByResourceResponseTypeDef = TypedDict(
     "GetComplianceDetailsByResourceResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
         "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
         "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
@@ -4730,15 +4483,15 @@
 )
 
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
         "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
@@ -4759,10 +4512,10 @@
     pass
 
 
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config/type_defs.pyi` & `mypy-boto3-config-1.28.15/mypy_boto3_config/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,47 +59,42 @@
 __all__ = (
     "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
-    "AggregateResourceIdentifierOutputTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
     "AggregationAuthorizationTypeDef",
     "BaseConfigurationItemTypeDef",
+    "ResponseMetadataTypeDef",
     "ResourceKeyTypeDef",
-    "ResourceKeyOutputTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
-    "EvaluationModeConfigurationOutputTypeDef",
-    "ScopeOutputTypeDef",
     "EvaluationModeConfigurationTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
-    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
     "OrganizationAggregationSourceOutputTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
-    "ConformancePackInputParameterOutputTypeDef",
-    "TemplateSSMDocumentDetailsOutputTypeDef",
-    "ConformancePackEvaluationFiltersTypeDef",
     "ConformancePackInputParameterTypeDef",
+    "TemplateSSMDocumentDetailsTypeDef",
+    "ConformancePackEvaluationFiltersTypeDef",
     "ConformancePackRuleComplianceTypeDef",
     "ConformancePackStatusDetailTypeDef",
-    "CustomPolicyDetailsOutputTypeDef",
     "CustomPolicyDetailsTypeDef",
     "DeleteAggregationAuthorizationRequestRequestTypeDef",
     "DeleteConfigRuleRequestRequestTypeDef",
     "DeleteConfigurationAggregatorRequestRequestTypeDef",
     "DeleteConfigurationRecorderRequestRequestTypeDef",
     "DeleteConformancePackRequestRequestTypeDef",
     "DeleteDeliveryChannelRequestRequestTypeDef",
@@ -109,233 +104,220 @@
     "DeletePendingAggregationRequestRequestRequestTypeDef",
     "DeleteRemediationConfigurationRequestRequestTypeDef",
     "RemediationExceptionResourceKeyTypeDef",
     "DeleteResourceConfigRequestRequestTypeDef",
     "DeleteRetentionConfigurationRequestRequestTypeDef",
     "DeleteStoredQueryRequestRequestTypeDef",
     "DeliverConfigSnapshotRequestRequestTypeDef",
-    "DeliverConfigSnapshotResponseTypeDef",
-    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
     "DescribeComplianceByResourceRequestRequestTypeDef",
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     "DescribeConfigRulesFiltersTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     "DescribeConfigurationRecorderStatusRequestRequestTypeDef",
     "DescribeConfigurationRecordersRequestRequestTypeDef",
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
     "DescribeConformancePackStatusRequestRequestTypeDef",
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
     "DescribeConformancePacksRequestRequestTypeDef",
     "DescribeDeliveryChannelStatusRequestRequestTypeDef",
     "DescribeDeliveryChannelsRequestRequestTypeDef",
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     "OrganizationConfigRuleStatusTypeDef",
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     "OrganizationConformancePackStatusTypeDef",
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EvaluationContextOutputTypeDef",
     "EvaluationContextTypeDef",
     "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
     "EvaluationTypeDef",
     "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
-    "SsmControlsOutputTypeDef",
     "SsmControlsTypeDef",
     "ExternalEvaluationTypeDef",
-    "RemediationExceptionResourceKeyOutputTypeDef",
     "FieldInfoTypeDef",
-    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
-    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
-    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     "GetConformancePackComplianceSummaryRequestRequestTypeDef",
     "GetCustomRulePolicyRequestRequestTypeDef",
-    "GetCustomRulePolicyResponseTypeDef",
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     "ResourceCountTypeDef",
     "StatusDetailFiltersTypeDef",
     "MemberAccountStatusTypeDef",
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
-    "ResourceDetailsOutputTypeDef",
+    "ResourceDetailsTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
-    "StoredQueryOutputTypeDef",
+    "StoredQueryTypeDef",
     "ResourceFiltersTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     "OrganizationCustomRuleMetadataOutputTypeDef",
     "OrganizationManagedRuleMetadataOutputTypeDef",
     "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
-    "PaginatorConfigTypeDef",
-    "TagTypeDef",
-    "TemplateSSMDocumentDetailsTypeDef",
-    "PutConformancePackResponseTypeDef",
-    "PutOrganizationConfigRuleResponseTypeDef",
-    "PutOrganizationConformancePackResponseTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
-    "StoredQueryTypeDef",
-    "PutStoredQueryResponseTypeDef",
-    "RecordingStrategyOutputTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
-    "ResourceValueOutputTypeDef",
-    "StaticValueOutputTypeDef",
     "ResourceValueTypeDef",
+    "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
-    "ResourceDetailsTypeDef",
     "TimeWindowTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
-    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
-    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    "SourceDetailOutputTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
-    "StartResourceEvaluationResponseTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
-    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "DeliverConfigSnapshotResponseTypeDef",
     "DescribeAggregationAuthorizationsResponseTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCustomRulePolicyResponseTypeDef",
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "PutAggregationAuthorizationResponseTypeDef",
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "PutConformancePackResponseTypeDef",
+    "PutOrganizationConfigRuleResponseTypeDef",
+    "PutOrganizationConformancePackResponseTypeDef",
+    "PutStoredQueryResponseTypeDef",
+    "StartResourceEvaluationResponseTypeDef",
     "BatchGetResourceConfigRequestRequestTypeDef",
-    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    "BatchGetResourceConfigResponseTypeDef",
     "DescribeRemediationExecutionStatusRequestRequestTypeDef",
     "StartRemediationExecutionRequestRequestTypeDef",
-    "BatchGetResourceConfigResponseTypeDef",
     "StartRemediationExecutionResponseTypeDef",
     "ComplianceSummaryTypeDef",
     "ComplianceTypeDef",
-    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     "GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
-    "DeliveryChannelOutputTypeDef",
     "DeliveryChannelTypeDef",
     "DeliveryChannelStatusTypeDef",
     "ConfigurationAggregatorTypeDef",
     "ConfigurationItemTypeDef",
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     "DescribeConformancePackComplianceRequestRequestTypeDef",
     "ListConformancePackComplianceScoresResponseTypeDef",
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     "GetConformancePackComplianceSummaryResponseTypeDef",
     "OrganizationConformancePackTypeDef",
+    "PutOrganizationConformancePackRequestRequestTypeDef",
     "ConformancePackDetailTypeDef",
+    "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
-    "PutOrganizationConformancePackRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "PutRemediationExceptionsRequestRequestTypeDef",
+    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
     "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
     "PutEvaluationsRequestRequestTypeDef",
-    "ExecutionControlsOutputTypeDef",
     "ExecutionControlsTypeDef",
     "PutExternalEvaluationRequestRequestTypeDef",
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     "GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     "GetResourceEvaluationSummaryResponseTypeDef",
+    "StartResourceEvaluationRequestRequestTypeDef",
     "GetStoredQueryResponseTypeDef",
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "OrganizationConfigRuleTypeDef",
-    "PutOrganizationConfigRuleRequestRequestTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "PutConformancePackRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
+    "OrganizationConfigRuleTypeDef",
+    "PutOrganizationConfigRuleRequestRequestTypeDef",
     "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
     "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "StartResourceEvaluationRequestRequestTypeDef",
     "ResourceEvaluationFiltersTypeDef",
     "SourceOutputTypeDef",
     "SourceTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
@@ -348,19 +330,19 @@
     "DescribeDeliveryChannelStatusResponseTypeDef",
     "DescribeConfigurationAggregatorsResponseTypeDef",
     "PutConfigurationAggregatorResponseTypeDef",
     "GetAggregateResourceConfigResponseTypeDef",
     "GetResourceConfigHistoryResponseTypeDef",
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
+    "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
-    "DeleteRemediationExceptionsResponseTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
     "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
     "RemediationConfigurationOutputTypeDef",
@@ -464,37 +446,14 @@
     {
         "AccountId": str,
         "AwsRegion": str,
     },
     total=False,
 )
 
-_RequiredAggregateResourceIdentifierOutputTypeDef = TypedDict(
-    "_RequiredAggregateResourceIdentifierOutputTypeDef",
-    {
-        "SourceAccountId": str,
-        "SourceRegion": str,
-        "ResourceId": str,
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalAggregateResourceIdentifierOutputTypeDef = TypedDict(
-    "_OptionalAggregateResourceIdentifierOutputTypeDef",
-    {
-        "ResourceName": str,
-    },
-    total=False,
-)
-
-class AggregateResourceIdentifierOutputTypeDef(
-    _RequiredAggregateResourceIdentifierOutputTypeDef,
-    _OptionalAggregateResourceIdentifierOutputTypeDef,
-):
-    pass
-
 _RequiredAggregateResourceIdentifierTypeDef = TypedDict(
     "_RequiredAggregateResourceIdentifierTypeDef",
     {
         "SourceAccountId": str,
         "SourceRegion": str,
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
@@ -555,24 +514,27 @@
         "resourceCreationTime": datetime,
         "configuration": str,
         "supplementaryConfiguration": Dict[str, str],
     },
     total=False,
 )
 
-ResourceKeyTypeDef = TypedDict(
-    "ResourceKeyTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ResourceKeyOutputTypeDef = TypedDict(
-    "ResourceKeyOutputTypeDef",
+ResourceKeyTypeDef = TypedDict(
+    "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
 
 ComplianceContributorCountTypeDef = TypedDict(
@@ -635,16 +597,16 @@
         "LastDebugLogDeliveryStatus": str,
         "LastDebugLogDeliveryStatusReason": str,
         "LastDebugLogDeliveryTime": datetime,
     },
     total=False,
 )
 
-EvaluationModeConfigurationOutputTypeDef = TypedDict(
-    "EvaluationModeConfigurationOutputTypeDef",
+EvaluationModeConfigurationTypeDef = TypedDict(
+    "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
 ScopeOutputTypeDef = TypedDict(
@@ -654,41 +616,25 @@
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
-EvaluationModeConfigurationTypeDef = TypedDict(
-    "EvaluationModeConfigurationTypeDef",
-    {
-        "Mode": EvaluationModeType,
-    },
-    total=False,
-)
-
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "ComplianceResourceTypes": Sequence[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
-ConfigSnapshotDeliveryPropertiesOutputTypeDef = TypedDict(
-    "ConfigSnapshotDeliveryPropertiesOutputTypeDef",
-    {
-        "deliveryFrequency": MaximumExecutionFrequencyType,
-    },
-    total=False,
-)
-
 ConfigSnapshotDeliveryPropertiesTypeDef = TypedDict(
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     {
         "deliveryFrequency": MaximumExecutionFrequencyType,
     },
     total=False,
 )
@@ -781,61 +727,52 @@
     "ConformancePackComplianceSummaryTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackComplianceStatus": ConformancePackComplianceTypeType,
     },
 )
 
-ConformancePackInputParameterOutputTypeDef = TypedDict(
-    "ConformancePackInputParameterOutputTypeDef",
+ConformancePackInputParameterTypeDef = TypedDict(
+    "ConformancePackInputParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
 )
 
-_RequiredTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
-    "_RequiredTemplateSSMDocumentDetailsOutputTypeDef",
+_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_RequiredTemplateSSMDocumentDetailsTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalTemplateSSMDocumentDetailsOutputTypeDef = TypedDict(
-    "_OptionalTemplateSSMDocumentDetailsOutputTypeDef",
+_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
+    "_OptionalTemplateSSMDocumentDetailsTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-class TemplateSSMDocumentDetailsOutputTypeDef(
-    _RequiredTemplateSSMDocumentDetailsOutputTypeDef,
-    _OptionalTemplateSSMDocumentDetailsOutputTypeDef,
+class TemplateSSMDocumentDetailsTypeDef(
+    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
 ):
     pass
 
 ConformancePackEvaluationFiltersTypeDef = TypedDict(
     "ConformancePackEvaluationFiltersTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceType": ConformancePackComplianceTypeType,
         "ResourceType": str,
         "ResourceIds": Sequence[str],
     },
     total=False,
 )
 
-ConformancePackInputParameterTypeDef = TypedDict(
-    "ConformancePackInputParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-    },
-)
-
 ConformancePackRuleComplianceTypeDef = TypedDict(
     "ConformancePackRuleComplianceTypeDef",
     {
         "ConfigRuleName": str,
         "ComplianceType": ConformancePackComplianceTypeType,
         "Controls": List[str],
     },
@@ -863,34 +800,14 @@
 )
 
 class ConformancePackStatusDetailTypeDef(
     _RequiredConformancePackStatusDetailTypeDef, _OptionalConformancePackStatusDetailTypeDef
 ):
     pass
 
-_RequiredCustomPolicyDetailsOutputTypeDef = TypedDict(
-    "_RequiredCustomPolicyDetailsOutputTypeDef",
-    {
-        "PolicyRuntime": str,
-        "PolicyText": str,
-    },
-)
-_OptionalCustomPolicyDetailsOutputTypeDef = TypedDict(
-    "_OptionalCustomPolicyDetailsOutputTypeDef",
-    {
-        "EnableDebugLogDelivery": bool,
-    },
-    total=False,
-)
-
-class CustomPolicyDetailsOutputTypeDef(
-    _RequiredCustomPolicyDetailsOutputTypeDef, _OptionalCustomPolicyDetailsOutputTypeDef
-):
-    pass
-
 _RequiredCustomPolicyDetailsTypeDef = TypedDict(
     "_RequiredCustomPolicyDetailsTypeDef",
     {
         "PolicyRuntime": str,
         "PolicyText": str,
     },
 )
@@ -1033,93 +950,55 @@
 DeliverConfigSnapshotRequestRequestTypeDef = TypedDict(
     "DeliverConfigSnapshotRequestRequestTypeDef",
     {
         "deliveryChannelName": str,
     },
 )
 
-DeliverConfigSnapshotResponseTypeDef = TypedDict(
-    "DeliverConfigSnapshotResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configSnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
-)
-
-DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
-    TypedDict(
-        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+    total=False,
 )
 
 DescribeAggregationAuthorizationsRequestRequestTypeDef = TypedDict(
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByConfigRuleRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByResourceRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigRuleEvaluationStatusRequestRequestTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1130,35 +1009,14 @@
     "DescribeConfigRulesFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
     },
     total=False,
 )
 
-_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
-    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
@@ -1173,23 +1031,14 @@
 
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
-DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
-    {
-        "ConfigurationAggregatorNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigurationAggregatorsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1208,42 +1057,24 @@
     "DescribeConfigurationRecordersRequestRequestTypeDef",
     {
         "ConfigurationRecorderNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePackStatusRequestRequestTypeDef = TypedDict(
     "DescribeConformancePackStatusRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeConformancePacksRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1262,23 +1093,14 @@
     "DescribeDeliveryChannelsRequestRequestTypeDef",
     {
         "DeliveryChannelNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1303,42 +1125,24 @@
 )
 
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
-DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePackStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1364,41 +1168,24 @@
 
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
-DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePendingAggregationRequestsRequestRequestTypeDef = TypedDict(
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1438,23 +1225,14 @@
 )
 
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
-DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
-    {
-        "RetentionConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRetentionConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -1464,29 +1242,14 @@
     "RetentionConfigurationTypeDef",
     {
         "Name": str,
         "RetentionPeriodInDays": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EvaluationContextOutputTypeDef = TypedDict(
-    "EvaluationContextOutputTypeDef",
-    {
-        "EvaluationContextIdentifier": str,
-    },
-    total=False,
-)
-
 EvaluationContextTypeDef = TypedDict(
     "EvaluationContextTypeDef",
     {
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
@@ -1571,23 +1334,14 @@
     "ExclusionByResourceTypesTypeDef",
     {
         "resourceTypes": Sequence[ResourceTypeType],
     },
     total=False,
 )
 
-SsmControlsOutputTypeDef = TypedDict(
-    "SsmControlsOutputTypeDef",
-    {
-        "ConcurrentExecutionRatePercentage": int,
-        "ErrorPercentage": int,
-    },
-    total=False,
-)
-
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
         "ConcurrentExecutionRatePercentage": int,
         "ErrorPercentage": int,
     },
     total=False,
@@ -1611,55 +1365,22 @@
 )
 
 class ExternalEvaluationTypeDef(
     _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
-RemediationExceptionResourceKeyOutputTypeDef = TypedDict(
-    "RemediationExceptionResourceKeyOutputTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-    },
-    total=False,
-)
-
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-        "ConfigRuleName": str,
-        "AccountId": str,
-        "AwsRegion": str,
-    },
-)
-_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceType": ComplianceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
 _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigRuleName": str,
         "AccountId": str,
         "AwsRegion": str,
@@ -1695,35 +1416,14 @@
     "GroupedResourceCountTypeDef",
     {
         "GroupName": str,
         "ResourceCount": int,
     },
 )
 
-_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleName": str,
-    },
-)
-_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
 _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
@@ -1738,26 +1438,14 @@
 
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "ResourceEvaluationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetComplianceDetailsByResourceRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
@@ -1770,34 +1458,14 @@
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
     {
         "ResourceTypes": Sequence[str],
     },
     total=False,
 )
 
-_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-    },
-)
-_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
-    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
     },
 )
 _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -1819,22 +1487,14 @@
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
 
-GetCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredResourceCountsRequestRequestTypeDef = TypedDict(
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[str],
         "limit": int,
         "nextToken": str,
     },
@@ -1918,46 +1578,14 @@
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
-GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
-    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
@@ -1982,98 +1610,71 @@
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
-_RequiredResourceDetailsOutputTypeDef = TypedDict(
-    "_RequiredResourceDetailsOutputTypeDef",
+_RequiredResourceDetailsTypeDef = TypedDict(
+    "_RequiredResourceDetailsTypeDef",
     {
         "ResourceId": str,
         "ResourceType": str,
         "ResourceConfiguration": str,
     },
 )
-_OptionalResourceDetailsOutputTypeDef = TypedDict(
-    "_OptionalResourceDetailsOutputTypeDef",
+_OptionalResourceDetailsTypeDef = TypedDict(
+    "_OptionalResourceDetailsTypeDef",
     {
         "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
     },
     total=False,
 )
 
-class ResourceDetailsOutputTypeDef(
-    _RequiredResourceDetailsOutputTypeDef, _OptionalResourceDetailsOutputTypeDef
-):
+class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
     pass
 
 GetStoredQueryRequestRequestTypeDef = TypedDict(
     "GetStoredQueryRequestRequestTypeDef",
     {
         "QueryName": str,
     },
 )
 
-_RequiredStoredQueryOutputTypeDef = TypedDict(
-    "_RequiredStoredQueryOutputTypeDef",
+_RequiredStoredQueryTypeDef = TypedDict(
+    "_RequiredStoredQueryTypeDef",
     {
         "QueryName": str,
     },
 )
-_OptionalStoredQueryOutputTypeDef = TypedDict(
-    "_OptionalStoredQueryOutputTypeDef",
+_OptionalStoredQueryTypeDef = TypedDict(
+    "_OptionalStoredQueryTypeDef",
     {
         "QueryId": str,
         "QueryArn": str,
         "Description": str,
         "Expression": str,
     },
     total=False,
 )
 
-class StoredQueryOutputTypeDef(
-    _RequiredStoredQueryOutputTypeDef, _OptionalStoredQueryOutputTypeDef
-):
+class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
     pass
 
 ResourceFiltersTypeDef = TypedDict(
     "ResourceFiltersTypeDef",
     {
         "AccountId": str,
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
     },
     total=False,
 )
 
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceIds": Sequence[str],
-        "resourceName": str,
-        "includeDeletedResources": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
@@ -2141,34 +1742,14 @@
 )
 
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -2182,16 +1763,16 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -2361,76 +1942,14 @@
 )
 
 class OrganizationManagedRuleMetadataTypeDef(
     _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
 ):
     pass
 
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
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-_RequiredTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_RequiredTemplateSSMDocumentDetailsTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalTemplateSSMDocumentDetailsTypeDef = TypedDict(
-    "_OptionalTemplateSSMDocumentDetailsTypeDef",
-    {
-        "DocumentVersion": str,
-    },
-    total=False,
-)
-
-class TemplateSSMDocumentDetailsTypeDef(
-    _RequiredTemplateSSMDocumentDetailsTypeDef, _OptionalTemplateSSMDocumentDetailsTypeDef
-):
-    pass
-
-PutConformancePackResponseTypeDef = TypedDict(
-    "PutConformancePackResponseTypeDef",
-    {
-        "ConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutOrganizationConfigRuleResponseTypeDef = TypedDict(
-    "PutOrganizationConfigRuleResponseTypeDef",
-    {
-        "OrganizationConfigRuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutOrganizationConformancePackResponseTypeDef = TypedDict(
-    "PutOrganizationConformancePackResponseTypeDef",
-    {
-        "OrganizationConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -2453,50 +1972,14 @@
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
-_RequiredStoredQueryTypeDef = TypedDict(
-    "_RequiredStoredQueryTypeDef",
-    {
-        "QueryName": str,
-    },
-)
-_OptionalStoredQueryTypeDef = TypedDict(
-    "_OptionalStoredQueryTypeDef",
-    {
-        "QueryId": str,
-        "QueryArn": str,
-        "Description": str,
-        "Expression": str,
-    },
-    total=False,
-)
-
-class StoredQueryTypeDef(_RequiredStoredQueryTypeDef, _OptionalStoredQueryTypeDef):
-    pass
-
-PutStoredQueryResponseTypeDef = TypedDict(
-    "PutStoredQueryResponseTypeDef",
-    {
-        "QueryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RecordingStrategyOutputTypeDef = TypedDict(
-    "RecordingStrategyOutputTypeDef",
-    {
-        "useOnly": RecordingStrategyTypeType,
-    },
-    total=False,
-)
-
 RecordingStrategyTypeDef = TypedDict(
     "RecordingStrategyTypeDef",
     {
         "useOnly": RecordingStrategyTypeType,
     },
     total=False,
 )
@@ -2509,81 +1992,44 @@
         "ErrorMessage": str,
         "StartTime": datetime,
         "StopTime": datetime,
     },
     total=False,
 )
 
-ResourceValueOutputTypeDef = TypedDict(
-    "ResourceValueOutputTypeDef",
+ResourceValueTypeDef = TypedDict(
+    "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
 StaticValueOutputTypeDef = TypedDict(
     "StaticValueOutputTypeDef",
     {
         "Values": List[str],
     },
 )
 
-ResourceValueTypeDef = TypedDict(
-    "ResourceValueTypeDef",
-    {
-        "Value": Literal["RESOURCE_ID"],
-    },
-)
-
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-_RequiredResourceDetailsTypeDef = TypedDict(
-    "_RequiredResourceDetailsTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ResourceConfiguration": str,
-    },
-)
-_OptionalResourceDetailsTypeDef = TypedDict(
-    "_OptionalResourceDetailsTypeDef",
-    {
-        "ResourceConfigurationSchemaType": Literal["CFN_RESOURCE_SCHEMA"],
-    },
-    total=False,
-)
-
-class ResourceDetailsTypeDef(_RequiredResourceDetailsTypeDef, _OptionalResourceDetailsTypeDef):
-    pass
-
 TimeWindowTypeDef = TypedDict(
     "TimeWindowTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
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
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
         "ConfigurationAggregatorName": str,
     },
 )
@@ -2599,40 +2045,14 @@
 
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "Expression": str,
-            "ConfigurationAggregatorName": str,
-        },
-    )
-)
-_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "MaxResults": int,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
-    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-):
-    pass
-
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2646,44 +2066,14 @@
 
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
-    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-):
-    pass
-
-SourceDetailOutputTypeDef = TypedDict(
-    "SourceDetailOutputTypeDef",
-    {
-        "EventSource": Literal["aws.config"],
-        "MessageType": MessageTypeType,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-    },
-    total=False,
-)
-
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
     },
@@ -2701,22 +2091,14 @@
 StartConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StartConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
-StartResourceEvaluationResponseTypeDef = TypedDict(
-    "StartResourceEvaluationResponseTypeDef",
-    {
-        "ResourceEvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StopConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
@@ -2744,35 +2126,14 @@
     {
         "ComplianceSummary": AggregateConformancePackComplianceCountTypeDef,
         "GroupName": str,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
@@ -2810,23 +2171,14 @@
 
 class GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef(
     _RequiredGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     _OptionalGetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
 ):
     pass
 
-ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
-    {
-        "ResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchGetAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifiers": Sequence[AggregateResourceIdentifierTypeDef],
     },
 )
@@ -2835,76 +2187,144 @@
     "GetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifier": AggregateResourceIdentifierTypeDef,
     },
 )
 
+BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetAggregateResourceConfigResponseTypeDef",
+    {
+        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeliverConfigSnapshotResponseTypeDef = TypedDict(
+    "DeliverConfigSnapshotResponseTypeDef",
+    {
+        "configSnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
+    "DescribeAggregationAuthorizationsResponseTypeDef",
+    {
+        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeConfigurationAggregatorSourcesStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     {
         "AggregatedSourceStatusList": List[AggregatedSourceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
-    "DescribeAggregationAuthorizationsResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
+    {
+        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAggregationAuthorizationResponseTypeDef = TypedDict(
     "PutAggregationAuthorizationResponseTypeDef",
     {
         "AggregationAuthorization": AggregationAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+PutConformancePackResponseTypeDef = TypedDict(
+    "PutConformancePackResponseTypeDef",
     {
-        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
-    "BatchGetResourceConfigRequestRequestTypeDef",
+PutOrganizationConfigRuleResponseTypeDef = TypedDict(
+    "PutOrganizationConfigRuleResponseTypeDef",
     {
-        "resourceKeys": Sequence[ResourceKeyTypeDef],
+        "OrganizationConfigRuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+PutOrganizationConformancePackResponseTypeDef = TypedDict(
+    "PutOrganizationConformancePackResponseTypeDef",
     {
-        "ConfigRuleName": str,
+        "OrganizationConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+
+PutStoredQueryResponseTypeDef = TypedDict(
+    "PutStoredQueryResponseTypeDef",
     {
-        "ResourceKeys": Sequence[ResourceKeyTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "QueryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
-    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-):
-    pass
+StartResourceEvaluationResponseTypeDef = TypedDict(
+    "StartResourceEvaluationResponseTypeDef",
+    {
+        "ResourceEvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
+    "BatchGetResourceConfigRequestRequestTypeDef",
+    {
+        "resourceKeys": Sequence[ResourceKeyTypeDef],
+    },
+)
+
+BatchGetResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetResourceConfigResponseTypeDef",
+    {
+        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
@@ -2928,29 +2348,20 @@
     "StartRemediationExecutionRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[ResourceKeyTypeDef],
     },
 )
 
-BatchGetResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetResourceConfigResponseTypeDef",
-    {
-        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "unprocessedResourceKeys": List[ResourceKeyOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartRemediationExecutionResponseTypeDef = TypedDict(
     "StartRemediationExecutionResponseTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[ResourceKeyOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FailedItems": List[ResourceKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryTypeDef = TypedDict(
     "ComplianceSummaryTypeDef",
     {
         "CompliantResourceCount": ComplianceContributorCountTypeDef,
@@ -2965,35 +2376,14 @@
     {
         "ComplianceType": ComplianceTypeType,
         "ComplianceContributorCount": ComplianceContributorCountTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "Filters": ConfigRuleComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
@@ -3036,29 +2426,16 @@
     pass
 
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeliveryChannelOutputTypeDef = TypedDict(
-    "DeliveryChannelOutputTypeDef",
-    {
-        "name": str,
-        "s3BucketName": str,
-        "s3KeyPrefix": str,
-        "s3KmsKeyArn": str,
-        "snsTopicARN": str,
-        "configSnapshotDeliveryProperties": ConfigSnapshotDeliveryPropertiesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DeliveryChannelTypeDef = TypedDict(
     "DeliveryChannelTypeDef",
     {
         "name": str,
         "s3BucketName": str,
@@ -3120,15 +2497,15 @@
     total=False,
 )
 
 DescribeConfigurationRecorderStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     {
         "ConfigurationRecordersStatus": List[ConfigurationRecorderStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeConformancePackComplianceRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConformancePackComplianceRequestRequestTypeDef",
     {
         "ConformancePackName": str,
@@ -3151,15 +2528,15 @@
     pass
 
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConformancePackComplianceScoresRequestRequestTypeDef = TypedDict(
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     {
         "Filters": ConformancePackComplianceScoresFiltersTypeDef,
@@ -3172,15 +2549,15 @@
 )
 
 GetConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetConformancePackComplianceSummaryResponseTypeDef",
     {
         "ConformancePackComplianceSummaryList": List[ConformancePackComplianceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOrganizationConformancePackTypeDef = TypedDict(
     "_RequiredOrganizationConformancePackTypeDef",
     {
         "OrganizationConformancePackName": str,
@@ -3189,114 +2566,139 @@
     },
 )
 _OptionalOrganizationConformancePackTypeDef = TypedDict(
     "_OptionalOrganizationConformancePackTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
         "ExcludedAccounts": List[str],
     },
     total=False,
 )
 
 class OrganizationConformancePackTypeDef(
     _RequiredOrganizationConformancePackTypeDef, _OptionalOrganizationConformancePackTypeDef
 ):
     pass
 
+_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "OrganizationConformancePackName": str,
+    },
+)
+_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
+    {
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "ExcludedAccounts": Sequence[str],
+    },
+    total=False,
+)
+
+class PutOrganizationConformancePackRequestRequestTypeDef(
+    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
+    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
+):
+    pass
+
 _RequiredConformancePackDetailTypeDef = TypedDict(
     "_RequiredConformancePackDetailTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackArn": str,
         "ConformancePackId": str,
     },
 )
 _OptionalConformancePackDetailTypeDef = TypedDict(
     "_OptionalConformancePackDetailTypeDef",
     {
         "DeliveryS3Bucket": str,
         "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": List[ConformancePackInputParameterOutputTypeDef],
+        "ConformancePackInputParameters": List[ConformancePackInputParameterTypeDef],
         "LastUpdateRequestedTime": datetime,
         "CreatedBy": str,
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsOutputTypeDef,
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
 class ConformancePackDetailTypeDef(
     _RequiredConformancePackDetailTypeDef, _OptionalConformancePackDetailTypeDef
 ):
     pass
 
-_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
+_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConformancePackRequestRequestTypeDef",
     {
         "ConformancePackName": str,
     },
 )
-_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef",
+_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConformancePackRequestRequestTypeDef",
     {
-        "Filters": ConformancePackEvaluationFiltersTypeDef,
-        "Limit": int,
-        "NextToken": str,
+        "TemplateS3Uri": str,
+        "TemplateBody": str,
+        "DeliveryS3Bucket": str,
+        "DeliveryS3KeyPrefix": str,
+        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
+        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
     },
     total=False,
 )
 
-class GetConformancePackComplianceDetailsRequestRequestTypeDef(
-    _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
-    _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
+class PutConformancePackRequestRequestTypeDef(
+    _RequiredPutConformancePackRequestRequestTypeDef,
+    _OptionalPutConformancePackRequestRequestTypeDef,
 ):
     pass
 
-_RequiredPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConformancePackRequestRequestTypeDef",
+_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
-        "OrganizationConformancePackName": str,
+        "ConformancePackName": str,
     },
 )
-_OptionalPutOrganizationConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConformancePackRequestRequestTypeDef",
+_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef",
     {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "ExcludedAccounts": Sequence[str],
+        "Filters": ConformancePackEvaluationFiltersTypeDef,
+        "Limit": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-class PutOrganizationConformancePackRequestRequestTypeDef(
-    _RequiredPutOrganizationConformancePackRequestRequestTypeDef,
-    _OptionalPutOrganizationConformancePackRequestRequestTypeDef,
+class GetConformancePackComplianceDetailsRequestRequestTypeDef(
+    _RequiredGetConformancePackComplianceDetailsRequestRequestTypeDef,
+    _OptionalGetConformancePackComplianceDetailsRequestRequestTypeDef,
 ):
     pass
 
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePackStatusResponseTypeDef = TypedDict(
     "DescribeConformancePackStatusResponseTypeDef",
     {
         "ConformancePackStatusDetails": List[ConformancePackStatusDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
@@ -3322,14 +2724,23 @@
 
 class DescribeRemediationExceptionsRequestRequestTypeDef(
     _RequiredDescribeRemediationExceptionsRequestRequestTypeDef,
     _OptionalDescribeRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
+FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
+    "FailedDeleteRemediationExceptionsBatchTypeDef",
+    {
+        "FailureMessage": str,
+        "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
+    },
+    total=False,
+)
+
 _RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
 )
@@ -3344,20 +2755,414 @@
 
 class PutRemediationExceptionsRequestRequestTypeDef(
     _RequiredPutRemediationExceptionsRequestRequestTypeDef,
     _OptionalPutRemediationExceptionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "Filters": ConfigRuleComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+):
+    pass
+
+DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
+    TypedDict(
+        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
+    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+):
+    pass
+
+DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    {
+        "ConfigurationAggregatorNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    {
+        "ConfigRuleName": str,
+    },
+)
+_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    {
+        "ResourceKeys": Sequence[ResourceKeyTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
+    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+):
+    pass
+
+DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    {
+        "RetentionConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+        "ConfigRuleName": str,
+        "AccountId": str,
+        "AwsRegion": str,
+    },
+)
+_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceType": ComplianceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleName": str,
+    },
+)
+_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "ResourceEvaluationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+    },
+)
+_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
+    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "laterTime": Union[datetime, str],
+        "earlierTime": Union[datetime, str],
+        "chronologicalOrder": ChronologicalOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
+    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceIds": Sequence[str],
+        "resourceName": str,
+        "includeDeletedResources": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "Expression": str,
+            "ConfigurationAggregatorName": str,
+        },
+    )
+)
+_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "MaxResults": int,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
+    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+):
+    pass
+
+_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "Expression": str,
+    },
+)
+_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
+    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+):
+    pass
+
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeConfigRulesRequestRequestTypeDef",
     {
@@ -3369,42 +3174,42 @@
 )
 
 DescribeOrganizationConfigRuleStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     {
         "OrganizationConfigRuleStatuses": List[OrganizationConfigRuleStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePackStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     {
         "OrganizationConformancePackStatuses": List[OrganizationConformancePackStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePendingAggregationRequestsResponseTypeDef = TypedDict(
     "DescribePendingAggregationRequestsResponseTypeDef",
     {
         "PendingAggregationRequests": List[PendingAggregationRequestTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRemediationExceptionsResponseTypeDef = TypedDict(
     "DescribeRemediationExceptionsResponseTypeDef",
     {
         "RemediationExceptions": List[RemediationExceptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationExceptionBatchTypeDef = TypedDict(
     "FailedRemediationExceptionBatchTypeDef",
     {
         "FailureMessage": str,
@@ -3414,31 +3219,31 @@
 )
 
 DescribeRetentionConfigurationsResponseTypeDef = TypedDict(
     "DescribeRetentionConfigurationsResponseTypeDef",
     {
         "RetentionConfigurations": List[RetentionConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRetentionConfigurationResponseTypeDef = TypedDict(
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEvaluationsResponseTypeDef = TypedDict(
     "PutEvaluationsResponseTypeDef",
     {
         "FailedEvaluations": List[EvaluationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
@@ -3464,22 +3269,14 @@
 )
 
 class PutEvaluationsRequestRequestTypeDef(
     _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
 ):
     pass
 
-ExecutionControlsOutputTypeDef = TypedDict(
-    "ExecutionControlsOutputTypeDef",
-    {
-        "SsmControls": SsmControlsOutputTypeDef,
-    },
-    total=False,
-)
-
 ExecutionControlsTypeDef = TypedDict(
     "ExecutionControlsTypeDef",
     {
         "SsmControls": SsmControlsTypeDef,
     },
     total=False,
 )
@@ -3488,23 +3285,14 @@
     "PutExternalEvaluationRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ExternalEvaluation": ExternalEvaluationTypeDef,
     },
 )
 
-FailedDeleteRemediationExceptionsBatchTypeDef = TypedDict(
-    "FailedDeleteRemediationExceptionsBatchTypeDef",
-    {
-        "FailureMessage": str,
-        "FailedItems": List[RemediationExceptionResourceKeyOutputTypeDef],
-    },
-    total=False,
-)
-
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
     total=False,
 )
@@ -3535,39 +3323,39 @@
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetDiscoveredResourceCountsResponseTypeDef",
     {
         "totalDiscoveredResources": int,
         "resourceCounts": List[ResourceCountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "Filters": StatusDetailFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
@@ -3597,29 +3385,29 @@
     pass
 
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
@@ -3651,52 +3439,75 @@
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceEvaluationSummaryResponseTypeDef = TypedDict(
     "GetResourceEvaluationSummaryResponseTypeDef",
     {
         "ResourceEvaluationId": str,
         "EvaluationMode": EvaluationModeType,
         "EvaluationStatus": EvaluationStatusTypeDef,
         "EvaluationStartTimestamp": datetime,
         "Compliance": ComplianceTypeType,
-        "EvaluationContext": EvaluationContextOutputTypeDef,
-        "ResourceDetails": ResourceDetailsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EvaluationContext": EvaluationContextTypeDef,
+        "ResourceDetails": ResourceDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "ResourceDetails": ResourceDetailsTypeDef,
+        "EvaluationMode": EvaluationModeType,
+    },
+)
+_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
+    {
+        "EvaluationContext": EvaluationContextTypeDef,
+        "EvaluationTimeout": int,
+        "ClientToken": str,
     },
+    total=False,
 )
 
+class StartResourceEvaluationRequestRequestTypeDef(
+    _RequiredStartResourceEvaluationRequestRequestTypeDef,
+    _OptionalStartResourceEvaluationRequestRequestTypeDef,
+):
+    pass
+
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
-        "StoredQuery": StoredQueryOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StoredQuery": StoredQueryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "Filters": ResourceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
@@ -3727,113 +3538,93 @@
     pass
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceEvaluationsResponseTypeDef = TypedDict(
     "ListResourceEvaluationsResponseTypeDef",
     {
         "ResourceEvaluations": List[ResourceEvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStoredQueriesResponseTypeDef = TypedDict(
     "ListStoredQueriesResponseTypeDef",
     {
         "StoredQueryMetadata": List[StoredQueryMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredOrganizationConfigRuleTypeDef = TypedDict(
-    "_RequiredOrganizationConfigRuleTypeDef",
+_RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
-        "OrganizationConfigRuleArn": str,
+        "AuthorizedAccountId": str,
+        "AuthorizedAwsRegion": str,
     },
 )
-_OptionalOrganizationConfigRuleTypeDef = TypedDict(
-    "_OptionalOrganizationConfigRuleTypeDef",
+_OptionalPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
-        "ExcludedAccounts": List[str],
-        "LastUpdateTime": datetime,
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class OrganizationConfigRuleTypeDef(
-    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
+class PutAggregationAuthorizationRequestRequestTypeDef(
+    _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
+    _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
+_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationConfigRuleName": str,
+        "StoredQuery": StoredQueryTypeDef,
     },
 )
-_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
+_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalPutStoredQueryRequestRequestTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
-        "ExcludedAccounts": Sequence[str],
-        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class PutOrganizationConfigRuleRequestRequestTypeDef(
-    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
-    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
+class PutStoredQueryRequestRequestTypeDef(
+    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
 ):
     pass
 
-_RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
-    {
-        "AuthorizedAccountId": str,
-        "AuthorizedAwsRegion": str,
-    },
-)
-_OptionalPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutAggregationAuthorizationRequestRequestTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
+        "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-class PutAggregationAuthorizationRequestRequestTypeDef(
-    _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
-    _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
@@ -3848,74 +3639,69 @@
 
 class PutConfigurationAggregatorRequestRequestTypeDef(
     _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
     _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-_RequiredPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConformancePackRequestRequestTypeDef",
+_RequiredOrganizationConfigRuleTypeDef = TypedDict(
+    "_RequiredOrganizationConfigRuleTypeDef",
     {
-        "ConformancePackName": str,
+        "OrganizationConfigRuleName": str,
+        "OrganizationConfigRuleArn": str,
     },
 )
-_OptionalPutConformancePackRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConformancePackRequestRequestTypeDef",
+_OptionalOrganizationConfigRuleTypeDef = TypedDict(
+    "_OptionalOrganizationConfigRuleTypeDef",
     {
-        "TemplateS3Uri": str,
-        "TemplateBody": str,
-        "DeliveryS3Bucket": str,
-        "DeliveryS3KeyPrefix": str,
-        "ConformancePackInputParameters": Sequence[ConformancePackInputParameterTypeDef],
-        "TemplateSSMDocumentDetails": TemplateSSMDocumentDetailsTypeDef,
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
+        "ExcludedAccounts": List[str],
+        "LastUpdateTime": datetime,
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
-class PutConformancePackRequestRequestTypeDef(
-    _RequiredPutConformancePackRequestRequestTypeDef,
-    _OptionalPutConformancePackRequestRequestTypeDef,
+class OrganizationConfigRuleTypeDef(
+    _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
-_RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredPutStoredQueryRequestRequestTypeDef",
+_RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
-        "StoredQuery": StoredQueryTypeDef,
+        "OrganizationConfigRuleName": str,
     },
 )
-_OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalPutStoredQueryRequestRequestTypeDef",
+_OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalPutOrganizationConfigRuleRequestRequestTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
+        "ExcludedAccounts": Sequence[str],
+        "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataTypeDef,
     },
     total=False,
 )
 
-class PutStoredQueryRequestRequestTypeDef(
-    _RequiredPutStoredQueryRequestRequestTypeDef, _OptionalPutStoredQueryRequestRequestTypeDef
+class PutOrganizationConfigRuleRequestRequestTypeDef(
+    _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
+    _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
 RecordingGroupOutputTypeDef = TypedDict(
     "RecordingGroupOutputTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
         "resourceTypes": List[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
-        "recordingStrategy": RecordingStrategyOutputTypeDef,
+        "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
@@ -3927,64 +3713,41 @@
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
     "RemediationExecutionStatusTypeDef",
     {
-        "ResourceKey": ResourceKeyOutputTypeDef,
+        "ResourceKey": ResourceKeyTypeDef,
         "State": RemediationExecutionStateType,
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
 RemediationParameterValueOutputTypeDef = TypedDict(
     "RemediationParameterValueOutputTypeDef",
     {
-        "ResourceValue": ResourceValueOutputTypeDef,
+        "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueOutputTypeDef,
     },
     total=False,
 )
 
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-_RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "ResourceDetails": ResourceDetailsTypeDef,
-        "EvaluationMode": EvaluationModeType,
-    },
-)
-_OptionalStartResourceEvaluationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartResourceEvaluationRequestRequestTypeDef",
-    {
-        "EvaluationContext": EvaluationContextTypeDef,
-        "EvaluationTimeout": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class StartResourceEvaluationRequestRequestTypeDef(
-    _RequiredStartResourceEvaluationRequestRequestTypeDef,
-    _OptionalStartResourceEvaluationRequestRequestTypeDef,
-):
-    pass
-
 ResourceEvaluationFiltersTypeDef = TypedDict(
     "ResourceEvaluationFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
         "TimeWindow": TimeWindowTypeDef,
         "EvaluationContextIdentifier": str,
     },
@@ -3997,16 +3760,16 @@
         "Owner": OwnerType,
     },
 )
 _OptionalSourceOutputTypeDef = TypedDict(
     "_OptionalSourceOutputTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailOutputTypeDef],
-        "CustomPolicyDetails": CustomPolicyDetailsOutputTypeDef,
+        "SourceDetails": List[SourceDetailTypeDef],
+        "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
 class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
     pass
 
@@ -4030,27 +3793,27 @@
     pass
 
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     {
         "AggregateConformancePackComplianceSummaries": List[
             AggregateConformancePackComplianceSummaryTypeDef
         ],
         "GroupByKey": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceCountTypeDef = TypedDict(
     "AggregateComplianceCountTypeDef",
     {
         "GroupName": str,
@@ -4068,15 +3831,15 @@
     total=False,
 )
 
 GetComplianceSummaryByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     {
         "ComplianceSummary": ComplianceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceByConfigRuleTypeDef = TypedDict(
     "AggregateComplianceByConfigRuleTypeDef",
     {
         "ConfigRuleName": str,
@@ -4105,91 +3868,99 @@
     },
     total=False,
 )
 
 DescribeDeliveryChannelsResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelsResponseTypeDef",
     {
-        "DeliveryChannels": List[DeliveryChannelOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeliveryChannels": List[DeliveryChannelTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDeliveryChannelRequestRequestTypeDef = TypedDict(
     "PutDeliveryChannelRequestRequestTypeDef",
     {
         "DeliveryChannel": DeliveryChannelTypeDef,
     },
 )
 
 DescribeDeliveryChannelStatusResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelStatusResponseTypeDef",
     {
         "DeliveryChannelsStatus": List[DeliveryChannelStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationAggregatorsResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsResponseTypeDef",
     {
         "ConfigurationAggregators": List[ConfigurationAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationAggregatorResponseTypeDef = TypedDict(
     "PutConfigurationAggregatorResponseTypeDef",
     {
         "ConfigurationAggregator": ConfigurationAggregatorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateResourceConfigResponseTypeDef = TypedDict(
     "GetAggregateResourceConfigResponseTypeDef",
     {
         "ConfigurationItem": ConfigurationItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceConfigHistoryResponseTypeDef = TypedDict(
     "GetResourceConfigHistoryResponseTypeDef",
     {
         "configurationItems": List[ConfigurationItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePacksResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksResponseTypeDef",
     {
         "OrganizationConformancePacks": List[OrganizationConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePacksResponseTypeDef = TypedDict(
     "DescribeConformancePacksResponseTypeDef",
     {
         "ConformancePackDetails": List[ConformancePackDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRemediationExceptionsResponseTypeDef = TypedDict(
+    "DeleteRemediationExceptionsResponseTypeDef",
+    {
+        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRemediationExceptionsResponseTypeDef = TypedDict(
     "PutRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationExceptionBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateEvaluationResultTypeDef = TypedDict(
     "AggregateEvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
@@ -4234,48 +4005,40 @@
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
-DeleteRemediationExceptionsResponseTypeDef = TypedDict(
-    "DeleteRemediationExceptionsResponseTypeDef",
-    {
-        "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectResourceConfigResponseTypeDef = TypedDict(
     "SelectResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigRulesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesResponseTypeDef",
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationRecorderOutputTypeDef = TypedDict(
     "ConfigurationRecorderOutputTypeDef",
     {
         "name": str,
@@ -4296,15 +4059,15 @@
 )
 
 DescribeRemediationExecutionStatusResponseTypeDef = TypedDict(
     "DescribeRemediationExecutionStatusResponseTypeDef",
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRemediationConfigurationOutputTypeDef = TypedDict(
     "_RequiredRemediationConfigurationOutputTypeDef",
     {
         "ConfigRuleName": str,
@@ -4315,15 +4078,15 @@
 _OptionalRemediationConfigurationOutputTypeDef = TypedDict(
     "_OptionalRemediationConfigurationOutputTypeDef",
     {
         "TargetVersion": str,
         "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
         "ResourceType": str,
         "Automatic": bool,
-        "ExecutionControls": ExecutionControlsOutputTypeDef,
+        "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
     },
     total=False,
 )
@@ -4362,15 +4125,15 @@
 ):
     pass
 
 ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     {
         "Filters": ResourceEvaluationFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
     "ListResourceEvaluationsRequestRequestTypeDef",
     {
@@ -4395,15 +4158,15 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeOutputTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationOutputTypeDef],
+        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
 class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
     pass
 
@@ -4435,110 +4198,110 @@
 
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceSummaryByResourceTypeResponseTypeDef = TypedDict(
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     {
         "ComplianceSummariesByResourceType": List[ComplianceSummaryByResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAggregateComplianceByConfigRulesResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     {
         "AggregateComplianceByConfigRules": List[AggregateComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByConfigRuleResponseTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleResponseTypeDef",
     {
         "ComplianceByConfigRules": List[ComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByResourceResponseTypeDef = TypedDict(
     "DescribeComplianceByResourceResponseTypeDef",
     {
         "ComplianceByResources": List[ComplianceByResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "AggregateEvaluationResults": List[AggregateEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConformancePackComplianceDetailsResponseTypeDef = TypedDict(
     "GetConformancePackComplianceDetailsResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleEvaluationResults": List[ConformancePackEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByResourceResponseTypeDef = TypedDict(
     "GetComplianceDetailsByResourceResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
         "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
         "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
@@ -4555,15 +4318,15 @@
 )
 
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
         "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
@@ -4582,10 +4345,10 @@
 ):
     pass
 
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/PKG-INFO` & `mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.28.12
-Summary: Type annotations for boto3.ConfigService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -512,47 +512,42 @@
 from mypy_boto3_config.type_defs import (
     AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
-    AggregateResourceIdentifierOutputTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
+    ResponseMetadataTypeDef,
     ResourceKeyTypeDef,
-    ResourceKeyOutputTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
-    EvaluationModeConfigurationOutputTypeDef,
-    ScopeOutputTypeDef,
     EvaluationModeConfigurationTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
-    ConfigSnapshotDeliveryPropertiesOutputTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
     OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
-    ConformancePackInputParameterOutputTypeDef,
-    TemplateSSMDocumentDetailsOutputTypeDef,
-    ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
+    TemplateSSMDocumentDetailsTypeDef,
+    ConformancePackEvaluationFiltersTypeDef,
     ConformancePackRuleComplianceTypeDef,
     ConformancePackStatusDetailTypeDef,
-    CustomPolicyDetailsOutputTypeDef,
     CustomPolicyDetailsTypeDef,
     DeleteAggregationAuthorizationRequestRequestTypeDef,
     DeleteConfigRuleRequestRequestTypeDef,
     DeleteConfigurationAggregatorRequestRequestTypeDef,
     DeleteConfigurationRecorderRequestRequestTypeDef,
     DeleteConformancePackRequestRequestTypeDef,
     DeleteDeliveryChannelRequestRequestTypeDef,
@@ -562,233 +557,220 @@
     DeletePendingAggregationRequestRequestRequestTypeDef,
     DeleteRemediationConfigurationRequestRequestTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     DeleteResourceConfigRequestRequestTypeDef,
     DeleteRetentionConfigurationRequestRequestTypeDef,
     DeleteStoredQueryRequestRequestTypeDef,
     DeliverConfigSnapshotRequestRequestTypeDef,
-    DeliverConfigSnapshotResponseTypeDef,
-    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAggregationAuthorizationsRequestRequestTypeDef,
-    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByConfigRuleRequestRequestTypeDef,
-    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeComplianceByResourceRequestRequestTypeDef,
-    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestRequestTypeDef,
     DescribeConfigRulesFiltersTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
-    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
     DescribeConfigurationAggregatorsRequestRequestTypeDef,
     DescribeConfigurationRecorderStatusRequestRequestTypeDef,
     DescribeConfigurationRecordersRequestRequestTypeDef,
-    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
     DescribeConformancePackStatusRequestRequestTypeDef,
-    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
     DescribeConformancePacksRequestRequestTypeDef,
     DescribeDeliveryChannelStatusRequestRequestTypeDef,
     DescribeDeliveryChannelsRequestRequestTypeDef,
-    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
     DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef,
     OrganizationConfigRuleStatusTypeDef,
-    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
     DescribeOrganizationConfigRulesRequestRequestTypeDef,
-    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
     DescribeOrganizationConformancePackStatusesRequestRequestTypeDef,
     OrganizationConformancePackStatusTypeDef,
-    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
     DescribeOrganizationConformancePacksRequestRequestTypeDef,
-    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribePendingAggregationRequestsRequestRequestTypeDef,
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
-    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluationContextOutputTypeDef,
     EvaluationContextTypeDef,
     EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
     EvaluationTypeDef,
     ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
-    SsmControlsOutputTypeDef,
     SsmControlsTypeDef,
     ExternalEvaluationTypeDef,
-    RemediationExceptionResourceKeyOutputTypeDef,
     FieldInfoTypeDef,
-    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
-    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
-    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
-    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     GetConformancePackComplianceSummaryRequestRequestTypeDef,
     GetCustomRulePolicyRequestRequestTypeDef,
-    GetCustomRulePolicyResponseTypeDef,
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetOrganizationCustomRulePolicyResponseTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
     GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
-    ResourceDetailsOutputTypeDef,
+    ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
-    StoredQueryOutputTypeDef,
+    StoredQueryTypeDef,
     ResourceFiltersTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     OrganizationCustomRuleMetadataOutputTypeDef,
     OrganizationManagedRuleMetadataOutputTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    TagTypeDef,
-    TemplateSSMDocumentDetailsTypeDef,
-    PutConformancePackResponseTypeDef,
-    PutOrganizationConfigRuleResponseTypeDef,
-    PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
-    StoredQueryTypeDef,
-    PutStoredQueryResponseTypeDef,
-    RecordingStrategyOutputTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
-    ResourceValueOutputTypeDef,
-    StaticValueOutputTypeDef,
     ResourceValueTypeDef,
+    StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    ResourceDetailsTypeDef,
     TimeWindowTypeDef,
-    ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
-    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
-    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-    SourceDetailOutputTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
-    StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
-    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    BatchGetAggregateResourceConfigResponseTypeDef,
+    DeliverConfigSnapshotResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCustomRulePolicyResponseTypeDef,
+    GetOrganizationCustomRulePolicyResponseTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
-    BatchGetAggregateResourceConfigResponseTypeDef,
+    PutConformancePackResponseTypeDef,
+    PutOrganizationConfigRuleResponseTypeDef,
+    PutOrganizationConformancePackResponseTypeDef,
+    PutStoredQueryResponseTypeDef,
+    StartResourceEvaluationResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
-    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    BatchGetResourceConfigResponseTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
-    BatchGetResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
-    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
-    DeliveryChannelOutputTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
     DescribeConfigurationRecorderStatusResponseTypeDef,
     DescribeConformancePackComplianceRequestRequestTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListConformancePackComplianceScoresRequestRequestTypeDef,
     GetConformancePackComplianceSummaryResponseTypeDef,
     OrganizationConformancePackTypeDef,
+    PutOrganizationConformancePackRequestRequestTypeDef,
     ConformancePackDetailTypeDef,
+    PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
-    PutOrganizationConformancePackRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
+    FailedDeleteRemediationExceptionsBatchTypeDef,
     PutRemediationExceptionsRequestRequestTypeDef,
+    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
+    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
+    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
+    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
+    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
+    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
+    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
+    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
+    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
+    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
+    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
+    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
+    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     EvaluationResultIdentifierTypeDef,
     PutEvaluationsRequestRequestTypeDef,
-    ExecutionControlsOutputTypeDef,
     ExecutionControlsTypeDef,
     PutExternalEvaluationRequestRequestTypeDef,
-    FailedDeleteRemediationExceptionsBatchTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef,
     GetOrganizationConformancePackDetailedStatusResponseTypeDef,
     GetResourceEvaluationSummaryResponseTypeDef,
+    StartResourceEvaluationRequestRequestTypeDef,
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationConfigRuleTypeDef,
-    PutOrganizationConfigRuleRequestRequestTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    PutConformancePackRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
+    OrganizationConfigRuleTypeDef,
+    PutOrganizationConfigRuleRequestRequestTypeDef,
     RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
     RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    StartResourceEvaluationRequestRequestTypeDef,
     ResourceEvaluationFiltersTypeDef,
     SourceOutputTypeDef,
     SourceTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
@@ -801,19 +783,19 @@
     DescribeDeliveryChannelStatusResponseTypeDef,
     DescribeConfigurationAggregatorsResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetResourceConfigHistoryResponseTypeDef,
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
+    DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
-    DeleteRemediationExceptionsResponseTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
     ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     RemediationConfigurationOutputTypeDef,
```

### Comparing `mypy-boto3-config-1.28.12/mypy_boto3_config.egg-info/SOURCES.txt` & `mypy-boto3-config-1.28.15/mypy_boto3_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.28.12/setup.py` & `mypy-boto3-config-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-config",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConfigService 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ConfigService 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

