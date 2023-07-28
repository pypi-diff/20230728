# Comparing `tmp/mypy-boto3-sesv2-1.28.12.tar.gz` & `tmp/mypy-boto3-sesv2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sesv2-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
+gzip compressed data, was "mypy-boto3-sesv2-1.28.15.tar", last modified: Fri Jul 28 20:43:45 2023, max compression
```

## Comparing `mypy-boto3-sesv2-1.28.12.tar` & `mypy-boto3-sesv2-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21930 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20451 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56738 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75683 2023-07-27 11:46:56.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75609 2023-07-27 11:46:55.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21930 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21181 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.225885 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56738 2023-07-28 20:39:28.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-28 20:39:28.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-07-28 20:39:28.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70472 2023-07-28 20:39:30.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70402 2023-07-28 20:39:29.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21181 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:45.000000 mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:45.241885 mypy-boto3-sesv2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:39:27.000000 mypy-boto3-sesv2-1.28.15/setup.py
```

### Comparing `mypy-boto3-sesv2-1.28.12/LICENSE` & `mypy-boto3-sesv2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.12/PKG-INFO` & `mypy-boto3-sesv2-1.28.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.28.12
-Summary: Type annotations for boto3.SESV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,102 +340,84 @@
     ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
-    ContactListDestinationOutputTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
-    TopicPreferenceOutputTypeDef,
+    TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
-    TopicPreferenceTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
-    DashboardAttributesOutputTypeDef,
     DashboardAttributesTypeDef,
-    DashboardOptionsOutputTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteContactListRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteCustomVerificationEmailTemplateRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
-    EmailTemplateContentOutputTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    PinpointDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     ReputationOptionsOutputTypeDef,
-    SendingOptionsOutputTypeDef,
     SuppressionOptionsOutputTypeDef,
-    TagOutputTypeDef,
-    TrackingOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
-    TopicOutputTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
-    ImportDataSourceOutputTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
-    GuardianAttributesOutputTypeDef,
     GuardianAttributesTypeDef,
-    GuardianOptionsOutputTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
-    SuppressionListDestinationOutputTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
@@ -490,49 +472,46 @@
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
+    CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateContactListRequestRequestTypeDef,
+    GetContactListResponseTypeDef,
     UpdateContactListRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
+    GetEmailTemplateResponseTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
-    GetEmailTemplateResponseTypeDef,
     ListEmailTemplatesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetContactListResponseTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
-    VdmAttributesOutputTypeDef,
     VdmAttributesTypeDef,
-    VdmOptionsOutputTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
-    ImportDestinationOutputTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
     MessageTypeDef,
@@ -541,20 +520,20 @@
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
-    GetConfigurationSetResponseTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
+    GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
+    CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
-    CreateImportJobRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-sesv2-1.28.12/README.md` & `mypy-boto3-sesv2-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,102 +308,84 @@
     ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
-    ContactListDestinationOutputTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
-    TopicPreferenceOutputTypeDef,
+    TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
-    TopicPreferenceTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
-    DashboardAttributesOutputTypeDef,
     DashboardAttributesTypeDef,
-    DashboardOptionsOutputTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteContactListRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteCustomVerificationEmailTemplateRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
-    EmailTemplateContentOutputTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    PinpointDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     ReputationOptionsOutputTypeDef,
-    SendingOptionsOutputTypeDef,
     SuppressionOptionsOutputTypeDef,
-    TagOutputTypeDef,
-    TrackingOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
-    TopicOutputTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
-    ImportDataSourceOutputTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
-    GuardianAttributesOutputTypeDef,
     GuardianAttributesTypeDef,
-    GuardianOptionsOutputTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
-    SuppressionListDestinationOutputTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
@@ -458,49 +440,46 @@
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
+    CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateContactListRequestRequestTypeDef,
+    GetContactListResponseTypeDef,
     UpdateContactListRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
+    GetEmailTemplateResponseTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
-    GetEmailTemplateResponseTypeDef,
     ListEmailTemplatesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetContactListResponseTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
-    VdmAttributesOutputTypeDef,
     VdmAttributesTypeDef,
-    VdmOptionsOutputTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
-    ImportDestinationOutputTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
     MessageTypeDef,
@@ -509,20 +488,20 @@
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
-    GetConfigurationSetResponseTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
+    GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
+    CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
-    CreateImportJobRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__main__.py` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SESV2 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
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

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.py` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.pyi` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.py` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.pyi` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.py` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -58,115 +58,96 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ReviewDetailsTypeDef",
     "BatchGetMetricDataQueryTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
     "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
-    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
-    "ContactListDestinationOutputTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
-    "TopicPreferenceOutputTypeDef",
+    "TopicPreferenceTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
-    "TopicPreferenceTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
-    "DashboardAttributesOutputTypeDef",
     "DashboardAttributesTypeDef",
-    "DashboardOptionsOutputTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteContactListRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteCustomVerificationEmailTemplateRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
-    "DeliveryOptionsOutputTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
-    "EmailTemplateContentOutputTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "PinpointDestinationOutputTypeDef",
-    "SnsDestinationOutputTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsOutputTypeDef",
-    "SendingOptionsOutputTypeDef",
     "SuppressionOptionsOutputTypeDef",
-    "TagOutputTypeDef",
-    "TrackingOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
-    "TopicOutputTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
-    "ImportDataSourceOutputTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
-    "GuardianAttributesOutputTypeDef",
     "GuardianAttributesTypeDef",
-    "GuardianOptionsOutputTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
-    "SuppressionListDestinationOutputTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
@@ -221,49 +202,46 @@
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
+    "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateContactListRequestRequestTypeDef",
+    "GetContactListResponseTypeDef",
     "UpdateContactListRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
+    "GetEmailTemplateResponseTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
-    "GetEmailTemplateResponseTypeDef",
     "ListEmailTemplatesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetContactListResponseTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
-    "VdmAttributesOutputTypeDef",
     "VdmAttributesTypeDef",
-    "VdmOptionsOutputTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
-    "ImportDestinationOutputTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
     "MessageTypeDef",
@@ -272,20 +250,20 @@
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
-    "GetConfigurationSetResponseTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
+    "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
+    "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
-    "CreateImportJobRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
@@ -318,21 +296,19 @@
     "_OptionalBatchGetMetricDataQueryTypeDef",
     {
         "Dimensions": Mapping[MetricDimensionNameType, str],
     },
     total=False,
 )
 
-
 class BatchGetMetricDataQueryTypeDef(
     _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
 ):
     pass
 
-
 MetricDataErrorTypeDef = TypedDict(
     "MetricDataErrorTypeDef",
     {
         "Id": str,
         "Code": QueryErrorCodeType,
         "Message": str,
     },
@@ -380,19 +356,17 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
-
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
-
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateName": str,
         "TemplateArn": str,
         "TemplateData": str,
     },
@@ -423,40 +397,23 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CloudWatchDimensionConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchDimensionConfigurationOutputTypeDef",
-    {
-        "DimensionName": str,
-        "DimensionValueSource": DimensionValueSourceType,
-        "DefaultDimensionValue": str,
-    },
-)
-
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
     },
 )
 
-ContactListDestinationOutputTypeDef = TypedDict(
-    "ContactListDestinationOutputTypeDef",
-    {
-        "ContactListName": str,
-        "ContactListImportAction": ContactListImportActionType,
-    },
-)
-
 ContactListDestinationTypeDef = TypedDict(
     "ContactListDestinationTypeDef",
     {
         "ContactListName": str,
         "ContactListImportAction": ContactListImportActionType,
     },
 )
@@ -466,16 +423,16 @@
     {
         "ContactListName": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-TopicPreferenceOutputTypeDef = TypedDict(
-    "TopicPreferenceOutputTypeDef",
+TopicPreferenceTypeDef = TypedDict(
+    "TopicPreferenceTypeDef",
     {
         "TopicName": str,
         "SubscriptionStatus": SubscriptionStatusType,
     },
 )
 
 DeliveryOptionsTypeDef = TypedDict(
@@ -539,27 +496,17 @@
     "_OptionalTopicTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class TopicTypeDef(_RequiredTopicTypeDef, _OptionalTopicTypeDef):
     pass
 
-
-TopicPreferenceTypeDef = TypedDict(
-    "TopicPreferenceTypeDef",
-    {
-        "TopicName": str,
-        "SubscriptionStatus": SubscriptionStatusType,
-    },
-)
-
 CreateCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "TemplateContent": str,
@@ -650,38 +597,22 @@
         "SpamRawCount": int,
         "ProjectedInbox": int,
         "ProjectedSpam": int,
     },
     total=False,
 )
 
-DashboardAttributesOutputTypeDef = TypedDict(
-    "DashboardAttributesOutputTypeDef",
-    {
-        "EngagementMetrics": FeatureStatusType,
-    },
-    total=False,
-)
-
 DashboardAttributesTypeDef = TypedDict(
     "DashboardAttributesTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
 
-DashboardOptionsOutputTypeDef = TypedDict(
-    "DashboardOptionsOutputTypeDef",
-    {
-        "EngagementMetrics": FeatureStatusType,
-    },
-    total=False,
-)
-
 DashboardOptionsTypeDef = TypedDict(
     "DashboardOptionsTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
@@ -706,19 +637,17 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
-
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
-
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -797,23 +726,14 @@
         "FromEmailAddress": str,
         "CreateDate": datetime,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
     },
     total=False,
 )
 
-DeliveryOptionsOutputTypeDef = TypedDict(
-    "DeliveryOptionsOutputTypeDef",
-    {
-        "TlsPolicy": TlsPolicyType,
-        "SendingPoolName": str,
-    },
-    total=False,
-)
-
 DomainDeliverabilityCampaignTypeDef = TypedDict(
     "DomainDeliverabilityCampaignTypeDef",
     {
         "CampaignId": str,
         "ImageUrl": str,
         "Subject": str,
         "FromAddress": str,
@@ -852,24 +772,14 @@
 RawMessageTypeDef = TypedDict(
     "RawMessageTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-EmailTemplateContentOutputTypeDef = TypedDict(
-    "EmailTemplateContentOutputTypeDef",
-    {
-        "Subject": str,
-        "Text": str,
-        "Html": str,
-    },
-    total=False,
-)
-
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
@@ -894,37 +804,14 @@
 SnsDestinationTypeDef = TypedDict(
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "DeliveryStreamArn": str,
-    },
-)
-
-PinpointDestinationOutputTypeDef = TypedDict(
-    "PinpointDestinationOutputTypeDef",
-    {
-        "ApplicationArn": str,
-    },
-    total=False,
-)
-
-SnsDestinationOutputTypeDef = TypedDict(
-    "SnsDestinationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "FailedRecordsS3Url": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -974,73 +861,29 @@
     {
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
-SendingOptionsOutputTypeDef = TypedDict(
-    "SendingOptionsOutputTypeDef",
-    {
-        "SendingEnabled": bool,
-    },
-    total=False,
-)
-
 SuppressionOptionsOutputTypeDef = TypedDict(
     "SuppressionOptionsOutputTypeDef",
     {
         "SuppressedReasons": List[SuppressionListReasonType],
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-TrackingOptionsOutputTypeDef = TypedDict(
-    "TrackingOptionsOutputTypeDef",
-    {
-        "CustomRedirectDomain": str,
-    },
-)
-
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
-_RequiredTopicOutputTypeDef = TypedDict(
-    "_RequiredTopicOutputTypeDef",
-    {
-        "TopicName": str,
-        "DisplayName": str,
-        "DefaultSubscriptionStatus": SubscriptionStatusType,
-    },
-)
-_OptionalTopicOutputTypeDef = TypedDict(
-    "_OptionalTopicOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class TopicOutputTypeDef(_RequiredTopicOutputTypeDef, _OptionalTopicOutputTypeDef):
-    pass
-
-
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
     },
 )
@@ -1144,53 +987,29 @@
 GetImportJobRequestRequestTypeDef = TypedDict(
     "GetImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-ImportDataSourceOutputTypeDef = TypedDict(
-    "ImportDataSourceOutputTypeDef",
-    {
-        "S3Url": str,
-        "DataFormat": DataFormatType,
-    },
-)
-
 GetSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "GetSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
-GuardianAttributesOutputTypeDef = TypedDict(
-    "GuardianAttributesOutputTypeDef",
-    {
-        "OptimizedSharedDelivery": FeatureStatusType,
-    },
-    total=False,
-)
-
 GuardianAttributesTypeDef = TypedDict(
     "GuardianAttributesTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
 
-GuardianOptionsOutputTypeDef = TypedDict(
-    "GuardianOptionsOutputTypeDef",
-    {
-        "OptimizedSharedDelivery": FeatureStatusType,
-    },
-    total=False,
-)
-
 GuardianOptionsTypeDef = TypedDict(
     "GuardianOptionsTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
@@ -1202,21 +1021,14 @@
         "IdentityName": str,
         "SendingEnabled": bool,
         "VerificationStatus": VerificationStatusType,
     },
     total=False,
 )
 
-SuppressionListDestinationOutputTypeDef = TypedDict(
-    "SuppressionListDestinationOutputTypeDef",
-    {
-        "SuppressionListImportAction": SuppressionListImportActionType,
-    },
-)
-
 SuppressionListDestinationTypeDef = TypedDict(
     "SuppressionListDestinationTypeDef",
     {
         "SuppressionListImportAction": SuppressionListImportActionType,
     },
 )
 
@@ -1287,22 +1099,20 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
-
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1337,21 +1147,19 @@
     "_OptionalListManagementOptionsTypeDef",
     {
         "TopicName": str,
     },
     total=False,
 )
 
-
 class ListManagementOptionsTypeDef(
     _RequiredListManagementOptionsTypeDef, _OptionalListManagementOptionsTypeDef
 ):
     pass
 
-
 ListRecommendationsRequestRequestTypeDef = TypedDict(
     "ListRecommendationsRequestRequestTypeDef",
     {
         "Filter": Mapping[ListRecommendationsFilterKeyType, str],
         "NextToken": str,
         "PageSize": int,
     },
@@ -1422,21 +1230,19 @@
         "ContactLanguage": ContactLanguageType,
         "AdditionalContactEmailAddresses": Sequence[str],
         "ProductionAccessEnabled": bool,
     },
     total=False,
 )
 
-
 class PutAccountDetailsRequestRequestTypeDef(
     _RequiredPutAccountDetailsRequestRequestTypeDef, _OptionalPutAccountDetailsRequestRequestTypeDef
 ):
     pass
 
-
 PutAccountSendingAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountSendingAttributesRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -1460,110 +1266,100 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "SuppressedReasons": Sequence[SuppressionListReasonType],
     },
     total=False,
 )
 
-
 class PutConfigurationSetSuppressionOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -1594,66 +1390,60 @@
     "_OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -1661,22 +1451,20 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
-
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 PutSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "PutSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
     },
 )
@@ -1700,22 +1488,20 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
-
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
     total=False,
@@ -1908,15 +1694,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CloudWatchDestinationOutputTypeDef = TypedDict(
     "CloudWatchDestinationOutputTypeDef",
     {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1932,37 +1718,81 @@
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicPreferences": List[TopicPreferenceTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
 GetContactResponseTypeDef = TypedDict(
     "GetContactResponseTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicPreferences": List[TopicPreferenceTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 _OptionalCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
@@ -1970,21 +1800,27 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ScalingMode": ScalingModeType,
     },
     total=False,
 )
 
-
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -2002,20 +1838,31 @@
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateContactListRequestRequestTypeDef(
     _RequiredCreateContactListRequestRequestTypeDef, _OptionalCreateContactListRequestRequestTypeDef
 ):
     pass
 
+GetContactListResponseTypeDef = TypedDict(
+    "GetContactListResponseTypeDef",
+    {
+        "ContactListName": str,
+        "Topics": List[TopicTypeDef],
+        "Description": str,
+        "CreatedTimestamp": datetime,
+        "LastUpdatedTimestamp": datetime,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
@@ -2024,69 +1871,19 @@
     {
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateContactListRequestRequestTypeDef(
     _RequiredUpdateContactListRequestRequestTypeDef, _OptionalUpdateContactListRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
@@ -2095,22 +1892,20 @@
         "Tags": Sequence[TagTypeDef],
         "DkimSigningAttributes": DkimSigningAttributesTypeDef,
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "SigningAttributesOrigin": DkimSigningAttributesOriginType,
     },
 )
@@ -2118,22 +1913,20 @@
     "_OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "SigningAttributes": DkimSigningAttributesTypeDef,
     },
     total=False,
 )
 
-
 class PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2144,14 +1937,23 @@
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 
+GetEmailTemplateResponseTypeDef = TypedDict(
+    "GetEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "TemplateContent": EmailTemplateContentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
@@ -2252,53 +2054,23 @@
         "Domain": str,
         "SubscriptionStartDate": Union[datetime, str],
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
-GetEmailTemplateResponseTypeDef = TypedDict(
-    "GetEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "TemplateContent": EmailTemplateContentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactListResponseTypeDef = TypedDict(
-    "GetContactListResponseTypeDef",
-    {
-        "ContactListName": str,
-        "Topics": List[TopicOutputTypeDef],
-        "Description": str,
-        "CreatedTimestamp": datetime,
-        "LastUpdatedTimestamp": datetime,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2309,43 +2081,21 @@
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredVdmAttributesOutputTypeDef = TypedDict(
-    "_RequiredVdmAttributesOutputTypeDef",
-    {
-        "VdmEnabled": FeatureStatusType,
-    },
-)
-_OptionalVdmAttributesOutputTypeDef = TypedDict(
-    "_OptionalVdmAttributesOutputTypeDef",
-    {
-        "DashboardAttributes": DashboardAttributesOutputTypeDef,
-        "GuardianAttributes": GuardianAttributesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VdmAttributesOutputTypeDef(
-    _RequiredVdmAttributesOutputTypeDef, _OptionalVdmAttributesOutputTypeDef
-):
-    pass
-
-
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
     },
 )
 _OptionalVdmAttributesTypeDef = TypedDict(
@@ -2353,28 +2103,17 @@
     {
         "DashboardAttributes": DashboardAttributesTypeDef,
         "GuardianAttributes": GuardianAttributesTypeDef,
     },
     total=False,
 )
 
-
 class VdmAttributesTypeDef(_RequiredVdmAttributesTypeDef, _OptionalVdmAttributesTypeDef):
     pass
 
-
-VdmOptionsOutputTypeDef = TypedDict(
-    "VdmOptionsOutputTypeDef",
-    {
-        "DashboardOptions": DashboardOptionsOutputTypeDef,
-        "GuardianOptions": GuardianOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 VdmOptionsTypeDef = TypedDict(
     "VdmOptionsTypeDef",
     {
         "DashboardOptions": DashboardOptionsTypeDef,
         "GuardianOptions": GuardianOptionsTypeDef,
     },
     total=False,
@@ -2385,23 +2124,14 @@
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportDestinationOutputTypeDef = TypedDict(
-    "ImportDestinationOutputTypeDef",
-    {
-        "SuppressionListDestination": SuppressionListDestinationOutputTypeDef,
-        "ContactListDestination": ContactListDestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
         "ContactListDestination": ContactListDestinationTypeDef,
     },
     total=False,
@@ -2454,21 +2184,19 @@
     "_OptionalSuppressedDestinationTypeDef",
     {
         "Attributes": SuppressedDestinationAttributesTypeDef,
     },
     total=False,
 )
 
-
 class SuppressedDestinationTypeDef(
     _RequiredSuppressedDestinationTypeDef, _OptionalSuppressedDestinationTypeDef
 ):
     pass
 
-
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -2480,27 +2208,25 @@
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SnsDestination": SnsDestinationOutputTypeDef,
-        "PinpointDestination": PinpointDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
-
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
-
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "Enabled": bool,
         "MatchingEventTypes": Sequence[EventTypeType],
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
@@ -2550,71 +2276,54 @@
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
     },
     total=False,
 )
 
-
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
     _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
 ):
     pass
 
-
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
-        "VdmAttributes": VdmAttributesOutputTypeDef,
+        "VdmAttributes": VdmAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
     },
 )
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsOutputTypeDef,
-        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
-        "ReputationOptions": ReputationOptionsOutputTypeDef,
-        "SendingOptions": SendingOptionsOutputTypeDef,
-        "Tags": List[TagOutputTypeDef],
-        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
-        "VdmOptions": VdmOptionsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -2627,21 +2336,34 @@
         "Tags": Sequence[TagTypeDef],
         "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+GetConfigurationSetResponseTypeDef = TypedDict(
+    "GetConfigurationSetResponseTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
+        "SendingOptions": SendingOptionsTypeDef,
+        "Tags": List[TagTypeDef],
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
+        "VdmOptions": VdmOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
@@ -2649,59 +2371,57 @@
     "_OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
-
 class PutConfigurationSetVdmOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef,
 ):
     pass
 
+CreateImportJobRequestRequestTypeDef = TypedDict(
+    "CreateImportJobRequestRequestTypeDef",
+    {
+        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDataSource": ImportDataSourceTypeDef,
+    },
+)
 
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationOutputTypeDef,
-        "ImportDataSource": ImportDataSourceOutputTypeDef,
+        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDataSource": ImportDataSourceTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationOutputTypeDef,
+        "ImportDestination": ImportDestinationTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
     },
     total=False,
 )
 
-CreateImportJobRequestRequestTypeDef = TypedDict(
-    "CreateImportJobRequestRequestTypeDef",
-    {
-        "ImportDestination": ImportDestinationTypeDef,
-        "ImportDataSource": ImportDataSourceTypeDef,
-    },
-)
-
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 _OptionalListContactsRequestRequestTypeDef = TypedDict(
@@ -2710,21 +2430,19 @@
         "Filter": ListContactsFilterTypeDef,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBulkEmailEntryTypeDef = TypedDict(
     "_RequiredBulkEmailEntryTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailEntryTypeDef = TypedDict(
@@ -2732,19 +2450,17 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementEmailContent": ReplacementEmailContentTypeDef,
     },
     total=False,
 )
 
-
 class BulkEmailEntryTypeDef(_RequiredBulkEmailEntryTypeDef, _OptionalBulkEmailEntryTypeDef):
     pass
 
-
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2811,21 +2527,19 @@
         "FeedbackForwardingEmailAddressIdentityArn": str,
         "DefaultEmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendBulkEmailRequestRequestTypeDef(
     _RequiredSendBulkEmailRequestRequestTypeDef, _OptionalSendBulkEmailRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -2834,22 +2548,20 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Content": EmailContentTypeDef,
     },
 )
 _OptionalSendEmailRequestRequestTypeDef = TypedDict(
@@ -2864,12 +2576,11 @@
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "ListManagementOptions": ListManagementOptionsTypeDef,
     },
     total=False,
 )
 
-
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.pyi` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,114 +58,97 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ReviewDetailsTypeDef",
     "BatchGetMetricDataQueryTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
     "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
-    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
-    "ContactListDestinationOutputTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
-    "TopicPreferenceOutputTypeDef",
+    "TopicPreferenceTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
-    "TopicPreferenceTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
-    "DashboardAttributesOutputTypeDef",
     "DashboardAttributesTypeDef",
-    "DashboardOptionsOutputTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteContactListRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteCustomVerificationEmailTemplateRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
-    "DeliveryOptionsOutputTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
-    "EmailTemplateContentOutputTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "PinpointDestinationOutputTypeDef",
-    "SnsDestinationOutputTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsOutputTypeDef",
-    "SendingOptionsOutputTypeDef",
     "SuppressionOptionsOutputTypeDef",
-    "TagOutputTypeDef",
-    "TrackingOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
-    "TopicOutputTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
-    "ImportDataSourceOutputTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
-    "GuardianAttributesOutputTypeDef",
     "GuardianAttributesTypeDef",
-    "GuardianOptionsOutputTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
-    "SuppressionListDestinationOutputTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
@@ -220,49 +203,46 @@
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
+    "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateContactListRequestRequestTypeDef",
+    "GetContactListResponseTypeDef",
     "UpdateContactListRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
+    "GetEmailTemplateResponseTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
-    "GetEmailTemplateResponseTypeDef",
     "ListEmailTemplatesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetContactListResponseTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
-    "VdmAttributesOutputTypeDef",
     "VdmAttributesTypeDef",
-    "VdmOptionsOutputTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
-    "ImportDestinationOutputTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
     "MessageTypeDef",
@@ -271,20 +251,20 @@
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
-    "GetConfigurationSetResponseTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
+    "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
+    "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
-    "CreateImportJobRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
@@ -317,19 +297,21 @@
     "_OptionalBatchGetMetricDataQueryTypeDef",
     {
         "Dimensions": Mapping[MetricDimensionNameType, str],
     },
     total=False,
 )
 
+
 class BatchGetMetricDataQueryTypeDef(
     _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
 ):
     pass
 
+
 MetricDataErrorTypeDef = TypedDict(
     "MetricDataErrorTypeDef",
     {
         "Id": str,
         "Code": QueryErrorCodeType,
         "Message": str,
     },
@@ -377,17 +359,19 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
+
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
+
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateName": str,
         "TemplateArn": str,
         "TemplateData": str,
     },
@@ -418,40 +402,23 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CloudWatchDimensionConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchDimensionConfigurationOutputTypeDef",
-    {
-        "DimensionName": str,
-        "DimensionValueSource": DimensionValueSourceType,
-        "DefaultDimensionValue": str,
-    },
-)
-
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
     },
 )
 
-ContactListDestinationOutputTypeDef = TypedDict(
-    "ContactListDestinationOutputTypeDef",
-    {
-        "ContactListName": str,
-        "ContactListImportAction": ContactListImportActionType,
-    },
-)
-
 ContactListDestinationTypeDef = TypedDict(
     "ContactListDestinationTypeDef",
     {
         "ContactListName": str,
         "ContactListImportAction": ContactListImportActionType,
     },
 )
@@ -461,16 +428,16 @@
     {
         "ContactListName": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-TopicPreferenceOutputTypeDef = TypedDict(
-    "TopicPreferenceOutputTypeDef",
+TopicPreferenceTypeDef = TypedDict(
+    "TopicPreferenceTypeDef",
     {
         "TopicName": str,
         "SubscriptionStatus": SubscriptionStatusType,
     },
 )
 
 DeliveryOptionsTypeDef = TypedDict(
@@ -534,24 +501,18 @@
     "_OptionalTopicTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class TopicTypeDef(_RequiredTopicTypeDef, _OptionalTopicTypeDef):
     pass
 
-TopicPreferenceTypeDef = TypedDict(
-    "TopicPreferenceTypeDef",
-    {
-        "TopicName": str,
-        "SubscriptionStatus": SubscriptionStatusType,
-    },
-)
 
 CreateCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
@@ -643,38 +604,22 @@
         "SpamRawCount": int,
         "ProjectedInbox": int,
         "ProjectedSpam": int,
     },
     total=False,
 )
 
-DashboardAttributesOutputTypeDef = TypedDict(
-    "DashboardAttributesOutputTypeDef",
-    {
-        "EngagementMetrics": FeatureStatusType,
-    },
-    total=False,
-)
-
 DashboardAttributesTypeDef = TypedDict(
     "DashboardAttributesTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
 
-DashboardOptionsOutputTypeDef = TypedDict(
-    "DashboardOptionsOutputTypeDef",
-    {
-        "EngagementMetrics": FeatureStatusType,
-    },
-    total=False,
-)
-
 DashboardOptionsTypeDef = TypedDict(
     "DashboardOptionsTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
@@ -699,17 +644,19 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
+
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
+
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -788,23 +735,14 @@
         "FromEmailAddress": str,
         "CreateDate": datetime,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
     },
     total=False,
 )
 
-DeliveryOptionsOutputTypeDef = TypedDict(
-    "DeliveryOptionsOutputTypeDef",
-    {
-        "TlsPolicy": TlsPolicyType,
-        "SendingPoolName": str,
-    },
-    total=False,
-)
-
 DomainDeliverabilityCampaignTypeDef = TypedDict(
     "DomainDeliverabilityCampaignTypeDef",
     {
         "CampaignId": str,
         "ImageUrl": str,
         "Subject": str,
         "FromAddress": str,
@@ -843,24 +781,14 @@
 RawMessageTypeDef = TypedDict(
     "RawMessageTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-EmailTemplateContentOutputTypeDef = TypedDict(
-    "EmailTemplateContentOutputTypeDef",
-    {
-        "Subject": str,
-        "Text": str,
-        "Html": str,
-    },
-    total=False,
-)
-
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
@@ -885,37 +813,14 @@
 SnsDestinationTypeDef = TypedDict(
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "DeliveryStreamArn": str,
-    },
-)
-
-PinpointDestinationOutputTypeDef = TypedDict(
-    "PinpointDestinationOutputTypeDef",
-    {
-        "ApplicationArn": str,
-    },
-    total=False,
-)
-
-SnsDestinationOutputTypeDef = TypedDict(
-    "SnsDestinationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "FailedRecordsS3Url": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -965,71 +870,29 @@
     {
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
-SendingOptionsOutputTypeDef = TypedDict(
-    "SendingOptionsOutputTypeDef",
-    {
-        "SendingEnabled": bool,
-    },
-    total=False,
-)
-
 SuppressionOptionsOutputTypeDef = TypedDict(
     "SuppressionOptionsOutputTypeDef",
     {
         "SuppressedReasons": List[SuppressionListReasonType],
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-TrackingOptionsOutputTypeDef = TypedDict(
-    "TrackingOptionsOutputTypeDef",
-    {
-        "CustomRedirectDomain": str,
-    },
-)
-
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
-_RequiredTopicOutputTypeDef = TypedDict(
-    "_RequiredTopicOutputTypeDef",
-    {
-        "TopicName": str,
-        "DisplayName": str,
-        "DefaultSubscriptionStatus": SubscriptionStatusType,
-    },
-)
-_OptionalTopicOutputTypeDef = TypedDict(
-    "_OptionalTopicOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class TopicOutputTypeDef(_RequiredTopicOutputTypeDef, _OptionalTopicOutputTypeDef):
-    pass
-
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
     },
 )
@@ -1133,53 +996,29 @@
 GetImportJobRequestRequestTypeDef = TypedDict(
     "GetImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-ImportDataSourceOutputTypeDef = TypedDict(
-    "ImportDataSourceOutputTypeDef",
-    {
-        "S3Url": str,
-        "DataFormat": DataFormatType,
-    },
-)
-
 GetSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "GetSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
-GuardianAttributesOutputTypeDef = TypedDict(
-    "GuardianAttributesOutputTypeDef",
-    {
-        "OptimizedSharedDelivery": FeatureStatusType,
-    },
-    total=False,
-)
-
 GuardianAttributesTypeDef = TypedDict(
     "GuardianAttributesTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
 
-GuardianOptionsOutputTypeDef = TypedDict(
-    "GuardianOptionsOutputTypeDef",
-    {
-        "OptimizedSharedDelivery": FeatureStatusType,
-    },
-    total=False,
-)
-
 GuardianOptionsTypeDef = TypedDict(
     "GuardianOptionsTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
@@ -1191,21 +1030,14 @@
         "IdentityName": str,
         "SendingEnabled": bool,
         "VerificationStatus": VerificationStatusType,
     },
     total=False,
 )
 
-SuppressionListDestinationOutputTypeDef = TypedDict(
-    "SuppressionListDestinationOutputTypeDef",
-    {
-        "SuppressionListImportAction": SuppressionListImportActionType,
-    },
-)
-
 SuppressionListDestinationTypeDef = TypedDict(
     "SuppressionListDestinationTypeDef",
     {
         "SuppressionListImportAction": SuppressionListImportActionType,
     },
 )
 
@@ -1276,20 +1108,22 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
+
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1324,19 +1158,21 @@
     "_OptionalListManagementOptionsTypeDef",
     {
         "TopicName": str,
     },
     total=False,
 )
 
+
 class ListManagementOptionsTypeDef(
     _RequiredListManagementOptionsTypeDef, _OptionalListManagementOptionsTypeDef
 ):
     pass
 
+
 ListRecommendationsRequestRequestTypeDef = TypedDict(
     "ListRecommendationsRequestRequestTypeDef",
     {
         "Filter": Mapping[ListRecommendationsFilterKeyType, str],
         "NextToken": str,
         "PageSize": int,
     },
@@ -1407,19 +1243,21 @@
         "ContactLanguage": ContactLanguageType,
         "AdditionalContactEmailAddresses": Sequence[str],
         "ProductionAccessEnabled": bool,
     },
     total=False,
 )
 
+
 class PutAccountDetailsRequestRequestTypeDef(
     _RequiredPutAccountDetailsRequestRequestTypeDef, _OptionalPutAccountDetailsRequestRequestTypeDef
 ):
     pass
 
+
 PutAccountSendingAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountSendingAttributesRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -1443,100 +1281,110 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "SuppressedReasons": Sequence[SuppressionListReasonType],
     },
     total=False,
 )
 
+
 class PutConfigurationSetSuppressionOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -1567,60 +1415,66 @@
     "_OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -1628,20 +1482,22 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
+
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 PutSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "PutSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
     },
 )
@@ -1665,20 +1521,22 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
+
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
     total=False,
@@ -1871,15 +1729,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CloudWatchDestinationOutputTypeDef = TypedDict(
     "CloudWatchDestinationOutputTypeDef",
     {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1895,37 +1753,85 @@
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicPreferences": List[TopicPreferenceTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
+
 GetContactResponseTypeDef = TypedDict(
     "GetContactResponseTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicPreferences": List[TopicPreferenceTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 _OptionalCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
@@ -1933,20 +1839,30 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ScalingMode": ScalingModeType,
     },
     total=False,
 )
 
+
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1963,19 +1879,34 @@
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateContactListRequestRequestTypeDef(
     _RequiredCreateContactListRequestRequestTypeDef, _OptionalCreateContactListRequestRequestTypeDef
 ):
     pass
 
+
+GetContactListResponseTypeDef = TypedDict(
+    "GetContactListResponseTypeDef",
+    {
+        "ContactListName": str,
+        "Topics": List[TopicTypeDef],
+        "Description": str,
+        "CreatedTimestamp": datetime,
+        "LastUpdatedTimestamp": datetime,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 _OptionalUpdateContactListRequestRequestTypeDef = TypedDict(
@@ -1983,62 +1914,20 @@
     {
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateContactListRequestRequestTypeDef(
     _RequiredUpdateContactListRequestRequestTypeDef, _OptionalUpdateContactListRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
 
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
@@ -2048,20 +1937,22 @@
         "Tags": Sequence[TagTypeDef],
         "DkimSigningAttributes": DkimSigningAttributesTypeDef,
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "SigningAttributesOrigin": DkimSigningAttributesOriginType,
     },
 )
@@ -2069,20 +1960,22 @@
     "_OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "SigningAttributes": DkimSigningAttributesTypeDef,
     },
     total=False,
 )
 
+
 class PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2093,14 +1986,23 @@
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 
+GetEmailTemplateResponseTypeDef = TypedDict(
+    "GetEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "TemplateContent": EmailTemplateContentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
@@ -2201,53 +2103,23 @@
         "Domain": str,
         "SubscriptionStartDate": Union[datetime, str],
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
-GetEmailTemplateResponseTypeDef = TypedDict(
-    "GetEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "TemplateContent": EmailTemplateContentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactListResponseTypeDef = TypedDict(
-    "GetContactListResponseTypeDef",
-    {
-        "ContactListName": str,
-        "Topics": List[TopicOutputTypeDef],
-        "Description": str,
-        "CreatedTimestamp": datetime,
-        "LastUpdatedTimestamp": datetime,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2258,41 +2130,21 @@
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredVdmAttributesOutputTypeDef = TypedDict(
-    "_RequiredVdmAttributesOutputTypeDef",
-    {
-        "VdmEnabled": FeatureStatusType,
-    },
-)
-_OptionalVdmAttributesOutputTypeDef = TypedDict(
-    "_OptionalVdmAttributesOutputTypeDef",
-    {
-        "DashboardAttributes": DashboardAttributesOutputTypeDef,
-        "GuardianAttributes": GuardianAttributesOutputTypeDef,
-    },
-    total=False,
-)
-
-class VdmAttributesOutputTypeDef(
-    _RequiredVdmAttributesOutputTypeDef, _OptionalVdmAttributesOutputTypeDef
-):
-    pass
-
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
     },
 )
 _OptionalVdmAttributesTypeDef = TypedDict(
@@ -2300,25 +2152,18 @@
     {
         "DashboardAttributes": DashboardAttributesTypeDef,
         "GuardianAttributes": GuardianAttributesTypeDef,
     },
     total=False,
 )
 
+
 class VdmAttributesTypeDef(_RequiredVdmAttributesTypeDef, _OptionalVdmAttributesTypeDef):
     pass
 
-VdmOptionsOutputTypeDef = TypedDict(
-    "VdmOptionsOutputTypeDef",
-    {
-        "DashboardOptions": DashboardOptionsOutputTypeDef,
-        "GuardianOptions": GuardianOptionsOutputTypeDef,
-    },
-    total=False,
-)
 
 VdmOptionsTypeDef = TypedDict(
     "VdmOptionsTypeDef",
     {
         "DashboardOptions": DashboardOptionsTypeDef,
         "GuardianOptions": GuardianOptionsTypeDef,
     },
@@ -2330,23 +2175,14 @@
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportDestinationOutputTypeDef = TypedDict(
-    "ImportDestinationOutputTypeDef",
-    {
-        "SuppressionListDestination": SuppressionListDestinationOutputTypeDef,
-        "ContactListDestination": ContactListDestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
         "ContactListDestination": ContactListDestinationTypeDef,
     },
     total=False,
@@ -2399,19 +2235,21 @@
     "_OptionalSuppressedDestinationTypeDef",
     {
         "Attributes": SuppressedDestinationAttributesTypeDef,
     },
     total=False,
 )
 
+
 class SuppressedDestinationTypeDef(
     _RequiredSuppressedDestinationTypeDef, _OptionalSuppressedDestinationTypeDef
 ):
     pass
 
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -2423,25 +2261,27 @@
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SnsDestination": SnsDestinationOutputTypeDef,
-        "PinpointDestination": PinpointDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
+
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
+
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "Enabled": bool,
         "MatchingEventTypes": Sequence[EventTypeType],
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
@@ -2491,69 +2331,56 @@
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
     },
     total=False,
 )
 
+
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
     _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
 ):
     pass
 
+
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
-        "VdmAttributes": VdmAttributesOutputTypeDef,
+        "VdmAttributes": VdmAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
     },
 )
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsOutputTypeDef,
-        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
-        "ReputationOptions": ReputationOptionsOutputTypeDef,
-        "SendingOptions": SendingOptionsOutputTypeDef,
-        "Tags": List[TagOutputTypeDef],
-        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
-        "VdmOptions": VdmOptionsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -2566,77 +2393,96 @@
         "Tags": Sequence[TagTypeDef],
         "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+
+GetConfigurationSetResponseTypeDef = TypedDict(
+    "GetConfigurationSetResponseTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
+        "SendingOptions": SendingOptionsTypeDef,
+        "Tags": List[TagTypeDef],
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
+        "VdmOptions": VdmOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
+
 class PutConfigurationSetVdmOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef,
 ):
     pass
 
+
+CreateImportJobRequestRequestTypeDef = TypedDict(
+    "CreateImportJobRequestRequestTypeDef",
+    {
+        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDataSource": ImportDataSourceTypeDef,
+    },
+)
+
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationOutputTypeDef,
-        "ImportDataSource": ImportDataSourceOutputTypeDef,
+        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDataSource": ImportDataSourceTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationOutputTypeDef,
+        "ImportDestination": ImportDestinationTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
     },
     total=False,
 )
 
-CreateImportJobRequestRequestTypeDef = TypedDict(
-    "CreateImportJobRequestRequestTypeDef",
-    {
-        "ImportDestination": ImportDestinationTypeDef,
-        "ImportDataSource": ImportDataSourceTypeDef,
-    },
-)
-
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 _OptionalListContactsRequestRequestTypeDef = TypedDict(
@@ -2645,19 +2491,21 @@
         "Filter": ListContactsFilterTypeDef,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBulkEmailEntryTypeDef = TypedDict(
     "_RequiredBulkEmailEntryTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailEntryTypeDef = TypedDict(
@@ -2665,17 +2513,19 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementEmailContent": ReplacementEmailContentTypeDef,
     },
     total=False,
 )
 
+
 class BulkEmailEntryTypeDef(_RequiredBulkEmailEntryTypeDef, _OptionalBulkEmailEntryTypeDef):
     pass
 
+
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2742,19 +2592,21 @@
         "FeedbackForwardingEmailAddressIdentityArn": str,
         "DefaultEmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendBulkEmailRequestRequestTypeDef(
     _RequiredSendBulkEmailRequestRequestTypeDef, _OptionalSendBulkEmailRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -2763,20 +2615,22 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Content": EmailContentTypeDef,
     },
 )
 _OptionalSendEmailRequestRequestTypeDef = TypedDict(
@@ -2791,11 +2645,12 @@
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "ListManagementOptions": ListManagementOptionsTypeDef,
     },
     total=False,
 )
 
+
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.28.12
-Summary: Type annotations for boto3.SESV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,102 +340,84 @@
     ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
-    ContactListDestinationOutputTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
-    TopicPreferenceOutputTypeDef,
+    TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
-    TopicPreferenceTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
-    DashboardAttributesOutputTypeDef,
     DashboardAttributesTypeDef,
-    DashboardOptionsOutputTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteContactListRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteCustomVerificationEmailTemplateRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
-    EmailTemplateContentOutputTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    PinpointDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     ReputationOptionsOutputTypeDef,
-    SendingOptionsOutputTypeDef,
     SuppressionOptionsOutputTypeDef,
-    TagOutputTypeDef,
-    TrackingOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
-    TopicOutputTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
-    ImportDataSourceOutputTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
-    GuardianAttributesOutputTypeDef,
     GuardianAttributesTypeDef,
-    GuardianOptionsOutputTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
-    SuppressionListDestinationOutputTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
@@ -490,49 +472,46 @@
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
+    CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateContactListRequestRequestTypeDef,
+    GetContactListResponseTypeDef,
     UpdateContactListRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
+    GetEmailTemplateResponseTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
-    GetEmailTemplateResponseTypeDef,
     ListEmailTemplatesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetContactListResponseTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
-    VdmAttributesOutputTypeDef,
     VdmAttributesTypeDef,
-    VdmOptionsOutputTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
-    ImportDestinationOutputTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
     MessageTypeDef,
@@ -541,20 +520,20 @@
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
-    GetConfigurationSetResponseTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
+    GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
+    CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
-    CreateImportJobRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy-boto3-sesv2-1.28.15/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.12/setup.py` & `mypy-boto3-sesv2-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SESV2 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SESV2 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

