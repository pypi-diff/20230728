# Comparing `tmp/mypy-boto3-kendra-1.28.12.tar.gz` & `tmp/mypy-boto3-kendra-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-1.28.12.tar", last modified: Thu Jul 27 05:34:52 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
```

## Comparing `mypy-boto3-kendra-1.28.12.tar` & `mypy-boto3-kendra-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27095 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25612 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-27 05:24:32.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   153110 2023-07-27 05:24:36.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   152891 2023-07-27 05:24:35.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27095 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:52.000000 mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:52.568472 mypy-boto3-kendra-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:24:31.000000 mypy-boto3-kendra-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.837303 mypy-boto3-kendra-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-07-28 20:43:02.833303 mypy-boto3-kendra-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24433 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.821303 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   144224 2023-07-28 20:29:07.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144013 2023-07-28 20:29:05.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:01.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.833303 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:02.000000 mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.837303 mypy-boto3-kendra-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:29:00.000000 mypy-boto3-kendra-1.28.15/setup.py
```

### Comparing `mypy-boto3-kendra-1.28.12/LICENSE` & `mypy-boto3-kendra-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.12/PKG-INFO` & `mypy-boto3-kendra-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-kendra
-Version: 1.28.12
-Summary: Type annotations for boto3.kendra 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kendra type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-kendra"></a>
 
 # mypy-boto3-kendra
 
 [![PyPI - mypy-boto3-kendra](https://img.shields.io/pypi/v/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra)](https://pepy.tech/project/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,135 +325,103 @@
 
 `mypy_boto3_kendra.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra.type_defs import (
     AccessControlConfigurationSummaryTypeDef,
-    AccessControlListConfigurationOutputTypeDef,
     AccessControlListConfigurationTypeDef,
-    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
-    DataSourceToIndexFieldMappingOutputTypeDef,
-    DataSourceVpcConfigurationOutputTypeDef,
-    S3PathOutputTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
-    DataSourceVpcConfigurationTypeDef,
+    DataSourceVpcConfigurationOutputTypeDef,
     S3PathTypeDef,
+    DataSourceVpcConfigurationTypeDef,
     EntityConfigurationTypeDef,
     FailedEntityTypeDef,
+    ResponseMetadataTypeDef,
     EntityPersonaConfigurationTypeDef,
-    SuggestableConfigOutputTypeDef,
     SuggestableConfigTypeDef,
-    BasicAuthenticationConfigurationOutputTypeDef,
     BasicAuthenticationConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
     BatchDeleteFeaturedResultsSetErrorTypeDef,
     BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
-    CapacityUnitsConfigurationOutputTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
     ClickFeedbackTypeDef,
-    ConfluenceAttachmentToIndexFieldMappingOutputTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
-    ConfluenceBlogToIndexFieldMappingOutputTypeDef,
     ConfluenceBlogToIndexFieldMappingTypeDef,
-    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
-    ConfluencePageToIndexFieldMappingOutputTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
-    ConfluenceSpaceToIndexFieldMappingOutputTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
-    ConnectionConfigurationOutputTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationOutputTypeDef,
     ContentSourceConfigurationTypeDef,
     CorrectionTypeDef,
     PrincipalTypeDef,
-    CreateAccessControlConfigurationResponseTypeDef,
     TagTypeDef,
-    CreateDataSourceResponseTypeDef,
-    CreateExperienceResponseTypeDef,
-    CreateFaqResponseTypeDef,
     FeaturedDocumentTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     UserGroupResolutionConfigurationTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateQuerySuggestionsBlockListResponseTypeDef,
-    CreateThesaurusResponseTypeDef,
     TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     DataSourceGroupTypeDef,
     DataSourceSummaryTypeDef,
     DataSourceSyncJobMetricsTypeDef,
-    SqlConfigurationOutputTypeDef,
     SqlConfigurationTypeDef,
     DeleteAccessControlConfigurationRequestRequestTypeDef,
     DeleteDataSourceRequestRequestTypeDef,
     DeleteExperienceRequestRequestTypeDef,
     DeleteFaqRequestRequestTypeDef,
     DeleteIndexRequestRequestTypeDef,
     DeletePrincipalMappingRequestRequestTypeDef,
     DeleteQuerySuggestionsBlockListRequestRequestTypeDef,
     DeleteThesaurusRequestRequestTypeDef,
     DescribeAccessControlConfigurationRequestRequestTypeDef,
-    PrincipalOutputTypeDef,
     DescribeDataSourceRequestRequestTypeDef,
     DescribeExperienceRequestRequestTypeDef,
     ExperienceEndpointTypeDef,
     DescribeFaqRequestRequestTypeDef,
     DescribeFeaturedResultsSetRequestRequestTypeDef,
     FeaturedDocumentMissingTypeDef,
     FeaturedDocumentWithMetadataTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
-    UserGroupResolutionConfigurationOutputTypeDef,
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueOutputTypeDef,
     DocumentAttributeValueTypeDef,
     RelevanceOutputTypeDef,
-    SearchOutputTypeDef,
-    RelevanceTypeDef,
     SearchTypeDef,
-    DocumentsMetadataConfigurationOutputTypeDef,
+    RelevanceTypeDef,
     DocumentsMetadataConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EntityDisplayDataTypeDef,
-    UserIdentityConfigurationOutputTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
     FacetTypeDef,
     FaqStatisticsTypeDef,
     FaqSummaryTypeDef,
-    FeaturedDocumentOutputTypeDef,
     FeaturedResultsSetSummaryTypeDef,
     GetSnapshotsRequestRequestTypeDef,
     TimeRangeOutputTypeDef,
-    GitHubDocumentCrawlPropertiesOutputTypeDef,
-    SaaSConfigurationOutputTypeDef,
     GitHubDocumentCrawlPropertiesTypeDef,
     SaaSConfigurationTypeDef,
     MemberGroupTypeDef,
     MemberUserTypeDef,
     GroupSummaryTypeDef,
     HighlightTypeDef,
     IndexConfigurationSummaryTypeDef,
     TextDocumentStatisticsTypeDef,
-    JsonTokenTypeConfigurationOutputTypeDef,
     JsonTokenTypeConfigurationTypeDef,
-    JwtTokenTypeConfigurationOutputTypeDef,
     JwtTokenTypeConfigurationTypeDef,
     ListAccessControlConfigurationsRequestRequestTypeDef,
     TimeRangeTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
@@ -493,81 +429,86 @@
     ListFaqsRequestRequestTypeDef,
     ListFeaturedResultsSetsRequestRequestTypeDef,
     ListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListQuerySuggestionsBlockListsRequestRequestTypeDef,
     QuerySuggestionsBlockListSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListThesauriRequestRequestTypeDef,
     ThesaurusSummaryTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     ScoreAttributesTypeDef,
     WarningTypeDef,
     RelevanceFeedbackTypeDef,
-    ResponseMetadataTypeDef,
     SeedUrlConfigurationOutputTypeDef,
     SeedUrlConfigurationTypeDef,
     SiteMapsConfigurationOutputTypeDef,
     SiteMapsConfigurationTypeDef,
     StartDataSourceSyncJobRequestRequestTypeDef,
-    StartDataSourceSyncJobResponseTypeDef,
     StopDataSourceSyncJobRequestRequestTypeDef,
     SuggestionHighlightTypeDef,
     TableCellTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAccessControlConfigurationsResponseTypeDef,
     ColumnConfigurationOutputTypeDef,
+    ColumnConfigurationTypeDef,
     GoogleDriveConfigurationOutputTypeDef,
+    GoogleDriveConfigurationTypeDef,
     SalesforceChatterFeedConfigurationOutputTypeDef,
+    SalesforceChatterFeedConfigurationTypeDef,
     SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
+    SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
+    SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardObjectAttachmentConfigurationOutputTypeDef,
+    SalesforceStandardObjectAttachmentConfigurationTypeDef,
     SalesforceStandardObjectConfigurationOutputTypeDef,
+    SalesforceStandardObjectConfigurationTypeDef,
     ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
+    ServiceNowKnowledgeArticleConfigurationTypeDef,
     ServiceNowServiceCatalogConfigurationOutputTypeDef,
+    ServiceNowServiceCatalogConfigurationTypeDef,
     WorkDocsConfigurationOutputTypeDef,
+    WorkDocsConfigurationTypeDef,
     BoxConfigurationOutputTypeDef,
     FsxConfigurationOutputTypeDef,
     JiraConfigurationOutputTypeDef,
     QuipConfigurationOutputTypeDef,
     SlackConfigurationOutputTypeDef,
     AlfrescoConfigurationOutputTypeDef,
-    DescribeFaqResponseTypeDef,
-    DescribeQuerySuggestionsBlockListResponseTypeDef,
-    DescribeThesaurusResponseTypeDef,
-    OnPremiseConfigurationOutputTypeDef,
+    OnPremiseConfigurationTypeDef,
     OneDriveUsersOutputTypeDef,
-    ColumnConfigurationTypeDef,
-    GoogleDriveConfigurationTypeDef,
-    SalesforceChatterFeedConfigurationTypeDef,
-    SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
-    SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
-    SalesforceStandardObjectAttachmentConfigurationTypeDef,
-    SalesforceStandardObjectConfigurationTypeDef,
-    ServiceNowKnowledgeArticleConfigurationTypeDef,
-    ServiceNowServiceCatalogConfigurationTypeDef,
-    WorkDocsConfigurationTypeDef,
+    OneDriveUsersTypeDef,
+    UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
+    UpdateThesaurusRequestRequestTypeDef,
+    AlfrescoConfigurationTypeDef,
     BoxConfigurationTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
-    AlfrescoConfigurationTypeDef,
-    OnPremiseConfigurationTypeDef,
-    OneDriveUsersTypeDef,
-    UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
-    UpdateThesaurusRequestRequestTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
+    CreateAccessControlConfigurationResponseTypeDef,
+    CreateDataSourceResponseTypeDef,
+    CreateExperienceResponseTypeDef,
+    CreateFaqResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateQuerySuggestionsBlockListResponseTypeDef,
+    CreateThesaurusResponseTypeDef,
+    DescribeFaqResponseTypeDef,
+    DescribeQuerySuggestionsBlockListResponseTypeDef,
+    DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAccessControlConfigurationsResponseTypeDef,
+    StartDataSourceSyncJobResponseTypeDef,
     AssociatePersonasToEntitiesRequestRequestTypeDef,
     AttributeSuggestionsDescribeConfigTypeDef,
     AttributeSuggestionsUpdateConfigTypeDef,
     AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
@@ -581,83 +522,84 @@
     SharePointConfigurationOutputTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationOutputTypeDef,
     ConfluencePageConfigurationTypeDef,
     ConfluenceSpaceConfigurationOutputTypeDef,
     ConfluenceSpaceConfigurationTypeDef,
     SpellCorrectedQueryTypeDef,
+    HierarchicalPrincipalOutputTypeDef,
     HierarchicalPrincipalTypeDef,
     CreateFaqRequestRequestTypeDef,
     CreateQuerySuggestionsBlockListRequestRequestTypeDef,
     CreateThesaurusRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedResultsSetTypeDef,
     UpdateFeaturedResultsSetRequestRequestTypeDef,
     UserContextTypeDef,
     ListDataSourcesResponseTypeDef,
     DataSourceSyncJobTypeDef,
-    HierarchicalPrincipalOutputTypeDef,
     ExperiencesSummaryTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionOutputTypeDef,
     DocumentAttributeOutputTypeDef,
     DocumentAttributeTargetOutputTypeDef,
     DocumentAttributeValueCountPairTypeDef,
     DocumentAttributeConditionTypeDef,
     DocumentAttributeTargetTypeDef,
     DocumentAttributeTypeDef,
     DocumentMetadataConfigurationOutputTypeDef,
-    DocumentRelevanceConfigurationTypeDef,
     DocumentMetadataConfigurationTypeDef,
+    DocumentRelevanceConfigurationTypeDef,
     S3DataSourceConfigurationOutputTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationOutputTypeDef,
     ExperienceConfigurationTypeDef,
     ListFaqsResponseTypeDef,
-    FeaturedResultsSetTypeDef,
     ListFeaturedResultsSetsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
-    UserTokenConfigurationOutputTypeDef,
     UserTokenConfigurationTypeDef,
     ListDataSourceSyncJobsRequestRequestTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListThesauriResponseTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     UrlsOutputTypeDef,
     UrlsTypeDef,
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationOutputTypeDef,
-    SalesforceKnowledgeArticleConfigurationOutputTypeDef,
-    ServiceNowConfigurationOutputTypeDef,
-    GitHubConfigurationOutputTypeDef,
-    OneDriveConfigurationOutputTypeDef,
     DatabaseConfigurationTypeDef,
+    SalesforceKnowledgeArticleConfigurationOutputTypeDef,
     SalesforceKnowledgeArticleConfigurationTypeDef,
+    ServiceNowConfigurationOutputTypeDef,
     ServiceNowConfigurationTypeDef,
+    GitHubConfigurationOutputTypeDef,
     GitHubConfigurationTypeDef,
+    OneDriveConfigurationOutputTypeDef,
     OneDriveConfigurationTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     UpdateQuerySuggestionsConfigRequestRequestTypeDef,
     ConfluenceConfigurationOutputTypeDef,
     ConfluenceConfigurationTypeDef,
+    DescribeAccessControlConfigurationResponseTypeDef,
     CreateAccessControlConfigurationRequestRequestTypeDef,
     UpdateAccessControlConfigurationRequestRequestTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
     AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
-    DescribeAccessControlConfigurationResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationOutputTypeDef,
     RetrieveResultItemTypeDef,
     SourceDocumentTypeDef,
     InlineCustomDocumentEnrichmentConfigurationOutputTypeDef,
     HookConfigurationTypeDef,
     InlineCustomDocumentEnrichmentConfigurationTypeDef,
@@ -666,20 +608,18 @@
     DocumentTypeDef,
     QueryRequestRequestTypeDef,
     RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
     UpdateExperienceRequestRequestTypeDef,
-    CreateFeaturedResultsSetResponseTypeDef,
-    UpdateFeaturedResultsSetResponseTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
-    DescribeIndexResponseTypeDef,
     CreateIndexRequestRequestTypeDef,
+    DescribeIndexResponseTypeDef,
     UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationOutputTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationOutputTypeDef,
     SalesforceConfigurationTypeDef,
```

### Comparing `mypy-boto3-kendra-1.28.12/README.md` & `mypy-boto3-kendra-1.28.15/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-kendra
+Version: 1.28.15
+Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 kendra type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-kendra"></a>
 
 # mypy-boto3-kendra
 
 [![PyPI - mypy-boto3-kendra](https://img.shields.io/pypi/v/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra)](https://pepy.tech/project/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,135 +357,103 @@
 
 `mypy_boto3_kendra.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra.type_defs import (
     AccessControlConfigurationSummaryTypeDef,
-    AccessControlListConfigurationOutputTypeDef,
     AccessControlListConfigurationTypeDef,
-    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
-    DataSourceToIndexFieldMappingOutputTypeDef,
-    DataSourceVpcConfigurationOutputTypeDef,
-    S3PathOutputTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
-    DataSourceVpcConfigurationTypeDef,
+    DataSourceVpcConfigurationOutputTypeDef,
     S3PathTypeDef,
+    DataSourceVpcConfigurationTypeDef,
     EntityConfigurationTypeDef,
     FailedEntityTypeDef,
+    ResponseMetadataTypeDef,
     EntityPersonaConfigurationTypeDef,
-    SuggestableConfigOutputTypeDef,
     SuggestableConfigTypeDef,
-    BasicAuthenticationConfigurationOutputTypeDef,
     BasicAuthenticationConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
     BatchDeleteFeaturedResultsSetErrorTypeDef,
     BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
-    CapacityUnitsConfigurationOutputTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
     ClickFeedbackTypeDef,
-    ConfluenceAttachmentToIndexFieldMappingOutputTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
-    ConfluenceBlogToIndexFieldMappingOutputTypeDef,
     ConfluenceBlogToIndexFieldMappingTypeDef,
-    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
-    ConfluencePageToIndexFieldMappingOutputTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
-    ConfluenceSpaceToIndexFieldMappingOutputTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
-    ConnectionConfigurationOutputTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationOutputTypeDef,
     ContentSourceConfigurationTypeDef,
     CorrectionTypeDef,
     PrincipalTypeDef,
-    CreateAccessControlConfigurationResponseTypeDef,
     TagTypeDef,
-    CreateDataSourceResponseTypeDef,
-    CreateExperienceResponseTypeDef,
-    CreateFaqResponseTypeDef,
     FeaturedDocumentTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     UserGroupResolutionConfigurationTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateQuerySuggestionsBlockListResponseTypeDef,
-    CreateThesaurusResponseTypeDef,
     TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     DataSourceGroupTypeDef,
     DataSourceSummaryTypeDef,
     DataSourceSyncJobMetricsTypeDef,
-    SqlConfigurationOutputTypeDef,
     SqlConfigurationTypeDef,
     DeleteAccessControlConfigurationRequestRequestTypeDef,
     DeleteDataSourceRequestRequestTypeDef,
     DeleteExperienceRequestRequestTypeDef,
     DeleteFaqRequestRequestTypeDef,
     DeleteIndexRequestRequestTypeDef,
     DeletePrincipalMappingRequestRequestTypeDef,
     DeleteQuerySuggestionsBlockListRequestRequestTypeDef,
     DeleteThesaurusRequestRequestTypeDef,
     DescribeAccessControlConfigurationRequestRequestTypeDef,
-    PrincipalOutputTypeDef,
     DescribeDataSourceRequestRequestTypeDef,
     DescribeExperienceRequestRequestTypeDef,
     ExperienceEndpointTypeDef,
     DescribeFaqRequestRequestTypeDef,
     DescribeFeaturedResultsSetRequestRequestTypeDef,
     FeaturedDocumentMissingTypeDef,
     FeaturedDocumentWithMetadataTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
-    UserGroupResolutionConfigurationOutputTypeDef,
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueOutputTypeDef,
     DocumentAttributeValueTypeDef,
     RelevanceOutputTypeDef,
-    SearchOutputTypeDef,
-    RelevanceTypeDef,
     SearchTypeDef,
-    DocumentsMetadataConfigurationOutputTypeDef,
+    RelevanceTypeDef,
     DocumentsMetadataConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EntityDisplayDataTypeDef,
-    UserIdentityConfigurationOutputTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
     FacetTypeDef,
     FaqStatisticsTypeDef,
     FaqSummaryTypeDef,
-    FeaturedDocumentOutputTypeDef,
     FeaturedResultsSetSummaryTypeDef,
     GetSnapshotsRequestRequestTypeDef,
     TimeRangeOutputTypeDef,
-    GitHubDocumentCrawlPropertiesOutputTypeDef,
-    SaaSConfigurationOutputTypeDef,
     GitHubDocumentCrawlPropertiesTypeDef,
     SaaSConfigurationTypeDef,
     MemberGroupTypeDef,
     MemberUserTypeDef,
     GroupSummaryTypeDef,
     HighlightTypeDef,
     IndexConfigurationSummaryTypeDef,
     TextDocumentStatisticsTypeDef,
-    JsonTokenTypeConfigurationOutputTypeDef,
     JsonTokenTypeConfigurationTypeDef,
-    JwtTokenTypeConfigurationOutputTypeDef,
     JwtTokenTypeConfigurationTypeDef,
     ListAccessControlConfigurationsRequestRequestTypeDef,
     TimeRangeTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
@@ -461,81 +461,86 @@
     ListFaqsRequestRequestTypeDef,
     ListFeaturedResultsSetsRequestRequestTypeDef,
     ListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListQuerySuggestionsBlockListsRequestRequestTypeDef,
     QuerySuggestionsBlockListSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListThesauriRequestRequestTypeDef,
     ThesaurusSummaryTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     ScoreAttributesTypeDef,
     WarningTypeDef,
     RelevanceFeedbackTypeDef,
-    ResponseMetadataTypeDef,
     SeedUrlConfigurationOutputTypeDef,
     SeedUrlConfigurationTypeDef,
     SiteMapsConfigurationOutputTypeDef,
     SiteMapsConfigurationTypeDef,
     StartDataSourceSyncJobRequestRequestTypeDef,
-    StartDataSourceSyncJobResponseTypeDef,
     StopDataSourceSyncJobRequestRequestTypeDef,
     SuggestionHighlightTypeDef,
     TableCellTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAccessControlConfigurationsResponseTypeDef,
     ColumnConfigurationOutputTypeDef,
+    ColumnConfigurationTypeDef,
     GoogleDriveConfigurationOutputTypeDef,
+    GoogleDriveConfigurationTypeDef,
     SalesforceChatterFeedConfigurationOutputTypeDef,
+    SalesforceChatterFeedConfigurationTypeDef,
     SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
+    SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
+    SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardObjectAttachmentConfigurationOutputTypeDef,
+    SalesforceStandardObjectAttachmentConfigurationTypeDef,
     SalesforceStandardObjectConfigurationOutputTypeDef,
+    SalesforceStandardObjectConfigurationTypeDef,
     ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
+    ServiceNowKnowledgeArticleConfigurationTypeDef,
     ServiceNowServiceCatalogConfigurationOutputTypeDef,
+    ServiceNowServiceCatalogConfigurationTypeDef,
     WorkDocsConfigurationOutputTypeDef,
+    WorkDocsConfigurationTypeDef,
     BoxConfigurationOutputTypeDef,
     FsxConfigurationOutputTypeDef,
     JiraConfigurationOutputTypeDef,
     QuipConfigurationOutputTypeDef,
     SlackConfigurationOutputTypeDef,
     AlfrescoConfigurationOutputTypeDef,
-    DescribeFaqResponseTypeDef,
-    DescribeQuerySuggestionsBlockListResponseTypeDef,
-    DescribeThesaurusResponseTypeDef,
-    OnPremiseConfigurationOutputTypeDef,
+    OnPremiseConfigurationTypeDef,
     OneDriveUsersOutputTypeDef,
-    ColumnConfigurationTypeDef,
-    GoogleDriveConfigurationTypeDef,
-    SalesforceChatterFeedConfigurationTypeDef,
-    SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
-    SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
-    SalesforceStandardObjectAttachmentConfigurationTypeDef,
-    SalesforceStandardObjectConfigurationTypeDef,
-    ServiceNowKnowledgeArticleConfigurationTypeDef,
-    ServiceNowServiceCatalogConfigurationTypeDef,
-    WorkDocsConfigurationTypeDef,
+    OneDriveUsersTypeDef,
+    UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
+    UpdateThesaurusRequestRequestTypeDef,
+    AlfrescoConfigurationTypeDef,
     BoxConfigurationTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
-    AlfrescoConfigurationTypeDef,
-    OnPremiseConfigurationTypeDef,
-    OneDriveUsersTypeDef,
-    UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
-    UpdateThesaurusRequestRequestTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
+    CreateAccessControlConfigurationResponseTypeDef,
+    CreateDataSourceResponseTypeDef,
+    CreateExperienceResponseTypeDef,
+    CreateFaqResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateQuerySuggestionsBlockListResponseTypeDef,
+    CreateThesaurusResponseTypeDef,
+    DescribeFaqResponseTypeDef,
+    DescribeQuerySuggestionsBlockListResponseTypeDef,
+    DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAccessControlConfigurationsResponseTypeDef,
+    StartDataSourceSyncJobResponseTypeDef,
     AssociatePersonasToEntitiesRequestRequestTypeDef,
     AttributeSuggestionsDescribeConfigTypeDef,
     AttributeSuggestionsUpdateConfigTypeDef,
     AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
@@ -549,83 +554,84 @@
     SharePointConfigurationOutputTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationOutputTypeDef,
     ConfluencePageConfigurationTypeDef,
     ConfluenceSpaceConfigurationOutputTypeDef,
     ConfluenceSpaceConfigurationTypeDef,
     SpellCorrectedQueryTypeDef,
+    HierarchicalPrincipalOutputTypeDef,
     HierarchicalPrincipalTypeDef,
     CreateFaqRequestRequestTypeDef,
     CreateQuerySuggestionsBlockListRequestRequestTypeDef,
     CreateThesaurusRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedResultsSetTypeDef,
     UpdateFeaturedResultsSetRequestRequestTypeDef,
     UserContextTypeDef,
     ListDataSourcesResponseTypeDef,
     DataSourceSyncJobTypeDef,
-    HierarchicalPrincipalOutputTypeDef,
     ExperiencesSummaryTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionOutputTypeDef,
     DocumentAttributeOutputTypeDef,
     DocumentAttributeTargetOutputTypeDef,
     DocumentAttributeValueCountPairTypeDef,
     DocumentAttributeConditionTypeDef,
     DocumentAttributeTargetTypeDef,
     DocumentAttributeTypeDef,
     DocumentMetadataConfigurationOutputTypeDef,
-    DocumentRelevanceConfigurationTypeDef,
     DocumentMetadataConfigurationTypeDef,
+    DocumentRelevanceConfigurationTypeDef,
     S3DataSourceConfigurationOutputTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationOutputTypeDef,
     ExperienceConfigurationTypeDef,
     ListFaqsResponseTypeDef,
-    FeaturedResultsSetTypeDef,
     ListFeaturedResultsSetsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
-    UserTokenConfigurationOutputTypeDef,
     UserTokenConfigurationTypeDef,
     ListDataSourceSyncJobsRequestRequestTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListThesauriResponseTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     UrlsOutputTypeDef,
     UrlsTypeDef,
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationOutputTypeDef,
-    SalesforceKnowledgeArticleConfigurationOutputTypeDef,
-    ServiceNowConfigurationOutputTypeDef,
-    GitHubConfigurationOutputTypeDef,
-    OneDriveConfigurationOutputTypeDef,
     DatabaseConfigurationTypeDef,
+    SalesforceKnowledgeArticleConfigurationOutputTypeDef,
     SalesforceKnowledgeArticleConfigurationTypeDef,
+    ServiceNowConfigurationOutputTypeDef,
     ServiceNowConfigurationTypeDef,
+    GitHubConfigurationOutputTypeDef,
     GitHubConfigurationTypeDef,
+    OneDriveConfigurationOutputTypeDef,
     OneDriveConfigurationTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     UpdateQuerySuggestionsConfigRequestRequestTypeDef,
     ConfluenceConfigurationOutputTypeDef,
     ConfluenceConfigurationTypeDef,
+    DescribeAccessControlConfigurationResponseTypeDef,
     CreateAccessControlConfigurationRequestRequestTypeDef,
     UpdateAccessControlConfigurationRequestRequestTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
     AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
-    DescribeAccessControlConfigurationResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationOutputTypeDef,
     RetrieveResultItemTypeDef,
     SourceDocumentTypeDef,
     InlineCustomDocumentEnrichmentConfigurationOutputTypeDef,
     HookConfigurationTypeDef,
     InlineCustomDocumentEnrichmentConfigurationTypeDef,
@@ -634,20 +640,18 @@
     DocumentTypeDef,
     QueryRequestRequestTypeDef,
     RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
     UpdateExperienceRequestRequestTypeDef,
-    CreateFeaturedResultsSetResponseTypeDef,
-    UpdateFeaturedResultsSetResponseTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
-    DescribeIndexResponseTypeDef,
     CreateIndexRequestRequestTypeDef,
+    DescribeIndexResponseTypeDef,
     UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationOutputTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationOutputTypeDef,
     SalesforceConfigurationTypeDef,
```

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/__main__.py` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.kendra 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.kendra 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.py` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/client.pyi` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.py` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/literals.pyi` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/type_defs.py` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -82,138 +82,105 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessControlConfigurationSummaryTypeDef",
-    "AccessControlListConfigurationOutputTypeDef",
     "AccessControlListConfigurationTypeDef",
-    "AclConfigurationOutputTypeDef",
     "AclConfigurationTypeDef",
-    "DataSourceToIndexFieldMappingOutputTypeDef",
-    "DataSourceVpcConfigurationOutputTypeDef",
-    "S3PathOutputTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
-    "DataSourceVpcConfigurationTypeDef",
+    "DataSourceVpcConfigurationOutputTypeDef",
     "S3PathTypeDef",
+    "DataSourceVpcConfigurationTypeDef",
     "EntityConfigurationTypeDef",
     "FailedEntityTypeDef",
+    "ResponseMetadataTypeDef",
     "EntityPersonaConfigurationTypeDef",
-    "SuggestableConfigOutputTypeDef",
     "SuggestableConfigTypeDef",
-    "BasicAuthenticationConfigurationOutputTypeDef",
     "BasicAuthenticationConfigurationTypeDef",
     "DataSourceSyncJobMetricTargetTypeDef",
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     "BatchDeleteFeaturedResultsSetErrorTypeDef",
     "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
     "BatchGetDocumentStatusResponseErrorTypeDef",
     "StatusTypeDef",
     "BatchPutDocumentResponseFailedDocumentTypeDef",
-    "CapacityUnitsConfigurationOutputTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "ClearQuerySuggestionsRequestRequestTypeDef",
     "ClickFeedbackTypeDef",
-    "ConfluenceAttachmentToIndexFieldMappingOutputTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
-    "ConfluenceBlogToIndexFieldMappingOutputTypeDef",
     "ConfluenceBlogToIndexFieldMappingTypeDef",
-    "ProxyConfigurationOutputTypeDef",
     "ProxyConfigurationTypeDef",
-    "ConfluencePageToIndexFieldMappingOutputTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
-    "ConfluenceSpaceToIndexFieldMappingOutputTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
-    "ConnectionConfigurationOutputTypeDef",
     "ConnectionConfigurationTypeDef",
     "ContentSourceConfigurationOutputTypeDef",
     "ContentSourceConfigurationTypeDef",
     "CorrectionTypeDef",
     "PrincipalTypeDef",
-    "CreateAccessControlConfigurationResponseTypeDef",
     "TagTypeDef",
-    "CreateDataSourceResponseTypeDef",
-    "CreateExperienceResponseTypeDef",
-    "CreateFaqResponseTypeDef",
     "FeaturedDocumentTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "UserGroupResolutionConfigurationTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    "CreateThesaurusResponseTypeDef",
     "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "DataSourceGroupTypeDef",
     "DataSourceSummaryTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
-    "SqlConfigurationOutputTypeDef",
     "SqlConfigurationTypeDef",
     "DeleteAccessControlConfigurationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
     "DeleteExperienceRequestRequestTypeDef",
     "DeleteFaqRequestRequestTypeDef",
     "DeleteIndexRequestRequestTypeDef",
     "DeletePrincipalMappingRequestRequestTypeDef",
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     "DeleteThesaurusRequestRequestTypeDef",
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
-    "PrincipalOutputTypeDef",
     "DescribeDataSourceRequestRequestTypeDef",
     "DescribeExperienceRequestRequestTypeDef",
     "ExperienceEndpointTypeDef",
     "DescribeFaqRequestRequestTypeDef",
     "DescribeFeaturedResultsSetRequestRequestTypeDef",
     "FeaturedDocumentMissingTypeDef",
     "FeaturedDocumentWithMetadataTypeDef",
     "DescribeIndexRequestRequestTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    "UserGroupResolutionConfigurationOutputTypeDef",
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
     "DocumentAttributeValueOutputTypeDef",
     "DocumentAttributeValueTypeDef",
     "RelevanceOutputTypeDef",
-    "SearchOutputTypeDef",
-    "RelevanceTypeDef",
     "SearchTypeDef",
-    "DocumentsMetadataConfigurationOutputTypeDef",
+    "RelevanceTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EntityDisplayDataTypeDef",
-    "UserIdentityConfigurationOutputTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
     "FacetTypeDef",
     "FaqStatisticsTypeDef",
     "FaqSummaryTypeDef",
-    "FeaturedDocumentOutputTypeDef",
     "FeaturedResultsSetSummaryTypeDef",
     "GetSnapshotsRequestRequestTypeDef",
     "TimeRangeOutputTypeDef",
-    "GitHubDocumentCrawlPropertiesOutputTypeDef",
-    "SaaSConfigurationOutputTypeDef",
     "GitHubDocumentCrawlPropertiesTypeDef",
     "SaaSConfigurationTypeDef",
     "MemberGroupTypeDef",
     "MemberUserTypeDef",
     "GroupSummaryTypeDef",
     "HighlightTypeDef",
     "IndexConfigurationSummaryTypeDef",
     "TextDocumentStatisticsTypeDef",
-    "JsonTokenTypeConfigurationOutputTypeDef",
     "JsonTokenTypeConfigurationTypeDef",
-    "JwtTokenTypeConfigurationOutputTypeDef",
     "JwtTokenTypeConfigurationTypeDef",
     "ListAccessControlConfigurationsRequestRequestTypeDef",
     "TimeRangeTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListEntityPersonasRequestRequestTypeDef",
     "PersonasSummaryTypeDef",
     "ListExperienceEntitiesRequestRequestTypeDef",
@@ -221,81 +188,86 @@
     "ListFaqsRequestRequestTypeDef",
     "ListFeaturedResultsSetsRequestRequestTypeDef",
     "ListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     "ListIndicesRequestRequestTypeDef",
     "ListQuerySuggestionsBlockListsRequestRequestTypeDef",
     "QuerySuggestionsBlockListSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListThesauriRequestRequestTypeDef",
     "ThesaurusSummaryTypeDef",
     "SortingConfigurationTypeDef",
     "SpellCorrectionConfigurationTypeDef",
     "ScoreAttributesTypeDef",
     "WarningTypeDef",
     "RelevanceFeedbackTypeDef",
-    "ResponseMetadataTypeDef",
     "SeedUrlConfigurationOutputTypeDef",
     "SeedUrlConfigurationTypeDef",
     "SiteMapsConfigurationOutputTypeDef",
     "SiteMapsConfigurationTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
-    "StartDataSourceSyncJobResponseTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "SuggestionHighlightTypeDef",
     "TableCellTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListAccessControlConfigurationsResponseTypeDef",
     "ColumnConfigurationOutputTypeDef",
+    "ColumnConfigurationTypeDef",
     "GoogleDriveConfigurationOutputTypeDef",
+    "GoogleDriveConfigurationTypeDef",
     "SalesforceChatterFeedConfigurationOutputTypeDef",
+    "SalesforceChatterFeedConfigurationTypeDef",
     "SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
+    "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
+    "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
+    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     "SalesforceStandardObjectConfigurationOutputTypeDef",
+    "SalesforceStandardObjectConfigurationTypeDef",
     "ServiceNowKnowledgeArticleConfigurationOutputTypeDef",
+    "ServiceNowKnowledgeArticleConfigurationTypeDef",
     "ServiceNowServiceCatalogConfigurationOutputTypeDef",
+    "ServiceNowServiceCatalogConfigurationTypeDef",
     "WorkDocsConfigurationOutputTypeDef",
+    "WorkDocsConfigurationTypeDef",
     "BoxConfigurationOutputTypeDef",
     "FsxConfigurationOutputTypeDef",
     "JiraConfigurationOutputTypeDef",
     "QuipConfigurationOutputTypeDef",
     "SlackConfigurationOutputTypeDef",
     "AlfrescoConfigurationOutputTypeDef",
-    "DescribeFaqResponseTypeDef",
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    "DescribeThesaurusResponseTypeDef",
-    "OnPremiseConfigurationOutputTypeDef",
+    "OnPremiseConfigurationTypeDef",
     "OneDriveUsersOutputTypeDef",
-    "ColumnConfigurationTypeDef",
-    "GoogleDriveConfigurationTypeDef",
-    "SalesforceChatterFeedConfigurationTypeDef",
-    "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
-    "SalesforceStandardObjectConfigurationTypeDef",
-    "ServiceNowKnowledgeArticleConfigurationTypeDef",
-    "ServiceNowServiceCatalogConfigurationTypeDef",
-    "WorkDocsConfigurationTypeDef",
+    "OneDriveUsersTypeDef",
+    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+    "UpdateThesaurusRequestRequestTypeDef",
+    "AlfrescoConfigurationTypeDef",
     "BoxConfigurationTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
-    "AlfrescoConfigurationTypeDef",
-    "OnPremiseConfigurationTypeDef",
-    "OneDriveUsersTypeDef",
-    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
-    "UpdateThesaurusRequestRequestTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
     "AssociatePersonasToEntitiesResponseTypeDef",
+    "CreateAccessControlConfigurationResponseTypeDef",
+    "CreateDataSourceResponseTypeDef",
+    "CreateExperienceResponseTypeDef",
+    "CreateFaqResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    "CreateThesaurusResponseTypeDef",
+    "DescribeFaqResponseTypeDef",
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    "DescribeThesaurusResponseTypeDef",
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     "DisassociatePersonasFromEntitiesResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAccessControlConfigurationsResponseTypeDef",
+    "StartDataSourceSyncJobResponseTypeDef",
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
     "AttributeSuggestionsDescribeConfigTypeDef",
     "AttributeSuggestionsUpdateConfigTypeDef",
     "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
@@ -309,83 +281,84 @@
     "SharePointConfigurationOutputTypeDef",
     "SharePointConfigurationTypeDef",
     "ConfluencePageConfigurationOutputTypeDef",
     "ConfluencePageConfigurationTypeDef",
     "ConfluenceSpaceConfigurationOutputTypeDef",
     "ConfluenceSpaceConfigurationTypeDef",
     "SpellCorrectedQueryTypeDef",
+    "HierarchicalPrincipalOutputTypeDef",
     "HierarchicalPrincipalTypeDef",
     "CreateFaqRequestRequestTypeDef",
     "CreateQuerySuggestionsBlockListRequestRequestTypeDef",
     "CreateThesaurusRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateFeaturedResultsSetRequestRequestTypeDef",
+    "FeaturedResultsSetTypeDef",
     "UpdateFeaturedResultsSetRequestRequestTypeDef",
     "UserContextTypeDef",
     "ListDataSourcesResponseTypeDef",
     "DataSourceSyncJobTypeDef",
-    "HierarchicalPrincipalOutputTypeDef",
     "ExperiencesSummaryTypeDef",
     "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
     "DocumentAttributeConditionOutputTypeDef",
     "DocumentAttributeOutputTypeDef",
     "DocumentAttributeTargetOutputTypeDef",
     "DocumentAttributeValueCountPairTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "DocumentMetadataConfigurationOutputTypeDef",
-    "DocumentRelevanceConfigurationTypeDef",
     "DocumentMetadataConfigurationTypeDef",
+    "DocumentRelevanceConfigurationTypeDef",
     "S3DataSourceConfigurationOutputTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
     "ExperienceConfigurationOutputTypeDef",
     "ExperienceConfigurationTypeDef",
     "ListFaqsResponseTypeDef",
-    "FeaturedResultsSetTypeDef",
     "ListFeaturedResultsSetsResponseTypeDef",
     "GetSnapshotsResponseTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
-    "UserTokenConfigurationOutputTypeDef",
     "UserTokenConfigurationTypeDef",
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     "ListEntityPersonasResponseTypeDef",
     "ListQuerySuggestionsBlockListsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListThesauriResponseTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "UrlsOutputTypeDef",
     "UrlsTypeDef",
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
     "DatabaseConfigurationOutputTypeDef",
-    "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
-    "ServiceNowConfigurationOutputTypeDef",
-    "GitHubConfigurationOutputTypeDef",
-    "OneDriveConfigurationOutputTypeDef",
     "DatabaseConfigurationTypeDef",
+    "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
     "SalesforceKnowledgeArticleConfigurationTypeDef",
+    "ServiceNowConfigurationOutputTypeDef",
     "ServiceNowConfigurationTypeDef",
+    "GitHubConfigurationOutputTypeDef",
     "GitHubConfigurationTypeDef",
+    "OneDriveConfigurationOutputTypeDef",
     "OneDriveConfigurationTypeDef",
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
     "ConfluenceConfigurationOutputTypeDef",
     "ConfluenceConfigurationTypeDef",
+    "DescribeAccessControlConfigurationResponseTypeDef",
     "CreateAccessControlConfigurationRequestRequestTypeDef",
     "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "CreateFeaturedResultsSetResponseTypeDef",
+    "UpdateFeaturedResultsSetResponseTypeDef",
     "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
-    "DescribeAccessControlConfigurationResponseTypeDef",
     "ListExperiencesResponseTypeDef",
     "HookConfigurationOutputTypeDef",
     "RetrieveResultItemTypeDef",
     "SourceDocumentTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
     "HookConfigurationTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
@@ -394,20 +367,18 @@
     "DocumentTypeDef",
     "QueryRequestRequestTypeDef",
     "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
     "DescribeExperienceResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
-    "CreateFeaturedResultsSetResponseTypeDef",
-    "UpdateFeaturedResultsSetResponseTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
-    "DescribeIndexResponseTypeDef",
     "CreateIndexRequestRequestTypeDef",
+    "DescribeIndexResponseTypeDef",
     "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationOutputTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
     "SalesforceConfigurationOutputTypeDef",
     "SalesforceConfigurationTypeDef",
@@ -433,121 +404,73 @@
 AccessControlConfigurationSummaryTypeDef = TypedDict(
     "AccessControlConfigurationSummaryTypeDef",
     {
         "Id": str,
     },
 )
 
-AccessControlListConfigurationOutputTypeDef = TypedDict(
-    "AccessControlListConfigurationOutputTypeDef",
-    {
-        "KeyPath": str,
-    },
-    total=False,
-)
-
 AccessControlListConfigurationTypeDef = TypedDict(
     "AccessControlListConfigurationTypeDef",
     {
         "KeyPath": str,
     },
     total=False,
 )
 
-AclConfigurationOutputTypeDef = TypedDict(
-    "AclConfigurationOutputTypeDef",
-    {
-        "AllowedGroupsColumnName": str,
-    },
-)
-
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "AllowedGroupsColumnName": str,
     },
 )
 
-_RequiredDataSourceToIndexFieldMappingOutputTypeDef = TypedDict(
-    "_RequiredDataSourceToIndexFieldMappingOutputTypeDef",
+_RequiredDataSourceToIndexFieldMappingTypeDef = TypedDict(
+    "_RequiredDataSourceToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": str,
         "IndexFieldName": str,
     },
 )
-_OptionalDataSourceToIndexFieldMappingOutputTypeDef = TypedDict(
-    "_OptionalDataSourceToIndexFieldMappingOutputTypeDef",
+_OptionalDataSourceToIndexFieldMappingTypeDef = TypedDict(
+    "_OptionalDataSourceToIndexFieldMappingTypeDef",
     {
         "DateFieldFormat": str,
     },
     total=False,
 )
 
-
-class DataSourceToIndexFieldMappingOutputTypeDef(
-    _RequiredDataSourceToIndexFieldMappingOutputTypeDef,
-    _OptionalDataSourceToIndexFieldMappingOutputTypeDef,
+class DataSourceToIndexFieldMappingTypeDef(
+    _RequiredDataSourceToIndexFieldMappingTypeDef, _OptionalDataSourceToIndexFieldMappingTypeDef
 ):
     pass
 
-
 DataSourceVpcConfigurationOutputTypeDef = TypedDict(
     "DataSourceVpcConfigurationOutputTypeDef",
     {
         "SubnetIds": List[str],
         "SecurityGroupIds": List[str],
     },
 )
 
-S3PathOutputTypeDef = TypedDict(
-    "S3PathOutputTypeDef",
+S3PathTypeDef = TypedDict(
+    "S3PathTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-_RequiredDataSourceToIndexFieldMappingTypeDef = TypedDict(
-    "_RequiredDataSourceToIndexFieldMappingTypeDef",
-    {
-        "DataSourceFieldName": str,
-        "IndexFieldName": str,
-    },
-)
-_OptionalDataSourceToIndexFieldMappingTypeDef = TypedDict(
-    "_OptionalDataSourceToIndexFieldMappingTypeDef",
-    {
-        "DateFieldFormat": str,
-    },
-    total=False,
-)
-
-
-class DataSourceToIndexFieldMappingTypeDef(
-    _RequiredDataSourceToIndexFieldMappingTypeDef, _OptionalDataSourceToIndexFieldMappingTypeDef
-):
-    pass
-
-
 DataSourceVpcConfigurationTypeDef = TypedDict(
     "DataSourceVpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
 
-S3PathTypeDef = TypedDict(
-    "S3PathTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-
 EntityConfigurationTypeDef = TypedDict(
     "EntityConfigurationTypeDef",
     {
         "EntityId": str,
         "EntityType": EntityTypeType,
     },
 )
@@ -557,49 +480,42 @@
     {
         "EntityId": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-EntityPersonaConfigurationTypeDef = TypedDict(
-    "EntityPersonaConfigurationTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EntityId": str,
-        "Persona": PersonaType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-SuggestableConfigOutputTypeDef = TypedDict(
-    "SuggestableConfigOutputTypeDef",
+EntityPersonaConfigurationTypeDef = TypedDict(
+    "EntityPersonaConfigurationTypeDef",
     {
-        "AttributeName": str,
-        "Suggestable": bool,
+        "EntityId": str,
+        "Persona": PersonaType,
     },
-    total=False,
 )
 
 SuggestableConfigTypeDef = TypedDict(
     "SuggestableConfigTypeDef",
     {
         "AttributeName": str,
         "Suggestable": bool,
     },
     total=False,
 )
 
-BasicAuthenticationConfigurationOutputTypeDef = TypedDict(
-    "BasicAuthenticationConfigurationOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Credentials": str,
-    },
-)
-
 BasicAuthenticationConfigurationTypeDef = TypedDict(
     "BasicAuthenticationConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
         "Credentials": str,
     },
@@ -615,21 +531,19 @@
     "_OptionalDataSourceSyncJobMetricTargetTypeDef",
     {
         "DataSourceSyncJobId": str,
     },
     total=False,
 )
 
-
 class DataSourceSyncJobMetricTargetTypeDef(
     _RequiredDataSourceSyncJobMetricTargetTypeDef, _OptionalDataSourceSyncJobMetricTargetTypeDef
 ):
     pass
 
-
 BatchDeleteDocumentResponseFailedDocumentTypeDef = TypedDict(
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     {
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
@@ -680,22 +594,14 @@
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-CapacityUnitsConfigurationOutputTypeDef = TypedDict(
-    "CapacityUnitsConfigurationOutputTypeDef",
-    {
-        "StorageCapacityUnits": int,
-        "QueryCapacityUnits": int,
-    },
-)
-
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
     {
         "StorageCapacityUnits": int,
         "QueryCapacityUnits": int,
     },
 )
@@ -711,76 +617,34 @@
     "ClickFeedbackTypeDef",
     {
         "ResultId": str,
         "ClickTime": Union[datetime, str],
     },
 )
 
-ConfluenceAttachmentToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluenceAttachmentToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
-
 ConfluenceAttachmentToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-ConfluenceBlogToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluenceBlogToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluenceBlogFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
-
 ConfluenceBlogToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceBlogToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceBlogFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-_RequiredProxyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProxyConfigurationOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-    },
-)
-_OptionalProxyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProxyConfigurationOutputTypeDef",
-    {
-        "Credentials": str,
-    },
-    total=False,
-)
-
-
-class ProxyConfigurationOutputTypeDef(
-    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
     },
 )
@@ -788,72 +652,39 @@
     "_OptionalProxyConfigurationTypeDef",
     {
         "Credentials": str,
     },
     total=False,
 )
 
-
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
-
-ConfluencePageToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluencePageToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluencePageFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
-
 ConfluencePageToIndexFieldMappingTypeDef = TypedDict(
     "ConfluencePageToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluencePageFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-ConfluenceSpaceToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluenceSpaceToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluenceSpaceFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
-
 ConfluenceSpaceToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceSpaceFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-ConnectionConfigurationOutputTypeDef = TypedDict(
-    "ConnectionConfigurationOutputTypeDef",
-    {
-        "DatabaseHost": str,
-        "DatabasePort": int,
-        "DatabaseName": str,
-        "TableName": str,
-        "SecretArn": str,
-    },
-)
-
 ConnectionConfigurationTypeDef = TypedDict(
     "ConnectionConfigurationTypeDef",
     {
         "DatabaseHost": str,
         "DatabasePort": int,
         "DatabaseName": str,
         "TableName": str,
@@ -904,59 +735,25 @@
     "_OptionalPrincipalTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
-
 class PrincipalTypeDef(_RequiredPrincipalTypeDef, _OptionalPrincipalTypeDef):
     pass
 
-
-CreateAccessControlConfigurationResponseTypeDef = TypedDict(
-    "CreateAccessControlConfigurationResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateDataSourceResponseTypeDef = TypedDict(
-    "CreateDataSourceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateExperienceResponseTypeDef = TypedDict(
-    "CreateExperienceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFaqResponseTypeDef = TypedDict(
-    "CreateFaqResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FeaturedDocumentTypeDef = TypedDict(
     "FeaturedDocumentTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
@@ -972,38 +769,14 @@
 UserGroupResolutionConfigurationTypeDef = TypedDict(
     "UserGroupResolutionConfigurationTypeDef",
     {
         "UserGroupResolutionMode": UserGroupResolutionModeType,
     },
 )
 
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThesaurusResponseTypeDef = TypedDict(
-    "CreateThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TemplateConfigurationOutputTypeDef = TypedDict(
     "TemplateConfigurationOutputTypeDef",
     {
         "Template": Dict[str, Any],
     },
     total=False,
 )
@@ -1046,22 +819,14 @@
         "DocumentsDeleted": str,
         "DocumentsFailed": str,
         "DocumentsScanned": str,
     },
     total=False,
 )
 
-SqlConfigurationOutputTypeDef = TypedDict(
-    "SqlConfigurationOutputTypeDef",
-    {
-        "QueryIdentifiersEnclosingOption": QueryIdentifiersEnclosingOptionType,
-    },
-    total=False,
-)
-
 SqlConfigurationTypeDef = TypedDict(
     "SqlConfigurationTypeDef",
     {
         "QueryIdentifiersEnclosingOption": QueryIdentifiersEnclosingOptionType,
     },
     total=False,
 )
@@ -1117,22 +882,20 @@
     {
         "DataSourceId": str,
         "OrderingId": int,
     },
     total=False,
 )
 
-
 class DeletePrincipalMappingRequestRequestTypeDef(
     _RequiredDeletePrincipalMappingRequestRequestTypeDef,
     _OptionalDeletePrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
@@ -1149,35 +912,14 @@
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
 
-_RequiredPrincipalOutputTypeDef = TypedDict(
-    "_RequiredPrincipalOutputTypeDef",
-    {
-        "Name": str,
-        "Type": PrincipalTypeType,
-        "Access": ReadAccessTypeType,
-    },
-)
-_OptionalPrincipalOutputTypeDef = TypedDict(
-    "_OptionalPrincipalOutputTypeDef",
-    {
-        "DataSourceId": str,
-    },
-    total=False,
-)
-
-
-class PrincipalOutputTypeDef(_RequiredPrincipalOutputTypeDef, _OptionalPrincipalOutputTypeDef):
-    pass
-
-
 DescribeDataSourceRequestRequestTypeDef = TypedDict(
     "DescribeDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -1236,29 +978,14 @@
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-UserGroupResolutionConfigurationOutputTypeDef = TypedDict(
-    "UserGroupResolutionConfigurationOutputTypeDef",
-    {
-        "UserGroupResolutionMode": UserGroupResolutionModeType,
-    },
-)
-
 _RequiredDescribePrincipalMappingRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePrincipalMappingRequestRequestTypeDef",
     {
         "IndexId": str,
         "GroupId": str,
     },
 )
@@ -1266,22 +993,20 @@
     "_OptionalDescribePrincipalMappingRequestRequestTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
-
 class DescribePrincipalMappingRequestRequestTypeDef(
     _RequiredDescribePrincipalMappingRequestRequestTypeDef,
     _OptionalDescribePrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
-
 GroupOrderingIdSummaryTypeDef = TypedDict(
     "GroupOrderingIdSummaryTypeDef",
     {
         "Status": PrincipalMappingStatusType,
         "LastUpdatedAt": datetime,
         "ReceivedAt": datetime,
         "OrderingId": int,
@@ -1352,16 +1077,16 @@
         "Duration": str,
         "RankOrder": OrderType,
         "ValueImportanceMap": Dict[str, int],
     },
     total=False,
 )
 
-SearchOutputTypeDef = TypedDict(
-    "SearchOutputTypeDef",
+SearchTypeDef = TypedDict(
+    "SearchTypeDef",
     {
         "Facetable": bool,
         "Searchable": bool,
         "Displayable": bool,
         "Sortable": bool,
     },
     total=False,
@@ -1375,68 +1100,34 @@
         "Duration": str,
         "RankOrder": OrderType,
         "ValueImportanceMap": Mapping[str, int],
     },
     total=False,
 )
 
-SearchTypeDef = TypedDict(
-    "SearchTypeDef",
-    {
-        "Facetable": bool,
-        "Searchable": bool,
-        "Displayable": bool,
-        "Sortable": bool,
-    },
-    total=False,
-)
-
-DocumentsMetadataConfigurationOutputTypeDef = TypedDict(
-    "DocumentsMetadataConfigurationOutputTypeDef",
-    {
-        "S3Prefix": str,
-    },
-    total=False,
-)
-
 DocumentsMetadataConfigurationTypeDef = TypedDict(
     "DocumentsMetadataConfigurationTypeDef",
     {
         "S3Prefix": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EntityDisplayDataTypeDef = TypedDict(
     "EntityDisplayDataTypeDef",
     {
         "UserName": str,
         "GroupName": str,
         "IdentifiedUserName": str,
         "FirstName": str,
         "LastName": str,
     },
     total=False,
 )
 
-UserIdentityConfigurationOutputTypeDef = TypedDict(
-    "UserIdentityConfigurationOutputTypeDef",
-    {
-        "IdentityAttributeName": str,
-    },
-    total=False,
-)
-
 UserIdentityConfigurationTypeDef = TypedDict(
     "UserIdentityConfigurationTypeDef",
     {
         "IdentityAttributeName": str,
     },
     total=False,
 )
@@ -1478,22 +1169,14 @@
         "UpdatedAt": datetime,
         "FileFormat": FaqFileFormatType,
         "LanguageCode": str,
     },
     total=False,
 )
 
-FeaturedDocumentOutputTypeDef = TypedDict(
-    "FeaturedDocumentOutputTypeDef",
-    {
-        "Id": str,
-    },
-    total=False,
-)
-
 FeaturedResultsSetSummaryTypeDef = TypedDict(
     "FeaturedResultsSetSummaryTypeDef",
     {
         "FeaturedResultsSetId": str,
         "FeaturedResultsSetName": str,
         "Status": FeaturedResultsSetStatusType,
         "LastUpdatedTimestamp": int,
@@ -1515,52 +1198,28 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetSnapshotsRequestRequestTypeDef(
     _RequiredGetSnapshotsRequestRequestTypeDef, _OptionalGetSnapshotsRequestRequestTypeDef
 ):
     pass
 
-
 TimeRangeOutputTypeDef = TypedDict(
     "TimeRangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
-GitHubDocumentCrawlPropertiesOutputTypeDef = TypedDict(
-    "GitHubDocumentCrawlPropertiesOutputTypeDef",
-    {
-        "CrawlRepositoryDocuments": bool,
-        "CrawlIssue": bool,
-        "CrawlIssueComment": bool,
-        "CrawlIssueCommentAttachment": bool,
-        "CrawlPullRequest": bool,
-        "CrawlPullRequestComment": bool,
-        "CrawlPullRequestCommentAttachment": bool,
-    },
-    total=False,
-)
-
-SaaSConfigurationOutputTypeDef = TypedDict(
-    "SaaSConfigurationOutputTypeDef",
-    {
-        "OrganizationName": str,
-        "HostUrl": str,
-    },
-)
-
 GitHubDocumentCrawlPropertiesTypeDef = TypedDict(
     "GitHubDocumentCrawlPropertiesTypeDef",
     {
         "CrawlRepositoryDocuments": bool,
         "CrawlIssue": bool,
         "CrawlIssueComment": bool,
         "CrawlIssueCommentAttachment": bool,
@@ -1589,19 +1248,17 @@
     "_OptionalMemberGroupTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
-
 class MemberGroupTypeDef(_RequiredMemberGroupTypeDef, _OptionalMemberGroupTypeDef):
     pass
 
-
 MemberUserTypeDef = TypedDict(
     "MemberUserTypeDef",
     {
         "UserId": str,
     },
 )
 
@@ -1626,19 +1283,17 @@
     {
         "TopAnswer": bool,
         "Type": HighlightTypeType,
     },
     total=False,
 )
 
-
 class HighlightTypeDef(_RequiredHighlightTypeDef, _OptionalHighlightTypeDef):
     pass
 
-
 _RequiredIndexConfigurationSummaryTypeDef = TypedDict(
     "_RequiredIndexConfigurationSummaryTypeDef",
     {
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": IndexStatusType,
     },
@@ -1649,71 +1304,35 @@
         "Name": str,
         "Id": str,
         "Edition": IndexEditionType,
     },
     total=False,
 )
 
-
 class IndexConfigurationSummaryTypeDef(
     _RequiredIndexConfigurationSummaryTypeDef, _OptionalIndexConfigurationSummaryTypeDef
 ):
     pass
 
-
 TextDocumentStatisticsTypeDef = TypedDict(
     "TextDocumentStatisticsTypeDef",
     {
         "IndexedTextDocumentsCount": int,
         "IndexedTextBytes": int,
     },
 )
 
-JsonTokenTypeConfigurationOutputTypeDef = TypedDict(
-    "JsonTokenTypeConfigurationOutputTypeDef",
-    {
-        "UserNameAttributeField": str,
-        "GroupAttributeField": str,
-    },
-)
-
 JsonTokenTypeConfigurationTypeDef = TypedDict(
     "JsonTokenTypeConfigurationTypeDef",
     {
         "UserNameAttributeField": str,
         "GroupAttributeField": str,
     },
 )
 
-_RequiredJwtTokenTypeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredJwtTokenTypeConfigurationOutputTypeDef",
-    {
-        "KeyLocation": KeyLocationType,
-    },
-)
-_OptionalJwtTokenTypeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalJwtTokenTypeConfigurationOutputTypeDef",
-    {
-        "URL": str,
-        "SecretManagerArn": str,
-        "UserNameAttributeField": str,
-        "GroupAttributeField": str,
-        "Issuer": str,
-        "ClaimRegex": str,
-    },
-    total=False,
-)
-
-
-class JwtTokenTypeConfigurationOutputTypeDef(
-    _RequiredJwtTokenTypeConfigurationOutputTypeDef, _OptionalJwtTokenTypeConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredJwtTokenTypeConfigurationTypeDef = TypedDict(
     "_RequiredJwtTokenTypeConfigurationTypeDef",
     {
         "KeyLocation": KeyLocationType,
     },
 )
 _OptionalJwtTokenTypeConfigurationTypeDef = TypedDict(
@@ -1725,21 +1344,19 @@
         "GroupAttributeField": str,
         "Issuer": str,
         "ClaimRegex": str,
     },
     total=False,
 )
 
-
 class JwtTokenTypeConfigurationTypeDef(
     _RequiredJwtTokenTypeConfigurationTypeDef, _OptionalJwtTokenTypeConfigurationTypeDef
 ):
     pass
 
-
 _RequiredListAccessControlConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessControlConfigurationsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListAccessControlConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1747,22 +1364,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAccessControlConfigurationsRequestRequestTypeDef(
     _RequiredListAccessControlConfigurationsRequestRequestTypeDef,
     _OptionalListAccessControlConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
@@ -1779,21 +1394,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDataSourcesRequestRequestTypeDef(
     _RequiredListDataSourcesRequestRequestTypeDef, _OptionalListDataSourcesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListEntityPersonasRequestRequestTypeDef = TypedDict(
     "_RequiredListEntityPersonasRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -1802,22 +1415,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEntityPersonasRequestRequestTypeDef(
     _RequiredListEntityPersonasRequestRequestTypeDef,
     _OptionalListEntityPersonasRequestRequestTypeDef,
 ):
     pass
 
-
 PersonasSummaryTypeDef = TypedDict(
     "PersonasSummaryTypeDef",
     {
         "EntityId": str,
         "Persona": PersonaType,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
@@ -1836,22 +1447,20 @@
     "_OptionalListExperienceEntitiesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListExperienceEntitiesRequestRequestTypeDef(
     _RequiredListExperienceEntitiesRequestRequestTypeDef,
     _OptionalListExperienceEntitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListExperiencesRequestRequestTypeDef = TypedDict(
     "_RequiredListExperiencesRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListExperiencesRequestRequestTypeDef = TypedDict(
@@ -1859,21 +1468,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListExperiencesRequestRequestTypeDef(
     _RequiredListExperiencesRequestRequestTypeDef, _OptionalListExperiencesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListFaqsRequestRequestTypeDef = TypedDict(
     "_RequiredListFaqsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListFaqsRequestRequestTypeDef = TypedDict(
@@ -1881,21 +1488,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListFaqsRequestRequestTypeDef(
     _RequiredListFaqsRequestRequestTypeDef, _OptionalListFaqsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturedResultsSetsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
@@ -1903,22 +1508,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListFeaturedResultsSetsRequestRequestTypeDef(
     _RequiredListFeaturedResultsSetsRequestRequestTypeDef,
     _OptionalListFeaturedResultsSetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     {
         "IndexId": str,
         "OrderingId": int,
     },
 )
@@ -1928,22 +1531,20 @@
         "DataSourceId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListGroupsOlderThanOrderingIdRequestRequestTypeDef(
     _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     _OptionalListGroupsOlderThanOrderingIdRequestRequestTypeDef,
 ):
     pass
 
-
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1960,22 +1561,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListQuerySuggestionsBlockListsRequestRequestTypeDef(
     _RequiredListQuerySuggestionsBlockListsRequestRequestTypeDef,
     _OptionalListQuerySuggestionsBlockListsRequestRequestTypeDef,
 ):
     pass
 
-
 QuerySuggestionsBlockListSummaryTypeDef = TypedDict(
     "QuerySuggestionsBlockListSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": QuerySuggestionsBlockListStatusType,
         "CreatedAt": datetime,
@@ -1988,22 +1587,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 _RequiredListThesauriRequestRequestTypeDef = TypedDict(
     "_RequiredListThesauriRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListThesauriRequestRequestTypeDef = TypedDict(
@@ -2011,21 +1602,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListThesauriRequestRequestTypeDef(
     _RequiredListThesauriRequestRequestTypeDef, _OptionalListThesauriRequestRequestTypeDef
 ):
     pass
 
-
 ThesaurusSummaryTypeDef = TypedDict(
     "ThesaurusSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": ThesaurusStatusType,
         "CreatedAt": datetime,
@@ -2070,67 +1659,52 @@
     "RelevanceFeedbackTypeDef",
     {
         "ResultId": str,
         "RelevanceValue": RelevanceTypeType,
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
 _RequiredSeedUrlConfigurationOutputTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationOutputTypeDef",
     {
         "SeedUrls": List[str],
     },
 )
 _OptionalSeedUrlConfigurationOutputTypeDef = TypedDict(
     "_OptionalSeedUrlConfigurationOutputTypeDef",
     {
         "WebCrawlerMode": WebCrawlerModeType,
     },
     total=False,
 )
 
-
 class SeedUrlConfigurationOutputTypeDef(
     _RequiredSeedUrlConfigurationOutputTypeDef, _OptionalSeedUrlConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredSeedUrlConfigurationTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationTypeDef",
     {
         "SeedUrls": Sequence[str],
     },
 )
 _OptionalSeedUrlConfigurationTypeDef = TypedDict(
     "_OptionalSeedUrlConfigurationTypeDef",
     {
         "WebCrawlerMode": WebCrawlerModeType,
     },
     total=False,
 )
 
-
 class SeedUrlConfigurationTypeDef(
     _RequiredSeedUrlConfigurationTypeDef, _OptionalSeedUrlConfigurationTypeDef
 ):
     pass
 
-
 SiteMapsConfigurationOutputTypeDef = TypedDict(
     "SiteMapsConfigurationOutputTypeDef",
     {
         "SiteMaps": List[str],
     },
 )
 
@@ -2145,22 +1719,14 @@
     "StartDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
 
-StartDataSourceSyncJobResponseTypeDef = TypedDict(
-    "StartDataSourceSyncJobResponseTypeDef",
-    {
-        "ExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StopDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -2189,149 +1755,250 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListAccessControlConfigurationsResponseTypeDef = TypedDict(
-    "ListAccessControlConfigurationsResponseTypeDef",
-    {
-        "NextToken": str,
-        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredColumnConfigurationOutputTypeDef = TypedDict(
     "_RequiredColumnConfigurationOutputTypeDef",
     {
         "DocumentIdColumnName": str,
         "DocumentDataColumnName": str,
         "ChangeDetectingColumns": List[str],
     },
 )
 _OptionalColumnConfigurationOutputTypeDef = TypedDict(
     "_OptionalColumnConfigurationOutputTypeDef",
     {
         "DocumentTitleColumnName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class ColumnConfigurationOutputTypeDef(
     _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
 ):
     pass
 
+_RequiredColumnConfigurationTypeDef = TypedDict(
+    "_RequiredColumnConfigurationTypeDef",
+    {
+        "DocumentIdColumnName": str,
+        "DocumentDataColumnName": str,
+        "ChangeDetectingColumns": Sequence[str],
+    },
+)
+_OptionalColumnConfigurationTypeDef = TypedDict(
+    "_OptionalColumnConfigurationTypeDef",
+    {
+        "DocumentTitleColumnName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+class ColumnConfigurationTypeDef(
+    _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
+):
+    pass
 
 _RequiredGoogleDriveConfigurationOutputTypeDef = TypedDict(
     "_RequiredGoogleDriveConfigurationOutputTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGoogleDriveConfigurationOutputTypeDef = TypedDict(
     "_OptionalGoogleDriveConfigurationOutputTypeDef",
     {
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "ExcludeMimeTypes": List[str],
         "ExcludeUserAccounts": List[str],
         "ExcludeSharedDrives": List[str],
     },
     total=False,
 )
 
-
 class GoogleDriveConfigurationOutputTypeDef(
     _RequiredGoogleDriveConfigurationOutputTypeDef, _OptionalGoogleDriveConfigurationOutputTypeDef
 ):
     pass
 
+_RequiredGoogleDriveConfigurationTypeDef = TypedDict(
+    "_RequiredGoogleDriveConfigurationTypeDef",
+    {
+        "SecretArn": str,
+    },
+)
+_OptionalGoogleDriveConfigurationTypeDef = TypedDict(
+    "_OptionalGoogleDriveConfigurationTypeDef",
+    {
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "ExcludeMimeTypes": Sequence[str],
+        "ExcludeUserAccounts": Sequence[str],
+        "ExcludeSharedDrives": Sequence[str],
+    },
+    total=False,
+)
+
+class GoogleDriveConfigurationTypeDef(
+    _RequiredGoogleDriveConfigurationTypeDef, _OptionalGoogleDriveConfigurationTypeDef
+):
+    pass
 
 _RequiredSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceChatterFeedConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceChatterFeedConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "IncludeFilterTypes": List[SalesforceChatterFeedIncludeFilterTypeType],
     },
     total=False,
 )
 
-
 class SalesforceChatterFeedConfigurationOutputTypeDef(
     _RequiredSalesforceChatterFeedConfigurationOutputTypeDef,
     _OptionalSalesforceChatterFeedConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredSalesforceChatterFeedConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceChatterFeedConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceChatterFeedConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceChatterFeedConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "IncludeFilterTypes": Sequence[SalesforceChatterFeedIncludeFilterTypeType],
+    },
+    total=False,
+)
+
+class SalesforceChatterFeedConfigurationTypeDef(
+    _RequiredSalesforceChatterFeedConfigurationTypeDef,
+    _OptionalSalesforceChatterFeedConfigurationTypeDef,
+):
+    pass
 
 _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "Name": str,
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef(
     _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
     _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "Name": str,
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(
+    _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
+    _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
+):
+    pass
 
 _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef(
     _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
     _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(
+    _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
+    _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
+):
+    pass
 
 SalesforceStandardObjectAttachmentConfigurationOutputTypeDef = TypedDict(
     "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+SalesforceStandardObjectAttachmentConfigurationTypeDef = TypedDict(
+    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 _RequiredSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceStandardObjectConfigurationOutputTypeDef",
     {
@@ -2339,104 +2006,190 @@
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceStandardObjectConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SalesforceStandardObjectConfigurationOutputTypeDef(
     _RequiredSalesforceStandardObjectConfigurationOutputTypeDef,
     _OptionalSalesforceStandardObjectConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredSalesforceStandardObjectConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceStandardObjectConfigurationTypeDef",
+    {
+        "Name": SalesforceStandardObjectNameType,
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceStandardObjectConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceStandardObjectConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+class SalesforceStandardObjectConfigurationTypeDef(
+    _RequiredSalesforceStandardObjectConfigurationTypeDef,
+    _OptionalSalesforceStandardObjectConfigurationTypeDef,
+):
+    pass
 
 _RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
     "_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "IncludeAttachmentFilePatterns": List[str],
         "ExcludeAttachmentFilePatterns": List[str],
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "FilterQuery": str,
     },
     total=False,
 )
 
-
 class ServiceNowKnowledgeArticleConfigurationOutputTypeDef(
     _RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef,
     _OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_RequiredServiceNowKnowledgeArticleConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_OptionalServiceNowKnowledgeArticleConfigurationTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "IncludeAttachmentFilePatterns": Sequence[str],
+        "ExcludeAttachmentFilePatterns": Sequence[str],
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "FilterQuery": str,
+    },
+    total=False,
+)
+
+class ServiceNowKnowledgeArticleConfigurationTypeDef(
+    _RequiredServiceNowKnowledgeArticleConfigurationTypeDef,
+    _OptionalServiceNowKnowledgeArticleConfigurationTypeDef,
+):
+    pass
 
 _RequiredServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
     "_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "IncludeAttachmentFilePatterns": List[str],
         "ExcludeAttachmentFilePatterns": List[str],
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class ServiceNowServiceCatalogConfigurationOutputTypeDef(
     _RequiredServiceNowServiceCatalogConfigurationOutputTypeDef,
     _OptionalServiceNowServiceCatalogConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
+    "_RequiredServiceNowServiceCatalogConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
+    "_OptionalServiceNowServiceCatalogConfigurationTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "IncludeAttachmentFilePatterns": Sequence[str],
+        "ExcludeAttachmentFilePatterns": Sequence[str],
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+class ServiceNowServiceCatalogConfigurationTypeDef(
+    _RequiredServiceNowServiceCatalogConfigurationTypeDef,
+    _OptionalServiceNowServiceCatalogConfigurationTypeDef,
+):
+    pass
 
 _RequiredWorkDocsConfigurationOutputTypeDef = TypedDict(
     "_RequiredWorkDocsConfigurationOutputTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalWorkDocsConfigurationOutputTypeDef = TypedDict(
     "_OptionalWorkDocsConfigurationOutputTypeDef",
     {
         "CrawlComments": bool,
         "UseChangeLog": bool,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class WorkDocsConfigurationOutputTypeDef(
     _RequiredWorkDocsConfigurationOutputTypeDef, _OptionalWorkDocsConfigurationOutputTypeDef
 ):
     pass
 
+_RequiredWorkDocsConfigurationTypeDef = TypedDict(
+    "_RequiredWorkDocsConfigurationTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalWorkDocsConfigurationTypeDef = TypedDict(
+    "_OptionalWorkDocsConfigurationTypeDef",
+    {
+        "CrawlComments": bool,
+        "UseChangeLog": bool,
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+class WorkDocsConfigurationTypeDef(
+    _RequiredWorkDocsConfigurationTypeDef, _OptionalWorkDocsConfigurationTypeDef
+):
+    pass
 
 _RequiredBoxConfigurationOutputTypeDef = TypedDict(
     "_RequiredBoxConfigurationOutputTypeDef",
     {
         "EnterpriseId": str,
         "SecretArn": str,
     },
@@ -2444,58 +2197,54 @@
 _OptionalBoxConfigurationOutputTypeDef = TypedDict(
     "_OptionalBoxConfigurationOutputTypeDef",
     {
         "UseChangeLog": bool,
         "CrawlComments": bool,
         "CrawlTasks": bool,
         "CrawlWebLinks": bool,
-        "FileFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "TaskFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "WebLinkFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FileFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "TaskFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "WebLinkFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class BoxConfigurationOutputTypeDef(
     _RequiredBoxConfigurationOutputTypeDef, _OptionalBoxConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredFsxConfigurationOutputTypeDef = TypedDict(
     "_RequiredFsxConfigurationOutputTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
 )
 _OptionalFsxConfigurationOutputTypeDef = TypedDict(
     "_OptionalFsxConfigurationOutputTypeDef",
     {
         "SecretArn": str,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class FsxConfigurationOutputTypeDef(
     _RequiredFsxConfigurationOutputTypeDef, _OptionalFsxConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredJiraConfigurationOutputTypeDef = TypedDict(
     "_RequiredJiraConfigurationOutputTypeDef",
     {
         "JiraAccountUrl": str,
         "SecretArn": str,
     },
 )
@@ -2503,64 +2252,60 @@
     "_OptionalJiraConfigurationOutputTypeDef",
     {
         "UseChangeLog": bool,
         "Project": List[str],
         "IssueType": List[str],
         "Status": List[str],
         "IssueSubEntityFilter": List[IssueSubEntityType],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "IssueFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "ProjectFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "WorkLogFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "IssueFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "ProjectFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "WorkLogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class JiraConfigurationOutputTypeDef(
     _RequiredJiraConfigurationOutputTypeDef, _OptionalJiraConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredQuipConfigurationOutputTypeDef = TypedDict(
     "_RequiredQuipConfigurationOutputTypeDef",
     {
         "Domain": str,
         "SecretArn": str,
     },
 )
 _OptionalQuipConfigurationOutputTypeDef = TypedDict(
     "_OptionalQuipConfigurationOutputTypeDef",
     {
         "CrawlFileComments": bool,
         "CrawlChatRooms": bool,
         "CrawlAttachments": bool,
         "FolderIds": List[str],
-        "ThreadFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "MessageFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "ThreadFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "MessageFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class QuipConfigurationOutputTypeDef(
     _RequiredQuipConfigurationOutputTypeDef, _OptionalQuipConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredSlackConfigurationOutputTypeDef = TypedDict(
     "_RequiredSlackConfigurationOutputTypeDef",
     {
         "TeamId": str,
         "SecretArn": str,
         "SlackEntityList": List[SlackEntityType],
         "SinceCrawlDate": str,
@@ -2574,366 +2319,158 @@
         "CrawlBotMessage": bool,
         "ExcludeArchived": bool,
         "LookBackPeriod": int,
         "PrivateChannelFilter": List[str],
         "PublicChannelFilter": List[str],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SlackConfigurationOutputTypeDef(
     _RequiredSlackConfigurationOutputTypeDef, _OptionalSlackConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredAlfrescoConfigurationOutputTypeDef = TypedDict(
     "_RequiredAlfrescoConfigurationOutputTypeDef",
     {
         "SiteUrl": str,
         "SiteId": str,
         "SecretArn": str,
-        "SslCertificateS3Path": S3PathOutputTypeDef,
+        "SslCertificateS3Path": S3PathTypeDef,
     },
 )
 _OptionalAlfrescoConfigurationOutputTypeDef = TypedDict(
     "_OptionalAlfrescoConfigurationOutputTypeDef",
     {
         "CrawlSystemFolders": bool,
         "CrawlComments": bool,
         "EntityFilter": List[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "BlogFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "WikiFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "DocumentLibraryFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "BlogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "WikiFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class AlfrescoConfigurationOutputTypeDef(
     _RequiredAlfrescoConfigurationOutputTypeDef, _OptionalAlfrescoConfigurationOutputTypeDef
 ):
     pass
 
-
-DescribeFaqResponseTypeDef = TypedDict(
-    "DescribeFaqResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "S3Path": S3PathOutputTypeDef,
-        "Status": FaqStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "FileFormat": FaqFileFormatType,
-        "LanguageCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "Status": QuerySuggestionsBlockListStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "SourceS3Path": S3PathOutputTypeDef,
-        "ItemCount": int,
-        "FileSizeBytes": int,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeThesaurusResponseTypeDef = TypedDict(
-    "DescribeThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "Status": ThesaurusStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "RoleArn": str,
-        "SourceS3Path": S3PathOutputTypeDef,
-        "FileSizeBytes": int,
-        "TermCount": int,
-        "SynonymRuleCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OnPremiseConfigurationOutputTypeDef = TypedDict(
-    "OnPremiseConfigurationOutputTypeDef",
+OnPremiseConfigurationTypeDef = TypedDict(
+    "OnPremiseConfigurationTypeDef",
     {
         "HostUrl": str,
         "OrganizationName": str,
-        "SslCertificateS3Path": S3PathOutputTypeDef,
+        "SslCertificateS3Path": S3PathTypeDef,
     },
 )
 
 OneDriveUsersOutputTypeDef = TypedDict(
     "OneDriveUsersOutputTypeDef",
     {
         "OneDriveUserList": List[str],
-        "OneDriveUserS3Path": S3PathOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredColumnConfigurationTypeDef = TypedDict(
-    "_RequiredColumnConfigurationTypeDef",
-    {
-        "DocumentIdColumnName": str,
-        "DocumentDataColumnName": str,
-        "ChangeDetectingColumns": Sequence[str],
-    },
-)
-_OptionalColumnConfigurationTypeDef = TypedDict(
-    "_OptionalColumnConfigurationTypeDef",
-    {
-        "DocumentTitleColumnName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "OneDriveUserS3Path": S3PathTypeDef,
     },
     total=False,
 )
 
-
-class ColumnConfigurationTypeDef(
-    _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
-):
-    pass
-
-
-_RequiredGoogleDriveConfigurationTypeDef = TypedDict(
-    "_RequiredGoogleDriveConfigurationTypeDef",
-    {
-        "SecretArn": str,
-    },
-)
-_OptionalGoogleDriveConfigurationTypeDef = TypedDict(
-    "_OptionalGoogleDriveConfigurationTypeDef",
+OneDriveUsersTypeDef = TypedDict(
+    "OneDriveUsersTypeDef",
     {
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "ExcludeMimeTypes": Sequence[str],
-        "ExcludeUserAccounts": Sequence[str],
-        "ExcludeSharedDrives": Sequence[str],
+        "OneDriveUserList": Sequence[str],
+        "OneDriveUserS3Path": S3PathTypeDef,
     },
     total=False,
 )
 
-
-class GoogleDriveConfigurationTypeDef(
-    _RequiredGoogleDriveConfigurationTypeDef, _OptionalGoogleDriveConfigurationTypeDef
-):
-    pass
-
-
-_RequiredSalesforceChatterFeedConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceChatterFeedConfigurationTypeDef",
+_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     {
-        "DocumentDataFieldName": str,
+        "IndexId": str,
+        "Id": str,
     },
 )
-_OptionalSalesforceChatterFeedConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceChatterFeedConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "IncludeFilterTypes": Sequence[SalesforceChatterFeedIncludeFilterTypeType],
-    },
-    total=False,
-)
-
-
-class SalesforceChatterFeedConfigurationTypeDef(
-    _RequiredSalesforceChatterFeedConfigurationTypeDef,
-    _OptionalSalesforceChatterFeedConfigurationTypeDef,
-):
-    pass
-
-
-_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
+_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "Name": str,
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(
-    _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
-    _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
-):
-    pass
-
-
-_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(
-    _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
-    _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
-):
-    pass
-
-
-SalesforceStandardObjectAttachmentConfigurationTypeDef = TypedDict(
-    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-_RequiredSalesforceStandardObjectConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceStandardObjectConfigurationTypeDef",
-    {
-        "Name": SalesforceStandardObjectNameType,
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceStandardObjectConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceStandardObjectConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class SalesforceStandardObjectConfigurationTypeDef(
-    _RequiredSalesforceStandardObjectConfigurationTypeDef,
-    _OptionalSalesforceStandardObjectConfigurationTypeDef,
-):
-    pass
-
-
-_RequiredServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_RequiredServiceNowKnowledgeArticleConfigurationTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_OptionalServiceNowKnowledgeArticleConfigurationTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": Sequence[str],
-        "ExcludeAttachmentFilePatterns": Sequence[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "FilterQuery": str,
+        "Description": str,
+        "SourceS3Path": S3PathTypeDef,
+        "RoleArn": str,
     },
     total=False,
 )
 
-
-class ServiceNowKnowledgeArticleConfigurationTypeDef(
-    _RequiredServiceNowKnowledgeArticleConfigurationTypeDef,
-    _OptionalServiceNowKnowledgeArticleConfigurationTypeDef,
+class UpdateQuerySuggestionsBlockListRequestRequestTypeDef(
+    _RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
+    _OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
-    "_RequiredServiceNowServiceCatalogConfigurationTypeDef",
+_RequiredUpdateThesaurusRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThesaurusRequestRequestTypeDef",
     {
-        "DocumentDataFieldName": str,
+        "Id": str,
+        "IndexId": str,
     },
 )
-_OptionalServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
-    "_OptionalServiceNowServiceCatalogConfigurationTypeDef",
+_OptionalUpdateThesaurusRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThesaurusRequestRequestTypeDef",
     {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": Sequence[str],
-        "ExcludeAttachmentFilePatterns": Sequence[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "Name": str,
+        "Description": str,
+        "RoleArn": str,
+        "SourceS3Path": S3PathTypeDef,
     },
     total=False,
 )
 
-
-class ServiceNowServiceCatalogConfigurationTypeDef(
-    _RequiredServiceNowServiceCatalogConfigurationTypeDef,
-    _OptionalServiceNowServiceCatalogConfigurationTypeDef,
+class UpdateThesaurusRequestRequestTypeDef(
+    _RequiredUpdateThesaurusRequestRequestTypeDef, _OptionalUpdateThesaurusRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredWorkDocsConfigurationTypeDef = TypedDict(
-    "_RequiredWorkDocsConfigurationTypeDef",
+_RequiredAlfrescoConfigurationTypeDef = TypedDict(
+    "_RequiredAlfrescoConfigurationTypeDef",
     {
-        "OrganizationId": str,
+        "SiteUrl": str,
+        "SiteId": str,
+        "SecretArn": str,
+        "SslCertificateS3Path": S3PathTypeDef,
     },
 )
-_OptionalWorkDocsConfigurationTypeDef = TypedDict(
-    "_OptionalWorkDocsConfigurationTypeDef",
+_OptionalAlfrescoConfigurationTypeDef = TypedDict(
+    "_OptionalAlfrescoConfigurationTypeDef",
     {
+        "CrawlSystemFolders": bool,
         "CrawlComments": bool,
-        "UseChangeLog": bool,
+        "EntityFilter": Sequence[AlfrescoEntityType],
+        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class WorkDocsConfigurationTypeDef(
-    _RequiredWorkDocsConfigurationTypeDef, _OptionalWorkDocsConfigurationTypeDef
+class AlfrescoConfigurationTypeDef(
+    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
 ):
     pass
 
-
 _RequiredBoxConfigurationTypeDef = TypedDict(
     "_RequiredBoxConfigurationTypeDef",
     {
         "EnterpriseId": str,
         "SecretArn": str,
     },
 )
@@ -2951,19 +2488,17 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
     pass
 
-
 _RequiredFsxConfigurationTypeDef = TypedDict(
     "_RequiredFsxConfigurationTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
@@ -2975,19 +2510,17 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class FsxConfigurationTypeDef(_RequiredFsxConfigurationTypeDef, _OptionalFsxConfigurationTypeDef):
     pass
 
-
 _RequiredJiraConfigurationTypeDef = TypedDict(
     "_RequiredJiraConfigurationTypeDef",
     {
         "JiraAccountUrl": str,
         "SecretArn": str,
     },
 )
@@ -3007,21 +2540,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class JiraConfigurationTypeDef(
     _RequiredJiraConfigurationTypeDef, _OptionalJiraConfigurationTypeDef
 ):
     pass
 
-
 _RequiredQuipConfigurationTypeDef = TypedDict(
     "_RequiredQuipConfigurationTypeDef",
     {
         "Domain": str,
         "SecretArn": str,
     },
 )
@@ -3038,21 +2569,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class QuipConfigurationTypeDef(
     _RequiredQuipConfigurationTypeDef, _OptionalQuipConfigurationTypeDef
 ):
     pass
 
-
 _RequiredSlackConfigurationTypeDef = TypedDict(
     "_RequiredSlackConfigurationTypeDef",
     {
         "TeamId": str,
         "SecretArn": str,
         "SlackEntityList": Sequence[SlackEntityType],
         "SinceCrawlDate": str,
@@ -3071,169 +2600,204 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-
 class SlackConfigurationTypeDef(
     _RequiredSlackConfigurationTypeDef, _OptionalSlackConfigurationTypeDef
 ):
     pass
 
-
-_RequiredAlfrescoConfigurationTypeDef = TypedDict(
-    "_RequiredAlfrescoConfigurationTypeDef",
+AssociateEntitiesToExperienceRequestRequestTypeDef = TypedDict(
+    "AssociateEntitiesToExperienceRequestRequestTypeDef",
     {
-        "SiteUrl": str,
-        "SiteId": str,
-        "SecretArn": str,
-        "SslCertificateS3Path": S3PathTypeDef,
+        "Id": str,
+        "IndexId": str,
+        "EntityList": Sequence[EntityConfigurationTypeDef],
     },
 )
-_OptionalAlfrescoConfigurationTypeDef = TypedDict(
-    "_OptionalAlfrescoConfigurationTypeDef",
+
+DisassociateEntitiesFromExperienceRequestRequestTypeDef = TypedDict(
+    "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     {
-        "CrawlSystemFolders": bool,
-        "CrawlComments": bool,
-        "EntityFilter": Sequence[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
+        "Id": str,
+        "IndexId": str,
+        "EntityList": Sequence[EntityConfigurationTypeDef],
     },
-    total=False,
 )
 
+AssociateEntitiesToExperienceResponseTypeDef = TypedDict(
+    "AssociateEntitiesToExperienceResponseTypeDef",
+    {
+        "FailedEntityList": List[FailedEntityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AlfrescoConfigurationTypeDef(
-    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
-):
-    pass
-
-
-OnPremiseConfigurationTypeDef = TypedDict(
-    "OnPremiseConfigurationTypeDef",
+AssociatePersonasToEntitiesResponseTypeDef = TypedDict(
+    "AssociatePersonasToEntitiesResponseTypeDef",
     {
-        "HostUrl": str,
-        "OrganizationName": str,
-        "SslCertificateS3Path": S3PathTypeDef,
+        "FailedEntityList": List[FailedEntityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OneDriveUsersTypeDef = TypedDict(
-    "OneDriveUsersTypeDef",
+CreateAccessControlConfigurationResponseTypeDef = TypedDict(
+    "CreateAccessControlConfigurationResponseTypeDef",
     {
-        "OneDriveUserList": Sequence[str],
-        "OneDriveUserS3Path": S3PathTypeDef,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+CreateDataSourceResponseTypeDef = TypedDict(
+    "CreateDataSourceResponseTypeDef",
     {
-        "IndexId": str,
         "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+
+CreateExperienceResponseTypeDef = TypedDict(
+    "CreateExperienceResponseTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "SourceS3Path": S3PathTypeDef,
-        "RoleArn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateFaqResponseTypeDef = TypedDict(
+    "CreateFaqResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateQuerySuggestionsBlockListRequestRequestTypeDef(
-    _RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
-    _OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
-):
-    pass
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateThesaurusRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThesaurusRequestRequestTypeDef",
+CreateThesaurusResponseTypeDef = TypedDict(
+    "CreateThesaurusResponseTypeDef",
     {
         "Id": str,
-        "IndexId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateThesaurusRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThesaurusRequestRequestTypeDef",
+
+DescribeFaqResponseTypeDef = TypedDict(
+    "DescribeFaqResponseTypeDef",
     {
+        "Id": str,
+        "IndexId": str,
         "Name": str,
         "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "S3Path": S3PathTypeDef,
+        "Status": FaqStatusType,
         "RoleArn": str,
-        "SourceS3Path": S3PathTypeDef,
+        "ErrorMessage": str,
+        "FileFormat": FaqFileFormatType,
+        "LanguageCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateThesaurusRequestRequestTypeDef(
-    _RequiredUpdateThesaurusRequestRequestTypeDef, _OptionalUpdateThesaurusRequestRequestTypeDef
-):
-    pass
-
-
-AssociateEntitiesToExperienceRequestRequestTypeDef = TypedDict(
-    "AssociateEntitiesToExperienceRequestRequestTypeDef",
+DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
     {
-        "Id": str,
         "IndexId": str,
-        "EntityList": Sequence[EntityConfigurationTypeDef],
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "Status": QuerySuggestionsBlockListStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "SourceS3Path": S3PathTypeDef,
+        "ItemCount": int,
+        "FileSizeBytes": int,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociateEntitiesFromExperienceRequestRequestTypeDef = TypedDict(
-    "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
+DescribeThesaurusResponseTypeDef = TypedDict(
+    "DescribeThesaurusResponseTypeDef",
     {
         "Id": str,
         "IndexId": str,
-        "EntityList": Sequence[EntityConfigurationTypeDef],
+        "Name": str,
+        "Description": str,
+        "Status": ThesaurusStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "RoleArn": str,
+        "SourceS3Path": S3PathTypeDef,
+        "FileSizeBytes": int,
+        "TermCount": int,
+        "SynonymRuleCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociateEntitiesToExperienceResponseTypeDef = TypedDict(
-    "AssociateEntitiesToExperienceResponseTypeDef",
+DisassociateEntitiesFromExperienceResponseTypeDef = TypedDict(
+    "DisassociateEntitiesFromExperienceResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePersonasToEntitiesResponseTypeDef = TypedDict(
-    "AssociatePersonasToEntitiesResponseTypeDef",
+DisassociatePersonasFromEntitiesResponseTypeDef = TypedDict(
+    "DisassociatePersonasFromEntitiesResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociateEntitiesFromExperienceResponseTypeDef = TypedDict(
-    "DisassociateEntitiesFromExperienceResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePersonasFromEntitiesResponseTypeDef = TypedDict(
-    "DisassociatePersonasFromEntitiesResponseTypeDef",
+ListAccessControlConfigurationsResponseTypeDef = TypedDict(
+    "ListAccessControlConfigurationsResponseTypeDef",
     {
-        "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextToken": str,
+        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataSourceSyncJobResponseTypeDef = TypedDict(
+    "StartDataSourceSyncJobResponseTypeDef",
+    {
+        "ExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociatePersonasToEntitiesRequestRequestTypeDef = TypedDict(
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
     {
         "Id": str,
@@ -3241,15 +2805,15 @@
         "Personas": Sequence[EntityPersonaConfigurationTypeDef],
     },
 )
 
 AttributeSuggestionsDescribeConfigTypeDef = TypedDict(
     "AttributeSuggestionsDescribeConfigTypeDef",
     {
-        "SuggestableConfigList": List[SuggestableConfigOutputTypeDef],
+        "SuggestableConfigList": List[SuggestableConfigTypeDef],
         "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
     total=False,
 )
 
 AttributeSuggestionsUpdateConfigTypeDef = TypedDict(
     "AttributeSuggestionsUpdateConfigTypeDef",
@@ -3259,15 +2823,15 @@
     },
     total=False,
 )
 
 AuthenticationConfigurationOutputTypeDef = TypedDict(
     "AuthenticationConfigurationOutputTypeDef",
     {
-        "BasicAuthentication": List[BasicAuthenticationConfigurationOutputTypeDef],
+        "BasicAuthentication": List[BasicAuthenticationConfigurationTypeDef],
     },
     total=False,
 )
 
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
@@ -3287,60 +2851,58 @@
     "_OptionalBatchDeleteDocumentRequestRequestTypeDef",
     {
         "DataSourceSyncJobMetricTarget": DataSourceSyncJobMetricTargetTypeDef,
     },
     total=False,
 )
 
-
 class BatchDeleteDocumentRequestRequestTypeDef(
     _RequiredBatchDeleteDocumentRequestRequestTypeDef,
     _OptionalBatchDeleteDocumentRequestRequestTypeDef,
 ):
     pass
 
-
 BatchDeleteDocumentResponseTypeDef = TypedDict(
     "BatchDeleteDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchDeleteDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteFeaturedResultsSetResponseTypeDef = TypedDict(
     "BatchDeleteFeaturedResultsSetResponseTypeDef",
     {
         "Errors": List[BatchDeleteFeaturedResultsSetErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDocumentStatusResponseTypeDef = TypedDict(
     "BatchGetDocumentStatusResponseTypeDef",
     {
         "Errors": List[BatchGetDocumentStatusResponseErrorTypeDef],
         "DocumentStatusList": List[StatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutDocumentResponseTypeDef = TypedDict(
     "BatchPutDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchPutDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfluenceAttachmentConfigurationOutputTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
-        "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingOutputTypeDef],
+        "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluenceAttachmentConfigurationTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationTypeDef",
     {
@@ -3349,15 +2911,15 @@
     },
     total=False,
 )
 
 ConfluenceBlogConfigurationOutputTypeDef = TypedDict(
     "ConfluenceBlogConfigurationOutputTypeDef",
     {
-        "BlogFieldMappings": List[ConfluenceBlogToIndexFieldMappingOutputTypeDef],
+        "BlogFieldMappings": List[ConfluenceBlogToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluenceBlogConfigurationTypeDef = TypedDict(
     "ConfluenceBlogConfigurationTypeDef",
     {
@@ -3378,31 +2940,29 @@
     "_OptionalSharePointConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "UseChangeLog": bool,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "DocumentTitleFieldName": str,
         "DisableLocalGroups": bool,
-        "SslCertificateS3Path": S3PathOutputTypeDef,
+        "SslCertificateS3Path": S3PathTypeDef,
         "AuthenticationType": SharePointOnlineAuthenticationTypeType,
-        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "ProxyConfiguration": ProxyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SharePointConfigurationOutputTypeDef(
     _RequiredSharePointConfigurationOutputTypeDef, _OptionalSharePointConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredSharePointConfigurationTypeDef = TypedDict(
     "_RequiredSharePointConfigurationTypeDef",
     {
         "SharePointVersion": SharePointVersionType,
         "Urls": Sequence[str],
         "SecretArn": str,
     },
@@ -3421,25 +2981,23 @@
         "SslCertificateS3Path": S3PathTypeDef,
         "AuthenticationType": SharePointOnlineAuthenticationTypeType,
         "ProxyConfiguration": ProxyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SharePointConfigurationTypeDef(
     _RequiredSharePointConfigurationTypeDef, _OptionalSharePointConfigurationTypeDef
 ):
     pass
 
-
 ConfluencePageConfigurationOutputTypeDef = TypedDict(
     "ConfluencePageConfigurationOutputTypeDef",
     {
-        "PageFieldMappings": List[ConfluencePageToIndexFieldMappingOutputTypeDef],
+        "PageFieldMappings": List[ConfluencePageToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluencePageConfigurationTypeDef = TypedDict(
     "ConfluencePageConfigurationTypeDef",
     {
@@ -3451,15 +3009,15 @@
 ConfluenceSpaceConfigurationOutputTypeDef = TypedDict(
     "ConfluenceSpaceConfigurationOutputTypeDef",
     {
         "CrawlPersonalSpaces": bool,
         "CrawlArchivedSpaces": bool,
         "IncludeSpaces": List[str],
         "ExcludeSpaces": List[str],
-        "SpaceFieldMappings": List[ConfluenceSpaceToIndexFieldMappingOutputTypeDef],
+        "SpaceFieldMappings": List[ConfluenceSpaceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluenceSpaceConfigurationTypeDef = TypedDict(
     "ConfluenceSpaceConfigurationTypeDef",
     {
@@ -3477,14 +3035,21 @@
     {
         "SuggestedQueryText": str,
         "Corrections": List[CorrectionTypeDef],
     },
     total=False,
 )
 
+HierarchicalPrincipalOutputTypeDef = TypedDict(
+    "HierarchicalPrincipalOutputTypeDef",
+    {
+        "PrincipalList": List[PrincipalTypeDef],
+    },
+)
+
 HierarchicalPrincipalTypeDef = TypedDict(
     "HierarchicalPrincipalTypeDef",
     {
         "PrincipalList": Sequence[PrincipalTypeDef],
     },
 )
 
@@ -3505,21 +3070,19 @@
         "FileFormat": FaqFileFormatType,
         "ClientToken": str,
         "LanguageCode": str,
     },
     total=False,
 )
 
-
 class CreateFaqRequestRequestTypeDef(
     _RequiredCreateFaqRequestRequestTypeDef, _OptionalCreateFaqRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
         "SourceS3Path": S3PathTypeDef,
         "RoleArn": str,
@@ -3531,22 +3094,20 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateQuerySuggestionsBlockListRequestRequestTypeDef(
     _RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef,
     _OptionalCreateQuerySuggestionsBlockListRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateThesaurusRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThesaurusRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
         "RoleArn": str,
         "SourceS3Path": S3PathTypeDef,
@@ -3558,20 +3119,26 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateThesaurusRequestRequestTypeDef(
     _RequiredCreateThesaurusRequestRequestTypeDef, _OptionalCreateThesaurusRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -3593,21 +3160,34 @@
         "QueryTexts": Sequence[str],
         "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFeaturedResultsSetRequestRequestTypeDef(
     _RequiredCreateFeaturedResultsSetRequestRequestTypeDef,
     _OptionalCreateFeaturedResultsSetRequestRequestTypeDef,
 ):
     pass
 
+FeaturedResultsSetTypeDef = TypedDict(
+    "FeaturedResultsSetTypeDef",
+    {
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": List[str],
+        "FeaturedDocuments": List[FeaturedDocumentTypeDef],
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
+    },
+    total=False,
+)
 
 _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFeaturedResultsSetRequestRequestTypeDef",
     {
         "IndexId": str,
         "FeaturedResultsSetId": str,
     },
@@ -3620,22 +3200,20 @@
         "Status": FeaturedResultsSetStatusType,
         "QueryTexts": Sequence[str],
         "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
     },
     total=False,
 )
 
-
 class UpdateFeaturedResultsSetRequestRequestTypeDef(
     _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef,
     _OptionalUpdateFeaturedResultsSetRequestRequestTypeDef,
 ):
     pass
 
-
 UserContextTypeDef = TypedDict(
     "UserContextTypeDef",
     {
         "Token": str,
         "UserId": str,
         "Groups": Sequence[str],
         "DataSourceGroups": Sequence[DataSourceGroupTypeDef],
@@ -3644,15 +3222,15 @@
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "SummaryItems": List[DataSourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataSourceSyncJobTypeDef = TypedDict(
     "DataSourceSyncJobTypeDef",
     {
         "ExecutionId": str,
@@ -3663,21 +3241,14 @@
         "ErrorCode": ErrorCodeType,
         "DataSourceErrorCode": str,
         "Metrics": DataSourceSyncJobMetricsTypeDef,
     },
     total=False,
 )
 
-HierarchicalPrincipalOutputTypeDef = TypedDict(
-    "HierarchicalPrincipalOutputTypeDef",
-    {
-        "PrincipalList": List[PrincipalOutputTypeDef],
-    },
-)
-
 ExperiencesSummaryTypeDef = TypedDict(
     "ExperiencesSummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "CreatedAt": datetime,
         "Status": ExperienceStatusType,
@@ -3694,26 +3265,26 @@
         "Description": str,
         "Status": FeaturedResultsSetStatusType,
         "QueryTexts": List[str],
         "FeaturedDocumentsWithMetadata": List[FeaturedDocumentWithMetadataTypeDef],
         "FeaturedDocumentsMissing": List[FeaturedDocumentMissingTypeDef],
         "LastUpdatedTimestamp": int,
         "CreationTimestamp": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePrincipalMappingResponseTypeDef = TypedDict(
     "DescribePrincipalMappingResponseTypeDef",
     {
         "IndexId": str,
         "DataSourceId": str,
         "GroupId": str,
         "GroupOrderingIdSummaries": List[GroupOrderingIdSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDocumentAttributeConditionOutputTypeDef = TypedDict(
     "_RequiredDocumentAttributeConditionOutputTypeDef",
     {
         "ConditionDocumentAttributeKey": str,
@@ -3724,22 +3295,20 @@
     "_OptionalDocumentAttributeConditionOutputTypeDef",
     {
         "ConditionOnValue": DocumentAttributeValueOutputTypeDef,
     },
     total=False,
 )
 
-
 class DocumentAttributeConditionOutputTypeDef(
     _RequiredDocumentAttributeConditionOutputTypeDef,
     _OptionalDocumentAttributeConditionOutputTypeDef,
 ):
     pass
 
-
 DocumentAttributeOutputTypeDef = TypedDict(
     "DocumentAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": DocumentAttributeValueOutputTypeDef,
     },
 )
@@ -3775,21 +3344,19 @@
     "_OptionalDocumentAttributeConditionTypeDef",
     {
         "ConditionOnValue": DocumentAttributeValueTypeDef,
     },
     total=False,
 )
 
-
 class DocumentAttributeConditionTypeDef(
     _RequiredDocumentAttributeConditionTypeDef, _OptionalDocumentAttributeConditionTypeDef
 ):
     pass
 
-
 DocumentAttributeTargetTypeDef = TypedDict(
     "DocumentAttributeTargetTypeDef",
     {
         "TargetDocumentAttributeKey": str,
         "TargetDocumentAttributeValueDeletion": bool,
         "TargetDocumentAttributeValue": DocumentAttributeValueTypeDef,
     },
@@ -3811,35 +3378,25 @@
         "Type": DocumentAttributeValueTypeType,
     },
 )
 _OptionalDocumentMetadataConfigurationOutputTypeDef = TypedDict(
     "_OptionalDocumentMetadataConfigurationOutputTypeDef",
     {
         "Relevance": RelevanceOutputTypeDef,
-        "Search": SearchOutputTypeDef,
+        "Search": SearchTypeDef,
     },
     total=False,
 )
 
-
 class DocumentMetadataConfigurationOutputTypeDef(
     _RequiredDocumentMetadataConfigurationOutputTypeDef,
     _OptionalDocumentMetadataConfigurationOutputTypeDef,
 ):
     pass
 
-
-DocumentRelevanceConfigurationTypeDef = TypedDict(
-    "DocumentRelevanceConfigurationTypeDef",
-    {
-        "Name": str,
-        "Relevance": RelevanceTypeDef,
-    },
-)
-
 _RequiredDocumentMetadataConfigurationTypeDef = TypedDict(
     "_RequiredDocumentMetadataConfigurationTypeDef",
     {
         "Name": str,
         "Type": DocumentAttributeValueTypeType,
     },
 )
@@ -3848,46 +3405,50 @@
     {
         "Relevance": RelevanceTypeDef,
         "Search": SearchTypeDef,
     },
     total=False,
 )
 
-
 class DocumentMetadataConfigurationTypeDef(
     _RequiredDocumentMetadataConfigurationTypeDef, _OptionalDocumentMetadataConfigurationTypeDef
 ):
     pass
 
+DocumentRelevanceConfigurationTypeDef = TypedDict(
+    "DocumentRelevanceConfigurationTypeDef",
+    {
+        "Name": str,
+        "Relevance": RelevanceTypeDef,
+    },
+)
 
 _RequiredS3DataSourceConfigurationOutputTypeDef = TypedDict(
     "_RequiredS3DataSourceConfigurationOutputTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3DataSourceConfigurationOutputTypeDef = TypedDict(
     "_OptionalS3DataSourceConfigurationOutputTypeDef",
     {
         "InclusionPrefixes": List[str],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationOutputTypeDef,
-        "AccessControlListConfiguration": AccessControlListConfigurationOutputTypeDef,
+        "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationTypeDef,
+        "AccessControlListConfiguration": AccessControlListConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class S3DataSourceConfigurationOutputTypeDef(
     _RequiredS3DataSourceConfigurationOutputTypeDef, _OptionalS3DataSourceConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredS3DataSourceConfigurationTypeDef = TypedDict(
     "_RequiredS3DataSourceConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3DataSourceConfigurationTypeDef = TypedDict(
@@ -3898,36 +3459,34 @@
         "ExclusionPatterns": Sequence[str],
         "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationTypeDef,
         "AccessControlListConfiguration": AccessControlListConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class S3DataSourceConfigurationTypeDef(
     _RequiredS3DataSourceConfigurationTypeDef, _OptionalS3DataSourceConfigurationTypeDef
 ):
     pass
 
-
 ExperienceEntitiesSummaryTypeDef = TypedDict(
     "ExperienceEntitiesSummaryTypeDef",
     {
         "EntityId": str,
         "EntityType": EntityTypeType,
         "DisplayData": EntityDisplayDataTypeDef,
     },
     total=False,
 )
 
 ExperienceConfigurationOutputTypeDef = TypedDict(
     "ExperienceConfigurationOutputTypeDef",
     {
         "ContentSourceConfiguration": ContentSourceConfigurationOutputTypeDef,
-        "UserIdentityConfiguration": UserIdentityConfigurationOutputTypeDef,
+        "UserIdentityConfiguration": UserIdentityConfigurationTypeDef,
     },
     total=False,
 )
 
 ExperienceConfigurationTypeDef = TypedDict(
     "ExperienceConfigurationTypeDef",
     {
@@ -3938,50 +3497,35 @@
 )
 
 ListFaqsResponseTypeDef = TypedDict(
     "ListFaqsResponseTypeDef",
     {
         "NextToken": str,
         "FaqSummaryItems": List[FaqSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FeaturedResultsSetTypeDef = TypedDict(
-    "FeaturedResultsSetTypeDef",
-    {
-        "FeaturedResultsSetId": str,
-        "FeaturedResultsSetName": str,
-        "Description": str,
-        "Status": FeaturedResultsSetStatusType,
-        "QueryTexts": List[str],
-        "FeaturedDocuments": List[FeaturedDocumentOutputTypeDef],
-        "LastUpdatedTimestamp": int,
-        "CreationTimestamp": int,
-    },
-    total=False,
-)
-
 ListFeaturedResultsSetsResponseTypeDef = TypedDict(
     "ListFeaturedResultsSetsResponseTypeDef",
     {
         "FeaturedResultsSetSummaryItems": List[FeaturedResultsSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotsResponseTypeDef = TypedDict(
     "GetSnapshotsResponseTypeDef",
     {
         "SnapShotTimeFilter": TimeRangeOutputTypeDef,
         "SnapshotsDataHeader": List[str],
         "SnapshotsData": List[List[str]],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupMembersTypeDef = TypedDict(
     "GroupMembersTypeDef",
     {
         "MemberGroups": Sequence[MemberGroupTypeDef],
@@ -3992,15 +3536,15 @@
 )
 
 ListGroupsOlderThanOrderingIdResponseTypeDef = TypedDict(
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     {
         "GroupsSummaries": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TextWithHighlightsTypeDef = TypedDict(
     "TextWithHighlightsTypeDef",
     {
         "Text": str,
@@ -4010,35 +3554,26 @@
 )
 
 ListIndicesResponseTypeDef = TypedDict(
     "ListIndicesResponseTypeDef",
     {
         "IndexConfigurationSummaryItems": List[IndexConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IndexStatisticsTypeDef = TypedDict(
     "IndexStatisticsTypeDef",
     {
         "FaqStatistics": FaqStatisticsTypeDef,
         "TextDocumentStatistics": TextDocumentStatisticsTypeDef,
     },
 )
 
-UserTokenConfigurationOutputTypeDef = TypedDict(
-    "UserTokenConfigurationOutputTypeDef",
-    {
-        "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationOutputTypeDef,
-        "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 UserTokenConfigurationTypeDef = TypedDict(
     "UserTokenConfigurationTypeDef",
     {
         "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationTypeDef,
         "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationTypeDef,
     },
     total=False,
@@ -4058,54 +3593,44 @@
         "MaxResults": int,
         "StartTimeFilter": TimeRangeTypeDef,
         "StatusFilter": DataSourceSyncJobStatusType,
     },
     total=False,
 )
 
-
 class ListDataSourceSyncJobsRequestRequestTypeDef(
     _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
     _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
 ):
     pass
 
-
 ListEntityPersonasResponseTypeDef = TypedDict(
     "ListEntityPersonasResponseTypeDef",
     {
         "SummaryItems": List[PersonasSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQuerySuggestionsBlockListsResponseTypeDef = TypedDict(
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     {
         "BlockListSummaryItems": List[QuerySuggestionsBlockListSummaryTypeDef],
         "NextToken": str,
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
 
 ListThesauriResponseTypeDef = TypedDict(
     "ListThesauriResponseTypeDef",
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -4117,21 +3642,19 @@
     {
         "ClickFeedbackItems": Sequence[ClickFeedbackTypeDef],
         "RelevanceFeedbackItems": Sequence[RelevanceFeedbackTypeDef],
     },
     total=False,
 )
 
-
 class SubmitFeedbackRequestRequestTypeDef(
     _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
 ):
     pass
 
-
 UrlsOutputTypeDef = TypedDict(
     "UrlsOutputTypeDef",
     {
         "SeedUrlConfiguration": SeedUrlConfigurationOutputTypeDef,
         "SiteMapsConfiguration": SiteMapsConfigurationOutputTypeDef,
     },
     total=False,
@@ -4163,34 +3686,55 @@
     total=False,
 )
 
 _RequiredDatabaseConfigurationOutputTypeDef = TypedDict(
     "_RequiredDatabaseConfigurationOutputTypeDef",
     {
         "DatabaseEngineType": DatabaseEngineTypeType,
-        "ConnectionConfiguration": ConnectionConfigurationOutputTypeDef,
+        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
         "ColumnConfiguration": ColumnConfigurationOutputTypeDef,
     },
 )
 _OptionalDatabaseConfigurationOutputTypeDef = TypedDict(
     "_OptionalDatabaseConfigurationOutputTypeDef",
     {
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "AclConfiguration": AclConfigurationOutputTypeDef,
-        "SqlConfiguration": SqlConfigurationOutputTypeDef,
+        "AclConfiguration": AclConfigurationTypeDef,
+        "SqlConfiguration": SqlConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseConfigurationOutputTypeDef(
     _RequiredDatabaseConfigurationOutputTypeDef, _OptionalDatabaseConfigurationOutputTypeDef
 ):
     pass
 
+_RequiredDatabaseConfigurationTypeDef = TypedDict(
+    "_RequiredDatabaseConfigurationTypeDef",
+    {
+        "DatabaseEngineType": DatabaseEngineTypeType,
+        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
+        "ColumnConfiguration": ColumnConfigurationTypeDef,
+    },
+)
+_OptionalDatabaseConfigurationTypeDef = TypedDict(
+    "_OptionalDatabaseConfigurationTypeDef",
+    {
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
+        "AclConfiguration": AclConfigurationTypeDef,
+        "SqlConfiguration": SqlConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class DatabaseConfigurationTypeDef(
+    _RequiredDatabaseConfigurationTypeDef, _OptionalDatabaseConfigurationTypeDef
+):
+    pass
 
 _RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef",
     {
         "IncludedStates": List[SalesforceKnowledgeArticleStateType],
     },
 )
@@ -4203,21 +3747,44 @@
         "CustomKnowledgeArticleTypeConfigurations": List[
             SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef
         ],
     },
     total=False,
 )
 
-
 class SalesforceKnowledgeArticleConfigurationOutputTypeDef(
     _RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef,
     _OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceKnowledgeArticleConfigurationTypeDef",
+    {
+        "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
+    },
+)
+_OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceKnowledgeArticleConfigurationTypeDef",
+    {
+        "StandardKnowledgeArticleTypeConfiguration": (
+            SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef
+        ),
+        "CustomKnowledgeArticleTypeConfigurations": Sequence[
+            SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef
+        ],
+    },
+    total=False,
+)
+
+class SalesforceKnowledgeArticleConfigurationTypeDef(
+    _RequiredSalesforceKnowledgeArticleConfigurationTypeDef,
+    _OptionalSalesforceKnowledgeArticleConfigurationTypeDef,
+):
+    pass
 
 _RequiredServiceNowConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceNowConfigurationOutputTypeDef",
     {
         "HostUrl": str,
         "SecretArn": str,
         "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
@@ -4229,179 +3796,89 @@
         "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
         "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationOutputTypeDef,
         "AuthenticationType": ServiceNowAuthenticationTypeType,
     },
     total=False,
 )
 
-
 class ServiceNowConfigurationOutputTypeDef(
     _RequiredServiceNowConfigurationOutputTypeDef, _OptionalServiceNowConfigurationOutputTypeDef
 ):
     pass
 
+_RequiredServiceNowConfigurationTypeDef = TypedDict(
+    "_RequiredServiceNowConfigurationTypeDef",
+    {
+        "HostUrl": str,
+        "SecretArn": str,
+        "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
+    },
+)
+_OptionalServiceNowConfigurationTypeDef = TypedDict(
+    "_OptionalServiceNowConfigurationTypeDef",
+    {
+        "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationTypeDef,
+        "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationTypeDef,
+        "AuthenticationType": ServiceNowAuthenticationTypeType,
+    },
+    total=False,
+)
+
+class ServiceNowConfigurationTypeDef(
+    _RequiredServiceNowConfigurationTypeDef, _OptionalServiceNowConfigurationTypeDef
+):
+    pass
 
 _RequiredGitHubConfigurationOutputTypeDef = TypedDict(
     "_RequiredGitHubConfigurationOutputTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGitHubConfigurationOutputTypeDef = TypedDict(
     "_OptionalGitHubConfigurationOutputTypeDef",
     {
-        "SaaSConfiguration": SaaSConfigurationOutputTypeDef,
-        "OnPremiseConfiguration": OnPremiseConfigurationOutputTypeDef,
+        "SaaSConfiguration": SaaSConfigurationTypeDef,
+        "OnPremiseConfiguration": OnPremiseConfigurationTypeDef,
         "Type": TypeType,
         "UseChangeLog": bool,
-        "GitHubDocumentCrawlProperties": GitHubDocumentCrawlPropertiesOutputTypeDef,
+        "GitHubDocumentCrawlProperties": GitHubDocumentCrawlPropertiesTypeDef,
         "RepositoryFilter": List[str],
         "InclusionFolderNamePatterns": List[str],
         "InclusionFileTypePatterns": List[str],
         "InclusionFileNamePatterns": List[str],
         "ExclusionFolderNamePatterns": List[str],
         "ExclusionFileTypePatterns": List[str],
         "ExclusionFileNamePatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "GitHubRepositoryConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
-        ],
-        "GitHubCommitConfigurationFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "GitHubIssueDocumentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
-        ],
-        "GitHubIssueCommentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
-        ],
+        "GitHubRepositoryConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "GitHubCommitConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "GitHubIssueDocumentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "GitHubIssueCommentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "GitHubIssueAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
         "GitHubPullRequestCommentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
         "GitHubPullRequestDocumentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
         "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
     },
     total=False,
 )
 
-
 class GitHubConfigurationOutputTypeDef(
     _RequiredGitHubConfigurationOutputTypeDef, _OptionalGitHubConfigurationOutputTypeDef
 ):
     pass
 
-
-_RequiredOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOneDriveConfigurationOutputTypeDef",
-    {
-        "TenantDomain": str,
-        "SecretArn": str,
-        "OneDriveUsers": OneDriveUsersOutputTypeDef,
-    },
-)
-_OptionalOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOneDriveConfigurationOutputTypeDef",
-    {
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "DisableLocalGroups": bool,
-    },
-    total=False,
-)
-
-
-class OneDriveConfigurationOutputTypeDef(
-    _RequiredOneDriveConfigurationOutputTypeDef, _OptionalOneDriveConfigurationOutputTypeDef
-):
-    pass
-
-
-_RequiredDatabaseConfigurationTypeDef = TypedDict(
-    "_RequiredDatabaseConfigurationTypeDef",
-    {
-        "DatabaseEngineType": DatabaseEngineTypeType,
-        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
-        "ColumnConfiguration": ColumnConfigurationTypeDef,
-    },
-)
-_OptionalDatabaseConfigurationTypeDef = TypedDict(
-    "_OptionalDatabaseConfigurationTypeDef",
-    {
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-        "AclConfiguration": AclConfigurationTypeDef,
-        "SqlConfiguration": SqlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class DatabaseConfigurationTypeDef(
-    _RequiredDatabaseConfigurationTypeDef, _OptionalDatabaseConfigurationTypeDef
-):
-    pass
-
-
-_RequiredSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceKnowledgeArticleConfigurationTypeDef",
-    {
-        "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
-    },
-)
-_OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceKnowledgeArticleConfigurationTypeDef",
-    {
-        "StandardKnowledgeArticleTypeConfiguration": (
-            SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef
-        ),
-        "CustomKnowledgeArticleTypeConfigurations": Sequence[
-            SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef
-        ],
-    },
-    total=False,
-)
-
-
-class SalesforceKnowledgeArticleConfigurationTypeDef(
-    _RequiredSalesforceKnowledgeArticleConfigurationTypeDef,
-    _OptionalSalesforceKnowledgeArticleConfigurationTypeDef,
-):
-    pass
-
-
-_RequiredServiceNowConfigurationTypeDef = TypedDict(
-    "_RequiredServiceNowConfigurationTypeDef",
-    {
-        "HostUrl": str,
-        "SecretArn": str,
-        "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
-    },
-)
-_OptionalServiceNowConfigurationTypeDef = TypedDict(
-    "_OptionalServiceNowConfigurationTypeDef",
-    {
-        "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationTypeDef,
-        "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationTypeDef,
-        "AuthenticationType": ServiceNowAuthenticationTypeType,
-    },
-    total=False,
-)
-
-
-class ServiceNowConfigurationTypeDef(
-    _RequiredServiceNowConfigurationTypeDef, _OptionalServiceNowConfigurationTypeDef
-):
-    pass
-
-
 _RequiredGitHubConfigurationTypeDef = TypedDict(
     "_RequiredGitHubConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGitHubConfigurationTypeDef = TypedDict(
@@ -4442,20 +3919,42 @@
         "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": Sequence[
             DataSourceToIndexFieldMappingTypeDef
         ],
     },
     total=False,
 )
 
-
 class GitHubConfigurationTypeDef(
     _RequiredGitHubConfigurationTypeDef, _OptionalGitHubConfigurationTypeDef
 ):
     pass
 
+_RequiredOneDriveConfigurationOutputTypeDef = TypedDict(
+    "_RequiredOneDriveConfigurationOutputTypeDef",
+    {
+        "TenantDomain": str,
+        "SecretArn": str,
+        "OneDriveUsers": OneDriveUsersOutputTypeDef,
+    },
+)
+_OptionalOneDriveConfigurationOutputTypeDef = TypedDict(
+    "_OptionalOneDriveConfigurationOutputTypeDef",
+    {
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "DisableLocalGroups": bool,
+    },
+    total=False,
+)
+
+class OneDriveConfigurationOutputTypeDef(
+    _RequiredOneDriveConfigurationOutputTypeDef, _OptionalOneDriveConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredOneDriveConfigurationTypeDef = TypedDict(
     "_RequiredOneDriveConfigurationTypeDef",
     {
         "TenantDomain": str,
         "SecretArn": str,
         "OneDriveUsers": OneDriveUsersTypeDef,
@@ -4468,35 +3967,33 @@
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
         "DisableLocalGroups": bool,
     },
     total=False,
 )
 
-
 class OneDriveConfigurationTypeDef(
     _RequiredOneDriveConfigurationTypeDef, _OptionalOneDriveConfigurationTypeDef
 ):
     pass
 
-
 DescribeQuerySuggestionsConfigResponseTypeDef = TypedDict(
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     {
         "Mode": ModeType,
         "Status": QuerySuggestionsStatusType,
         "QueryLogLookBackWindowInDays": int,
         "IncludeQueriesWithoutUserInformation": bool,
         "MinimumNumberOfQueryingUsers": int,
         "MinimumQueryCount": int,
         "LastSuggestionsBuildTime": datetime,
         "LastClearTime": datetime,
         "TotalSuggestionsCount": int,
         "AttributeSuggestionsConfig": AttributeSuggestionsDescribeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -4511,22 +4008,20 @@
         "MinimumNumberOfQueryingUsers": int,
         "MinimumQueryCount": int,
         "AttributeSuggestionsConfig": AttributeSuggestionsUpdateConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
     _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
     _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredConfluenceConfigurationOutputTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationOutputTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4537,27 +4032,25 @@
         "SpaceConfiguration": ConfluenceSpaceConfigurationOutputTypeDef,
         "PageConfiguration": ConfluencePageConfigurationOutputTypeDef,
         "BlogConfiguration": ConfluenceBlogConfigurationOutputTypeDef,
         "AttachmentConfiguration": ConfluenceAttachmentConfigurationOutputTypeDef,
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationType": ConfluenceAuthenticationTypeType,
     },
     total=False,
 )
 
-
 class ConfluenceConfigurationOutputTypeDef(
     _RequiredConfluenceConfigurationOutputTypeDef, _OptionalConfluenceConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredConfluenceConfigurationTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4574,20 +4067,30 @@
         "ExclusionPatterns": Sequence[str],
         "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationType": ConfluenceAuthenticationTypeType,
     },
     total=False,
 )
 
-
 class ConfluenceConfigurationTypeDef(
     _RequiredConfluenceConfigurationTypeDef, _OptionalConfluenceConfigurationTypeDef
 ):
     pass
 
+DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccessControlConfigurationResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "ErrorMessage": str,
+        "AccessControlList": List[PrincipalTypeDef],
+        "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
     },
@@ -4599,22 +4102,20 @@
         "AccessControlList": Sequence[PrincipalTypeDef],
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
@@ -4625,21 +4126,35 @@
         "Description": str,
         "AccessControlList": Sequence[PrincipalTypeDef],
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
     },
     total=False,
 )
 
-
 class UpdateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
+CreateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "CreateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "UpdateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AttributeSuggestionsGetConfigTypeDef = TypedDict(
     "AttributeSuggestionsGetConfigTypeDef",
     {
         "SuggestionAttributes": Sequence[str],
         "AdditionalResponseAttributes": Sequence[str],
         "AttributeFilter": "AttributeFilterTypeDef",
@@ -4649,36 +4164,24 @@
 )
 
 ListDataSourceSyncJobsResponseTypeDef = TypedDict(
     "ListDataSourceSyncJobsResponseTypeDef",
     {
         "History": List[DataSourceSyncJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
-    "DescribeAccessControlConfigurationResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "ErrorMessage": str,
-        "AccessControlList": List[PrincipalOutputTypeDef],
-        "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExperiencesResponseTypeDef = TypedDict(
     "ListExperiencesResponseTypeDef",
     {
         "SummaryItems": List[ExperiencesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHookConfigurationOutputTypeDef = TypedDict(
     "_RequiredHookConfigurationOutputTypeDef",
     {
         "LambdaArn": str,
@@ -4689,21 +4192,19 @@
     "_OptionalHookConfigurationOutputTypeDef",
     {
         "InvocationCondition": DocumentAttributeConditionOutputTypeDef,
     },
     total=False,
 )
 
-
 class HookConfigurationOutputTypeDef(
     _RequiredHookConfigurationOutputTypeDef, _OptionalHookConfigurationOutputTypeDef
 ):
     pass
 
-
 RetrieveResultItemTypeDef = TypedDict(
     "RetrieveResultItemTypeDef",
     {
         "Id": str,
         "DocumentId": str,
         "DocumentTitle": str,
         "Content": str,
@@ -4744,21 +4245,19 @@
     "_OptionalHookConfigurationTypeDef",
     {
         "InvocationCondition": DocumentAttributeConditionTypeDef,
     },
     total=False,
 )
 
-
 class HookConfigurationTypeDef(
     _RequiredHookConfigurationTypeDef, _OptionalHookConfigurationTypeDef
 ):
     pass
 
-
 InlineCustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     {
         "Condition": DocumentAttributeConditionTypeDef,
         "Target": DocumentAttributeTargetTypeDef,
         "DocumentContentDeletion": bool,
     },
@@ -4792,19 +4291,17 @@
     "_OptionalDocumentInfoTypeDef",
     {
         "Attributes": Sequence[DocumentAttributeTypeDef],
     },
     total=False,
 )
 
-
 class DocumentInfoTypeDef(_RequiredDocumentInfoTypeDef, _OptionalDocumentInfoTypeDef):
     pass
 
-
 _RequiredDocumentTypeDef = TypedDict(
     "_RequiredDocumentTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDocumentTypeDef = TypedDict(
@@ -4818,19 +4315,17 @@
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
         "ContentType": ContentTypeType,
         "AccessControlConfigurationId": str,
     },
     total=False,
 )
 
-
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
-
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -4848,21 +4343,19 @@
         "UserContext": UserContextTypeDef,
         "VisitorId": str,
         "SpellCorrectionConfiguration": SpellCorrectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredRetrieveRequestRequestTypeDef = TypedDict(
     "_RequiredRetrieveRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -4875,27 +4368,25 @@
         "PageNumber": int,
         "PageSize": int,
         "UserContext": UserContextTypeDef,
     },
     total=False,
 )
 
-
 class RetrieveRequestRequestTypeDef(
     _RequiredRetrieveRequestRequestTypeDef, _OptionalRetrieveRequestRequestTypeDef
 ):
     pass
 
-
 ListExperienceEntitiesResponseTypeDef = TypedDict(
     "ListExperienceEntitiesResponseTypeDef",
     {
         "SummaryItems": List[ExperienceEntitiesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExperienceResponseTypeDef = TypedDict(
     "DescribeExperienceResponseTypeDef",
     {
         "Id": str,
@@ -4905,15 +4396,15 @@
         "Configuration": ExperienceConfigurationOutputTypeDef,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Description": str,
         "Status": ExperienceStatusType,
         "RoleArn": str,
         "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperienceRequestRequestTypeDef",
     {
         "Name": str,
@@ -4927,21 +4418,19 @@
         "Configuration": ExperienceConfigurationTypeDef,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateExperienceRequestRequestTypeDef(
     _RequiredCreateExperienceRequestRequestTypeDef, _OptionalCreateExperienceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4952,37 +4441,19 @@
         "RoleArn": str,
         "Configuration": ExperienceConfigurationTypeDef,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateExperienceRequestRequestTypeDef(
     _RequiredUpdateExperienceRequestRequestTypeDef, _OptionalUpdateExperienceRequestRequestTypeDef
 ):
     pass
 
-
-CreateFeaturedResultsSetResponseTypeDef = TypedDict(
-    "CreateFeaturedResultsSetResponseTypeDef",
-    {
-        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
-    "UpdateFeaturedResultsSetResponseTypeDef",
-    {
-        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutPrincipalMappingRequestRequestTypeDef = TypedDict(
     "_RequiredPutPrincipalMappingRequestRequestTypeDef",
     {
         "IndexId": str,
         "GroupId": str,
         "GroupMembers": GroupMembersTypeDef,
     },
@@ -4993,53 +4464,28 @@
         "DataSourceId": str,
         "OrderingId": int,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class PutPrincipalMappingRequestRequestTypeDef(
     _RequiredPutPrincipalMappingRequestRequestTypeDef,
     _OptionalPutPrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
-
 AdditionalResultAttributeValueTypeDef = TypedDict(
     "AdditionalResultAttributeValueTypeDef",
     {
         "TextWithHighlightsValue": TextWithHighlightsTypeDef,
     },
     total=False,
 )
 
-DescribeIndexResponseTypeDef = TypedDict(
-    "DescribeIndexResponseTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Edition": IndexEditionType,
-        "RoleArn": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "Status": IndexStatusType,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationOutputTypeDef],
-        "IndexStatistics": IndexStatisticsTypeDef,
-        "ErrorMessage": str,
-        "CapacityUnits": CapacityUnitsConfigurationOutputTypeDef,
-        "UserTokenConfigurations": List[UserTokenConfigurationOutputTypeDef],
-        "UserContextPolicy": UserContextPolicyType,
-        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIndexRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -5054,20 +4500,41 @@
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
+DescribeIndexResponseTypeDef = TypedDict(
+    "DescribeIndexResponseTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Edition": IndexEditionType,
+        "RoleArn": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "Status": IndexStatusType,
+        "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationOutputTypeDef],
+        "IndexStatistics": IndexStatisticsTypeDef,
+        "ErrorMessage": str,
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
+        "UserContextPolicy": UserContextPolicyType,
+        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -5082,21 +4549,19 @@
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateIndexRequestRequestTypeDef(
     _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredWebCrawlerConfigurationOutputTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationOutputTypeDef",
     {
         "Urls": UrlsOutputTypeDef,
     },
 )
 _OptionalWebCrawlerConfigurationOutputTypeDef = TypedDict(
@@ -5104,27 +4569,25 @@
     {
         "CrawlDepth": int,
         "MaxLinksPerPage": int,
         "MaxContentSizePerPageInMegaBytes": float,
         "MaxUrlsPerMinuteCrawlRate": int,
         "UrlInclusionPatterns": List[str],
         "UrlExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class WebCrawlerConfigurationOutputTypeDef(
     _RequiredWebCrawlerConfigurationOutputTypeDef, _OptionalWebCrawlerConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredWebCrawlerConfigurationTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationTypeDef",
     {
         "Urls": UrlsTypeDef,
     },
 )
 _OptionalWebCrawlerConfigurationTypeDef = TypedDict(
@@ -5138,21 +4601,19 @@
         "UrlExclusionPatterns": Sequence[str],
         "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class WebCrawlerConfigurationTypeDef(
     _RequiredWebCrawlerConfigurationTypeDef, _OptionalWebCrawlerConfigurationTypeDef
 ):
     pass
 
-
 SuggestionValueTypeDef = TypedDict(
     "SuggestionValueTypeDef",
     {
         "Text": SuggestionTextWithHighlightsTypeDef,
     },
     total=False,
 )
@@ -5185,21 +4646,19 @@
         ),
         "IncludeAttachmentFilePatterns": List[str],
         "ExcludeAttachmentFilePatterns": List[str],
     },
     total=False,
 )
 
-
 class SalesforceConfigurationOutputTypeDef(
     _RequiredSalesforceConfigurationOutputTypeDef, _OptionalSalesforceConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredSalesforceConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
     },
 )
@@ -5215,21 +4674,19 @@
         ),
         "IncludeAttachmentFilePatterns": Sequence[str],
         "ExcludeAttachmentFilePatterns": Sequence[str],
     },
     total=False,
 )
 
-
 class SalesforceConfigurationTypeDef(
     _RequiredSalesforceConfigurationTypeDef, _OptionalSalesforceConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -5239,28 +4696,26 @@
         "MaxSuggestionsCount": int,
         "SuggestionTypes": Sequence[SuggestionTypeType],
         "AttributeSuggestionsConfig": AttributeSuggestionsGetConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetQuerySuggestionsRequestRequestTypeDef(
     _RequiredGetQuerySuggestionsRequestRequestTypeDef,
     _OptionalGetQuerySuggestionsRequestRequestTypeDef,
 ):
     pass
 
-
 RetrieveResultTypeDef = TypedDict(
     "RetrieveResultTypeDef",
     {
         "QueryId": str,
         "ResultItems": List[RetrieveResultItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
     "CustomDocumentEnrichmentConfigurationOutputTypeDef",
     {
         "InlineConfigurations": List[InlineCustomDocumentEnrichmentConfigurationOutputTypeDef],
@@ -5371,21 +4826,19 @@
     {
         "RoleArn": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class BatchPutDocumentRequestRequestTypeDef(
     _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
 ):
     pass
 
-
 FeaturedResultsItemTypeDef = TypedDict(
     "FeaturedResultsItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
@@ -5418,15 +4871,15 @@
 )
 
 GetQuerySuggestionsResponseTypeDef = TypedDict(
     "GetQuerySuggestionsResponseTypeDef",
     {
         "QuerySuggestionsId": str,
         "Suggestions": List[SuggestionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSourceResponseTypeDef = TypedDict(
     "DescribeDataSourceResponseTypeDef",
     {
         "Id": str,
@@ -5440,15 +4893,15 @@
         "Description": str,
         "Status": DataSourceStatusType,
         "Schedule": str,
         "RoleArn": str,
         "ErrorMessage": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "Name": str,
@@ -5468,21 +4921,19 @@
         "ClientToken": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -5497,27 +4948,25 @@
         "RoleArn": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDataSourceRequestRequestTypeDef(
     _RequiredUpdateDataSourceRequestRequestTypeDef, _OptionalUpdateDataSourceRequestRequestTypeDef
 ):
     pass
 
-
 QueryResultTypeDef = TypedDict(
     "QueryResultTypeDef",
     {
         "QueryId": str,
         "ResultItems": List[QueryResultItemTypeDef],
         "FacetResults": List["FacetResultTypeDef"],
         "TotalNumberOfResults": int,
         "Warnings": List[WarningTypeDef],
         "SpellCorrectedQueries": List[SpellCorrectedQueryTypeDef],
         "FeaturedResultsItems": List[FeaturedResultsItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra/type_defs.pyi` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,137 +82,106 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessControlConfigurationSummaryTypeDef",
-    "AccessControlListConfigurationOutputTypeDef",
     "AccessControlListConfigurationTypeDef",
-    "AclConfigurationOutputTypeDef",
     "AclConfigurationTypeDef",
-    "DataSourceToIndexFieldMappingOutputTypeDef",
-    "DataSourceVpcConfigurationOutputTypeDef",
-    "S3PathOutputTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
-    "DataSourceVpcConfigurationTypeDef",
+    "DataSourceVpcConfigurationOutputTypeDef",
     "S3PathTypeDef",
+    "DataSourceVpcConfigurationTypeDef",
     "EntityConfigurationTypeDef",
     "FailedEntityTypeDef",
+    "ResponseMetadataTypeDef",
     "EntityPersonaConfigurationTypeDef",
-    "SuggestableConfigOutputTypeDef",
     "SuggestableConfigTypeDef",
-    "BasicAuthenticationConfigurationOutputTypeDef",
     "BasicAuthenticationConfigurationTypeDef",
     "DataSourceSyncJobMetricTargetTypeDef",
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     "BatchDeleteFeaturedResultsSetErrorTypeDef",
     "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
     "BatchGetDocumentStatusResponseErrorTypeDef",
     "StatusTypeDef",
     "BatchPutDocumentResponseFailedDocumentTypeDef",
-    "CapacityUnitsConfigurationOutputTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "ClearQuerySuggestionsRequestRequestTypeDef",
     "ClickFeedbackTypeDef",
-    "ConfluenceAttachmentToIndexFieldMappingOutputTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
-    "ConfluenceBlogToIndexFieldMappingOutputTypeDef",
     "ConfluenceBlogToIndexFieldMappingTypeDef",
-    "ProxyConfigurationOutputTypeDef",
     "ProxyConfigurationTypeDef",
-    "ConfluencePageToIndexFieldMappingOutputTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
-    "ConfluenceSpaceToIndexFieldMappingOutputTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
-    "ConnectionConfigurationOutputTypeDef",
     "ConnectionConfigurationTypeDef",
     "ContentSourceConfigurationOutputTypeDef",
     "ContentSourceConfigurationTypeDef",
     "CorrectionTypeDef",
     "PrincipalTypeDef",
-    "CreateAccessControlConfigurationResponseTypeDef",
     "TagTypeDef",
-    "CreateDataSourceResponseTypeDef",
-    "CreateExperienceResponseTypeDef",
-    "CreateFaqResponseTypeDef",
     "FeaturedDocumentTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "UserGroupResolutionConfigurationTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    "CreateThesaurusResponseTypeDef",
     "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "DataSourceGroupTypeDef",
     "DataSourceSummaryTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
-    "SqlConfigurationOutputTypeDef",
     "SqlConfigurationTypeDef",
     "DeleteAccessControlConfigurationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
     "DeleteExperienceRequestRequestTypeDef",
     "DeleteFaqRequestRequestTypeDef",
     "DeleteIndexRequestRequestTypeDef",
     "DeletePrincipalMappingRequestRequestTypeDef",
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     "DeleteThesaurusRequestRequestTypeDef",
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
-    "PrincipalOutputTypeDef",
     "DescribeDataSourceRequestRequestTypeDef",
     "DescribeExperienceRequestRequestTypeDef",
     "ExperienceEndpointTypeDef",
     "DescribeFaqRequestRequestTypeDef",
     "DescribeFeaturedResultsSetRequestRequestTypeDef",
     "FeaturedDocumentMissingTypeDef",
     "FeaturedDocumentWithMetadataTypeDef",
     "DescribeIndexRequestRequestTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    "UserGroupResolutionConfigurationOutputTypeDef",
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
     "DocumentAttributeValueOutputTypeDef",
     "DocumentAttributeValueTypeDef",
     "RelevanceOutputTypeDef",
-    "SearchOutputTypeDef",
-    "RelevanceTypeDef",
     "SearchTypeDef",
-    "DocumentsMetadataConfigurationOutputTypeDef",
+    "RelevanceTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EntityDisplayDataTypeDef",
-    "UserIdentityConfigurationOutputTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
     "FacetTypeDef",
     "FaqStatisticsTypeDef",
     "FaqSummaryTypeDef",
-    "FeaturedDocumentOutputTypeDef",
     "FeaturedResultsSetSummaryTypeDef",
     "GetSnapshotsRequestRequestTypeDef",
     "TimeRangeOutputTypeDef",
-    "GitHubDocumentCrawlPropertiesOutputTypeDef",
-    "SaaSConfigurationOutputTypeDef",
     "GitHubDocumentCrawlPropertiesTypeDef",
     "SaaSConfigurationTypeDef",
     "MemberGroupTypeDef",
     "MemberUserTypeDef",
     "GroupSummaryTypeDef",
     "HighlightTypeDef",
     "IndexConfigurationSummaryTypeDef",
     "TextDocumentStatisticsTypeDef",
-    "JsonTokenTypeConfigurationOutputTypeDef",
     "JsonTokenTypeConfigurationTypeDef",
-    "JwtTokenTypeConfigurationOutputTypeDef",
     "JwtTokenTypeConfigurationTypeDef",
     "ListAccessControlConfigurationsRequestRequestTypeDef",
     "TimeRangeTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListEntityPersonasRequestRequestTypeDef",
     "PersonasSummaryTypeDef",
     "ListExperienceEntitiesRequestRequestTypeDef",
@@ -220,81 +189,86 @@
     "ListFaqsRequestRequestTypeDef",
     "ListFeaturedResultsSetsRequestRequestTypeDef",
     "ListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     "ListIndicesRequestRequestTypeDef",
     "ListQuerySuggestionsBlockListsRequestRequestTypeDef",
     "QuerySuggestionsBlockListSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListThesauriRequestRequestTypeDef",
     "ThesaurusSummaryTypeDef",
     "SortingConfigurationTypeDef",
     "SpellCorrectionConfigurationTypeDef",
     "ScoreAttributesTypeDef",
     "WarningTypeDef",
     "RelevanceFeedbackTypeDef",
-    "ResponseMetadataTypeDef",
     "SeedUrlConfigurationOutputTypeDef",
     "SeedUrlConfigurationTypeDef",
     "SiteMapsConfigurationOutputTypeDef",
     "SiteMapsConfigurationTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
-    "StartDataSourceSyncJobResponseTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "SuggestionHighlightTypeDef",
     "TableCellTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListAccessControlConfigurationsResponseTypeDef",
     "ColumnConfigurationOutputTypeDef",
+    "ColumnConfigurationTypeDef",
     "GoogleDriveConfigurationOutputTypeDef",
+    "GoogleDriveConfigurationTypeDef",
     "SalesforceChatterFeedConfigurationOutputTypeDef",
+    "SalesforceChatterFeedConfigurationTypeDef",
     "SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
+    "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
+    "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
+    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     "SalesforceStandardObjectConfigurationOutputTypeDef",
+    "SalesforceStandardObjectConfigurationTypeDef",
     "ServiceNowKnowledgeArticleConfigurationOutputTypeDef",
+    "ServiceNowKnowledgeArticleConfigurationTypeDef",
     "ServiceNowServiceCatalogConfigurationOutputTypeDef",
+    "ServiceNowServiceCatalogConfigurationTypeDef",
     "WorkDocsConfigurationOutputTypeDef",
+    "WorkDocsConfigurationTypeDef",
     "BoxConfigurationOutputTypeDef",
     "FsxConfigurationOutputTypeDef",
     "JiraConfigurationOutputTypeDef",
     "QuipConfigurationOutputTypeDef",
     "SlackConfigurationOutputTypeDef",
     "AlfrescoConfigurationOutputTypeDef",
-    "DescribeFaqResponseTypeDef",
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    "DescribeThesaurusResponseTypeDef",
-    "OnPremiseConfigurationOutputTypeDef",
+    "OnPremiseConfigurationTypeDef",
     "OneDriveUsersOutputTypeDef",
-    "ColumnConfigurationTypeDef",
-    "GoogleDriveConfigurationTypeDef",
-    "SalesforceChatterFeedConfigurationTypeDef",
-    "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
-    "SalesforceStandardObjectConfigurationTypeDef",
-    "ServiceNowKnowledgeArticleConfigurationTypeDef",
-    "ServiceNowServiceCatalogConfigurationTypeDef",
-    "WorkDocsConfigurationTypeDef",
+    "OneDriveUsersTypeDef",
+    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+    "UpdateThesaurusRequestRequestTypeDef",
+    "AlfrescoConfigurationTypeDef",
     "BoxConfigurationTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
-    "AlfrescoConfigurationTypeDef",
-    "OnPremiseConfigurationTypeDef",
-    "OneDriveUsersTypeDef",
-    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
-    "UpdateThesaurusRequestRequestTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
     "AssociatePersonasToEntitiesResponseTypeDef",
+    "CreateAccessControlConfigurationResponseTypeDef",
+    "CreateDataSourceResponseTypeDef",
+    "CreateExperienceResponseTypeDef",
+    "CreateFaqResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    "CreateThesaurusResponseTypeDef",
+    "DescribeFaqResponseTypeDef",
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    "DescribeThesaurusResponseTypeDef",
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     "DisassociatePersonasFromEntitiesResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAccessControlConfigurationsResponseTypeDef",
+    "StartDataSourceSyncJobResponseTypeDef",
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
     "AttributeSuggestionsDescribeConfigTypeDef",
     "AttributeSuggestionsUpdateConfigTypeDef",
     "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
@@ -308,83 +282,84 @@
     "SharePointConfigurationOutputTypeDef",
     "SharePointConfigurationTypeDef",
     "ConfluencePageConfigurationOutputTypeDef",
     "ConfluencePageConfigurationTypeDef",
     "ConfluenceSpaceConfigurationOutputTypeDef",
     "ConfluenceSpaceConfigurationTypeDef",
     "SpellCorrectedQueryTypeDef",
+    "HierarchicalPrincipalOutputTypeDef",
     "HierarchicalPrincipalTypeDef",
     "CreateFaqRequestRequestTypeDef",
     "CreateQuerySuggestionsBlockListRequestRequestTypeDef",
     "CreateThesaurusRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateFeaturedResultsSetRequestRequestTypeDef",
+    "FeaturedResultsSetTypeDef",
     "UpdateFeaturedResultsSetRequestRequestTypeDef",
     "UserContextTypeDef",
     "ListDataSourcesResponseTypeDef",
     "DataSourceSyncJobTypeDef",
-    "HierarchicalPrincipalOutputTypeDef",
     "ExperiencesSummaryTypeDef",
     "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
     "DocumentAttributeConditionOutputTypeDef",
     "DocumentAttributeOutputTypeDef",
     "DocumentAttributeTargetOutputTypeDef",
     "DocumentAttributeValueCountPairTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "DocumentMetadataConfigurationOutputTypeDef",
-    "DocumentRelevanceConfigurationTypeDef",
     "DocumentMetadataConfigurationTypeDef",
+    "DocumentRelevanceConfigurationTypeDef",
     "S3DataSourceConfigurationOutputTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
     "ExperienceConfigurationOutputTypeDef",
     "ExperienceConfigurationTypeDef",
     "ListFaqsResponseTypeDef",
-    "FeaturedResultsSetTypeDef",
     "ListFeaturedResultsSetsResponseTypeDef",
     "GetSnapshotsResponseTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
-    "UserTokenConfigurationOutputTypeDef",
     "UserTokenConfigurationTypeDef",
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     "ListEntityPersonasResponseTypeDef",
     "ListQuerySuggestionsBlockListsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListThesauriResponseTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "UrlsOutputTypeDef",
     "UrlsTypeDef",
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
     "DatabaseConfigurationOutputTypeDef",
-    "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
-    "ServiceNowConfigurationOutputTypeDef",
-    "GitHubConfigurationOutputTypeDef",
-    "OneDriveConfigurationOutputTypeDef",
     "DatabaseConfigurationTypeDef",
+    "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
     "SalesforceKnowledgeArticleConfigurationTypeDef",
+    "ServiceNowConfigurationOutputTypeDef",
     "ServiceNowConfigurationTypeDef",
+    "GitHubConfigurationOutputTypeDef",
     "GitHubConfigurationTypeDef",
+    "OneDriveConfigurationOutputTypeDef",
     "OneDriveConfigurationTypeDef",
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
     "ConfluenceConfigurationOutputTypeDef",
     "ConfluenceConfigurationTypeDef",
+    "DescribeAccessControlConfigurationResponseTypeDef",
     "CreateAccessControlConfigurationRequestRequestTypeDef",
     "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "CreateFeaturedResultsSetResponseTypeDef",
+    "UpdateFeaturedResultsSetResponseTypeDef",
     "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
-    "DescribeAccessControlConfigurationResponseTypeDef",
     "ListExperiencesResponseTypeDef",
     "HookConfigurationOutputTypeDef",
     "RetrieveResultItemTypeDef",
     "SourceDocumentTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
     "HookConfigurationTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
@@ -393,20 +368,18 @@
     "DocumentTypeDef",
     "QueryRequestRequestTypeDef",
     "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
     "DescribeExperienceResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
-    "CreateFeaturedResultsSetResponseTypeDef",
-    "UpdateFeaturedResultsSetResponseTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
-    "DescribeIndexResponseTypeDef",
     "CreateIndexRequestRequestTypeDef",
+    "DescribeIndexResponseTypeDef",
     "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationOutputTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
     "SalesforceConfigurationOutputTypeDef",
     "SalesforceConfigurationTypeDef",
@@ -432,117 +405,75 @@
 AccessControlConfigurationSummaryTypeDef = TypedDict(
     "AccessControlConfigurationSummaryTypeDef",
     {
         "Id": str,
     },
 )
 
-AccessControlListConfigurationOutputTypeDef = TypedDict(
-    "AccessControlListConfigurationOutputTypeDef",
-    {
-        "KeyPath": str,
-    },
-    total=False,
-)
-
 AccessControlListConfigurationTypeDef = TypedDict(
     "AccessControlListConfigurationTypeDef",
     {
         "KeyPath": str,
     },
     total=False,
 )
 
-AclConfigurationOutputTypeDef = TypedDict(
-    "AclConfigurationOutputTypeDef",
-    {
-        "AllowedGroupsColumnName": str,
-    },
-)
-
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "AllowedGroupsColumnName": str,
     },
 )
 
-_RequiredDataSourceToIndexFieldMappingOutputTypeDef = TypedDict(
-    "_RequiredDataSourceToIndexFieldMappingOutputTypeDef",
+_RequiredDataSourceToIndexFieldMappingTypeDef = TypedDict(
+    "_RequiredDataSourceToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": str,
         "IndexFieldName": str,
     },
 )
-_OptionalDataSourceToIndexFieldMappingOutputTypeDef = TypedDict(
-    "_OptionalDataSourceToIndexFieldMappingOutputTypeDef",
+_OptionalDataSourceToIndexFieldMappingTypeDef = TypedDict(
+    "_OptionalDataSourceToIndexFieldMappingTypeDef",
     {
         "DateFieldFormat": str,
     },
     total=False,
 )
 
-class DataSourceToIndexFieldMappingOutputTypeDef(
-    _RequiredDataSourceToIndexFieldMappingOutputTypeDef,
-    _OptionalDataSourceToIndexFieldMappingOutputTypeDef,
+
+class DataSourceToIndexFieldMappingTypeDef(
+    _RequiredDataSourceToIndexFieldMappingTypeDef, _OptionalDataSourceToIndexFieldMappingTypeDef
 ):
     pass
 
+
 DataSourceVpcConfigurationOutputTypeDef = TypedDict(
     "DataSourceVpcConfigurationOutputTypeDef",
     {
         "SubnetIds": List[str],
         "SecurityGroupIds": List[str],
     },
 )
 
-S3PathOutputTypeDef = TypedDict(
-    "S3PathOutputTypeDef",
+S3PathTypeDef = TypedDict(
+    "S3PathTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-_RequiredDataSourceToIndexFieldMappingTypeDef = TypedDict(
-    "_RequiredDataSourceToIndexFieldMappingTypeDef",
-    {
-        "DataSourceFieldName": str,
-        "IndexFieldName": str,
-    },
-)
-_OptionalDataSourceToIndexFieldMappingTypeDef = TypedDict(
-    "_OptionalDataSourceToIndexFieldMappingTypeDef",
-    {
-        "DateFieldFormat": str,
-    },
-    total=False,
-)
-
-class DataSourceToIndexFieldMappingTypeDef(
-    _RequiredDataSourceToIndexFieldMappingTypeDef, _OptionalDataSourceToIndexFieldMappingTypeDef
-):
-    pass
-
 DataSourceVpcConfigurationTypeDef = TypedDict(
     "DataSourceVpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
 
-S3PathTypeDef = TypedDict(
-    "S3PathTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-
 EntityConfigurationTypeDef = TypedDict(
     "EntityConfigurationTypeDef",
     {
         "EntityId": str,
         "EntityType": EntityTypeType,
     },
 )
@@ -552,49 +483,42 @@
     {
         "EntityId": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-EntityPersonaConfigurationTypeDef = TypedDict(
-    "EntityPersonaConfigurationTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EntityId": str,
-        "Persona": PersonaType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-SuggestableConfigOutputTypeDef = TypedDict(
-    "SuggestableConfigOutputTypeDef",
+EntityPersonaConfigurationTypeDef = TypedDict(
+    "EntityPersonaConfigurationTypeDef",
     {
-        "AttributeName": str,
-        "Suggestable": bool,
+        "EntityId": str,
+        "Persona": PersonaType,
     },
-    total=False,
 )
 
 SuggestableConfigTypeDef = TypedDict(
     "SuggestableConfigTypeDef",
     {
         "AttributeName": str,
         "Suggestable": bool,
     },
     total=False,
 )
 
-BasicAuthenticationConfigurationOutputTypeDef = TypedDict(
-    "BasicAuthenticationConfigurationOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Credentials": str,
-    },
-)
-
 BasicAuthenticationConfigurationTypeDef = TypedDict(
     "BasicAuthenticationConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
         "Credentials": str,
     },
@@ -610,19 +534,21 @@
     "_OptionalDataSourceSyncJobMetricTargetTypeDef",
     {
         "DataSourceSyncJobId": str,
     },
     total=False,
 )
 
+
 class DataSourceSyncJobMetricTargetTypeDef(
     _RequiredDataSourceSyncJobMetricTargetTypeDef, _OptionalDataSourceSyncJobMetricTargetTypeDef
 ):
     pass
 
+
 BatchDeleteDocumentResponseFailedDocumentTypeDef = TypedDict(
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     {
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
@@ -673,22 +599,14 @@
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-CapacityUnitsConfigurationOutputTypeDef = TypedDict(
-    "CapacityUnitsConfigurationOutputTypeDef",
-    {
-        "StorageCapacityUnits": int,
-        "QueryCapacityUnits": int,
-    },
-)
-
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
     {
         "StorageCapacityUnits": int,
         "QueryCapacityUnits": int,
     },
 )
@@ -704,74 +622,34 @@
     "ClickFeedbackTypeDef",
     {
         "ResultId": str,
         "ClickTime": Union[datetime, str],
     },
 )
 
-ConfluenceAttachmentToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluenceAttachmentToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
-
 ConfluenceAttachmentToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-ConfluenceBlogToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluenceBlogToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluenceBlogFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
-
 ConfluenceBlogToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceBlogToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceBlogFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-_RequiredProxyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProxyConfigurationOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-    },
-)
-_OptionalProxyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProxyConfigurationOutputTypeDef",
-    {
-        "Credentials": str,
-    },
-    total=False,
-)
-
-class ProxyConfigurationOutputTypeDef(
-    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
     },
 )
@@ -779,70 +657,41 @@
     "_OptionalProxyConfigurationTypeDef",
     {
         "Credentials": str,
     },
     total=False,
 )
 
+
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
-ConfluencePageToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluencePageToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluencePageFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
 
 ConfluencePageToIndexFieldMappingTypeDef = TypedDict(
     "ConfluencePageToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluencePageFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-ConfluenceSpaceToIndexFieldMappingOutputTypeDef = TypedDict(
-    "ConfluenceSpaceToIndexFieldMappingOutputTypeDef",
-    {
-        "DataSourceFieldName": ConfluenceSpaceFieldNameType,
-        "DateFieldFormat": str,
-        "IndexFieldName": str,
-    },
-    total=False,
-)
-
 ConfluenceSpaceToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceSpaceFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
     total=False,
 )
 
-ConnectionConfigurationOutputTypeDef = TypedDict(
-    "ConnectionConfigurationOutputTypeDef",
-    {
-        "DatabaseHost": str,
-        "DatabasePort": int,
-        "DatabaseName": str,
-        "TableName": str,
-        "SecretArn": str,
-    },
-)
-
 ConnectionConfigurationTypeDef = TypedDict(
     "ConnectionConfigurationTypeDef",
     {
         "DatabaseHost": str,
         "DatabasePort": int,
         "DatabaseName": str,
         "TableName": str,
@@ -893,57 +742,27 @@
     "_OptionalPrincipalTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
+
 class PrincipalTypeDef(_RequiredPrincipalTypeDef, _OptionalPrincipalTypeDef):
     pass
 
-CreateAccessControlConfigurationResponseTypeDef = TypedDict(
-    "CreateAccessControlConfigurationResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateDataSourceResponseTypeDef = TypedDict(
-    "CreateDataSourceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateExperienceResponseTypeDef = TypedDict(
-    "CreateExperienceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFaqResponseTypeDef = TypedDict(
-    "CreateFaqResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FeaturedDocumentTypeDef = TypedDict(
     "FeaturedDocumentTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
@@ -959,38 +778,14 @@
 UserGroupResolutionConfigurationTypeDef = TypedDict(
     "UserGroupResolutionConfigurationTypeDef",
     {
         "UserGroupResolutionMode": UserGroupResolutionModeType,
     },
 )
 
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThesaurusResponseTypeDef = TypedDict(
-    "CreateThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TemplateConfigurationOutputTypeDef = TypedDict(
     "TemplateConfigurationOutputTypeDef",
     {
         "Template": Dict[str, Any],
     },
     total=False,
 )
@@ -1033,22 +828,14 @@
         "DocumentsDeleted": str,
         "DocumentsFailed": str,
         "DocumentsScanned": str,
     },
     total=False,
 )
 
-SqlConfigurationOutputTypeDef = TypedDict(
-    "SqlConfigurationOutputTypeDef",
-    {
-        "QueryIdentifiersEnclosingOption": QueryIdentifiersEnclosingOptionType,
-    },
-    total=False,
-)
-
 SqlConfigurationTypeDef = TypedDict(
     "SqlConfigurationTypeDef",
     {
         "QueryIdentifiersEnclosingOption": QueryIdentifiersEnclosingOptionType,
     },
     total=False,
 )
@@ -1104,20 +891,22 @@
     {
         "DataSourceId": str,
         "OrderingId": int,
     },
     total=False,
 )
 
+
 class DeletePrincipalMappingRequestRequestTypeDef(
     _RequiredDeletePrincipalMappingRequestRequestTypeDef,
     _OptionalDeletePrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
@@ -1134,33 +923,14 @@
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
 
-_RequiredPrincipalOutputTypeDef = TypedDict(
-    "_RequiredPrincipalOutputTypeDef",
-    {
-        "Name": str,
-        "Type": PrincipalTypeType,
-        "Access": ReadAccessTypeType,
-    },
-)
-_OptionalPrincipalOutputTypeDef = TypedDict(
-    "_OptionalPrincipalOutputTypeDef",
-    {
-        "DataSourceId": str,
-    },
-    total=False,
-)
-
-class PrincipalOutputTypeDef(_RequiredPrincipalOutputTypeDef, _OptionalPrincipalOutputTypeDef):
-    pass
-
 DescribeDataSourceRequestRequestTypeDef = TypedDict(
     "DescribeDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -1219,29 +989,14 @@
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-UserGroupResolutionConfigurationOutputTypeDef = TypedDict(
-    "UserGroupResolutionConfigurationOutputTypeDef",
-    {
-        "UserGroupResolutionMode": UserGroupResolutionModeType,
-    },
-)
-
 _RequiredDescribePrincipalMappingRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePrincipalMappingRequestRequestTypeDef",
     {
         "IndexId": str,
         "GroupId": str,
     },
 )
@@ -1249,20 +1004,22 @@
     "_OptionalDescribePrincipalMappingRequestRequestTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
+
 class DescribePrincipalMappingRequestRequestTypeDef(
     _RequiredDescribePrincipalMappingRequestRequestTypeDef,
     _OptionalDescribePrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
+
 GroupOrderingIdSummaryTypeDef = TypedDict(
     "GroupOrderingIdSummaryTypeDef",
     {
         "Status": PrincipalMappingStatusType,
         "LastUpdatedAt": datetime,
         "ReceivedAt": datetime,
         "OrderingId": int,
@@ -1333,16 +1090,16 @@
         "Duration": str,
         "RankOrder": OrderType,
         "ValueImportanceMap": Dict[str, int],
     },
     total=False,
 )
 
-SearchOutputTypeDef = TypedDict(
-    "SearchOutputTypeDef",
+SearchTypeDef = TypedDict(
+    "SearchTypeDef",
     {
         "Facetable": bool,
         "Searchable": bool,
         "Displayable": bool,
         "Sortable": bool,
     },
     total=False,
@@ -1356,68 +1113,34 @@
         "Duration": str,
         "RankOrder": OrderType,
         "ValueImportanceMap": Mapping[str, int],
     },
     total=False,
 )
 
-SearchTypeDef = TypedDict(
-    "SearchTypeDef",
-    {
-        "Facetable": bool,
-        "Searchable": bool,
-        "Displayable": bool,
-        "Sortable": bool,
-    },
-    total=False,
-)
-
-DocumentsMetadataConfigurationOutputTypeDef = TypedDict(
-    "DocumentsMetadataConfigurationOutputTypeDef",
-    {
-        "S3Prefix": str,
-    },
-    total=False,
-)
-
 DocumentsMetadataConfigurationTypeDef = TypedDict(
     "DocumentsMetadataConfigurationTypeDef",
     {
         "S3Prefix": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EntityDisplayDataTypeDef = TypedDict(
     "EntityDisplayDataTypeDef",
     {
         "UserName": str,
         "GroupName": str,
         "IdentifiedUserName": str,
         "FirstName": str,
         "LastName": str,
     },
     total=False,
 )
 
-UserIdentityConfigurationOutputTypeDef = TypedDict(
-    "UserIdentityConfigurationOutputTypeDef",
-    {
-        "IdentityAttributeName": str,
-    },
-    total=False,
-)
-
 UserIdentityConfigurationTypeDef = TypedDict(
     "UserIdentityConfigurationTypeDef",
     {
         "IdentityAttributeName": str,
     },
     total=False,
 )
@@ -1459,22 +1182,14 @@
         "UpdatedAt": datetime,
         "FileFormat": FaqFileFormatType,
         "LanguageCode": str,
     },
     total=False,
 )
 
-FeaturedDocumentOutputTypeDef = TypedDict(
-    "FeaturedDocumentOutputTypeDef",
-    {
-        "Id": str,
-    },
-    total=False,
-)
-
 FeaturedResultsSetSummaryTypeDef = TypedDict(
     "FeaturedResultsSetSummaryTypeDef",
     {
         "FeaturedResultsSetId": str,
         "FeaturedResultsSetName": str,
         "Status": FeaturedResultsSetStatusType,
         "LastUpdatedTimestamp": int,
@@ -1496,50 +1211,30 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetSnapshotsRequestRequestTypeDef(
     _RequiredGetSnapshotsRequestRequestTypeDef, _OptionalGetSnapshotsRequestRequestTypeDef
 ):
     pass
 
+
 TimeRangeOutputTypeDef = TypedDict(
     "TimeRangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
-GitHubDocumentCrawlPropertiesOutputTypeDef = TypedDict(
-    "GitHubDocumentCrawlPropertiesOutputTypeDef",
-    {
-        "CrawlRepositoryDocuments": bool,
-        "CrawlIssue": bool,
-        "CrawlIssueComment": bool,
-        "CrawlIssueCommentAttachment": bool,
-        "CrawlPullRequest": bool,
-        "CrawlPullRequestComment": bool,
-        "CrawlPullRequestCommentAttachment": bool,
-    },
-    total=False,
-)
-
-SaaSConfigurationOutputTypeDef = TypedDict(
-    "SaaSConfigurationOutputTypeDef",
-    {
-        "OrganizationName": str,
-        "HostUrl": str,
-    },
-)
-
 GitHubDocumentCrawlPropertiesTypeDef = TypedDict(
     "GitHubDocumentCrawlPropertiesTypeDef",
     {
         "CrawlRepositoryDocuments": bool,
         "CrawlIssue": bool,
         "CrawlIssueComment": bool,
         "CrawlIssueCommentAttachment": bool,
@@ -1568,17 +1263,19 @@
     "_OptionalMemberGroupTypeDef",
     {
         "DataSourceId": str,
     },
     total=False,
 )
 
+
 class MemberGroupTypeDef(_RequiredMemberGroupTypeDef, _OptionalMemberGroupTypeDef):
     pass
 
+
 MemberUserTypeDef = TypedDict(
     "MemberUserTypeDef",
     {
         "UserId": str,
     },
 )
 
@@ -1603,17 +1300,19 @@
     {
         "TopAnswer": bool,
         "Type": HighlightTypeType,
     },
     total=False,
 )
 
+
 class HighlightTypeDef(_RequiredHighlightTypeDef, _OptionalHighlightTypeDef):
     pass
 
+
 _RequiredIndexConfigurationSummaryTypeDef = TypedDict(
     "_RequiredIndexConfigurationSummaryTypeDef",
     {
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": IndexStatusType,
     },
@@ -1624,67 +1323,37 @@
         "Name": str,
         "Id": str,
         "Edition": IndexEditionType,
     },
     total=False,
 )
 
+
 class IndexConfigurationSummaryTypeDef(
     _RequiredIndexConfigurationSummaryTypeDef, _OptionalIndexConfigurationSummaryTypeDef
 ):
     pass
 
+
 TextDocumentStatisticsTypeDef = TypedDict(
     "TextDocumentStatisticsTypeDef",
     {
         "IndexedTextDocumentsCount": int,
         "IndexedTextBytes": int,
     },
 )
 
-JsonTokenTypeConfigurationOutputTypeDef = TypedDict(
-    "JsonTokenTypeConfigurationOutputTypeDef",
-    {
-        "UserNameAttributeField": str,
-        "GroupAttributeField": str,
-    },
-)
-
 JsonTokenTypeConfigurationTypeDef = TypedDict(
     "JsonTokenTypeConfigurationTypeDef",
     {
         "UserNameAttributeField": str,
         "GroupAttributeField": str,
     },
 )
 
-_RequiredJwtTokenTypeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredJwtTokenTypeConfigurationOutputTypeDef",
-    {
-        "KeyLocation": KeyLocationType,
-    },
-)
-_OptionalJwtTokenTypeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalJwtTokenTypeConfigurationOutputTypeDef",
-    {
-        "URL": str,
-        "SecretManagerArn": str,
-        "UserNameAttributeField": str,
-        "GroupAttributeField": str,
-        "Issuer": str,
-        "ClaimRegex": str,
-    },
-    total=False,
-)
-
-class JwtTokenTypeConfigurationOutputTypeDef(
-    _RequiredJwtTokenTypeConfigurationOutputTypeDef, _OptionalJwtTokenTypeConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredJwtTokenTypeConfigurationTypeDef = TypedDict(
     "_RequiredJwtTokenTypeConfigurationTypeDef",
     {
         "KeyLocation": KeyLocationType,
     },
 )
 _OptionalJwtTokenTypeConfigurationTypeDef = TypedDict(
@@ -1696,19 +1365,21 @@
         "GroupAttributeField": str,
         "Issuer": str,
         "ClaimRegex": str,
     },
     total=False,
 )
 
+
 class JwtTokenTypeConfigurationTypeDef(
     _RequiredJwtTokenTypeConfigurationTypeDef, _OptionalJwtTokenTypeConfigurationTypeDef
 ):
     pass
 
+
 _RequiredListAccessControlConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessControlConfigurationsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListAccessControlConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1716,20 +1387,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAccessControlConfigurationsRequestRequestTypeDef(
     _RequiredListAccessControlConfigurationsRequestRequestTypeDef,
     _OptionalListAccessControlConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
@@ -1746,19 +1419,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDataSourcesRequestRequestTypeDef(
     _RequiredListDataSourcesRequestRequestTypeDef, _OptionalListDataSourcesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListEntityPersonasRequestRequestTypeDef = TypedDict(
     "_RequiredListEntityPersonasRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -1767,20 +1442,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListEntityPersonasRequestRequestTypeDef(
     _RequiredListEntityPersonasRequestRequestTypeDef,
     _OptionalListEntityPersonasRequestRequestTypeDef,
 ):
     pass
 
+
 PersonasSummaryTypeDef = TypedDict(
     "PersonasSummaryTypeDef",
     {
         "EntityId": str,
         "Persona": PersonaType,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
@@ -1799,20 +1476,22 @@
     "_OptionalListExperienceEntitiesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListExperienceEntitiesRequestRequestTypeDef(
     _RequiredListExperienceEntitiesRequestRequestTypeDef,
     _OptionalListExperienceEntitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListExperiencesRequestRequestTypeDef = TypedDict(
     "_RequiredListExperiencesRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListExperiencesRequestRequestTypeDef = TypedDict(
@@ -1820,19 +1499,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListExperiencesRequestRequestTypeDef(
     _RequiredListExperiencesRequestRequestTypeDef, _OptionalListExperiencesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListFaqsRequestRequestTypeDef = TypedDict(
     "_RequiredListFaqsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListFaqsRequestRequestTypeDef = TypedDict(
@@ -1840,19 +1521,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListFaqsRequestRequestTypeDef(
     _RequiredListFaqsRequestRequestTypeDef, _OptionalListFaqsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturedResultsSetsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
@@ -1860,20 +1543,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListFeaturedResultsSetsRequestRequestTypeDef(
     _RequiredListFeaturedResultsSetsRequestRequestTypeDef,
     _OptionalListFeaturedResultsSetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     {
         "IndexId": str,
         "OrderingId": int,
     },
 )
@@ -1883,20 +1568,22 @@
         "DataSourceId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListGroupsOlderThanOrderingIdRequestRequestTypeDef(
     _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     _OptionalListGroupsOlderThanOrderingIdRequestRequestTypeDef,
 ):
     pass
 
+
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1913,20 +1600,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListQuerySuggestionsBlockListsRequestRequestTypeDef(
     _RequiredListQuerySuggestionsBlockListsRequestRequestTypeDef,
     _OptionalListQuerySuggestionsBlockListsRequestRequestTypeDef,
 ):
     pass
 
+
 QuerySuggestionsBlockListSummaryTypeDef = TypedDict(
     "QuerySuggestionsBlockListSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": QuerySuggestionsBlockListStatusType,
         "CreatedAt": datetime,
@@ -1939,22 +1628,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 _RequiredListThesauriRequestRequestTypeDef = TypedDict(
     "_RequiredListThesauriRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListThesauriRequestRequestTypeDef = TypedDict(
@@ -1962,19 +1643,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListThesauriRequestRequestTypeDef(
     _RequiredListThesauriRequestRequestTypeDef, _OptionalListThesauriRequestRequestTypeDef
 ):
     pass
 
+
 ThesaurusSummaryTypeDef = TypedDict(
     "ThesaurusSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": ThesaurusStatusType,
         "CreatedAt": datetime,
@@ -2019,63 +1702,56 @@
     "RelevanceFeedbackTypeDef",
     {
         "ResultId": str,
         "RelevanceValue": RelevanceTypeType,
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
 _RequiredSeedUrlConfigurationOutputTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationOutputTypeDef",
     {
         "SeedUrls": List[str],
     },
 )
 _OptionalSeedUrlConfigurationOutputTypeDef = TypedDict(
     "_OptionalSeedUrlConfigurationOutputTypeDef",
     {
         "WebCrawlerMode": WebCrawlerModeType,
     },
     total=False,
 )
 
+
 class SeedUrlConfigurationOutputTypeDef(
     _RequiredSeedUrlConfigurationOutputTypeDef, _OptionalSeedUrlConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredSeedUrlConfigurationTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationTypeDef",
     {
         "SeedUrls": Sequence[str],
     },
 )
 _OptionalSeedUrlConfigurationTypeDef = TypedDict(
     "_OptionalSeedUrlConfigurationTypeDef",
     {
         "WebCrawlerMode": WebCrawlerModeType,
     },
     total=False,
 )
 
+
 class SeedUrlConfigurationTypeDef(
     _RequiredSeedUrlConfigurationTypeDef, _OptionalSeedUrlConfigurationTypeDef
 ):
     pass
 
+
 SiteMapsConfigurationOutputTypeDef = TypedDict(
     "SiteMapsConfigurationOutputTypeDef",
     {
         "SiteMaps": List[str],
     },
 )
 
@@ -2090,22 +1766,14 @@
     "StartDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
 
-StartDataSourceSyncJobResponseTypeDef = TypedDict(
-    "StartDataSourceSyncJobResponseTypeDef",
-    {
-        "ExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StopDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -2134,139 +1802,270 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListAccessControlConfigurationsResponseTypeDef = TypedDict(
-    "ListAccessControlConfigurationsResponseTypeDef",
-    {
-        "NextToken": str,
-        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredColumnConfigurationOutputTypeDef = TypedDict(
     "_RequiredColumnConfigurationOutputTypeDef",
     {
         "DocumentIdColumnName": str,
         "DocumentDataColumnName": str,
         "ChangeDetectingColumns": List[str],
     },
 )
 _OptionalColumnConfigurationOutputTypeDef = TypedDict(
     "_OptionalColumnConfigurationOutputTypeDef",
     {
         "DocumentTitleColumnName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class ColumnConfigurationOutputTypeDef(
     _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
 ):
     pass
 
+
+_RequiredColumnConfigurationTypeDef = TypedDict(
+    "_RequiredColumnConfigurationTypeDef",
+    {
+        "DocumentIdColumnName": str,
+        "DocumentDataColumnName": str,
+        "ChangeDetectingColumns": Sequence[str],
+    },
+)
+_OptionalColumnConfigurationTypeDef = TypedDict(
+    "_OptionalColumnConfigurationTypeDef",
+    {
+        "DocumentTitleColumnName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+
+class ColumnConfigurationTypeDef(
+    _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
+):
+    pass
+
+
 _RequiredGoogleDriveConfigurationOutputTypeDef = TypedDict(
     "_RequiredGoogleDriveConfigurationOutputTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGoogleDriveConfigurationOutputTypeDef = TypedDict(
     "_OptionalGoogleDriveConfigurationOutputTypeDef",
     {
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "ExcludeMimeTypes": List[str],
         "ExcludeUserAccounts": List[str],
         "ExcludeSharedDrives": List[str],
     },
     total=False,
 )
 
+
 class GoogleDriveConfigurationOutputTypeDef(
     _RequiredGoogleDriveConfigurationOutputTypeDef, _OptionalGoogleDriveConfigurationOutputTypeDef
 ):
     pass
 
+
+_RequiredGoogleDriveConfigurationTypeDef = TypedDict(
+    "_RequiredGoogleDriveConfigurationTypeDef",
+    {
+        "SecretArn": str,
+    },
+)
+_OptionalGoogleDriveConfigurationTypeDef = TypedDict(
+    "_OptionalGoogleDriveConfigurationTypeDef",
+    {
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "ExcludeMimeTypes": Sequence[str],
+        "ExcludeUserAccounts": Sequence[str],
+        "ExcludeSharedDrives": Sequence[str],
+    },
+    total=False,
+)
+
+
+class GoogleDriveConfigurationTypeDef(
+    _RequiredGoogleDriveConfigurationTypeDef, _OptionalGoogleDriveConfigurationTypeDef
+):
+    pass
+
+
 _RequiredSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceChatterFeedConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceChatterFeedConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "IncludeFilterTypes": List[SalesforceChatterFeedIncludeFilterTypeType],
     },
     total=False,
 )
 
+
 class SalesforceChatterFeedConfigurationOutputTypeDef(
     _RequiredSalesforceChatterFeedConfigurationOutputTypeDef,
     _OptionalSalesforceChatterFeedConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredSalesforceChatterFeedConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceChatterFeedConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceChatterFeedConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceChatterFeedConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "IncludeFilterTypes": Sequence[SalesforceChatterFeedIncludeFilterTypeType],
+    },
+    total=False,
+)
+
+
+class SalesforceChatterFeedConfigurationTypeDef(
+    _RequiredSalesforceChatterFeedConfigurationTypeDef,
+    _OptionalSalesforceChatterFeedConfigurationTypeDef,
+):
+    pass
+
+
 _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "Name": str,
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef(
     _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
     _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "Name": str,
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+
+class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(
+    _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
+    _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
+):
+    pass
+
+
 _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef(
     _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
     _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+
+class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(
+    _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
+    _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
+):
+    pass
+
+
 SalesforceStandardObjectAttachmentConfigurationOutputTypeDef = TypedDict(
     "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+SalesforceStandardObjectAttachmentConfigurationTypeDef = TypedDict(
+    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 _RequiredSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceStandardObjectConfigurationOutputTypeDef",
     {
@@ -2274,151 +2073,265 @@
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
     "_OptionalSalesforceStandardObjectConfigurationOutputTypeDef",
     {
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class SalesforceStandardObjectConfigurationOutputTypeDef(
     _RequiredSalesforceStandardObjectConfigurationOutputTypeDef,
     _OptionalSalesforceStandardObjectConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredSalesforceStandardObjectConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceStandardObjectConfigurationTypeDef",
+    {
+        "Name": SalesforceStandardObjectNameType,
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalSalesforceStandardObjectConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceStandardObjectConfigurationTypeDef",
+    {
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+
+class SalesforceStandardObjectConfigurationTypeDef(
+    _RequiredSalesforceStandardObjectConfigurationTypeDef,
+    _OptionalSalesforceStandardObjectConfigurationTypeDef,
+):
+    pass
+
+
 _RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
     "_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "IncludeAttachmentFilePatterns": List[str],
         "ExcludeAttachmentFilePatterns": List[str],
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "FilterQuery": str,
     },
     total=False,
 )
 
+
 class ServiceNowKnowledgeArticleConfigurationOutputTypeDef(
     _RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef,
     _OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_RequiredServiceNowKnowledgeArticleConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_OptionalServiceNowKnowledgeArticleConfigurationTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "IncludeAttachmentFilePatterns": Sequence[str],
+        "ExcludeAttachmentFilePatterns": Sequence[str],
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "FilterQuery": str,
+    },
+    total=False,
+)
+
+
+class ServiceNowKnowledgeArticleConfigurationTypeDef(
+    _RequiredServiceNowKnowledgeArticleConfigurationTypeDef,
+    _OptionalServiceNowKnowledgeArticleConfigurationTypeDef,
+):
+    pass
+
+
 _RequiredServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
     "_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "IncludeAttachmentFilePatterns": List[str],
         "ExcludeAttachmentFilePatterns": List[str],
         "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class ServiceNowServiceCatalogConfigurationOutputTypeDef(
     _RequiredServiceNowServiceCatalogConfigurationOutputTypeDef,
     _OptionalServiceNowServiceCatalogConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
+    "_RequiredServiceNowServiceCatalogConfigurationTypeDef",
+    {
+        "DocumentDataFieldName": str,
+    },
+)
+_OptionalServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
+    "_OptionalServiceNowServiceCatalogConfigurationTypeDef",
+    {
+        "CrawlAttachments": bool,
+        "IncludeAttachmentFilePatterns": Sequence[str],
+        "ExcludeAttachmentFilePatterns": Sequence[str],
+        "DocumentTitleFieldName": str,
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+
+class ServiceNowServiceCatalogConfigurationTypeDef(
+    _RequiredServiceNowServiceCatalogConfigurationTypeDef,
+    _OptionalServiceNowServiceCatalogConfigurationTypeDef,
+):
+    pass
+
+
 _RequiredWorkDocsConfigurationOutputTypeDef = TypedDict(
     "_RequiredWorkDocsConfigurationOutputTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalWorkDocsConfigurationOutputTypeDef = TypedDict(
     "_OptionalWorkDocsConfigurationOutputTypeDef",
     {
         "CrawlComments": bool,
         "UseChangeLog": bool,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class WorkDocsConfigurationOutputTypeDef(
     _RequiredWorkDocsConfigurationOutputTypeDef, _OptionalWorkDocsConfigurationOutputTypeDef
 ):
     pass
 
+
+_RequiredWorkDocsConfigurationTypeDef = TypedDict(
+    "_RequiredWorkDocsConfigurationTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalWorkDocsConfigurationTypeDef = TypedDict(
+    "_OptionalWorkDocsConfigurationTypeDef",
+    {
+        "CrawlComments": bool,
+        "UseChangeLog": bool,
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+    },
+    total=False,
+)
+
+
+class WorkDocsConfigurationTypeDef(
+    _RequiredWorkDocsConfigurationTypeDef, _OptionalWorkDocsConfigurationTypeDef
+):
+    pass
+
+
 _RequiredBoxConfigurationOutputTypeDef = TypedDict(
     "_RequiredBoxConfigurationOutputTypeDef",
     {
         "EnterpriseId": str,
         "SecretArn": str,
     },
 )
 _OptionalBoxConfigurationOutputTypeDef = TypedDict(
     "_OptionalBoxConfigurationOutputTypeDef",
     {
         "UseChangeLog": bool,
         "CrawlComments": bool,
         "CrawlTasks": bool,
         "CrawlWebLinks": bool,
-        "FileFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "TaskFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "WebLinkFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FileFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "TaskFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "WebLinkFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class BoxConfigurationOutputTypeDef(
     _RequiredBoxConfigurationOutputTypeDef, _OptionalBoxConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredFsxConfigurationOutputTypeDef = TypedDict(
     "_RequiredFsxConfigurationOutputTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
 )
 _OptionalFsxConfigurationOutputTypeDef = TypedDict(
     "_OptionalFsxConfigurationOutputTypeDef",
     {
         "SecretArn": str,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class FsxConfigurationOutputTypeDef(
     _RequiredFsxConfigurationOutputTypeDef, _OptionalFsxConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredJiraConfigurationOutputTypeDef = TypedDict(
     "_RequiredJiraConfigurationOutputTypeDef",
     {
         "JiraAccountUrl": str,
         "SecretArn": str,
     },
 )
@@ -2426,60 +2339,64 @@
     "_OptionalJiraConfigurationOutputTypeDef",
     {
         "UseChangeLog": bool,
         "Project": List[str],
         "IssueType": List[str],
         "Status": List[str],
         "IssueSubEntityFilter": List[IssueSubEntityType],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "IssueFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "ProjectFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "WorkLogFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "IssueFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "ProjectFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "WorkLogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class JiraConfigurationOutputTypeDef(
     _RequiredJiraConfigurationOutputTypeDef, _OptionalJiraConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredQuipConfigurationOutputTypeDef = TypedDict(
     "_RequiredQuipConfigurationOutputTypeDef",
     {
         "Domain": str,
         "SecretArn": str,
     },
 )
 _OptionalQuipConfigurationOutputTypeDef = TypedDict(
     "_OptionalQuipConfigurationOutputTypeDef",
     {
         "CrawlFileComments": bool,
         "CrawlChatRooms": bool,
         "CrawlAttachments": bool,
         "FolderIds": List[str],
-        "ThreadFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "MessageFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "ThreadFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "MessageFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class QuipConfigurationOutputTypeDef(
     _RequiredQuipConfigurationOutputTypeDef, _OptionalQuipConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredSlackConfigurationOutputTypeDef = TypedDict(
     "_RequiredSlackConfigurationOutputTypeDef",
     {
         "TeamId": str,
         "SecretArn": str,
         "SlackEntityList": List[SlackEntityType],
         "SinceCrawlDate": str,
@@ -2493,344 +2410,168 @@
         "CrawlBotMessage": bool,
         "ExcludeArchived": bool,
         "LookBackPeriod": int,
         "PrivateChannelFilter": List[str],
         "PublicChannelFilter": List[str],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class SlackConfigurationOutputTypeDef(
     _RequiredSlackConfigurationOutputTypeDef, _OptionalSlackConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredAlfrescoConfigurationOutputTypeDef = TypedDict(
     "_RequiredAlfrescoConfigurationOutputTypeDef",
     {
         "SiteUrl": str,
         "SiteId": str,
         "SecretArn": str,
-        "SslCertificateS3Path": S3PathOutputTypeDef,
+        "SslCertificateS3Path": S3PathTypeDef,
     },
 )
 _OptionalAlfrescoConfigurationOutputTypeDef = TypedDict(
     "_OptionalAlfrescoConfigurationOutputTypeDef",
     {
         "CrawlSystemFolders": bool,
         "CrawlComments": bool,
         "EntityFilter": List[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "BlogFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "WikiFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "DocumentLibraryFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "BlogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "WikiFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class AlfrescoConfigurationOutputTypeDef(
     _RequiredAlfrescoConfigurationOutputTypeDef, _OptionalAlfrescoConfigurationOutputTypeDef
 ):
     pass
 
-DescribeFaqResponseTypeDef = TypedDict(
-    "DescribeFaqResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "S3Path": S3PathOutputTypeDef,
-        "Status": FaqStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "FileFormat": FaqFileFormatType,
-        "LanguageCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "Status": QuerySuggestionsBlockListStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "SourceS3Path": S3PathOutputTypeDef,
-        "ItemCount": int,
-        "FileSizeBytes": int,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeThesaurusResponseTypeDef = TypedDict(
-    "DescribeThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "Status": ThesaurusStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "RoleArn": str,
-        "SourceS3Path": S3PathOutputTypeDef,
-        "FileSizeBytes": int,
-        "TermCount": int,
-        "SynonymRuleCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OnPremiseConfigurationOutputTypeDef = TypedDict(
-    "OnPremiseConfigurationOutputTypeDef",
+OnPremiseConfigurationTypeDef = TypedDict(
+    "OnPremiseConfigurationTypeDef",
     {
         "HostUrl": str,
         "OrganizationName": str,
-        "SslCertificateS3Path": S3PathOutputTypeDef,
+        "SslCertificateS3Path": S3PathTypeDef,
     },
 )
 
 OneDriveUsersOutputTypeDef = TypedDict(
     "OneDriveUsersOutputTypeDef",
     {
         "OneDriveUserList": List[str],
-        "OneDriveUserS3Path": S3PathOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredColumnConfigurationTypeDef = TypedDict(
-    "_RequiredColumnConfigurationTypeDef",
-    {
-        "DocumentIdColumnName": str,
-        "DocumentDataColumnName": str,
-        "ChangeDetectingColumns": Sequence[str],
-    },
-)
-_OptionalColumnConfigurationTypeDef = TypedDict(
-    "_OptionalColumnConfigurationTypeDef",
-    {
-        "DocumentTitleColumnName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "OneDriveUserS3Path": S3PathTypeDef,
     },
     total=False,
 )
 
-class ColumnConfigurationTypeDef(
-    _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
-):
-    pass
-
-_RequiredGoogleDriveConfigurationTypeDef = TypedDict(
-    "_RequiredGoogleDriveConfigurationTypeDef",
-    {
-        "SecretArn": str,
-    },
-)
-_OptionalGoogleDriveConfigurationTypeDef = TypedDict(
-    "_OptionalGoogleDriveConfigurationTypeDef",
+OneDriveUsersTypeDef = TypedDict(
+    "OneDriveUsersTypeDef",
     {
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "ExcludeMimeTypes": Sequence[str],
-        "ExcludeUserAccounts": Sequence[str],
-        "ExcludeSharedDrives": Sequence[str],
+        "OneDriveUserList": Sequence[str],
+        "OneDriveUserS3Path": S3PathTypeDef,
     },
     total=False,
 )
 
-class GoogleDriveConfigurationTypeDef(
-    _RequiredGoogleDriveConfigurationTypeDef, _OptionalGoogleDriveConfigurationTypeDef
-):
-    pass
-
-_RequiredSalesforceChatterFeedConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceChatterFeedConfigurationTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceChatterFeedConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceChatterFeedConfigurationTypeDef",
+_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "IncludeFilterTypes": Sequence[SalesforceChatterFeedIncludeFilterTypeType],
+        "IndexId": str,
+        "Id": str,
     },
-    total=False,
 )
-
-class SalesforceChatterFeedConfigurationTypeDef(
-    _RequiredSalesforceChatterFeedConfigurationTypeDef,
-    _OptionalSalesforceChatterFeedConfigurationTypeDef,
-):
-    pass
-
-_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
+_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "Name": str,
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "Description": str,
+        "SourceS3Path": S3PathTypeDef,
+        "RoleArn": str,
     },
     total=False,
 )
 
-class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(
-    _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
-    _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
-):
-    pass
 
-_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(
-    _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
-    _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
+class UpdateQuerySuggestionsBlockListRequestRequestTypeDef(
+    _RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
+    _OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
 ):
     pass
 
-SalesforceStandardObjectAttachmentConfigurationTypeDef = TypedDict(
-    "SalesforceStandardObjectAttachmentConfigurationTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
 
-_RequiredSalesforceStandardObjectConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceStandardObjectConfigurationTypeDef",
+_RequiredUpdateThesaurusRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThesaurusRequestRequestTypeDef",
     {
-        "Name": SalesforceStandardObjectNameType,
-        "DocumentDataFieldName": str,
+        "Id": str,
+        "IndexId": str,
     },
 )
-_OptionalSalesforceStandardObjectConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceStandardObjectConfigurationTypeDef",
+_OptionalUpdateThesaurusRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThesaurusRequestRequestTypeDef",
     {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "Name": str,
+        "Description": str,
+        "RoleArn": str,
+        "SourceS3Path": S3PathTypeDef,
     },
     total=False,
 )
 
-class SalesforceStandardObjectConfigurationTypeDef(
-    _RequiredSalesforceStandardObjectConfigurationTypeDef,
-    _OptionalSalesforceStandardObjectConfigurationTypeDef,
-):
-    pass
 
-_RequiredServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_RequiredServiceNowKnowledgeArticleConfigurationTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_OptionalServiceNowKnowledgeArticleConfigurationTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": Sequence[str],
-        "ExcludeAttachmentFilePatterns": Sequence[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "FilterQuery": str,
-    },
-    total=False,
-)
-
-class ServiceNowKnowledgeArticleConfigurationTypeDef(
-    _RequiredServiceNowKnowledgeArticleConfigurationTypeDef,
-    _OptionalServiceNowKnowledgeArticleConfigurationTypeDef,
+class UpdateThesaurusRequestRequestTypeDef(
+    _RequiredUpdateThesaurusRequestRequestTypeDef, _OptionalUpdateThesaurusRequestRequestTypeDef
 ):
     pass
 
-_RequiredServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
-    "_RequiredServiceNowServiceCatalogConfigurationTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
-    "_OptionalServiceNowServiceCatalogConfigurationTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": Sequence[str],
-        "ExcludeAttachmentFilePatterns": Sequence[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
 
-class ServiceNowServiceCatalogConfigurationTypeDef(
-    _RequiredServiceNowServiceCatalogConfigurationTypeDef,
-    _OptionalServiceNowServiceCatalogConfigurationTypeDef,
-):
-    pass
-
-_RequiredWorkDocsConfigurationTypeDef = TypedDict(
-    "_RequiredWorkDocsConfigurationTypeDef",
+_RequiredAlfrescoConfigurationTypeDef = TypedDict(
+    "_RequiredAlfrescoConfigurationTypeDef",
     {
-        "OrganizationId": str,
+        "SiteUrl": str,
+        "SiteId": str,
+        "SecretArn": str,
+        "SslCertificateS3Path": S3PathTypeDef,
     },
 )
-_OptionalWorkDocsConfigurationTypeDef = TypedDict(
-    "_OptionalWorkDocsConfigurationTypeDef",
+_OptionalAlfrescoConfigurationTypeDef = TypedDict(
+    "_OptionalAlfrescoConfigurationTypeDef",
     {
+        "CrawlSystemFolders": bool,
         "CrawlComments": bool,
-        "UseChangeLog": bool,
+        "EntityFilter": Sequence[AlfrescoEntityType],
+        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-class WorkDocsConfigurationTypeDef(
-    _RequiredWorkDocsConfigurationTypeDef, _OptionalWorkDocsConfigurationTypeDef
+
+class AlfrescoConfigurationTypeDef(
+    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
 ):
     pass
 
+
 _RequiredBoxConfigurationTypeDef = TypedDict(
     "_RequiredBoxConfigurationTypeDef",
     {
         "EnterpriseId": str,
         "SecretArn": str,
     },
 )
@@ -2848,17 +2589,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
     pass
 
+
 _RequiredFsxConfigurationTypeDef = TypedDict(
     "_RequiredFsxConfigurationTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
@@ -2870,17 +2613,19 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class FsxConfigurationTypeDef(_RequiredFsxConfigurationTypeDef, _OptionalFsxConfigurationTypeDef):
     pass
 
+
 _RequiredJiraConfigurationTypeDef = TypedDict(
     "_RequiredJiraConfigurationTypeDef",
     {
         "JiraAccountUrl": str,
         "SecretArn": str,
     },
 )
@@ -2900,19 +2645,21 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class JiraConfigurationTypeDef(
     _RequiredJiraConfigurationTypeDef, _OptionalJiraConfigurationTypeDef
 ):
     pass
 
+
 _RequiredQuipConfigurationTypeDef = TypedDict(
     "_RequiredQuipConfigurationTypeDef",
     {
         "Domain": str,
         "SecretArn": str,
     },
 )
@@ -2929,19 +2676,21 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class QuipConfigurationTypeDef(
     _RequiredQuipConfigurationTypeDef, _OptionalQuipConfigurationTypeDef
 ):
     pass
 
+
 _RequiredSlackConfigurationTypeDef = TypedDict(
     "_RequiredSlackConfigurationTypeDef",
     {
         "TeamId": str,
         "SecretArn": str,
         "SlackEntityList": Sequence[SlackEntityType],
         "SinceCrawlDate": str,
@@ -2960,161 +2709,206 @@
         "InclusionPatterns": Sequence[str],
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
+
 class SlackConfigurationTypeDef(
     _RequiredSlackConfigurationTypeDef, _OptionalSlackConfigurationTypeDef
 ):
     pass
 
-_RequiredAlfrescoConfigurationTypeDef = TypedDict(
-    "_RequiredAlfrescoConfigurationTypeDef",
+
+AssociateEntitiesToExperienceRequestRequestTypeDef = TypedDict(
+    "AssociateEntitiesToExperienceRequestRequestTypeDef",
     {
-        "SiteUrl": str,
-        "SiteId": str,
-        "SecretArn": str,
-        "SslCertificateS3Path": S3PathTypeDef,
+        "Id": str,
+        "IndexId": str,
+        "EntityList": Sequence[EntityConfigurationTypeDef],
     },
 )
-_OptionalAlfrescoConfigurationTypeDef = TypedDict(
-    "_OptionalAlfrescoConfigurationTypeDef",
+
+DisassociateEntitiesFromExperienceRequestRequestTypeDef = TypedDict(
+    "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     {
-        "CrawlSystemFolders": bool,
-        "CrawlComments": bool,
-        "EntityFilter": Sequence[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
+        "Id": str,
+        "IndexId": str,
+        "EntityList": Sequence[EntityConfigurationTypeDef],
     },
-    total=False,
 )
 
-class AlfrescoConfigurationTypeDef(
-    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
-):
-    pass
-
-OnPremiseConfigurationTypeDef = TypedDict(
-    "OnPremiseConfigurationTypeDef",
+AssociateEntitiesToExperienceResponseTypeDef = TypedDict(
+    "AssociateEntitiesToExperienceResponseTypeDef",
     {
-        "HostUrl": str,
-        "OrganizationName": str,
-        "SslCertificateS3Path": S3PathTypeDef,
+        "FailedEntityList": List[FailedEntityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OneDriveUsersTypeDef = TypedDict(
-    "OneDriveUsersTypeDef",
+AssociatePersonasToEntitiesResponseTypeDef = TypedDict(
+    "AssociatePersonasToEntitiesResponseTypeDef",
     {
-        "OneDriveUserList": Sequence[str],
-        "OneDriveUserS3Path": S3PathTypeDef,
+        "FailedEntityList": List[FailedEntityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+CreateAccessControlConfigurationResponseTypeDef = TypedDict(
+    "CreateAccessControlConfigurationResponseTypeDef",
     {
-        "IndexId": str,
         "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+
+CreateDataSourceResponseTypeDef = TypedDict(
+    "CreateDataSourceResponseTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "SourceS3Path": S3PathTypeDef,
-        "RoleArn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateQuerySuggestionsBlockListRequestRequestTypeDef(
-    _RequiredUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
-    _OptionalUpdateQuerySuggestionsBlockListRequestRequestTypeDef,
-):
-    pass
+CreateExperienceResponseTypeDef = TypedDict(
+    "CreateExperienceResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateThesaurusRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThesaurusRequestRequestTypeDef",
+CreateFaqResponseTypeDef = TypedDict(
+    "CreateFaqResponseTypeDef",
     {
         "Id": str,
-        "IndexId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateThesaurusRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThesaurusRequestRequestTypeDef",
+
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "RoleArn": str,
-        "SourceS3Path": S3PathTypeDef,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateThesaurusRequestRequestTypeDef(
-    _RequiredUpdateThesaurusRequestRequestTypeDef, _OptionalUpdateThesaurusRequestRequestTypeDef
-):
-    pass
+CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-AssociateEntitiesToExperienceRequestRequestTypeDef = TypedDict(
-    "AssociateEntitiesToExperienceRequestRequestTypeDef",
+CreateThesaurusResponseTypeDef = TypedDict(
+    "CreateThesaurusResponseTypeDef",
     {
         "Id": str,
-        "IndexId": str,
-        "EntityList": Sequence[EntityConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociateEntitiesFromExperienceRequestRequestTypeDef = TypedDict(
-    "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
+DescribeFaqResponseTypeDef = TypedDict(
+    "DescribeFaqResponseTypeDef",
     {
         "Id": str,
         "IndexId": str,
-        "EntityList": Sequence[EntityConfigurationTypeDef],
+        "Name": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "S3Path": S3PathTypeDef,
+        "Status": FaqStatusType,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "FileFormat": FaqFileFormatType,
+        "LanguageCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociateEntitiesToExperienceResponseTypeDef = TypedDict(
-    "AssociateEntitiesToExperienceResponseTypeDef",
+DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
     {
-        "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IndexId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "Status": QuerySuggestionsBlockListStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "SourceS3Path": S3PathTypeDef,
+        "ItemCount": int,
+        "FileSizeBytes": int,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePersonasToEntitiesResponseTypeDef = TypedDict(
-    "AssociatePersonasToEntitiesResponseTypeDef",
+DescribeThesaurusResponseTypeDef = TypedDict(
+    "DescribeThesaurusResponseTypeDef",
     {
-        "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Description": str,
+        "Status": ThesaurusStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "RoleArn": str,
+        "SourceS3Path": S3PathTypeDef,
+        "FileSizeBytes": int,
+        "TermCount": int,
+        "SynonymRuleCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateEntitiesFromExperienceResponseTypeDef = TypedDict(
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociatePersonasFromEntitiesResponseTypeDef = TypedDict(
     "DisassociatePersonasFromEntitiesResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+ListAccessControlConfigurationsResponseTypeDef = TypedDict(
+    "ListAccessControlConfigurationsResponseTypeDef",
+    {
+        "NextToken": str,
+        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataSourceSyncJobResponseTypeDef = TypedDict(
+    "StartDataSourceSyncJobResponseTypeDef",
+    {
+        "ExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociatePersonasToEntitiesRequestRequestTypeDef = TypedDict(
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
     {
         "Id": str,
@@ -3122,15 +2916,15 @@
         "Personas": Sequence[EntityPersonaConfigurationTypeDef],
     },
 )
 
 AttributeSuggestionsDescribeConfigTypeDef = TypedDict(
     "AttributeSuggestionsDescribeConfigTypeDef",
     {
-        "SuggestableConfigList": List[SuggestableConfigOutputTypeDef],
+        "SuggestableConfigList": List[SuggestableConfigTypeDef],
         "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
     total=False,
 )
 
 AttributeSuggestionsUpdateConfigTypeDef = TypedDict(
     "AttributeSuggestionsUpdateConfigTypeDef",
@@ -3140,15 +2934,15 @@
     },
     total=False,
 )
 
 AuthenticationConfigurationOutputTypeDef = TypedDict(
     "AuthenticationConfigurationOutputTypeDef",
     {
-        "BasicAuthentication": List[BasicAuthenticationConfigurationOutputTypeDef],
+        "BasicAuthentication": List[BasicAuthenticationConfigurationTypeDef],
     },
     total=False,
 )
 
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
@@ -3168,58 +2962,60 @@
     "_OptionalBatchDeleteDocumentRequestRequestTypeDef",
     {
         "DataSourceSyncJobMetricTarget": DataSourceSyncJobMetricTargetTypeDef,
     },
     total=False,
 )
 
+
 class BatchDeleteDocumentRequestRequestTypeDef(
     _RequiredBatchDeleteDocumentRequestRequestTypeDef,
     _OptionalBatchDeleteDocumentRequestRequestTypeDef,
 ):
     pass
 
+
 BatchDeleteDocumentResponseTypeDef = TypedDict(
     "BatchDeleteDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchDeleteDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteFeaturedResultsSetResponseTypeDef = TypedDict(
     "BatchDeleteFeaturedResultsSetResponseTypeDef",
     {
         "Errors": List[BatchDeleteFeaturedResultsSetErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDocumentStatusResponseTypeDef = TypedDict(
     "BatchGetDocumentStatusResponseTypeDef",
     {
         "Errors": List[BatchGetDocumentStatusResponseErrorTypeDef],
         "DocumentStatusList": List[StatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutDocumentResponseTypeDef = TypedDict(
     "BatchPutDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchPutDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfluenceAttachmentConfigurationOutputTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
-        "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingOutputTypeDef],
+        "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluenceAttachmentConfigurationTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationTypeDef",
     {
@@ -3228,15 +3024,15 @@
     },
     total=False,
 )
 
 ConfluenceBlogConfigurationOutputTypeDef = TypedDict(
     "ConfluenceBlogConfigurationOutputTypeDef",
     {
-        "BlogFieldMappings": List[ConfluenceBlogToIndexFieldMappingOutputTypeDef],
+        "BlogFieldMappings": List[ConfluenceBlogToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluenceBlogConfigurationTypeDef = TypedDict(
     "ConfluenceBlogConfigurationTypeDef",
     {
@@ -3257,29 +3053,31 @@
     "_OptionalSharePointConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "UseChangeLog": bool,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "DocumentTitleFieldName": str,
         "DisableLocalGroups": bool,
-        "SslCertificateS3Path": S3PathOutputTypeDef,
+        "SslCertificateS3Path": S3PathTypeDef,
         "AuthenticationType": SharePointOnlineAuthenticationTypeType,
-        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "ProxyConfiguration": ProxyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SharePointConfigurationOutputTypeDef(
     _RequiredSharePointConfigurationOutputTypeDef, _OptionalSharePointConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredSharePointConfigurationTypeDef = TypedDict(
     "_RequiredSharePointConfigurationTypeDef",
     {
         "SharePointVersion": SharePointVersionType,
         "Urls": Sequence[str],
         "SecretArn": str,
     },
@@ -3298,23 +3096,25 @@
         "SslCertificateS3Path": S3PathTypeDef,
         "AuthenticationType": SharePointOnlineAuthenticationTypeType,
         "ProxyConfiguration": ProxyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SharePointConfigurationTypeDef(
     _RequiredSharePointConfigurationTypeDef, _OptionalSharePointConfigurationTypeDef
 ):
     pass
 
+
 ConfluencePageConfigurationOutputTypeDef = TypedDict(
     "ConfluencePageConfigurationOutputTypeDef",
     {
-        "PageFieldMappings": List[ConfluencePageToIndexFieldMappingOutputTypeDef],
+        "PageFieldMappings": List[ConfluencePageToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluencePageConfigurationTypeDef = TypedDict(
     "ConfluencePageConfigurationTypeDef",
     {
@@ -3326,15 +3126,15 @@
 ConfluenceSpaceConfigurationOutputTypeDef = TypedDict(
     "ConfluenceSpaceConfigurationOutputTypeDef",
     {
         "CrawlPersonalSpaces": bool,
         "CrawlArchivedSpaces": bool,
         "IncludeSpaces": List[str],
         "ExcludeSpaces": List[str],
-        "SpaceFieldMappings": List[ConfluenceSpaceToIndexFieldMappingOutputTypeDef],
+        "SpaceFieldMappings": List[ConfluenceSpaceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 ConfluenceSpaceConfigurationTypeDef = TypedDict(
     "ConfluenceSpaceConfigurationTypeDef",
     {
@@ -3352,14 +3152,21 @@
     {
         "SuggestedQueryText": str,
         "Corrections": List[CorrectionTypeDef],
     },
     total=False,
 )
 
+HierarchicalPrincipalOutputTypeDef = TypedDict(
+    "HierarchicalPrincipalOutputTypeDef",
+    {
+        "PrincipalList": List[PrincipalTypeDef],
+    },
+)
+
 HierarchicalPrincipalTypeDef = TypedDict(
     "HierarchicalPrincipalTypeDef",
     {
         "PrincipalList": Sequence[PrincipalTypeDef],
     },
 )
 
@@ -3380,19 +3187,21 @@
         "FileFormat": FaqFileFormatType,
         "ClientToken": str,
         "LanguageCode": str,
     },
     total=False,
 )
 
+
 class CreateFaqRequestRequestTypeDef(
     _RequiredCreateFaqRequestRequestTypeDef, _OptionalCreateFaqRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
         "SourceS3Path": S3PathTypeDef,
         "RoleArn": str,
@@ -3404,20 +3213,22 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateQuerySuggestionsBlockListRequestRequestTypeDef(
     _RequiredCreateQuerySuggestionsBlockListRequestRequestTypeDef,
     _OptionalCreateQuerySuggestionsBlockListRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateThesaurusRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThesaurusRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
         "RoleArn": str,
         "SourceS3Path": S3PathTypeDef,
@@ -3429,19 +3240,29 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateThesaurusRequestRequestTypeDef(
     _RequiredCreateThesaurusRequestRequestTypeDef, _OptionalCreateThesaurusRequestRequestTypeDef
 ):
     pass
 
+
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
@@ -3462,20 +3283,37 @@
         "QueryTexts": Sequence[str],
         "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFeaturedResultsSetRequestRequestTypeDef(
     _RequiredCreateFeaturedResultsSetRequestRequestTypeDef,
     _OptionalCreateFeaturedResultsSetRequestRequestTypeDef,
 ):
     pass
 
+
+FeaturedResultsSetTypeDef = TypedDict(
+    "FeaturedResultsSetTypeDef",
+    {
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": List[str],
+        "FeaturedDocuments": List[FeaturedDocumentTypeDef],
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
+    },
+    total=False,
+)
+
 _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFeaturedResultsSetRequestRequestTypeDef",
     {
         "IndexId": str,
         "FeaturedResultsSetId": str,
     },
 )
@@ -3487,20 +3325,22 @@
         "Status": FeaturedResultsSetStatusType,
         "QueryTexts": Sequence[str],
         "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
     },
     total=False,
 )
 
+
 class UpdateFeaturedResultsSetRequestRequestTypeDef(
     _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef,
     _OptionalUpdateFeaturedResultsSetRequestRequestTypeDef,
 ):
     pass
 
+
 UserContextTypeDef = TypedDict(
     "UserContextTypeDef",
     {
         "Token": str,
         "UserId": str,
         "Groups": Sequence[str],
         "DataSourceGroups": Sequence[DataSourceGroupTypeDef],
@@ -3509,15 +3349,15 @@
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "SummaryItems": List[DataSourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataSourceSyncJobTypeDef = TypedDict(
     "DataSourceSyncJobTypeDef",
     {
         "ExecutionId": str,
@@ -3528,21 +3368,14 @@
         "ErrorCode": ErrorCodeType,
         "DataSourceErrorCode": str,
         "Metrics": DataSourceSyncJobMetricsTypeDef,
     },
     total=False,
 )
 
-HierarchicalPrincipalOutputTypeDef = TypedDict(
-    "HierarchicalPrincipalOutputTypeDef",
-    {
-        "PrincipalList": List[PrincipalOutputTypeDef],
-    },
-)
-
 ExperiencesSummaryTypeDef = TypedDict(
     "ExperiencesSummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "CreatedAt": datetime,
         "Status": ExperienceStatusType,
@@ -3559,26 +3392,26 @@
         "Description": str,
         "Status": FeaturedResultsSetStatusType,
         "QueryTexts": List[str],
         "FeaturedDocumentsWithMetadata": List[FeaturedDocumentWithMetadataTypeDef],
         "FeaturedDocumentsMissing": List[FeaturedDocumentMissingTypeDef],
         "LastUpdatedTimestamp": int,
         "CreationTimestamp": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePrincipalMappingResponseTypeDef = TypedDict(
     "DescribePrincipalMappingResponseTypeDef",
     {
         "IndexId": str,
         "DataSourceId": str,
         "GroupId": str,
         "GroupOrderingIdSummaries": List[GroupOrderingIdSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDocumentAttributeConditionOutputTypeDef = TypedDict(
     "_RequiredDocumentAttributeConditionOutputTypeDef",
     {
         "ConditionDocumentAttributeKey": str,
@@ -3589,20 +3422,22 @@
     "_OptionalDocumentAttributeConditionOutputTypeDef",
     {
         "ConditionOnValue": DocumentAttributeValueOutputTypeDef,
     },
     total=False,
 )
 
+
 class DocumentAttributeConditionOutputTypeDef(
     _RequiredDocumentAttributeConditionOutputTypeDef,
     _OptionalDocumentAttributeConditionOutputTypeDef,
 ):
     pass
 
+
 DocumentAttributeOutputTypeDef = TypedDict(
     "DocumentAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": DocumentAttributeValueOutputTypeDef,
     },
 )
@@ -3638,19 +3473,21 @@
     "_OptionalDocumentAttributeConditionTypeDef",
     {
         "ConditionOnValue": DocumentAttributeValueTypeDef,
     },
     total=False,
 )
 
+
 class DocumentAttributeConditionTypeDef(
     _RequiredDocumentAttributeConditionTypeDef, _OptionalDocumentAttributeConditionTypeDef
 ):
     pass
 
+
 DocumentAttributeTargetTypeDef = TypedDict(
     "DocumentAttributeTargetTypeDef",
     {
         "TargetDocumentAttributeKey": str,
         "TargetDocumentAttributeValueDeletion": bool,
         "TargetDocumentAttributeValue": DocumentAttributeValueTypeDef,
     },
@@ -3672,32 +3509,26 @@
         "Type": DocumentAttributeValueTypeType,
     },
 )
 _OptionalDocumentMetadataConfigurationOutputTypeDef = TypedDict(
     "_OptionalDocumentMetadataConfigurationOutputTypeDef",
     {
         "Relevance": RelevanceOutputTypeDef,
-        "Search": SearchOutputTypeDef,
+        "Search": SearchTypeDef,
     },
     total=False,
 )
 
+
 class DocumentMetadataConfigurationOutputTypeDef(
     _RequiredDocumentMetadataConfigurationOutputTypeDef,
     _OptionalDocumentMetadataConfigurationOutputTypeDef,
 ):
     pass
 
-DocumentRelevanceConfigurationTypeDef = TypedDict(
-    "DocumentRelevanceConfigurationTypeDef",
-    {
-        "Name": str,
-        "Relevance": RelevanceTypeDef,
-    },
-)
 
 _RequiredDocumentMetadataConfigurationTypeDef = TypedDict(
     "_RequiredDocumentMetadataConfigurationTypeDef",
     {
         "Name": str,
         "Type": DocumentAttributeValueTypeType,
     },
@@ -3707,42 +3538,54 @@
     {
         "Relevance": RelevanceTypeDef,
         "Search": SearchTypeDef,
     },
     total=False,
 )
 
+
 class DocumentMetadataConfigurationTypeDef(
     _RequiredDocumentMetadataConfigurationTypeDef, _OptionalDocumentMetadataConfigurationTypeDef
 ):
     pass
 
+
+DocumentRelevanceConfigurationTypeDef = TypedDict(
+    "DocumentRelevanceConfigurationTypeDef",
+    {
+        "Name": str,
+        "Relevance": RelevanceTypeDef,
+    },
+)
+
 _RequiredS3DataSourceConfigurationOutputTypeDef = TypedDict(
     "_RequiredS3DataSourceConfigurationOutputTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3DataSourceConfigurationOutputTypeDef = TypedDict(
     "_OptionalS3DataSourceConfigurationOutputTypeDef",
     {
         "InclusionPrefixes": List[str],
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationOutputTypeDef,
-        "AccessControlListConfiguration": AccessControlListConfigurationOutputTypeDef,
+        "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationTypeDef,
+        "AccessControlListConfiguration": AccessControlListConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class S3DataSourceConfigurationOutputTypeDef(
     _RequiredS3DataSourceConfigurationOutputTypeDef, _OptionalS3DataSourceConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredS3DataSourceConfigurationTypeDef = TypedDict(
     "_RequiredS3DataSourceConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3DataSourceConfigurationTypeDef = TypedDict(
@@ -3753,34 +3596,36 @@
         "ExclusionPatterns": Sequence[str],
         "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationTypeDef,
         "AccessControlListConfiguration": AccessControlListConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class S3DataSourceConfigurationTypeDef(
     _RequiredS3DataSourceConfigurationTypeDef, _OptionalS3DataSourceConfigurationTypeDef
 ):
     pass
 
+
 ExperienceEntitiesSummaryTypeDef = TypedDict(
     "ExperienceEntitiesSummaryTypeDef",
     {
         "EntityId": str,
         "EntityType": EntityTypeType,
         "DisplayData": EntityDisplayDataTypeDef,
     },
     total=False,
 )
 
 ExperienceConfigurationOutputTypeDef = TypedDict(
     "ExperienceConfigurationOutputTypeDef",
     {
         "ContentSourceConfiguration": ContentSourceConfigurationOutputTypeDef,
-        "UserIdentityConfiguration": UserIdentityConfigurationOutputTypeDef,
+        "UserIdentityConfiguration": UserIdentityConfigurationTypeDef,
     },
     total=False,
 )
 
 ExperienceConfigurationTypeDef = TypedDict(
     "ExperienceConfigurationTypeDef",
     {
@@ -3791,50 +3636,35 @@
 )
 
 ListFaqsResponseTypeDef = TypedDict(
     "ListFaqsResponseTypeDef",
     {
         "NextToken": str,
         "FaqSummaryItems": List[FaqSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FeaturedResultsSetTypeDef = TypedDict(
-    "FeaturedResultsSetTypeDef",
-    {
-        "FeaturedResultsSetId": str,
-        "FeaturedResultsSetName": str,
-        "Description": str,
-        "Status": FeaturedResultsSetStatusType,
-        "QueryTexts": List[str],
-        "FeaturedDocuments": List[FeaturedDocumentOutputTypeDef],
-        "LastUpdatedTimestamp": int,
-        "CreationTimestamp": int,
-    },
-    total=False,
-)
-
 ListFeaturedResultsSetsResponseTypeDef = TypedDict(
     "ListFeaturedResultsSetsResponseTypeDef",
     {
         "FeaturedResultsSetSummaryItems": List[FeaturedResultsSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotsResponseTypeDef = TypedDict(
     "GetSnapshotsResponseTypeDef",
     {
         "SnapShotTimeFilter": TimeRangeOutputTypeDef,
         "SnapshotsDataHeader": List[str],
         "SnapshotsData": List[List[str]],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupMembersTypeDef = TypedDict(
     "GroupMembersTypeDef",
     {
         "MemberGroups": Sequence[MemberGroupTypeDef],
@@ -3845,15 +3675,15 @@
 )
 
 ListGroupsOlderThanOrderingIdResponseTypeDef = TypedDict(
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     {
         "GroupsSummaries": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TextWithHighlightsTypeDef = TypedDict(
     "TextWithHighlightsTypeDef",
     {
         "Text": str,
@@ -3863,35 +3693,26 @@
 )
 
 ListIndicesResponseTypeDef = TypedDict(
     "ListIndicesResponseTypeDef",
     {
         "IndexConfigurationSummaryItems": List[IndexConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IndexStatisticsTypeDef = TypedDict(
     "IndexStatisticsTypeDef",
     {
         "FaqStatistics": FaqStatisticsTypeDef,
         "TextDocumentStatistics": TextDocumentStatisticsTypeDef,
     },
 )
 
-UserTokenConfigurationOutputTypeDef = TypedDict(
-    "UserTokenConfigurationOutputTypeDef",
-    {
-        "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationOutputTypeDef,
-        "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 UserTokenConfigurationTypeDef = TypedDict(
     "UserTokenConfigurationTypeDef",
     {
         "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationTypeDef,
         "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationTypeDef,
     },
     total=False,
@@ -3911,52 +3732,46 @@
         "MaxResults": int,
         "StartTimeFilter": TimeRangeTypeDef,
         "StatusFilter": DataSourceSyncJobStatusType,
     },
     total=False,
 )
 
+
 class ListDataSourceSyncJobsRequestRequestTypeDef(
     _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
     _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
 ):
     pass
 
+
 ListEntityPersonasResponseTypeDef = TypedDict(
     "ListEntityPersonasResponseTypeDef",
     {
         "SummaryItems": List[PersonasSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQuerySuggestionsBlockListsResponseTypeDef = TypedDict(
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     {
         "BlockListSummaryItems": List[QuerySuggestionsBlockListSummaryTypeDef],
         "NextToken": str,
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
 
 ListThesauriResponseTypeDef = TypedDict(
     "ListThesauriResponseTypeDef",
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -3968,19 +3783,21 @@
     {
         "ClickFeedbackItems": Sequence[ClickFeedbackTypeDef],
         "RelevanceFeedbackItems": Sequence[RelevanceFeedbackTypeDef],
     },
     total=False,
 )
 
+
 class SubmitFeedbackRequestRequestTypeDef(
     _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
 ):
     pass
 
+
 UrlsOutputTypeDef = TypedDict(
     "UrlsOutputTypeDef",
     {
         "SeedUrlConfiguration": SeedUrlConfigurationOutputTypeDef,
         "SiteMapsConfiguration": SiteMapsConfigurationOutputTypeDef,
     },
     total=False,
@@ -4012,33 +3829,60 @@
     total=False,
 )
 
 _RequiredDatabaseConfigurationOutputTypeDef = TypedDict(
     "_RequiredDatabaseConfigurationOutputTypeDef",
     {
         "DatabaseEngineType": DatabaseEngineTypeType,
-        "ConnectionConfiguration": ConnectionConfigurationOutputTypeDef,
+        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
         "ColumnConfiguration": ColumnConfigurationOutputTypeDef,
     },
 )
 _OptionalDatabaseConfigurationOutputTypeDef = TypedDict(
     "_OptionalDatabaseConfigurationOutputTypeDef",
     {
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "AclConfiguration": AclConfigurationOutputTypeDef,
-        "SqlConfiguration": SqlConfigurationOutputTypeDef,
+        "AclConfiguration": AclConfigurationTypeDef,
+        "SqlConfiguration": SqlConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseConfigurationOutputTypeDef(
     _RequiredDatabaseConfigurationOutputTypeDef, _OptionalDatabaseConfigurationOutputTypeDef
 ):
     pass
 
+
+_RequiredDatabaseConfigurationTypeDef = TypedDict(
+    "_RequiredDatabaseConfigurationTypeDef",
+    {
+        "DatabaseEngineType": DatabaseEngineTypeType,
+        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
+        "ColumnConfiguration": ColumnConfigurationTypeDef,
+    },
+)
+_OptionalDatabaseConfigurationTypeDef = TypedDict(
+    "_OptionalDatabaseConfigurationTypeDef",
+    {
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
+        "AclConfiguration": AclConfigurationTypeDef,
+        "SqlConfiguration": SqlConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class DatabaseConfigurationTypeDef(
+    _RequiredDatabaseConfigurationTypeDef, _OptionalDatabaseConfigurationTypeDef
+):
+    pass
+
+
 _RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
     "_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef",
     {
         "IncludedStates": List[SalesforceKnowledgeArticleStateType],
     },
 )
 _OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
@@ -4050,20 +3894,49 @@
         "CustomKnowledgeArticleTypeConfigurations": List[
             SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef
         ],
     },
     total=False,
 )
 
+
 class SalesforceKnowledgeArticleConfigurationOutputTypeDef(
     _RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef,
     _OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_RequiredSalesforceKnowledgeArticleConfigurationTypeDef",
+    {
+        "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
+    },
+)
+_OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
+    "_OptionalSalesforceKnowledgeArticleConfigurationTypeDef",
+    {
+        "StandardKnowledgeArticleTypeConfiguration": (
+            SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef
+        ),
+        "CustomKnowledgeArticleTypeConfigurations": Sequence[
+            SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef
+        ],
+    },
+    total=False,
+)
+
+
+class SalesforceKnowledgeArticleConfigurationTypeDef(
+    _RequiredSalesforceKnowledgeArticleConfigurationTypeDef,
+    _OptionalSalesforceKnowledgeArticleConfigurationTypeDef,
+):
+    pass
+
+
 _RequiredServiceNowConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceNowConfigurationOutputTypeDef",
     {
         "HostUrl": str,
         "SecretArn": str,
         "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
     },
@@ -4074,166 +3947,94 @@
         "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
         "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationOutputTypeDef,
         "AuthenticationType": ServiceNowAuthenticationTypeType,
     },
     total=False,
 )
 
+
 class ServiceNowConfigurationOutputTypeDef(
     _RequiredServiceNowConfigurationOutputTypeDef, _OptionalServiceNowConfigurationOutputTypeDef
 ):
     pass
 
+
+_RequiredServiceNowConfigurationTypeDef = TypedDict(
+    "_RequiredServiceNowConfigurationTypeDef",
+    {
+        "HostUrl": str,
+        "SecretArn": str,
+        "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
+    },
+)
+_OptionalServiceNowConfigurationTypeDef = TypedDict(
+    "_OptionalServiceNowConfigurationTypeDef",
+    {
+        "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationTypeDef,
+        "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationTypeDef,
+        "AuthenticationType": ServiceNowAuthenticationTypeType,
+    },
+    total=False,
+)
+
+
+class ServiceNowConfigurationTypeDef(
+    _RequiredServiceNowConfigurationTypeDef, _OptionalServiceNowConfigurationTypeDef
+):
+    pass
+
+
 _RequiredGitHubConfigurationOutputTypeDef = TypedDict(
     "_RequiredGitHubConfigurationOutputTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGitHubConfigurationOutputTypeDef = TypedDict(
     "_OptionalGitHubConfigurationOutputTypeDef",
     {
-        "SaaSConfiguration": SaaSConfigurationOutputTypeDef,
-        "OnPremiseConfiguration": OnPremiseConfigurationOutputTypeDef,
+        "SaaSConfiguration": SaaSConfigurationTypeDef,
+        "OnPremiseConfiguration": OnPremiseConfigurationTypeDef,
         "Type": TypeType,
         "UseChangeLog": bool,
-        "GitHubDocumentCrawlProperties": GitHubDocumentCrawlPropertiesOutputTypeDef,
+        "GitHubDocumentCrawlProperties": GitHubDocumentCrawlPropertiesTypeDef,
         "RepositoryFilter": List[str],
         "InclusionFolderNamePatterns": List[str],
         "InclusionFileTypePatterns": List[str],
         "InclusionFileNamePatterns": List[str],
         "ExclusionFolderNamePatterns": List[str],
         "ExclusionFileTypePatterns": List[str],
         "ExclusionFileNamePatterns": List[str],
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "GitHubRepositoryConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
-        ],
-        "GitHubCommitConfigurationFieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "GitHubIssueDocumentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
-        ],
-        "GitHubIssueCommentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
-        ],
+        "GitHubRepositoryConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "GitHubCommitConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "GitHubIssueDocumentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "GitHubIssueCommentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
         "GitHubIssueAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
         "GitHubPullRequestCommentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
         "GitHubPullRequestDocumentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
         "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingOutputTypeDef
+            DataSourceToIndexFieldMappingTypeDef
         ],
     },
     total=False,
 )
 
+
 class GitHubConfigurationOutputTypeDef(
     _RequiredGitHubConfigurationOutputTypeDef, _OptionalGitHubConfigurationOutputTypeDef
 ):
     pass
 
-_RequiredOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOneDriveConfigurationOutputTypeDef",
-    {
-        "TenantDomain": str,
-        "SecretArn": str,
-        "OneDriveUsers": OneDriveUsersOutputTypeDef,
-    },
-)
-_OptionalOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOneDriveConfigurationOutputTypeDef",
-    {
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingOutputTypeDef],
-        "DisableLocalGroups": bool,
-    },
-    total=False,
-)
-
-class OneDriveConfigurationOutputTypeDef(
-    _RequiredOneDriveConfigurationOutputTypeDef, _OptionalOneDriveConfigurationOutputTypeDef
-):
-    pass
-
-_RequiredDatabaseConfigurationTypeDef = TypedDict(
-    "_RequiredDatabaseConfigurationTypeDef",
-    {
-        "DatabaseEngineType": DatabaseEngineTypeType,
-        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
-        "ColumnConfiguration": ColumnConfigurationTypeDef,
-    },
-)
-_OptionalDatabaseConfigurationTypeDef = TypedDict(
-    "_OptionalDatabaseConfigurationTypeDef",
-    {
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-        "AclConfiguration": AclConfigurationTypeDef,
-        "SqlConfiguration": SqlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class DatabaseConfigurationTypeDef(
-    _RequiredDatabaseConfigurationTypeDef, _OptionalDatabaseConfigurationTypeDef
-):
-    pass
-
-_RequiredSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_RequiredSalesforceKnowledgeArticleConfigurationTypeDef",
-    {
-        "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
-    },
-)
-_OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
-    "_OptionalSalesforceKnowledgeArticleConfigurationTypeDef",
-    {
-        "StandardKnowledgeArticleTypeConfiguration": (
-            SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef
-        ),
-        "CustomKnowledgeArticleTypeConfigurations": Sequence[
-            SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef
-        ],
-    },
-    total=False,
-)
-
-class SalesforceKnowledgeArticleConfigurationTypeDef(
-    _RequiredSalesforceKnowledgeArticleConfigurationTypeDef,
-    _OptionalSalesforceKnowledgeArticleConfigurationTypeDef,
-):
-    pass
-
-_RequiredServiceNowConfigurationTypeDef = TypedDict(
-    "_RequiredServiceNowConfigurationTypeDef",
-    {
-        "HostUrl": str,
-        "SecretArn": str,
-        "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
-    },
-)
-_OptionalServiceNowConfigurationTypeDef = TypedDict(
-    "_OptionalServiceNowConfigurationTypeDef",
-    {
-        "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationTypeDef,
-        "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationTypeDef,
-        "AuthenticationType": ServiceNowAuthenticationTypeType,
-    },
-    total=False,
-)
-
-class ServiceNowConfigurationTypeDef(
-    _RequiredServiceNowConfigurationTypeDef, _OptionalServiceNowConfigurationTypeDef
-):
-    pass
 
 _RequiredGitHubConfigurationTypeDef = TypedDict(
     "_RequiredGitHubConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
@@ -4275,19 +4076,47 @@
         "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": Sequence[
             DataSourceToIndexFieldMappingTypeDef
         ],
     },
     total=False,
 )
 
+
 class GitHubConfigurationTypeDef(
     _RequiredGitHubConfigurationTypeDef, _OptionalGitHubConfigurationTypeDef
 ):
     pass
 
+
+_RequiredOneDriveConfigurationOutputTypeDef = TypedDict(
+    "_RequiredOneDriveConfigurationOutputTypeDef",
+    {
+        "TenantDomain": str,
+        "SecretArn": str,
+        "OneDriveUsers": OneDriveUsersOutputTypeDef,
+    },
+)
+_OptionalOneDriveConfigurationOutputTypeDef = TypedDict(
+    "_OptionalOneDriveConfigurationOutputTypeDef",
+    {
+        "InclusionPatterns": List[str],
+        "ExclusionPatterns": List[str],
+        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "DisableLocalGroups": bool,
+    },
+    total=False,
+)
+
+
+class OneDriveConfigurationOutputTypeDef(
+    _RequiredOneDriveConfigurationOutputTypeDef, _OptionalOneDriveConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredOneDriveConfigurationTypeDef = TypedDict(
     "_RequiredOneDriveConfigurationTypeDef",
     {
         "TenantDomain": str,
         "SecretArn": str,
         "OneDriveUsers": OneDriveUsersTypeDef,
     },
@@ -4299,33 +4128,35 @@
         "ExclusionPatterns": Sequence[str],
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
         "DisableLocalGroups": bool,
     },
     total=False,
 )
 
+
 class OneDriveConfigurationTypeDef(
     _RequiredOneDriveConfigurationTypeDef, _OptionalOneDriveConfigurationTypeDef
 ):
     pass
 
+
 DescribeQuerySuggestionsConfigResponseTypeDef = TypedDict(
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     {
         "Mode": ModeType,
         "Status": QuerySuggestionsStatusType,
         "QueryLogLookBackWindowInDays": int,
         "IncludeQueriesWithoutUserInformation": bool,
         "MinimumNumberOfQueryingUsers": int,
         "MinimumQueryCount": int,
         "LastSuggestionsBuildTime": datetime,
         "LastClearTime": datetime,
         "TotalSuggestionsCount": int,
         "AttributeSuggestionsConfig": AttributeSuggestionsDescribeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -4340,20 +4171,22 @@
         "MinimumNumberOfQueryingUsers": int,
         "MinimumQueryCount": int,
         "AttributeSuggestionsConfig": AttributeSuggestionsUpdateConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
     _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
     _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredConfluenceConfigurationOutputTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationOutputTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4364,25 +4197,27 @@
         "SpaceConfiguration": ConfluenceSpaceConfigurationOutputTypeDef,
         "PageConfiguration": ConfluencePageConfigurationOutputTypeDef,
         "BlogConfiguration": ConfluenceBlogConfigurationOutputTypeDef,
         "AttachmentConfiguration": ConfluenceAttachmentConfigurationOutputTypeDef,
         "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
         "InclusionPatterns": List[str],
         "ExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationType": ConfluenceAuthenticationTypeType,
     },
     total=False,
 )
 
+
 class ConfluenceConfigurationOutputTypeDef(
     _RequiredConfluenceConfigurationOutputTypeDef, _OptionalConfluenceConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredConfluenceConfigurationTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4399,19 +4234,33 @@
         "ExclusionPatterns": Sequence[str],
         "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationType": ConfluenceAuthenticationTypeType,
     },
     total=False,
 )
 
+
 class ConfluenceConfigurationTypeDef(
     _RequiredConfluenceConfigurationTypeDef, _OptionalConfluenceConfigurationTypeDef
 ):
     pass
 
+
+DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccessControlConfigurationResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "ErrorMessage": str,
+        "AccessControlList": List[PrincipalTypeDef],
+        "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Name": str,
     },
 )
@@ -4422,20 +4271,22 @@
         "AccessControlList": Sequence[PrincipalTypeDef],
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
         "Id": str,
     },
 )
@@ -4446,20 +4297,38 @@
         "Description": str,
         "AccessControlList": Sequence[PrincipalTypeDef],
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
     },
     total=False,
 )
 
+
 class UpdateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
+CreateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "CreateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "UpdateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AttributeSuggestionsGetConfigTypeDef = TypedDict(
     "AttributeSuggestionsGetConfigTypeDef",
     {
         "SuggestionAttributes": Sequence[str],
         "AdditionalResponseAttributes": Sequence[str],
         "AttributeFilter": "AttributeFilterTypeDef",
         "UserContext": UserContextTypeDef,
@@ -4468,36 +4337,24 @@
 )
 
 ListDataSourceSyncJobsResponseTypeDef = TypedDict(
     "ListDataSourceSyncJobsResponseTypeDef",
     {
         "History": List[DataSourceSyncJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
-    "DescribeAccessControlConfigurationResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "ErrorMessage": str,
-        "AccessControlList": List[PrincipalOutputTypeDef],
-        "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExperiencesResponseTypeDef = TypedDict(
     "ListExperiencesResponseTypeDef",
     {
         "SummaryItems": List[ExperiencesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHookConfigurationOutputTypeDef = TypedDict(
     "_RequiredHookConfigurationOutputTypeDef",
     {
         "LambdaArn": str,
@@ -4508,19 +4365,21 @@
     "_OptionalHookConfigurationOutputTypeDef",
     {
         "InvocationCondition": DocumentAttributeConditionOutputTypeDef,
     },
     total=False,
 )
 
+
 class HookConfigurationOutputTypeDef(
     _RequiredHookConfigurationOutputTypeDef, _OptionalHookConfigurationOutputTypeDef
 ):
     pass
 
+
 RetrieveResultItemTypeDef = TypedDict(
     "RetrieveResultItemTypeDef",
     {
         "Id": str,
         "DocumentId": str,
         "DocumentTitle": str,
         "Content": str,
@@ -4561,19 +4420,21 @@
     "_OptionalHookConfigurationTypeDef",
     {
         "InvocationCondition": DocumentAttributeConditionTypeDef,
     },
     total=False,
 )
 
+
 class HookConfigurationTypeDef(
     _RequiredHookConfigurationTypeDef, _OptionalHookConfigurationTypeDef
 ):
     pass
 
+
 InlineCustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     {
         "Condition": DocumentAttributeConditionTypeDef,
         "Target": DocumentAttributeTargetTypeDef,
         "DocumentContentDeletion": bool,
     },
@@ -4607,17 +4468,19 @@
     "_OptionalDocumentInfoTypeDef",
     {
         "Attributes": Sequence[DocumentAttributeTypeDef],
     },
     total=False,
 )
 
+
 class DocumentInfoTypeDef(_RequiredDocumentInfoTypeDef, _OptionalDocumentInfoTypeDef):
     pass
 
+
 _RequiredDocumentTypeDef = TypedDict(
     "_RequiredDocumentTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDocumentTypeDef = TypedDict(
@@ -4631,17 +4494,19 @@
         "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
         "ContentType": ContentTypeType,
         "AccessControlConfigurationId": str,
     },
     total=False,
 )
 
+
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
+
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -4659,19 +4524,21 @@
         "UserContext": UserContextTypeDef,
         "VisitorId": str,
         "SpellCorrectionConfiguration": SpellCorrectionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredRetrieveRequestRequestTypeDef = TypedDict(
     "_RequiredRetrieveRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -4684,25 +4551,27 @@
         "PageNumber": int,
         "PageSize": int,
         "UserContext": UserContextTypeDef,
     },
     total=False,
 )
 
+
 class RetrieveRequestRequestTypeDef(
     _RequiredRetrieveRequestRequestTypeDef, _OptionalRetrieveRequestRequestTypeDef
 ):
     pass
 
+
 ListExperienceEntitiesResponseTypeDef = TypedDict(
     "ListExperienceEntitiesResponseTypeDef",
     {
         "SummaryItems": List[ExperienceEntitiesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExperienceResponseTypeDef = TypedDict(
     "DescribeExperienceResponseTypeDef",
     {
         "Id": str,
@@ -4712,15 +4581,15 @@
         "Configuration": ExperienceConfigurationOutputTypeDef,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Description": str,
         "Status": ExperienceStatusType,
         "RoleArn": str,
         "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperienceRequestRequestTypeDef",
     {
         "Name": str,
@@ -4734,19 +4603,21 @@
         "Configuration": ExperienceConfigurationTypeDef,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateExperienceRequestRequestTypeDef(
     _RequiredCreateExperienceRequestRequestTypeDef, _OptionalCreateExperienceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4757,34 +4628,20 @@
         "RoleArn": str,
         "Configuration": ExperienceConfigurationTypeDef,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateExperienceRequestRequestTypeDef(
     _RequiredUpdateExperienceRequestRequestTypeDef, _OptionalUpdateExperienceRequestRequestTypeDef
 ):
     pass
 
-CreateFeaturedResultsSetResponseTypeDef = TypedDict(
-    "CreateFeaturedResultsSetResponseTypeDef",
-    {
-        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
-    "UpdateFeaturedResultsSetResponseTypeDef",
-    {
-        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredPutPrincipalMappingRequestRequestTypeDef = TypedDict(
     "_RequiredPutPrincipalMappingRequestRequestTypeDef",
     {
         "IndexId": str,
         "GroupId": str,
         "GroupMembers": GroupMembersTypeDef,
@@ -4796,51 +4653,30 @@
         "DataSourceId": str,
         "OrderingId": int,
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class PutPrincipalMappingRequestRequestTypeDef(
     _RequiredPutPrincipalMappingRequestRequestTypeDef,
     _OptionalPutPrincipalMappingRequestRequestTypeDef,
 ):
     pass
 
+
 AdditionalResultAttributeValueTypeDef = TypedDict(
     "AdditionalResultAttributeValueTypeDef",
     {
         "TextWithHighlightsValue": TextWithHighlightsTypeDef,
     },
     total=False,
 )
 
-DescribeIndexResponseTypeDef = TypedDict(
-    "DescribeIndexResponseTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Edition": IndexEditionType,
-        "RoleArn": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "Status": IndexStatusType,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationOutputTypeDef],
-        "IndexStatistics": IndexStatisticsTypeDef,
-        "ErrorMessage": str,
-        "CapacityUnits": CapacityUnitsConfigurationOutputTypeDef,
-        "UserTokenConfigurations": List[UserTokenConfigurationOutputTypeDef],
-        "UserContextPolicy": UserContextPolicyType,
-        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIndexRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -4855,19 +4691,44 @@
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
+
+DescribeIndexResponseTypeDef = TypedDict(
+    "DescribeIndexResponseTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Edition": IndexEditionType,
+        "RoleArn": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "Status": IndexStatusType,
+        "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationOutputTypeDef],
+        "IndexStatistics": IndexStatisticsTypeDef,
+        "ErrorMessage": str,
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
+        "UserContextPolicy": UserContextPolicyType,
+        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
@@ -4881,19 +4742,21 @@
         "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateIndexRequestRequestTypeDef(
     _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredWebCrawlerConfigurationOutputTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationOutputTypeDef",
     {
         "Urls": UrlsOutputTypeDef,
     },
 )
 _OptionalWebCrawlerConfigurationOutputTypeDef = TypedDict(
@@ -4901,25 +4764,27 @@
     {
         "CrawlDepth": int,
         "MaxLinksPerPage": int,
         "MaxContentSizePerPageInMegaBytes": float,
         "MaxUrlsPerMinuteCrawlRate": int,
         "UrlInclusionPatterns": List[str],
         "UrlExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class WebCrawlerConfigurationOutputTypeDef(
     _RequiredWebCrawlerConfigurationOutputTypeDef, _OptionalWebCrawlerConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredWebCrawlerConfigurationTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationTypeDef",
     {
         "Urls": UrlsTypeDef,
     },
 )
 _OptionalWebCrawlerConfigurationTypeDef = TypedDict(
@@ -4933,19 +4798,21 @@
         "UrlExclusionPatterns": Sequence[str],
         "ProxyConfiguration": ProxyConfigurationTypeDef,
         "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class WebCrawlerConfigurationTypeDef(
     _RequiredWebCrawlerConfigurationTypeDef, _OptionalWebCrawlerConfigurationTypeDef
 ):
     pass
 
+
 SuggestionValueTypeDef = TypedDict(
     "SuggestionValueTypeDef",
     {
         "Text": SuggestionTextWithHighlightsTypeDef,
     },
     total=False,
 )
@@ -4978,19 +4845,21 @@
         ),
         "IncludeAttachmentFilePatterns": List[str],
         "ExcludeAttachmentFilePatterns": List[str],
     },
     total=False,
 )
 
+
 class SalesforceConfigurationOutputTypeDef(
     _RequiredSalesforceConfigurationOutputTypeDef, _OptionalSalesforceConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredSalesforceConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
     },
 )
@@ -5006,19 +4875,21 @@
         ),
         "IncludeAttachmentFilePatterns": Sequence[str],
         "ExcludeAttachmentFilePatterns": Sequence[str],
     },
     total=False,
 )
 
+
 class SalesforceConfigurationTypeDef(
     _RequiredSalesforceConfigurationTypeDef, _OptionalSalesforceConfigurationTypeDef
 ):
     pass
 
+
 _RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -5028,26 +4899,28 @@
         "MaxSuggestionsCount": int,
         "SuggestionTypes": Sequence[SuggestionTypeType],
         "AttributeSuggestionsConfig": AttributeSuggestionsGetConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetQuerySuggestionsRequestRequestTypeDef(
     _RequiredGetQuerySuggestionsRequestRequestTypeDef,
     _OptionalGetQuerySuggestionsRequestRequestTypeDef,
 ):
     pass
 
+
 RetrieveResultTypeDef = TypedDict(
     "RetrieveResultTypeDef",
     {
         "QueryId": str,
         "ResultItems": List[RetrieveResultItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
     "CustomDocumentEnrichmentConfigurationOutputTypeDef",
     {
         "InlineConfigurations": List[InlineCustomDocumentEnrichmentConfigurationOutputTypeDef],
@@ -5158,19 +5031,21 @@
     {
         "RoleArn": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class BatchPutDocumentRequestRequestTypeDef(
     _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
 ):
     pass
 
+
 FeaturedResultsItemTypeDef = TypedDict(
     "FeaturedResultsItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
@@ -5203,15 +5078,15 @@
 )
 
 GetQuerySuggestionsResponseTypeDef = TypedDict(
     "GetQuerySuggestionsResponseTypeDef",
     {
         "QuerySuggestionsId": str,
         "Suggestions": List[SuggestionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSourceResponseTypeDef = TypedDict(
     "DescribeDataSourceResponseTypeDef",
     {
         "Id": str,
@@ -5225,15 +5100,15 @@
         "Description": str,
         "Status": DataSourceStatusType,
         "Schedule": str,
         "RoleArn": str,
         "ErrorMessage": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "Name": str,
@@ -5253,19 +5128,21 @@
         "ClientToken": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -5280,25 +5157,27 @@
         "RoleArn": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDataSourceRequestRequestTypeDef(
     _RequiredUpdateDataSourceRequestRequestTypeDef, _OptionalUpdateDataSourceRequestRequestTypeDef
 ):
     pass
 
+
 QueryResultTypeDef = TypedDict(
     "QueryResultTypeDef",
     {
         "QueryId": str,
         "ResultItems": List[QueryResultItemTypeDef],
         "FacetResults": List["FacetResultTypeDef"],
         "TotalNumberOfResults": int,
         "Warnings": List[WarningTypeDef],
         "SpellCorrectedQueries": List[SpellCorrectedQueryTypeDef],
         "FeaturedResultsItems": List[FeaturedResultsItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/PKG-INFO` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.28.12
-Summary: Type annotations for boto3.kendra 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra)](https://pepy.tech/project/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,135 +357,103 @@
 
 `mypy_boto3_kendra.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kendra.type_defs import (
     AccessControlConfigurationSummaryTypeDef,
-    AccessControlListConfigurationOutputTypeDef,
     AccessControlListConfigurationTypeDef,
-    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
-    DataSourceToIndexFieldMappingOutputTypeDef,
-    DataSourceVpcConfigurationOutputTypeDef,
-    S3PathOutputTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
-    DataSourceVpcConfigurationTypeDef,
+    DataSourceVpcConfigurationOutputTypeDef,
     S3PathTypeDef,
+    DataSourceVpcConfigurationTypeDef,
     EntityConfigurationTypeDef,
     FailedEntityTypeDef,
+    ResponseMetadataTypeDef,
     EntityPersonaConfigurationTypeDef,
-    SuggestableConfigOutputTypeDef,
     SuggestableConfigTypeDef,
-    BasicAuthenticationConfigurationOutputTypeDef,
     BasicAuthenticationConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
     BatchDeleteFeaturedResultsSetErrorTypeDef,
     BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
-    CapacityUnitsConfigurationOutputTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
     ClickFeedbackTypeDef,
-    ConfluenceAttachmentToIndexFieldMappingOutputTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
-    ConfluenceBlogToIndexFieldMappingOutputTypeDef,
     ConfluenceBlogToIndexFieldMappingTypeDef,
-    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
-    ConfluencePageToIndexFieldMappingOutputTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
-    ConfluenceSpaceToIndexFieldMappingOutputTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
-    ConnectionConfigurationOutputTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationOutputTypeDef,
     ContentSourceConfigurationTypeDef,
     CorrectionTypeDef,
     PrincipalTypeDef,
-    CreateAccessControlConfigurationResponseTypeDef,
     TagTypeDef,
-    CreateDataSourceResponseTypeDef,
-    CreateExperienceResponseTypeDef,
-    CreateFaqResponseTypeDef,
     FeaturedDocumentTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     UserGroupResolutionConfigurationTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateQuerySuggestionsBlockListResponseTypeDef,
-    CreateThesaurusResponseTypeDef,
     TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     DataSourceGroupTypeDef,
     DataSourceSummaryTypeDef,
     DataSourceSyncJobMetricsTypeDef,
-    SqlConfigurationOutputTypeDef,
     SqlConfigurationTypeDef,
     DeleteAccessControlConfigurationRequestRequestTypeDef,
     DeleteDataSourceRequestRequestTypeDef,
     DeleteExperienceRequestRequestTypeDef,
     DeleteFaqRequestRequestTypeDef,
     DeleteIndexRequestRequestTypeDef,
     DeletePrincipalMappingRequestRequestTypeDef,
     DeleteQuerySuggestionsBlockListRequestRequestTypeDef,
     DeleteThesaurusRequestRequestTypeDef,
     DescribeAccessControlConfigurationRequestRequestTypeDef,
-    PrincipalOutputTypeDef,
     DescribeDataSourceRequestRequestTypeDef,
     DescribeExperienceRequestRequestTypeDef,
     ExperienceEndpointTypeDef,
     DescribeFaqRequestRequestTypeDef,
     DescribeFeaturedResultsSetRequestRequestTypeDef,
     FeaturedDocumentMissingTypeDef,
     FeaturedDocumentWithMetadataTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
-    UserGroupResolutionConfigurationOutputTypeDef,
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueOutputTypeDef,
     DocumentAttributeValueTypeDef,
     RelevanceOutputTypeDef,
-    SearchOutputTypeDef,
-    RelevanceTypeDef,
     SearchTypeDef,
-    DocumentsMetadataConfigurationOutputTypeDef,
+    RelevanceTypeDef,
     DocumentsMetadataConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EntityDisplayDataTypeDef,
-    UserIdentityConfigurationOutputTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
     FacetTypeDef,
     FaqStatisticsTypeDef,
     FaqSummaryTypeDef,
-    FeaturedDocumentOutputTypeDef,
     FeaturedResultsSetSummaryTypeDef,
     GetSnapshotsRequestRequestTypeDef,
     TimeRangeOutputTypeDef,
-    GitHubDocumentCrawlPropertiesOutputTypeDef,
-    SaaSConfigurationOutputTypeDef,
     GitHubDocumentCrawlPropertiesTypeDef,
     SaaSConfigurationTypeDef,
     MemberGroupTypeDef,
     MemberUserTypeDef,
     GroupSummaryTypeDef,
     HighlightTypeDef,
     IndexConfigurationSummaryTypeDef,
     TextDocumentStatisticsTypeDef,
-    JsonTokenTypeConfigurationOutputTypeDef,
     JsonTokenTypeConfigurationTypeDef,
-    JwtTokenTypeConfigurationOutputTypeDef,
     JwtTokenTypeConfigurationTypeDef,
     ListAccessControlConfigurationsRequestRequestTypeDef,
     TimeRangeTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
@@ -493,81 +461,86 @@
     ListFaqsRequestRequestTypeDef,
     ListFeaturedResultsSetsRequestRequestTypeDef,
     ListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListQuerySuggestionsBlockListsRequestRequestTypeDef,
     QuerySuggestionsBlockListSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListThesauriRequestRequestTypeDef,
     ThesaurusSummaryTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     ScoreAttributesTypeDef,
     WarningTypeDef,
     RelevanceFeedbackTypeDef,
-    ResponseMetadataTypeDef,
     SeedUrlConfigurationOutputTypeDef,
     SeedUrlConfigurationTypeDef,
     SiteMapsConfigurationOutputTypeDef,
     SiteMapsConfigurationTypeDef,
     StartDataSourceSyncJobRequestRequestTypeDef,
-    StartDataSourceSyncJobResponseTypeDef,
     StopDataSourceSyncJobRequestRequestTypeDef,
     SuggestionHighlightTypeDef,
     TableCellTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListAccessControlConfigurationsResponseTypeDef,
     ColumnConfigurationOutputTypeDef,
+    ColumnConfigurationTypeDef,
     GoogleDriveConfigurationOutputTypeDef,
+    GoogleDriveConfigurationTypeDef,
     SalesforceChatterFeedConfigurationOutputTypeDef,
+    SalesforceChatterFeedConfigurationTypeDef,
     SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
+    SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
+    SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardObjectAttachmentConfigurationOutputTypeDef,
+    SalesforceStandardObjectAttachmentConfigurationTypeDef,
     SalesforceStandardObjectConfigurationOutputTypeDef,
+    SalesforceStandardObjectConfigurationTypeDef,
     ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
+    ServiceNowKnowledgeArticleConfigurationTypeDef,
     ServiceNowServiceCatalogConfigurationOutputTypeDef,
+    ServiceNowServiceCatalogConfigurationTypeDef,
     WorkDocsConfigurationOutputTypeDef,
+    WorkDocsConfigurationTypeDef,
     BoxConfigurationOutputTypeDef,
     FsxConfigurationOutputTypeDef,
     JiraConfigurationOutputTypeDef,
     QuipConfigurationOutputTypeDef,
     SlackConfigurationOutputTypeDef,
     AlfrescoConfigurationOutputTypeDef,
-    DescribeFaqResponseTypeDef,
-    DescribeQuerySuggestionsBlockListResponseTypeDef,
-    DescribeThesaurusResponseTypeDef,
-    OnPremiseConfigurationOutputTypeDef,
+    OnPremiseConfigurationTypeDef,
     OneDriveUsersOutputTypeDef,
-    ColumnConfigurationTypeDef,
-    GoogleDriveConfigurationTypeDef,
-    SalesforceChatterFeedConfigurationTypeDef,
-    SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
-    SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
-    SalesforceStandardObjectAttachmentConfigurationTypeDef,
-    SalesforceStandardObjectConfigurationTypeDef,
-    ServiceNowKnowledgeArticleConfigurationTypeDef,
-    ServiceNowServiceCatalogConfigurationTypeDef,
-    WorkDocsConfigurationTypeDef,
+    OneDriveUsersTypeDef,
+    UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
+    UpdateThesaurusRequestRequestTypeDef,
+    AlfrescoConfigurationTypeDef,
     BoxConfigurationTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
-    AlfrescoConfigurationTypeDef,
-    OnPremiseConfigurationTypeDef,
-    OneDriveUsersTypeDef,
-    UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
-    UpdateThesaurusRequestRequestTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
+    CreateAccessControlConfigurationResponseTypeDef,
+    CreateDataSourceResponseTypeDef,
+    CreateExperienceResponseTypeDef,
+    CreateFaqResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateQuerySuggestionsBlockListResponseTypeDef,
+    CreateThesaurusResponseTypeDef,
+    DescribeFaqResponseTypeDef,
+    DescribeQuerySuggestionsBlockListResponseTypeDef,
+    DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAccessControlConfigurationsResponseTypeDef,
+    StartDataSourceSyncJobResponseTypeDef,
     AssociatePersonasToEntitiesRequestRequestTypeDef,
     AttributeSuggestionsDescribeConfigTypeDef,
     AttributeSuggestionsUpdateConfigTypeDef,
     AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
@@ -581,83 +554,84 @@
     SharePointConfigurationOutputTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationOutputTypeDef,
     ConfluencePageConfigurationTypeDef,
     ConfluenceSpaceConfigurationOutputTypeDef,
     ConfluenceSpaceConfigurationTypeDef,
     SpellCorrectedQueryTypeDef,
+    HierarchicalPrincipalOutputTypeDef,
     HierarchicalPrincipalTypeDef,
     CreateFaqRequestRequestTypeDef,
     CreateQuerySuggestionsBlockListRequestRequestTypeDef,
     CreateThesaurusRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedResultsSetTypeDef,
     UpdateFeaturedResultsSetRequestRequestTypeDef,
     UserContextTypeDef,
     ListDataSourcesResponseTypeDef,
     DataSourceSyncJobTypeDef,
-    HierarchicalPrincipalOutputTypeDef,
     ExperiencesSummaryTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionOutputTypeDef,
     DocumentAttributeOutputTypeDef,
     DocumentAttributeTargetOutputTypeDef,
     DocumentAttributeValueCountPairTypeDef,
     DocumentAttributeConditionTypeDef,
     DocumentAttributeTargetTypeDef,
     DocumentAttributeTypeDef,
     DocumentMetadataConfigurationOutputTypeDef,
-    DocumentRelevanceConfigurationTypeDef,
     DocumentMetadataConfigurationTypeDef,
+    DocumentRelevanceConfigurationTypeDef,
     S3DataSourceConfigurationOutputTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationOutputTypeDef,
     ExperienceConfigurationTypeDef,
     ListFaqsResponseTypeDef,
-    FeaturedResultsSetTypeDef,
     ListFeaturedResultsSetsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
-    UserTokenConfigurationOutputTypeDef,
     UserTokenConfigurationTypeDef,
     ListDataSourceSyncJobsRequestRequestTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListThesauriResponseTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     UrlsOutputTypeDef,
     UrlsTypeDef,
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationOutputTypeDef,
-    SalesforceKnowledgeArticleConfigurationOutputTypeDef,
-    ServiceNowConfigurationOutputTypeDef,
-    GitHubConfigurationOutputTypeDef,
-    OneDriveConfigurationOutputTypeDef,
     DatabaseConfigurationTypeDef,
+    SalesforceKnowledgeArticleConfigurationOutputTypeDef,
     SalesforceKnowledgeArticleConfigurationTypeDef,
+    ServiceNowConfigurationOutputTypeDef,
     ServiceNowConfigurationTypeDef,
+    GitHubConfigurationOutputTypeDef,
     GitHubConfigurationTypeDef,
+    OneDriveConfigurationOutputTypeDef,
     OneDriveConfigurationTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     UpdateQuerySuggestionsConfigRequestRequestTypeDef,
     ConfluenceConfigurationOutputTypeDef,
     ConfluenceConfigurationTypeDef,
+    DescribeAccessControlConfigurationResponseTypeDef,
     CreateAccessControlConfigurationRequestRequestTypeDef,
     UpdateAccessControlConfigurationRequestRequestTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
     AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
-    DescribeAccessControlConfigurationResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationOutputTypeDef,
     RetrieveResultItemTypeDef,
     SourceDocumentTypeDef,
     InlineCustomDocumentEnrichmentConfigurationOutputTypeDef,
     HookConfigurationTypeDef,
     InlineCustomDocumentEnrichmentConfigurationTypeDef,
@@ -666,20 +640,18 @@
     DocumentTypeDef,
     QueryRequestRequestTypeDef,
     RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
     UpdateExperienceRequestRequestTypeDef,
-    CreateFeaturedResultsSetResponseTypeDef,
-    UpdateFeaturedResultsSetResponseTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
-    DescribeIndexResponseTypeDef,
     CreateIndexRequestRequestTypeDef,
+    DescribeIndexResponseTypeDef,
     UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationOutputTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationOutputTypeDef,
     SalesforceConfigurationTypeDef,
```

### Comparing `mypy-boto3-kendra-1.28.12/mypy_boto3_kendra.egg-info/SOURCES.txt` & `mypy-boto3-kendra-1.28.15/mypy_boto3_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.12/setup.py` & `mypy-boto3-kendra-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.kendra 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

