# Comparing `tmp/mypy-boto3-customer-profiles-1.28.12.tar.gz` & `tmp/mypy-boto3-customer-profiles-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-customer-profiles-1.28.12.tar", last modified: Thu Jul 27 05:34:32 2023, max compression
+gzip compressed data, was "mypy-boto3-customer-profiles-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-customer-profiles-1.28.12.tar` & `mypy-boto3-customer-profiles-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19129 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.724539 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    72206 2023-07-27 05:19:54.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72102 2023-07-27 05:19:53.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.880915 mypy-boto3-customer-profiles-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-28 20:42:34.872915 mypy-boto3-customer-profiles-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.860915 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-28 20:22:25.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-28 20:22:25.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69309 2023-07-28 20:22:27.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69209 2023-07-28 20:22:26.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.872915 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:34.000000 mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.880915 mypy-boto3-customer-profiles-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:22:24.000000 mypy-boto3-customer-profiles-1.28.15/setup.py
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/LICENSE` & `mypy-boto3-customer-profiles-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.12
-Summary: Type annotations for boto3.CustomerProfiles 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,189 +349,179 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    AddProfileKeyResponseTypeDef,
+    ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
-    AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
-    AttributeItemOutputTypeDef,
     AttributeItemTypeDef,
     AttributeTypesSelectorOutputTypeDef,
     AttributeTypesSelectorTypeDef,
-    ConflictResolutionOutputTypeDef,
-    ConsolidationOutputTypeDef,
     ConflictResolutionTypeDef,
+    ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
-    RangeOutputTypeDef,
-    ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
-    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
-    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
-    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
-    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
-    S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
-    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
-    ObjectTypeFieldOutputTypeDef,
+    ObjectTypeFieldTypeDef,
     ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetSimilarProfilesRequestRequestTypeDef,
-    GetSimilarProfilesResponseTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
-    JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
-    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
-    MergeProfilesResponseTypeDef,
-    ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
-    PaginatorConfigTypeDef,
-    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
-    PutProfileObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
+    AddProfileKeyResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteIntegrationResponseTypeDef,
+    DeleteProfileKeyResponseTypeDef,
+    DeleteProfileObjectResponseTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
+    DeleteProfileResponseTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
+    GetIntegrationResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MergeProfilesResponseTypeDef,
+    PutIntegrationResponseTypeDef,
+    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
-    ConditionsOutputTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
-    ExportingConfigOutputTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
-    UpdateCalculatedAttributeDefinitionResponseTypeDef,
-    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
     ListEventStreamsResponseTypeDef,
-    MatchingResponseTypeDef,
-    RuleBasedMatchingResponseTypeDef,
     MatchingRequestTypeDef,
+    MatchingResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
+    RuleBasedMatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainRequestRequestTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/README.md` & `mypy-boto3-customer-profiles-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,189 +317,179 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    AddProfileKeyResponseTypeDef,
+    ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
-    AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
-    AttributeItemOutputTypeDef,
     AttributeItemTypeDef,
     AttributeTypesSelectorOutputTypeDef,
     AttributeTypesSelectorTypeDef,
-    ConflictResolutionOutputTypeDef,
-    ConsolidationOutputTypeDef,
     ConflictResolutionTypeDef,
+    ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
-    RangeOutputTypeDef,
-    ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
-    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
-    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
-    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
-    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
-    S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
-    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
-    ObjectTypeFieldOutputTypeDef,
+    ObjectTypeFieldTypeDef,
     ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetSimilarProfilesRequestRequestTypeDef,
-    GetSimilarProfilesResponseTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
-    JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
-    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
-    MergeProfilesResponseTypeDef,
-    ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
-    PaginatorConfigTypeDef,
-    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
-    PutProfileObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
+    AddProfileKeyResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteIntegrationResponseTypeDef,
+    DeleteProfileKeyResponseTypeDef,
+    DeleteProfileObjectResponseTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
+    DeleteProfileResponseTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
+    GetIntegrationResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MergeProfilesResponseTypeDef,
+    PutIntegrationResponseTypeDef,
+    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
-    ConditionsOutputTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
-    ExportingConfigOutputTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
-    UpdateCalculatedAttributeDefinitionResponseTypeDef,
-    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
     ListEventStreamsResponseTypeDef,
-    MatchingResponseTypeDef,
-    RuleBasedMatchingResponseTypeDef,
     MatchingRequestTypeDef,
+    MatchingResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
+    RuleBasedMatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainRequestRequestTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.py` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.pyi` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__main__.py` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CustomerProfiles 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CustomerProfiles 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.py` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.pyi` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.py` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.pyi` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.py` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,28 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEventStreamsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEventStreamsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEventStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.pyi` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEventStreamsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEventStreamsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEventStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.py` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,189 +52,179 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "AddProfileKeyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
-    "AttributeItemOutputTypeDef",
     "AttributeItemTypeDef",
     "AttributeTypesSelectorOutputTypeDef",
     "AttributeTypesSelectorTypeDef",
-    "ConflictResolutionOutputTypeDef",
-    "ConsolidationOutputTypeDef",
     "ConflictResolutionTypeDef",
+    "ConsolidationOutputTypeDef",
     "ConsolidationTypeDef",
-    "RangeOutputTypeDef",
-    "ThresholdOutputTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
-    "CreateEventStreamResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
-    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
-    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
     "EventStreamDestinationDetailsTypeDef",
-    "S3ExportingConfigOutputTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     "GetCalculatedAttributeForProfileRequestRequestTypeDef",
-    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
-    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
-    "ObjectTypeFieldOutputTypeDef",
+    "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyOutputTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetSimilarProfilesRequestRequestTypeDef",
-    "GetSimilarProfilesResponseTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
-    "JobScheduleOutputTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
     "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     "ListCalculatedAttributeForProfileItemTypeDef",
     "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListRuleBasedMatchesRequestRequestTypeDef",
-    "ListRuleBasedMatchesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "MatchingRuleOutputTypeDef",
     "MatchingRuleTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutIntegrationResponseTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
-    "PutProfileObjectResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
+    "AddProfileKeyResponseTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DeleteIntegrationResponseTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
+    "DeleteProfileResponseTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    "GetIntegrationResponseTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MergeProfilesResponseTypeDef",
+    "PutIntegrationResponseTypeDef",
+    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
     "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
     "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
-    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
     "GetEventStreamResponseTypeDef",
-    "ExportingConfigOutputTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "PutProfileObjectTypeRequestRequestTypeDef",
     "TriggerPropertiesTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
+    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
-    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
-    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
-    "MatchingResponseTypeDef",
-    "RuleBasedMatchingResponseTypeDef",
     "MatchingRequestTypeDef",
+    "MatchingResponseTypeDef",
     "RuleBasedMatchingRequestTypeDef",
+    "RuleBasedMatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "TriggerConfigTypeDef",
     "SourceFlowConfigTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "UpdateDomainRequestRequestTypeDef",
     "ListIdentityResolutionJobsResponseTypeDef",
     "FlowDefinitionTypeDef",
     "AppflowIntegrationTypeDef",
     "PutIntegrationRequestRequestTypeDef",
     "IntegrationConfigTypeDef",
     "CreateIntegrationWorkflowRequestRequestTypeDef",
 )
@@ -245,48 +235,33 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
-AddressOutputTypeDef = TypedDict(
-    "AddressOutputTypeDef",
-    {
-        "Address1": str,
-        "Address2": str,
-        "Address3": str,
-        "Address4": str,
-        "City": str,
-        "County": str,
-        "State": str,
-        "Province": str,
-        "Country": str,
-        "PostalCode": str,
-    },
-    total=False,
-)
-
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "Address1": str,
         "Address2": str,
         "Address3": str,
         "Address4": str,
@@ -350,21 +325,14 @@
         "BatchRecordsStartTime": str,
         "BatchRecordsEndTime": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
-AttributeItemOutputTypeDef = TypedDict(
-    "AttributeItemOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -410,42 +378,14 @@
 
 class AttributeTypesSelectorTypeDef(
     _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
 ):
     pass
 
 
-_RequiredConflictResolutionOutputTypeDef = TypedDict(
-    "_RequiredConflictResolutionOutputTypeDef",
-    {
-        "ConflictResolvingModel": ConflictResolvingModelType,
-    },
-)
-_OptionalConflictResolutionOutputTypeDef = TypedDict(
-    "_OptionalConflictResolutionOutputTypeDef",
-    {
-        "SourceName": str,
-    },
-    total=False,
-)
-
-
-class ConflictResolutionOutputTypeDef(
-    _RequiredConflictResolutionOutputTypeDef, _OptionalConflictResolutionOutputTypeDef
-):
-    pass
-
-
-ConsolidationOutputTypeDef = TypedDict(
-    "ConsolidationOutputTypeDef",
-    {
-        "MatchingAttributesList": List[List[str]],
-    },
-)
-
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -459,34 +399,25 @@
 
 class ConflictResolutionTypeDef(
     _RequiredConflictResolutionTypeDef, _OptionalConflictResolutionTypeDef
 ):
     pass
 
 
-ConsolidationTypeDef = TypedDict(
-    "ConsolidationTypeDef",
-    {
-        "MatchingAttributesList": Sequence[Sequence[str]],
-    },
-)
-
-RangeOutputTypeDef = TypedDict(
-    "RangeOutputTypeDef",
+ConsolidationOutputTypeDef = TypedDict(
+    "ConsolidationOutputTypeDef",
     {
-        "Value": int,
-        "Unit": Literal["DAYS"],
+        "MatchingAttributesList": List[List[str]],
     },
 )
 
-ThresholdOutputTypeDef = TypedDict(
-    "ThresholdOutputTypeDef",
+ConsolidationTypeDef = TypedDict(
+    "ConsolidationTypeDef",
     {
-        "Value": str,
-        "Operator": OperatorType,
+        "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Value": int,
@@ -533,40 +464,14 @@
 
 class CreateEventStreamRequestRequestTypeDef(
     _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
 ):
     pass
 
 
-CreateEventStreamResponseTypeDef = TypedDict(
-    "CreateEventStreamResponseTypeDef",
-    {
-        "EventStreamArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -574,22 +479,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEventStreamRequestRequestTypeDef = TypedDict(
     "DeleteEventStreamRequestRequestTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
     },
 )
@@ -598,90 +495,50 @@
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -738,35 +595,14 @@
 
 class EventStreamDestinationDetailsTypeDef(
     _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
 ):
     pass
 
 
-_RequiredS3ExportingConfigOutputTypeDef = TypedDict(
-    "_RequiredS3ExportingConfigOutputTypeDef",
-    {
-        "S3BucketName": str,
-    },
-)
-_OptionalS3ExportingConfigOutputTypeDef = TypedDict(
-    "_OptionalS3ExportingConfigOutputTypeDef",
-    {
-        "S3KeyName": str,
-    },
-    total=False,
-)
-
-
-class S3ExportingConfigOutputTypeDef(
-    _RequiredS3ExportingConfigOutputTypeDef, _OptionalS3ExportingConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalS3ExportingConfigTypeDef = TypedDict(
@@ -826,25 +662,14 @@
     {
         "KeyName": str,
         "Values": List[str],
     },
     total=False,
 )
 
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -854,25 +679,14 @@
     {
         "DomainName": str,
         "ProfileId": str,
         "CalculatedAttributeName": str,
     },
 )
 
-GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    {
-        "CalculatedAttributeName": str,
-        "DisplayName": str,
-        "IsDataPartial": str,
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -906,30 +720,14 @@
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -962,16 +760,16 @@
     "GetProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-ObjectTypeFieldOutputTypeDef = TypedDict(
-    "ObjectTypeFieldOutputTypeDef",
+ObjectTypeFieldTypeDef = TypedDict(
+    "ObjectTypeFieldTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
     total=False,
 )
@@ -1014,27 +812,14 @@
 class GetSimilarProfilesRequestRequestTypeDef(
     _RequiredGetSimilarProfilesRequestRequestTypeDef,
     _OptionalGetSimilarProfilesRequestRequestTypeDef,
 ):
     pass
 
 
-GetSimilarProfilesResponseTypeDef = TypedDict(
-    "GetSimilarProfilesResponseTypeDef",
-    {
-        "ProfileIds": List[str],
-        "MatchId": str,
-        "MatchType": MatchTypeType,
-        "RuleLevel": int,
-        "ConfidenceScore": float,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -1066,22 +851,14 @@
     "IncrementalPullConfigTypeDef",
     {
         "DatetimeTypeFieldName": str,
     },
     total=False,
 )
 
-JobScheduleOutputTypeDef = TypedDict(
-    "JobScheduleOutputTypeDef",
-    {
-        "DayOfTheWeek": JobScheduleDayOfTheWeekType,
-        "Time": str,
-    },
-)
-
 JobScheduleTypeDef = TypedDict(
     "JobScheduleTypeDef",
     {
         "DayOfTheWeek": JobScheduleDayOfTheWeekType,
         "Time": str,
     },
 )
@@ -1235,36 +1012,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
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
 
-
-class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
-    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
-    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventStreamsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
@@ -1432,38 +1197,21 @@
 class ListRuleBasedMatchesRequestRequestTypeDef(
     _RequiredListRuleBasedMatchesRequestRequestTypeDef,
     _OptionalListRuleBasedMatchesRequestRequestTypeDef,
 ):
     pass
 
 
-ListRuleBasedMatchesResponseTypeDef = TypedDict(
-    "ListRuleBasedMatchesResponseTypeDef",
-    {
-        "MatchIds": List[str],
-        "NextToken": str,
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
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "WorkflowId": str,
         "Status": StatusType,
         "StatusDescription": str,
@@ -1515,95 +1263,32 @@
 MatchingRuleTypeDef = TypedDict(
     "MatchingRuleTypeDef",
     {
         "Rule": Sequence[str],
     },
 )
 
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ObjectTypeFieldTypeDef = TypedDict(
-    "ObjectTypeFieldTypeDef",
-    {
-        "Source": str,
-        "Target": str,
-        "ContentType": FieldContentTypeType,
-    },
-    total=False,
-)
-
 ObjectTypeKeyTypeDef = TypedDict(
     "ObjectTypeKeyTypeDef",
     {
         "StandardIdentifiers": Sequence[StandardIdentifierType],
         "FieldNames": Sequence[str],
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
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1712,19 +1397,202 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
+    {
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1816,15 +1684,15 @@
     },
     total=False,
 )
 
 AttributeDetailsOutputTypeDef = TypedDict(
     "AttributeDetailsOutputTypeDef",
     {
-        "Attributes": List[AttributeItemOutputTypeDef],
+        "Attributes": List[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
 AttributeDetailsTypeDef = TypedDict(
     "AttributeDetailsTypeDef",
     {
@@ -1839,15 +1707,15 @@
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingOutputTypeDef = TypedDict(
     "_OptionalAutoMergingOutputTypeDef",
     {
         "Consolidation": ConsolidationOutputTypeDef,
-        "ConflictResolution": ConflictResolutionOutputTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
         "MinAllowedConfidenceScoreForMerging": float,
     },
     total=False,
 )
 
 
 class AutoMergingOutputTypeDef(
@@ -1897,24 +1765,14 @@
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
 
-ConditionsOutputTypeDef = TypedDict(
-    "ConditionsOutputTypeDef",
-    {
-        "Range": RangeOutputTypeDef,
-        "ObjectCount": int,
-        "Threshold": ThresholdOutputTypeDef,
-    },
-    total=False,
-)
-
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdTypeDef,
     },
@@ -1975,24 +1833,16 @@
         "DomainName": str,
         "EventStreamArn": str,
         "CreatedAt": datetime,
         "State": EventStreamStateType,
         "StoppedSince": datetime,
         "DestinationDetails": EventStreamDestinationDetailsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExportingConfigOutputTypeDef = TypedDict(
-    "ExportingConfigOutputTypeDef",
-    {
-        "S3Exporting": S3ExportingConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
     },
@@ -2046,18 +1896,18 @@
         "PhoneNumber": str,
         "MobilePhoneNumber": str,
         "HomePhoneNumber": str,
         "BusinessPhoneNumber": str,
         "EmailAddress": str,
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
-        "Address": AddressOutputTypeDef,
-        "ShippingAddress": AddressOutputTypeDef,
-        "MailingAddress": AddressOutputTypeDef,
-        "BillingAddress": AddressOutputTypeDef,
+        "Address": AddressTypeDef,
+        "ShippingAddress": AddressTypeDef,
+        "MailingAddress": AddressTypeDef,
+        "BillingAddress": AddressTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
         "PartyTypeString": str,
         "GenderString": str,
     },
     total=False,
 )
@@ -2065,139 +1915,161 @@
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
     "ListCalculatedAttributesForProfileResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
+
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2224,15 +2096,15 @@
 
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2334,165 +2206,139 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
+        "DomainName": str,
         "CalculatedAttributeName": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Statistic": StatisticType,
+    },
+)
+_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
         "DisplayName": str,
         "Description": str,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
-        "Conditions": ConditionsOutputTypeDef,
-        "Statistic": StatisticType,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Conditions": ConditionsTypeDef,
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
-GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeDefinitionResponseTypeDef",
+
+class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "Conditions": ConditionsTypeDef,
+        "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
-        "Statistic": StatisticType,
-        "Conditions": ConditionsOutputTypeDef,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
-        "Conditions": ConditionsOutputTypeDef,
+        "Conditions": ConditionsTypeDef,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Statistic": StatisticType,
     },
 )
-_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DisplayName": str,
         "Description": str,
         "Conditions": ConditionsTypeDef,
-        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     {
-        "DomainName": str,
         "CalculatedAttributeName": str,
-    },
-)
-_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
-    {
         "DisplayName": str,
         "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
     {
         "Items": List[EventStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MatchingResponseTypeDef = TypedDict(
-    "MatchingResponseTypeDef",
-    {
-        "Enabled": bool,
-        "JobSchedule": JobScheduleOutputTypeDef,
-        "AutoMerging": AutoMergingOutputTypeDef,
-        "ExportingConfig": ExportingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-RuleBasedMatchingResponseTypeDef = TypedDict(
-    "RuleBasedMatchingResponseTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingRules": List[MatchingRuleOutputTypeDef],
-        "Status": RuleBasedMatchingStatusType,
-        "MaxAllowedRuleLevelForMerging": int,
-        "MaxAllowedRuleLevelForMatching": int,
-        "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
-        "ConflictResolution": ConflictResolutionOutputTypeDef,
-        "ExportingConfig": ExportingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalMatchingRequestTypeDef = TypedDict(
@@ -2506,14 +2352,25 @@
 )
 
 
 class MatchingRequestTypeDef(_RequiredMatchingRequestTypeDef, _OptionalMatchingRequestTypeDef):
     pass
 
 
+MatchingResponseTypeDef = TypedDict(
+    "MatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "JobSchedule": JobScheduleTypeDef,
+        "AutoMerging": AutoMergingOutputTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRuleBasedMatchingRequestTypeDef = TypedDict(
     "_RequiredRuleBasedMatchingRequestTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalRuleBasedMatchingRequestTypeDef = TypedDict(
@@ -2532,29 +2389,44 @@
 
 class RuleBasedMatchingRequestTypeDef(
     _RequiredRuleBasedMatchingRequestTypeDef, _OptionalRuleBasedMatchingRequestTypeDef
 ):
     pass
 
 
+RuleBasedMatchingResponseTypeDef = TypedDict(
+    "RuleBasedMatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingRules": List[MatchingRuleOutputTypeDef],
+        "Status": RuleBasedMatchingStatusType,
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
     {
         "DomainName": str,
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
         "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -2570,15 +2442,15 @@
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -2614,63 +2486,14 @@
 )
 
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Stats": DomainStatsTypeDef,
-        "Matching": MatchingResponseTypeDef,
-        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainResponseTypeDef = TypedDict(
-    "UpdateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
     },
 )
@@ -2715,20 +2538,69 @@
 
 class UpdateDomainRequestRequestTypeDef(
     _RequiredUpdateDomainRequestRequestTypeDef, _OptionalUpdateDomainRequestRequestTypeDef
 ):
     pass
 
 
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Stats": DomainStatsTypeDef,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainResponseTypeDef = TypedDict(
+    "UpdateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.pyi` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,189 +51,179 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "AddProfileKeyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
-    "AttributeItemOutputTypeDef",
     "AttributeItemTypeDef",
     "AttributeTypesSelectorOutputTypeDef",
     "AttributeTypesSelectorTypeDef",
-    "ConflictResolutionOutputTypeDef",
-    "ConsolidationOutputTypeDef",
     "ConflictResolutionTypeDef",
+    "ConsolidationOutputTypeDef",
     "ConsolidationTypeDef",
-    "RangeOutputTypeDef",
-    "ThresholdOutputTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
-    "CreateEventStreamResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
-    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
-    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
     "EventStreamDestinationDetailsTypeDef",
-    "S3ExportingConfigOutputTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     "GetCalculatedAttributeForProfileRequestRequestTypeDef",
-    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
-    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
-    "ObjectTypeFieldOutputTypeDef",
+    "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyOutputTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetSimilarProfilesRequestRequestTypeDef",
-    "GetSimilarProfilesResponseTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
-    "JobScheduleOutputTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
     "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     "ListCalculatedAttributeForProfileItemTypeDef",
     "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListRuleBasedMatchesRequestRequestTypeDef",
-    "ListRuleBasedMatchesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "MatchingRuleOutputTypeDef",
     "MatchingRuleTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutIntegrationResponseTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
-    "PutProfileObjectResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
+    "AddProfileKeyResponseTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DeleteIntegrationResponseTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
+    "DeleteProfileResponseTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    "GetIntegrationResponseTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MergeProfilesResponseTypeDef",
+    "PutIntegrationResponseTypeDef",
+    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
     "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
     "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
-    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
     "GetEventStreamResponseTypeDef",
-    "ExportingConfigOutputTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "PutProfileObjectTypeRequestRequestTypeDef",
     "TriggerPropertiesTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
+    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
-    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
-    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
-    "MatchingResponseTypeDef",
-    "RuleBasedMatchingResponseTypeDef",
     "MatchingRequestTypeDef",
+    "MatchingResponseTypeDef",
     "RuleBasedMatchingRequestTypeDef",
+    "RuleBasedMatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "TriggerConfigTypeDef",
     "SourceFlowConfigTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "UpdateDomainRequestRequestTypeDef",
     "ListIdentityResolutionJobsResponseTypeDef",
     "FlowDefinitionTypeDef",
     "AppflowIntegrationTypeDef",
     "PutIntegrationRequestRequestTypeDef",
     "IntegrationConfigTypeDef",
     "CreateIntegrationWorkflowRequestRequestTypeDef",
 )
@@ -244,48 +234,33 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
-AddressOutputTypeDef = TypedDict(
-    "AddressOutputTypeDef",
-    {
-        "Address1": str,
-        "Address2": str,
-        "Address3": str,
-        "Address4": str,
-        "City": str,
-        "County": str,
-        "State": str,
-        "Province": str,
-        "Country": str,
-        "PostalCode": str,
-    },
-    total=False,
-)
-
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "Address1": str,
         "Address2": str,
         "Address3": str,
         "Address4": str,
@@ -347,21 +322,14 @@
         "BatchRecordsStartTime": str,
         "BatchRecordsEndTime": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
-AttributeItemOutputTypeDef = TypedDict(
-    "AttributeItemOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -403,40 +371,14 @@
 )
 
 class AttributeTypesSelectorTypeDef(
     _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
 ):
     pass
 
-_RequiredConflictResolutionOutputTypeDef = TypedDict(
-    "_RequiredConflictResolutionOutputTypeDef",
-    {
-        "ConflictResolvingModel": ConflictResolvingModelType,
-    },
-)
-_OptionalConflictResolutionOutputTypeDef = TypedDict(
-    "_OptionalConflictResolutionOutputTypeDef",
-    {
-        "SourceName": str,
-    },
-    total=False,
-)
-
-class ConflictResolutionOutputTypeDef(
-    _RequiredConflictResolutionOutputTypeDef, _OptionalConflictResolutionOutputTypeDef
-):
-    pass
-
-ConsolidationOutputTypeDef = TypedDict(
-    "ConsolidationOutputTypeDef",
-    {
-        "MatchingAttributesList": List[List[str]],
-    },
-)
-
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -448,34 +390,25 @@
 )
 
 class ConflictResolutionTypeDef(
     _RequiredConflictResolutionTypeDef, _OptionalConflictResolutionTypeDef
 ):
     pass
 
-ConsolidationTypeDef = TypedDict(
-    "ConsolidationTypeDef",
-    {
-        "MatchingAttributesList": Sequence[Sequence[str]],
-    },
-)
-
-RangeOutputTypeDef = TypedDict(
-    "RangeOutputTypeDef",
+ConsolidationOutputTypeDef = TypedDict(
+    "ConsolidationOutputTypeDef",
     {
-        "Value": int,
-        "Unit": Literal["DAYS"],
+        "MatchingAttributesList": List[List[str]],
     },
 )
 
-ThresholdOutputTypeDef = TypedDict(
-    "ThresholdOutputTypeDef",
+ConsolidationTypeDef = TypedDict(
+    "ConsolidationTypeDef",
     {
-        "Value": str,
-        "Operator": OperatorType,
+        "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Value": int,
@@ -520,40 +453,14 @@
 )
 
 class CreateEventStreamRequestRequestTypeDef(
     _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
 ):
     pass
 
-CreateEventStreamResponseTypeDef = TypedDict(
-    "CreateEventStreamResponseTypeDef",
-    {
-        "EventStreamArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -561,22 +468,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEventStreamRequestRequestTypeDef = TypedDict(
     "DeleteEventStreamRequestRequestTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
     },
 )
@@ -585,90 +484,50 @@
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -721,33 +580,14 @@
 )
 
 class EventStreamDestinationDetailsTypeDef(
     _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
 ):
     pass
 
-_RequiredS3ExportingConfigOutputTypeDef = TypedDict(
-    "_RequiredS3ExportingConfigOutputTypeDef",
-    {
-        "S3BucketName": str,
-    },
-)
-_OptionalS3ExportingConfigOutputTypeDef = TypedDict(
-    "_OptionalS3ExportingConfigOutputTypeDef",
-    {
-        "S3KeyName": str,
-    },
-    total=False,
-)
-
-class S3ExportingConfigOutputTypeDef(
-    _RequiredS3ExportingConfigOutputTypeDef, _OptionalS3ExportingConfigOutputTypeDef
-):
-    pass
-
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalS3ExportingConfigTypeDef = TypedDict(
@@ -805,25 +645,14 @@
     {
         "KeyName": str,
         "Values": List[str],
     },
     total=False,
 )
 
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -833,25 +662,14 @@
     {
         "DomainName": str,
         "ProfileId": str,
         "CalculatedAttributeName": str,
     },
 )
 
-GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    {
-        "CalculatedAttributeName": str,
-        "DisplayName": str,
-        "IsDataPartial": str,
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -885,30 +703,14 @@
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -939,16 +741,16 @@
     "GetProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
-ObjectTypeFieldOutputTypeDef = TypedDict(
-    "ObjectTypeFieldOutputTypeDef",
+ObjectTypeFieldTypeDef = TypedDict(
+    "ObjectTypeFieldTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
     total=False,
 )
@@ -989,27 +791,14 @@
 
 class GetSimilarProfilesRequestRequestTypeDef(
     _RequiredGetSimilarProfilesRequestRequestTypeDef,
     _OptionalGetSimilarProfilesRequestRequestTypeDef,
 ):
     pass
 
-GetSimilarProfilesResponseTypeDef = TypedDict(
-    "GetSimilarProfilesResponseTypeDef",
-    {
-        "ProfileIds": List[str],
-        "MatchId": str,
-        "MatchType": MatchTypeType,
-        "RuleLevel": int,
-        "ConfidenceScore": float,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -1039,22 +828,14 @@
     "IncrementalPullConfigTypeDef",
     {
         "DatetimeTypeFieldName": str,
     },
     total=False,
 )
 
-JobScheduleOutputTypeDef = TypedDict(
-    "JobScheduleOutputTypeDef",
-    {
-        "DayOfTheWeek": JobScheduleDayOfTheWeekType,
-        "Time": str,
-    },
-)
-
 JobScheduleTypeDef = TypedDict(
     "JobScheduleTypeDef",
     {
         "DayOfTheWeek": JobScheduleDayOfTheWeekType,
         "Time": str,
     },
 )
@@ -1198,34 +979,24 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
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
 
-class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
-    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
-    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventStreamsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
@@ -1381,38 +1152,21 @@
 
 class ListRuleBasedMatchesRequestRequestTypeDef(
     _RequiredListRuleBasedMatchesRequestRequestTypeDef,
     _OptionalListRuleBasedMatchesRequestRequestTypeDef,
 ):
     pass
 
-ListRuleBasedMatchesResponseTypeDef = TypedDict(
-    "ListRuleBasedMatchesResponseTypeDef",
-    {
-        "MatchIds": List[str],
-        "NextToken": str,
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
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "WorkflowId": str,
         "Status": StatusType,
         "StatusDescription": str,
@@ -1462,95 +1216,32 @@
 MatchingRuleTypeDef = TypedDict(
     "MatchingRuleTypeDef",
     {
         "Rule": Sequence[str],
     },
 )
 
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ObjectTypeFieldTypeDef = TypedDict(
-    "ObjectTypeFieldTypeDef",
-    {
-        "Source": str,
-        "Target": str,
-        "ContentType": FieldContentTypeType,
-    },
-    total=False,
-)
-
 ObjectTypeKeyTypeDef = TypedDict(
     "ObjectTypeKeyTypeDef",
     {
         "StandardIdentifiers": Sequence[StandardIdentifierType],
         "FieldNames": Sequence[str],
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
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1653,19 +1344,202 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
+    {
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1753,15 +1627,15 @@
     },
     total=False,
 )
 
 AttributeDetailsOutputTypeDef = TypedDict(
     "AttributeDetailsOutputTypeDef",
     {
-        "Attributes": List[AttributeItemOutputTypeDef],
+        "Attributes": List[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
 AttributeDetailsTypeDef = TypedDict(
     "AttributeDetailsTypeDef",
     {
@@ -1776,15 +1650,15 @@
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingOutputTypeDef = TypedDict(
     "_OptionalAutoMergingOutputTypeDef",
     {
         "Consolidation": ConsolidationOutputTypeDef,
-        "ConflictResolution": ConflictResolutionOutputTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
         "MinAllowedConfidenceScoreForMerging": float,
     },
     total=False,
 )
 
 class AutoMergingOutputTypeDef(
     _RequiredAutoMergingOutputTypeDef, _OptionalAutoMergingOutputTypeDef
@@ -1828,24 +1702,14 @@
 
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
-ConditionsOutputTypeDef = TypedDict(
-    "ConditionsOutputTypeDef",
-    {
-        "Range": RangeOutputTypeDef,
-        "ObjectCount": int,
-        "Threshold": ThresholdOutputTypeDef,
-    },
-    total=False,
-)
-
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdTypeDef,
     },
@@ -1902,26 +1766,18 @@
         "DomainName": str,
         "EventStreamArn": str,
         "CreatedAt": datetime,
         "State": EventStreamStateType,
         "StoppedSince": datetime,
         "DestinationDetails": EventStreamDestinationDetailsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExportingConfigOutputTypeDef = TypedDict(
-    "ExportingConfigOutputTypeDef",
-    {
-        "S3Exporting": S3ExportingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
     },
     total=False,
 )
@@ -1971,18 +1827,18 @@
         "PhoneNumber": str,
         "MobilePhoneNumber": str,
         "HomePhoneNumber": str,
         "BusinessPhoneNumber": str,
         "EmailAddress": str,
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
-        "Address": AddressOutputTypeDef,
-        "ShippingAddress": AddressOutputTypeDef,
-        "MailingAddress": AddressOutputTypeDef,
-        "BillingAddress": AddressOutputTypeDef,
+        "Address": AddressTypeDef,
+        "ShippingAddress": AddressTypeDef,
+        "MailingAddress": AddressTypeDef,
+        "BillingAddress": AddressTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
         "PartyTypeString": str,
         "GenderString": str,
     },
     total=False,
 )
@@ -1990,139 +1846,159 @@
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
+        "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
     "ListCalculatedAttributesForProfileResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2147,15 +2023,15 @@
     pass
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2253,159 +2129,133 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
+        "DomainName": str,
         "CalculatedAttributeName": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Statistic": StatisticType,
+    },
+)
+_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
         "DisplayName": str,
         "Description": str,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
-        "Conditions": ConditionsOutputTypeDef,
-        "Statistic": StatisticType,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Conditions": ConditionsTypeDef,
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
-GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeDefinitionResponseTypeDef",
+class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
+CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "Conditions": ConditionsTypeDef,
+        "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
-        "Statistic": StatisticType,
-        "Conditions": ConditionsOutputTypeDef,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
-    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
-        "Conditions": ConditionsOutputTypeDef,
+        "Conditions": ConditionsTypeDef,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
-        "AttributeDetails": AttributeDetailsTypeDef,
-        "Statistic": StatisticType,
     },
 )
-_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DisplayName": str,
         "Description": str,
         "Conditions": ConditionsTypeDef,
-        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     {
-        "DomainName": str,
         "CalculatedAttributeName": str,
-    },
-)
-_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
-    {
         "DisplayName": str,
         "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
+        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
-):
-    pass
-
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
     {
         "Items": List[EventStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MatchingResponseTypeDef = TypedDict(
-    "MatchingResponseTypeDef",
-    {
-        "Enabled": bool,
-        "JobSchedule": JobScheduleOutputTypeDef,
-        "AutoMerging": AutoMergingOutputTypeDef,
-        "ExportingConfig": ExportingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-RuleBasedMatchingResponseTypeDef = TypedDict(
-    "RuleBasedMatchingResponseTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingRules": List[MatchingRuleOutputTypeDef],
-        "Status": RuleBasedMatchingStatusType,
-        "MaxAllowedRuleLevelForMerging": int,
-        "MaxAllowedRuleLevelForMatching": int,
-        "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
-        "ConflictResolution": ConflictResolutionOutputTypeDef,
-        "ExportingConfig": ExportingConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
     },
@@ -2419,14 +2269,25 @@
     },
     total=False,
 )
 
 class MatchingRequestTypeDef(_RequiredMatchingRequestTypeDef, _OptionalMatchingRequestTypeDef):
     pass
 
+MatchingResponseTypeDef = TypedDict(
+    "MatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "JobSchedule": JobScheduleTypeDef,
+        "AutoMerging": AutoMergingOutputTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRuleBasedMatchingRequestTypeDef = TypedDict(
     "_RequiredRuleBasedMatchingRequestTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalRuleBasedMatchingRequestTypeDef = TypedDict(
@@ -2443,29 +2304,44 @@
 )
 
 class RuleBasedMatchingRequestTypeDef(
     _RequiredRuleBasedMatchingRequestTypeDef, _OptionalRuleBasedMatchingRequestTypeDef
 ):
     pass
 
+RuleBasedMatchingResponseTypeDef = TypedDict(
+    "RuleBasedMatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingRules": List[MatchingRuleOutputTypeDef],
+        "Status": RuleBasedMatchingStatusType,
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
     {
         "DomainName": str,
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
         "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -2481,15 +2357,15 @@
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -2521,63 +2397,14 @@
     },
     total=False,
 )
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Stats": DomainStatsTypeDef,
-        "Matching": MatchingResponseTypeDef,
-        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainResponseTypeDef = TypedDict(
-    "UpdateDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DefaultExpirationDays": int,
-        "DefaultEncryptionKey": str,
-        "DeadLetterQueueUrl": str,
-        "Matching": MatchingResponseTypeDef,
-        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
     },
 )
@@ -2618,20 +2445,69 @@
 )
 
 class UpdateDomainRequestRequestTypeDef(
     _RequiredUpdateDomainRequestRequestTypeDef, _OptionalUpdateDomainRequestRequestTypeDef
 ):
     pass
 
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Stats": DomainStatsTypeDef,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainResponseTypeDef = TypedDict(
+    "UpdateDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DefaultExpirationDays": int,
+        "DefaultEncryptionKey": str,
+        "DeadLetterQueueUrl": str,
+        "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.12
-Summary: Type annotations for boto3.CustomerProfiles 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,189 +349,179 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    AddProfileKeyResponseTypeDef,
+    ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
-    AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
-    AttributeItemOutputTypeDef,
     AttributeItemTypeDef,
     AttributeTypesSelectorOutputTypeDef,
     AttributeTypesSelectorTypeDef,
-    ConflictResolutionOutputTypeDef,
-    ConsolidationOutputTypeDef,
     ConflictResolutionTypeDef,
+    ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
-    RangeOutputTypeDef,
-    ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
-    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
-    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
-    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
-    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
-    S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
-    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
-    ObjectTypeFieldOutputTypeDef,
+    ObjectTypeFieldTypeDef,
     ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetSimilarProfilesRequestRequestTypeDef,
-    GetSimilarProfilesResponseTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
-    JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
-    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
-    MergeProfilesResponseTypeDef,
-    ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
-    PaginatorConfigTypeDef,
-    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
-    PutProfileObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
+    AddProfileKeyResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteIntegrationResponseTypeDef,
+    DeleteProfileKeyResponseTypeDef,
+    DeleteProfileObjectResponseTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
+    DeleteProfileResponseTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
+    GetIntegrationResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MergeProfilesResponseTypeDef,
+    PutIntegrationResponseTypeDef,
+    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
-    ConditionsOutputTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
-    ExportingConfigOutputTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
-    UpdateCalculatedAttributeDefinitionResponseTypeDef,
-    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
     ListEventStreamsResponseTypeDef,
-    MatchingResponseTypeDef,
-    RuleBasedMatchingResponseTypeDef,
     MatchingRequestTypeDef,
+    MatchingResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
+    RuleBasedMatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateDomainRequestRequestTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/SOURCES.txt` & `mypy-boto3-customer-profiles-1.28.15/mypy_boto3_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.12/setup.py` & `mypy-boto3-customer-profiles-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-customer-profiles",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CustomerProfiles 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CustomerProfiles 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

