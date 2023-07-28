# Comparing `tmp/mypy-boto3-pinpoint-1.28.12.tar.gz` & `tmp/mypy-boto3-pinpoint-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-1.28.12.tar` & `mypy-boto3-pinpoint-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31664 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-27 11:41:27.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   182450 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   182215 2023-07-27 11:41:30.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31664 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:41:26.000000 mypy-boto3-pinpoint-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28667 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   170188 2023-07-28 19:47:22.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169965 2023-07-28 19:47:20.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 19:47:31.000000 mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.676180 mypy-boto3-pinpoint-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 19:47:17.000000 mypy-boto3-pinpoint-1.28.15/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.28.12/LICENSE` & `mypy-boto3-pinpoint-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.12/PKG-INFO` & `mypy-boto3-pinpoint-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.28.12
-Summary: Type annotations for boto3.Pinpoint 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,74 +329,61 @@
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
     APNSChannelResponseTypeDef,
     APNSMessageTypeDef,
-    APNSPushNotificationTemplateOutputTypeDef,
     APNSPushNotificationTemplateTypeDef,
     APNSSandboxChannelRequestTypeDef,
     APNSSandboxChannelResponseTypeDef,
     APNSVoipChannelRequestTypeDef,
     APNSVoipChannelResponseTypeDef,
     APNSVoipSandboxChannelRequestTypeDef,
     APNSVoipSandboxChannelResponseTypeDef,
     ActivityResponseTypeDef,
-    ContactCenterActivityOutputTypeDef,
-    HoldoutActivityOutputTypeDef,
     ContactCenterActivityTypeDef,
     HoldoutActivityTypeDef,
     AddressConfigurationTypeDef,
-    AndroidPushNotificationTemplateOutputTypeDef,
     AndroidPushNotificationTemplateTypeDef,
     ApplicationResponseTypeDef,
-    CampaignHookOutputTypeDef,
-    CampaignLimitsOutputTypeDef,
-    QuietTimeOutputTypeDef,
+    JourneyTimeframeCapTypeDef,
+    CampaignHookTypeDef,
+    CampaignLimitsTypeDef,
+    QuietTimeTypeDef,
     AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
-    CampaignCustomMessageOutputTypeDef,
     CampaignCustomMessageTypeDef,
-    CampaignEmailMessageOutputTypeDef,
     CampaignEmailMessageTypeDef,
-    CampaignHookTypeDef,
-    CampaignLimitsTypeDef,
     CampaignStateTypeDef,
     CustomDeliveryConfigurationOutputTypeDef,
-    CampaignSmsMessageOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
-    ClosedDaysRuleOutputTypeDef,
     ClosedDaysRuleTypeDef,
-    WaitTimeOutputTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
     ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
     SMSTemplateRequestTypeDef,
     VoiceTemplateRequestTypeDef,
     CustomDeliveryConfigurationTypeDef,
-    JourneyCustomMessageOutputTypeDef,
     JourneyCustomMessageTypeDef,
-    DefaultButtonConfigurationOutputTypeDef,
     DefaultButtonConfigurationTypeDef,
     DefaultMessageTypeDef,
     DefaultPushNotificationMessageTypeDef,
-    DefaultPushNotificationTemplateOutputTypeDef,
     DefaultPushNotificationTemplateTypeDef,
     DeleteAdmChannelRequestRequestTypeDef,
     DeleteApnsChannelRequestRequestTypeDef,
     DeleteApnsSandboxChannelRequestRequestTypeDef,
     DeleteApnsVoipChannelRequestRequestTypeDef,
     DeleteApnsVoipSandboxChannelRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
@@ -423,36 +410,31 @@
     DeleteVoiceChannelRequestRequestTypeDef,
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
-    JourneyEmailMessageOutputTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
-    EndpointDemographicOutputTypeDef,
     EndpointItemResponseTypeDef,
-    EndpointLocationOutputTypeDef,
     EndpointMessageResultTypeDef,
     EndpointUserOutputTypeDef,
     EndpointSendConfigurationTypeDef,
-    MetricDimensionOutputTypeDef,
-    SetDimensionOutputTypeDef,
     MetricDimensionTypeDef,
+    SetDimensionOutputTypeDef,
     SetDimensionTypeDef,
     EventItemResponseTypeDef,
     SessionTypeDef,
     ExportJobResourceTypeDef,
     GCMChannelRequestTypeDef,
-    GPSCoordinatesOutputTypeDef,
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
@@ -502,63 +484,47 @@
     GetSmsTemplateRequestRequestTypeDef,
     SMSTemplateResponseTypeDef,
     GetUserEndpointsRequestRequestTypeDef,
     GetVoiceChannelRequestRequestTypeDef,
     GetVoiceTemplateRequestRequestTypeDef,
     VoiceTemplateResponseTypeDef,
     ImportJobResourceTypeDef,
-    InAppMessageBodyConfigOutputTypeDef,
     InAppMessageBodyConfigTypeDef,
-    OverrideButtonConfigurationOutputTypeDef,
     OverrideButtonConfigurationTypeDef,
-    InAppMessageHeaderConfigOutputTypeDef,
     InAppMessageHeaderConfigTypeDef,
-    JourneyChannelSettingsOutputTypeDef,
     JourneyChannelSettingsTypeDef,
-    JourneyLimitsOutputTypeDef,
-    JourneyLimitsTypeDef,
-    JourneyPushMessageOutputTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
-    JourneySMSMessageOutputTypeDef,
     JourneySMSMessageTypeDef,
     JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
-    MessageOutputTypeDef,
     MessageTypeDef,
     MessageResultTypeDef,
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
-    OpenHoursRuleOutputTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
-    QuietTimeTypeDef,
-    RandomSplitEntryOutputTypeDef,
     RandomSplitEntryTypeDef,
-    RecencyDimensionOutputTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
-    SegmentConditionOutputTypeDef,
     SegmentConditionTypeDef,
-    SegmentReferenceOutputTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
     TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
-    TemplateOutputTypeDef,
     TemplateTypeDef,
     TemplateResponseTypeDef,
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
@@ -566,20 +532,20 @@
     UpdateAdmChannelRequestRequestTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    ApplicationSettingsResourceTypeDef,
+    ApplicationSettingsJourneyLimitsTypeDef,
+    JourneyLimitsTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
-    WaitActivityOutputTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     DeleteAdmChannelResponseTypeDef,
     DeleteApnsChannelResponseTypeDef,
     DeleteApnsSandboxChannelResponseTypeDef,
     DeleteApnsVoipChannelResponseTypeDef,
@@ -618,16 +584,16 @@
     UpdateRecommenderConfigurationResponseTypeDef,
     CreateSmsTemplateRequestRequestTypeDef,
     UpdateSmsTemplateRequestRequestTypeDef,
     CreateVoiceTemplateRequestRequestTypeDef,
     UpdateVoiceTemplateRequestRequestTypeDef,
     CustomMessageActivityOutputTypeDef,
     CustomMessageActivityTypeDef,
-    PushNotificationTemplateResponseTypeDef,
     PushNotificationTemplateRequestTypeDef,
+    PushNotificationTemplateResponseTypeDef,
     DeleteEmailChannelResponseTypeDef,
     GetEmailChannelResponseTypeDef,
     UpdateEmailChannelResponseTypeDef,
     DeleteEmailTemplateResponseTypeDef,
     DeleteInAppTemplateResponseTypeDef,
     DeletePushTemplateResponseTypeDef,
     DeleteSmsTemplateResponseTypeDef,
@@ -649,15 +615,14 @@
     DeleteSmsChannelResponseTypeDef,
     GetSmsChannelResponseTypeDef,
     UpdateSmsChannelResponseTypeDef,
     DeleteVoiceChannelResponseTypeDef,
     GetVoiceChannelResponseTypeDef,
     UpdateVoiceChannelResponseTypeDef,
     UpdateEmailChannelRequestRequestTypeDef,
-    EmailMessageActivityOutputTypeDef,
     EmailMessageActivityTypeDef,
     GetEmailTemplateResponseTypeDef,
     EndpointBatchItemTypeDef,
     EndpointRequestTypeDef,
     PublicEndpointTypeDef,
     SendUsersMessageResponseTypeDef,
     EndpointResponseTypeDef,
@@ -665,67 +630,60 @@
     SegmentDemographicsOutputTypeDef,
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
-    GPSPointDimensionOutputTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
-    InAppMessageButtonOutputTypeDef,
     InAppMessageButtonTypeDef,
-    PushMessageActivityOutputTypeDef,
     PushMessageActivityTypeDef,
     JourneyRunsResponseTypeDef,
-    SMSMessageActivityOutputTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
     OpenHoursOutputTypeDef,
     OpenHoursTypeDef,
     PutEventStreamRequestRequestTypeDef,
-    WriteApplicationSettingsRequestTypeDef,
     RandomSplitActivityOutputTypeDef,
     RandomSplitActivityTypeDef,
-    SegmentBehaviorsOutputTypeDef,
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
-    TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
     VerifyOTPMessageRequestRequestTypeDef,
     GetCampaignActivitiesResponseTypeDef,
     GetAppsResponseTypeDef,
-    GetApplicationSettingsResponseTypeDef,
-    UpdateApplicationSettingsResponseTypeDef,
+    ApplicationSettingsResourceTypeDef,
+    WriteApplicationSettingsRequestTypeDef,
     GetChannelsResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
-    GetPushTemplateResponseTypeDef,
     CreatePushTemplateRequestRequestTypeDef,
     UpdatePushTemplateRequestRequestTypeDef,
+    GetPushTemplateResponseTypeDef,
     EndpointBatchRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     EndpointsResponseTypeDef,
     GetEndpointResponseTypeDef,
     CampaignEventFilterOutputTypeDef,
@@ -740,24 +698,25 @@
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
     SegmentLocationOutputTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
-    InAppMessageContentOutputTypeDef,
     InAppMessageContentTypeDef,
     GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
-    UpdateApplicationSettingsRequestRequestTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
+    GetApplicationSettingsResponseTypeDef,
+    UpdateApplicationSettingsResponseTypeDef,
+    UpdateApplicationSettingsRequestRequestTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
     DeleteUserEndpointsResponseTypeDef,
     GetUserEndpointsResponseTypeDef,
     InAppCampaignScheduleTypeDef,
     ScheduleOutputTypeDef,
     EventStartConditionOutputTypeDef,
     ScheduleTypeDef,
@@ -767,60 +726,60 @@
     GetExportJobsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
     SegmentDimensionsOutputTypeDef,
     SegmentDimensionsTypeDef,
     GetImportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
     CampaignInAppMessageOutputTypeDef,
-    InAppMessageTypeDef,
-    InAppTemplateResponseTypeDef,
     CampaignInAppMessageTypeDef,
+    InAppMessageTypeDef,
     InAppTemplateRequestTypeDef,
+    InAppTemplateResponseTypeDef,
     ApplicationDateRangeKpiResponseTypeDef,
     CampaignDateRangeKpiResponseTypeDef,
     JourneyDateRangeKpiResponseTypeDef,
     DirectMessageConfigurationTypeDef,
     StartConditionOutputTypeDef,
     StartConditionTypeDef,
     PutEventsRequestRequestTypeDef,
     SegmentGroupOutputTypeDef,
     SimpleConditionOutputTypeDef,
     SegmentGroupTypeDef,
     SimpleConditionTypeDef,
     MessageConfigurationOutputTypeDef,
-    InAppMessageCampaignTypeDef,
-    GetInAppTemplateResponseTypeDef,
     MessageConfigurationTypeDef,
+    InAppMessageCampaignTypeDef,
     CreateInAppTemplateRequestRequestTypeDef,
     UpdateInAppTemplateRequestRequestTypeDef,
+    GetInAppTemplateResponseTypeDef,
     GetApplicationDateRangeKpiResponseTypeDef,
     GetCampaignDateRangeKpiResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     MessageRequestTypeDef,
     SendUsersMessageRequestTypeDef,
     SegmentGroupListOutputTypeDef,
     ConditionOutputTypeDef,
     MultiConditionalBranchOutputTypeDef,
     SegmentGroupListTypeDef,
     ConditionTypeDef,
     MultiConditionalBranchTypeDef,
     TreatmentResourceTypeDef,
-    InAppMessagesResponseTypeDef,
     WriteTreatmentResourceTypeDef,
+    InAppMessagesResponseTypeDef,
     SendMessagesRequestRequestTypeDef,
     SendUsersMessagesRequestRequestTypeDef,
     SegmentResponseTypeDef,
     ConditionalSplitActivityOutputTypeDef,
     MultiConditionalSplitActivityOutputTypeDef,
     WriteSegmentRequestTypeDef,
     ConditionalSplitActivityTypeDef,
     MultiConditionalSplitActivityTypeDef,
     CampaignResponseTypeDef,
-    GetInAppMessagesResponseTypeDef,
     WriteCampaignRequestTypeDef,
+    GetInAppMessagesResponseTypeDef,
     CreateSegmentResponseTypeDef,
     DeleteSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentVersionResponseTypeDef,
     SegmentsResponseTypeDef,
     UpdateSegmentResponseTypeDef,
     ActivityOutputTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.28.12/README.md` & `mypy-boto3-pinpoint-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,74 +297,61 @@
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
     APNSChannelResponseTypeDef,
     APNSMessageTypeDef,
-    APNSPushNotificationTemplateOutputTypeDef,
     APNSPushNotificationTemplateTypeDef,
     APNSSandboxChannelRequestTypeDef,
     APNSSandboxChannelResponseTypeDef,
     APNSVoipChannelRequestTypeDef,
     APNSVoipChannelResponseTypeDef,
     APNSVoipSandboxChannelRequestTypeDef,
     APNSVoipSandboxChannelResponseTypeDef,
     ActivityResponseTypeDef,
-    ContactCenterActivityOutputTypeDef,
-    HoldoutActivityOutputTypeDef,
     ContactCenterActivityTypeDef,
     HoldoutActivityTypeDef,
     AddressConfigurationTypeDef,
-    AndroidPushNotificationTemplateOutputTypeDef,
     AndroidPushNotificationTemplateTypeDef,
     ApplicationResponseTypeDef,
-    CampaignHookOutputTypeDef,
-    CampaignLimitsOutputTypeDef,
-    QuietTimeOutputTypeDef,
+    JourneyTimeframeCapTypeDef,
+    CampaignHookTypeDef,
+    CampaignLimitsTypeDef,
+    QuietTimeTypeDef,
     AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
-    CampaignCustomMessageOutputTypeDef,
     CampaignCustomMessageTypeDef,
-    CampaignEmailMessageOutputTypeDef,
     CampaignEmailMessageTypeDef,
-    CampaignHookTypeDef,
-    CampaignLimitsTypeDef,
     CampaignStateTypeDef,
     CustomDeliveryConfigurationOutputTypeDef,
-    CampaignSmsMessageOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
-    ClosedDaysRuleOutputTypeDef,
     ClosedDaysRuleTypeDef,
-    WaitTimeOutputTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
     ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
     SMSTemplateRequestTypeDef,
     VoiceTemplateRequestTypeDef,
     CustomDeliveryConfigurationTypeDef,
-    JourneyCustomMessageOutputTypeDef,
     JourneyCustomMessageTypeDef,
-    DefaultButtonConfigurationOutputTypeDef,
     DefaultButtonConfigurationTypeDef,
     DefaultMessageTypeDef,
     DefaultPushNotificationMessageTypeDef,
-    DefaultPushNotificationTemplateOutputTypeDef,
     DefaultPushNotificationTemplateTypeDef,
     DeleteAdmChannelRequestRequestTypeDef,
     DeleteApnsChannelRequestRequestTypeDef,
     DeleteApnsSandboxChannelRequestRequestTypeDef,
     DeleteApnsVoipChannelRequestRequestTypeDef,
     DeleteApnsVoipSandboxChannelRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
@@ -391,36 +378,31 @@
     DeleteVoiceChannelRequestRequestTypeDef,
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
-    JourneyEmailMessageOutputTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
-    EndpointDemographicOutputTypeDef,
     EndpointItemResponseTypeDef,
-    EndpointLocationOutputTypeDef,
     EndpointMessageResultTypeDef,
     EndpointUserOutputTypeDef,
     EndpointSendConfigurationTypeDef,
-    MetricDimensionOutputTypeDef,
-    SetDimensionOutputTypeDef,
     MetricDimensionTypeDef,
+    SetDimensionOutputTypeDef,
     SetDimensionTypeDef,
     EventItemResponseTypeDef,
     SessionTypeDef,
     ExportJobResourceTypeDef,
     GCMChannelRequestTypeDef,
-    GPSCoordinatesOutputTypeDef,
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
@@ -470,63 +452,47 @@
     GetSmsTemplateRequestRequestTypeDef,
     SMSTemplateResponseTypeDef,
     GetUserEndpointsRequestRequestTypeDef,
     GetVoiceChannelRequestRequestTypeDef,
     GetVoiceTemplateRequestRequestTypeDef,
     VoiceTemplateResponseTypeDef,
     ImportJobResourceTypeDef,
-    InAppMessageBodyConfigOutputTypeDef,
     InAppMessageBodyConfigTypeDef,
-    OverrideButtonConfigurationOutputTypeDef,
     OverrideButtonConfigurationTypeDef,
-    InAppMessageHeaderConfigOutputTypeDef,
     InAppMessageHeaderConfigTypeDef,
-    JourneyChannelSettingsOutputTypeDef,
     JourneyChannelSettingsTypeDef,
-    JourneyLimitsOutputTypeDef,
-    JourneyLimitsTypeDef,
-    JourneyPushMessageOutputTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
-    JourneySMSMessageOutputTypeDef,
     JourneySMSMessageTypeDef,
     JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
-    MessageOutputTypeDef,
     MessageTypeDef,
     MessageResultTypeDef,
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
-    OpenHoursRuleOutputTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
-    QuietTimeTypeDef,
-    RandomSplitEntryOutputTypeDef,
     RandomSplitEntryTypeDef,
-    RecencyDimensionOutputTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
-    SegmentConditionOutputTypeDef,
     SegmentConditionTypeDef,
-    SegmentReferenceOutputTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
     TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
-    TemplateOutputTypeDef,
     TemplateTypeDef,
     TemplateResponseTypeDef,
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
@@ -534,20 +500,20 @@
     UpdateAdmChannelRequestRequestTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    ApplicationSettingsResourceTypeDef,
+    ApplicationSettingsJourneyLimitsTypeDef,
+    JourneyLimitsTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
-    WaitActivityOutputTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     DeleteAdmChannelResponseTypeDef,
     DeleteApnsChannelResponseTypeDef,
     DeleteApnsSandboxChannelResponseTypeDef,
     DeleteApnsVoipChannelResponseTypeDef,
@@ -586,16 +552,16 @@
     UpdateRecommenderConfigurationResponseTypeDef,
     CreateSmsTemplateRequestRequestTypeDef,
     UpdateSmsTemplateRequestRequestTypeDef,
     CreateVoiceTemplateRequestRequestTypeDef,
     UpdateVoiceTemplateRequestRequestTypeDef,
     CustomMessageActivityOutputTypeDef,
     CustomMessageActivityTypeDef,
-    PushNotificationTemplateResponseTypeDef,
     PushNotificationTemplateRequestTypeDef,
+    PushNotificationTemplateResponseTypeDef,
     DeleteEmailChannelResponseTypeDef,
     GetEmailChannelResponseTypeDef,
     UpdateEmailChannelResponseTypeDef,
     DeleteEmailTemplateResponseTypeDef,
     DeleteInAppTemplateResponseTypeDef,
     DeletePushTemplateResponseTypeDef,
     DeleteSmsTemplateResponseTypeDef,
@@ -617,15 +583,14 @@
     DeleteSmsChannelResponseTypeDef,
     GetSmsChannelResponseTypeDef,
     UpdateSmsChannelResponseTypeDef,
     DeleteVoiceChannelResponseTypeDef,
     GetVoiceChannelResponseTypeDef,
     UpdateVoiceChannelResponseTypeDef,
     UpdateEmailChannelRequestRequestTypeDef,
-    EmailMessageActivityOutputTypeDef,
     EmailMessageActivityTypeDef,
     GetEmailTemplateResponseTypeDef,
     EndpointBatchItemTypeDef,
     EndpointRequestTypeDef,
     PublicEndpointTypeDef,
     SendUsersMessageResponseTypeDef,
     EndpointResponseTypeDef,
@@ -633,67 +598,60 @@
     SegmentDemographicsOutputTypeDef,
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
-    GPSPointDimensionOutputTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
-    InAppMessageButtonOutputTypeDef,
     InAppMessageButtonTypeDef,
-    PushMessageActivityOutputTypeDef,
     PushMessageActivityTypeDef,
     JourneyRunsResponseTypeDef,
-    SMSMessageActivityOutputTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
     OpenHoursOutputTypeDef,
     OpenHoursTypeDef,
     PutEventStreamRequestRequestTypeDef,
-    WriteApplicationSettingsRequestTypeDef,
     RandomSplitActivityOutputTypeDef,
     RandomSplitActivityTypeDef,
-    SegmentBehaviorsOutputTypeDef,
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
-    TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
     VerifyOTPMessageRequestRequestTypeDef,
     GetCampaignActivitiesResponseTypeDef,
     GetAppsResponseTypeDef,
-    GetApplicationSettingsResponseTypeDef,
-    UpdateApplicationSettingsResponseTypeDef,
+    ApplicationSettingsResourceTypeDef,
+    WriteApplicationSettingsRequestTypeDef,
     GetChannelsResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
-    GetPushTemplateResponseTypeDef,
     CreatePushTemplateRequestRequestTypeDef,
     UpdatePushTemplateRequestRequestTypeDef,
+    GetPushTemplateResponseTypeDef,
     EndpointBatchRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     EndpointsResponseTypeDef,
     GetEndpointResponseTypeDef,
     CampaignEventFilterOutputTypeDef,
@@ -708,24 +666,25 @@
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
     SegmentLocationOutputTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
-    InAppMessageContentOutputTypeDef,
     InAppMessageContentTypeDef,
     GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
-    UpdateApplicationSettingsRequestRequestTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
+    GetApplicationSettingsResponseTypeDef,
+    UpdateApplicationSettingsResponseTypeDef,
+    UpdateApplicationSettingsRequestRequestTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
     DeleteUserEndpointsResponseTypeDef,
     GetUserEndpointsResponseTypeDef,
     InAppCampaignScheduleTypeDef,
     ScheduleOutputTypeDef,
     EventStartConditionOutputTypeDef,
     ScheduleTypeDef,
@@ -735,60 +694,60 @@
     GetExportJobsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
     SegmentDimensionsOutputTypeDef,
     SegmentDimensionsTypeDef,
     GetImportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
     CampaignInAppMessageOutputTypeDef,
-    InAppMessageTypeDef,
-    InAppTemplateResponseTypeDef,
     CampaignInAppMessageTypeDef,
+    InAppMessageTypeDef,
     InAppTemplateRequestTypeDef,
+    InAppTemplateResponseTypeDef,
     ApplicationDateRangeKpiResponseTypeDef,
     CampaignDateRangeKpiResponseTypeDef,
     JourneyDateRangeKpiResponseTypeDef,
     DirectMessageConfigurationTypeDef,
     StartConditionOutputTypeDef,
     StartConditionTypeDef,
     PutEventsRequestRequestTypeDef,
     SegmentGroupOutputTypeDef,
     SimpleConditionOutputTypeDef,
     SegmentGroupTypeDef,
     SimpleConditionTypeDef,
     MessageConfigurationOutputTypeDef,
-    InAppMessageCampaignTypeDef,
-    GetInAppTemplateResponseTypeDef,
     MessageConfigurationTypeDef,
+    InAppMessageCampaignTypeDef,
     CreateInAppTemplateRequestRequestTypeDef,
     UpdateInAppTemplateRequestRequestTypeDef,
+    GetInAppTemplateResponseTypeDef,
     GetApplicationDateRangeKpiResponseTypeDef,
     GetCampaignDateRangeKpiResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     MessageRequestTypeDef,
     SendUsersMessageRequestTypeDef,
     SegmentGroupListOutputTypeDef,
     ConditionOutputTypeDef,
     MultiConditionalBranchOutputTypeDef,
     SegmentGroupListTypeDef,
     ConditionTypeDef,
     MultiConditionalBranchTypeDef,
     TreatmentResourceTypeDef,
-    InAppMessagesResponseTypeDef,
     WriteTreatmentResourceTypeDef,
+    InAppMessagesResponseTypeDef,
     SendMessagesRequestRequestTypeDef,
     SendUsersMessagesRequestRequestTypeDef,
     SegmentResponseTypeDef,
     ConditionalSplitActivityOutputTypeDef,
     MultiConditionalSplitActivityOutputTypeDef,
     WriteSegmentRequestTypeDef,
     ConditionalSplitActivityTypeDef,
     MultiConditionalSplitActivityTypeDef,
     CampaignResponseTypeDef,
-    GetInAppMessagesResponseTypeDef,
     WriteCampaignRequestTypeDef,
+    GetInAppMessagesResponseTypeDef,
     CreateSegmentResponseTypeDef,
     DeleteSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentVersionResponseTypeDef,
     SegmentsResponseTypeDef,
     UpdateSegmentResponseTypeDef,
     ActivityOutputTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Pinpoint 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
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

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,74 +57,61 @@
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
-    "APNSPushNotificationTemplateOutputTypeDef",
     "APNSPushNotificationTemplateTypeDef",
     "APNSSandboxChannelRequestTypeDef",
     "APNSSandboxChannelResponseTypeDef",
     "APNSVoipChannelRequestTypeDef",
     "APNSVoipChannelResponseTypeDef",
     "APNSVoipSandboxChannelRequestTypeDef",
     "APNSVoipSandboxChannelResponseTypeDef",
     "ActivityResponseTypeDef",
-    "ContactCenterActivityOutputTypeDef",
-    "HoldoutActivityOutputTypeDef",
     "ContactCenterActivityTypeDef",
     "HoldoutActivityTypeDef",
     "AddressConfigurationTypeDef",
-    "AndroidPushNotificationTemplateOutputTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
-    "CampaignHookOutputTypeDef",
-    "CampaignLimitsOutputTypeDef",
-    "QuietTimeOutputTypeDef",
+    "JourneyTimeframeCapTypeDef",
+    "CampaignHookTypeDef",
+    "CampaignLimitsTypeDef",
+    "QuietTimeTypeDef",
     "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
-    "CampaignCustomMessageOutputTypeDef",
     "CampaignCustomMessageTypeDef",
-    "CampaignEmailMessageOutputTypeDef",
     "CampaignEmailMessageTypeDef",
-    "CampaignHookTypeDef",
-    "CampaignLimitsTypeDef",
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationOutputTypeDef",
-    "CampaignSmsMessageOutputTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
-    "ClosedDaysRuleOutputTypeDef",
     "ClosedDaysRuleTypeDef",
-    "WaitTimeOutputTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
     "CustomDeliveryConfigurationTypeDef",
-    "JourneyCustomMessageOutputTypeDef",
     "JourneyCustomMessageTypeDef",
-    "DefaultButtonConfigurationOutputTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
-    "DefaultPushNotificationTemplateOutputTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
     "DeleteApnsSandboxChannelRequestRequestTypeDef",
     "DeleteApnsVoipChannelRequestRequestTypeDef",
     "DeleteApnsVoipSandboxChannelRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
@@ -151,36 +138,31 @@
     "DeleteVoiceChannelRequestRequestTypeDef",
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
-    "JourneyEmailMessageOutputTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
-    "EndpointDemographicOutputTypeDef",
     "EndpointItemResponseTypeDef",
-    "EndpointLocationOutputTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
-    "MetricDimensionOutputTypeDef",
-    "SetDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
+    "SetDimensionOutputTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
-    "GPSCoordinatesOutputTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
     "GetApnsChannelRequestRequestTypeDef",
     "GetApnsSandboxChannelRequestRequestTypeDef",
     "GetApnsVoipChannelRequestRequestTypeDef",
     "GetApnsVoipSandboxChannelRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
@@ -230,63 +212,47 @@
     "GetSmsTemplateRequestRequestTypeDef",
     "SMSTemplateResponseTypeDef",
     "GetUserEndpointsRequestRequestTypeDef",
     "GetVoiceChannelRequestRequestTypeDef",
     "GetVoiceTemplateRequestRequestTypeDef",
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
-    "InAppMessageBodyConfigOutputTypeDef",
     "InAppMessageBodyConfigTypeDef",
-    "OverrideButtonConfigurationOutputTypeDef",
     "OverrideButtonConfigurationTypeDef",
-    "InAppMessageHeaderConfigOutputTypeDef",
     "InAppMessageHeaderConfigTypeDef",
-    "JourneyChannelSettingsOutputTypeDef",
     "JourneyChannelSettingsTypeDef",
-    "JourneyLimitsOutputTypeDef",
-    "JourneyLimitsTypeDef",
-    "JourneyPushMessageOutputTypeDef",
     "JourneyPushMessageTypeDef",
     "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
-    "JourneySMSMessageOutputTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyScheduleTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagsModelOutputTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
-    "MessageOutputTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
-    "OpenHoursRuleOutputTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
-    "QuietTimeTypeDef",
-    "RandomSplitEntryOutputTypeDef",
     "RandomSplitEntryTypeDef",
-    "RecencyDimensionOutputTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
-    "SegmentConditionOutputTypeDef",
     "SegmentConditionTypeDef",
-    "SegmentReferenceOutputTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
     "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
-    "TemplateOutputTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
@@ -294,20 +260,20 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "ApplicationSettingsResourceTypeDef",
+    "ApplicationSettingsJourneyLimitsTypeDef",
+    "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
-    "WaitActivityOutputTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
     "DeleteApnsChannelResponseTypeDef",
     "DeleteApnsSandboxChannelResponseTypeDef",
     "DeleteApnsVoipChannelResponseTypeDef",
@@ -346,16 +312,16 @@
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
     "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
-    "PushNotificationTemplateResponseTypeDef",
     "PushNotificationTemplateRequestTypeDef",
+    "PushNotificationTemplateResponseTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
     "DeleteInAppTemplateResponseTypeDef",
     "DeletePushTemplateResponseTypeDef",
     "DeleteSmsTemplateResponseTypeDef",
@@ -377,15 +343,14 @@
     "DeleteSmsChannelResponseTypeDef",
     "GetSmsChannelResponseTypeDef",
     "UpdateSmsChannelResponseTypeDef",
     "DeleteVoiceChannelResponseTypeDef",
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
-    "EmailMessageActivityOutputTypeDef",
     "EmailMessageActivityTypeDef",
     "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
     "EndpointResponseTypeDef",
@@ -393,67 +358,60 @@
     "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
-    "GPSPointDimensionOutputTypeDef",
     "GPSPointDimensionTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
-    "InAppMessageButtonOutputTypeDef",
     "InAppMessageButtonTypeDef",
-    "PushMessageActivityOutputTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
-    "SMSMessageActivityOutputTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
     "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
-    "WriteApplicationSettingsRequestTypeDef",
     "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
-    "SegmentBehaviorsOutputTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
-    "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
-    "GetApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsResponseTypeDef",
+    "ApplicationSettingsResourceTypeDef",
+    "WriteApplicationSettingsRequestTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
-    "GetPushTemplateResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
+    "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
     "CampaignEventFilterOutputTypeDef",
@@ -468,24 +426,25 @@
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
     "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
-    "InAppMessageContentOutputTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
-    "UpdateApplicationSettingsRequestRequestTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
+    "GetApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsRequestRequestTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
     "ScheduleOutputTypeDef",
     "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
@@ -495,60 +454,60 @@
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
     "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
     "CampaignInAppMessageOutputTypeDef",
-    "InAppMessageTypeDef",
-    "InAppTemplateResponseTypeDef",
     "CampaignInAppMessageTypeDef",
+    "InAppMessageTypeDef",
     "InAppTemplateRequestTypeDef",
+    "InAppTemplateResponseTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
     "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
     "SegmentGroupOutputTypeDef",
     "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
     "MessageConfigurationOutputTypeDef",
-    "InAppMessageCampaignTypeDef",
-    "GetInAppTemplateResponseTypeDef",
     "MessageConfigurationTypeDef",
+    "InAppMessageCampaignTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
+    "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
     "SegmentGroupListOutputTypeDef",
     "ConditionOutputTypeDef",
     "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
-    "InAppMessagesResponseTypeDef",
     "WriteTreatmentResourceTypeDef",
+    "InAppMessagesResponseTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
     "ConditionalSplitActivityOutputTypeDef",
     "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
-    "GetInAppMessagesResponseTypeDef",
     "WriteCampaignRequestTypeDef",
+    "GetInAppMessagesResponseTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
     "ActivityOutputTypeDef",
@@ -721,28 +680,14 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
-APNSPushNotificationTemplateOutputTypeDef = TypedDict(
-    "APNSPushNotificationTemplateOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "MediaUrl": str,
-        "RawContent": str,
-        "Sound": str,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 APNSPushNotificationTemplateTypeDef = TypedDict(
     "APNSPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "MediaUrl": str,
         "RawContent": str,
@@ -918,43 +863,14 @@
 )
 
 
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
 
-ContactCenterActivityOutputTypeDef = TypedDict(
-    "ContactCenterActivityOutputTypeDef",
-    {
-        "NextActivity": str,
-    },
-    total=False,
-)
-
-_RequiredHoldoutActivityOutputTypeDef = TypedDict(
-    "_RequiredHoldoutActivityOutputTypeDef",
-    {
-        "Percentage": int,
-    },
-)
-_OptionalHoldoutActivityOutputTypeDef = TypedDict(
-    "_OptionalHoldoutActivityOutputTypeDef",
-    {
-        "NextActivity": str,
-    },
-    total=False,
-)
-
-
-class HoldoutActivityOutputTypeDef(
-    _RequiredHoldoutActivityOutputTypeDef, _OptionalHoldoutActivityOutputTypeDef
-):
-    pass
-
-
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
@@ -987,30 +903,14 @@
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
-AndroidPushNotificationTemplateOutputTypeDef = TypedDict(
-    "AndroidPushNotificationTemplateOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "ImageIconUrl": str,
-        "ImageUrl": str,
-        "RawContent": str,
-        "SmallImageIconUrl": str,
-        "Sound": str,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 AndroidPushNotificationTemplateTypeDef = TypedDict(
     "AndroidPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
@@ -1043,38 +943,47 @@
 
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
 
-CampaignHookOutputTypeDef = TypedDict(
-    "CampaignHookOutputTypeDef",
+JourneyTimeframeCapTypeDef = TypedDict(
+    "JourneyTimeframeCapTypeDef",
+    {
+        "Cap": int,
+        "Days": int,
+    },
+    total=False,
+)
+
+CampaignHookTypeDef = TypedDict(
+    "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
     total=False,
 )
 
-CampaignLimitsOutputTypeDef = TypedDict(
-    "CampaignLimitsOutputTypeDef",
+CampaignLimitsTypeDef = TypedDict(
+    "CampaignLimitsTypeDef",
     {
         "Daily": int,
         "MaximumDuration": int,
         "MessagesPerSecond": int,
         "Total": int,
         "Session": int,
     },
     total=False,
 )
 
-QuietTimeOutputTypeDef = TypedDict(
-    "QuietTimeOutputTypeDef",
+QuietTimeTypeDef = TypedDict(
+    "QuietTimeTypeDef",
     {
         "End": str,
         "Start": str,
     },
     total=False,
 )
 
@@ -1211,74 +1120,33 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
-CampaignCustomMessageOutputTypeDef = TypedDict(
-    "CampaignCustomMessageOutputTypeDef",
-    {
-        "Data": str,
-    },
-    total=False,
-)
-
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
-CampaignEmailMessageOutputTypeDef = TypedDict(
-    "CampaignEmailMessageOutputTypeDef",
-    {
-        "Body": str,
-        "FromAddress": str,
-        "HtmlBody": str,
-        "Title": str,
-    },
-    total=False,
-)
-
 CampaignEmailMessageTypeDef = TypedDict(
     "CampaignEmailMessageTypeDef",
     {
         "Body": str,
         "FromAddress": str,
         "HtmlBody": str,
         "Title": str,
     },
     total=False,
 )
 
-CampaignHookTypeDef = TypedDict(
-    "CampaignHookTypeDef",
-    {
-        "LambdaFunctionName": str,
-        "Mode": ModeType,
-        "WebUrl": str,
-    },
-    total=False,
-)
-
-CampaignLimitsTypeDef = TypedDict(
-    "CampaignLimitsTypeDef",
-    {
-        "Daily": int,
-        "MaximumDuration": int,
-        "MessagesPerSecond": int,
-        "Total": int,
-        "Session": int,
-    },
-    total=False,
-)
-
 CampaignStateTypeDef = TypedDict(
     "CampaignStateTypeDef",
     {
         "CampaignStatus": CampaignStatusType,
     },
     total=False,
 )
@@ -1301,27 +1169,14 @@
 class CustomDeliveryConfigurationOutputTypeDef(
     _RequiredCustomDeliveryConfigurationOutputTypeDef,
     _OptionalCustomDeliveryConfigurationOutputTypeDef,
 ):
     pass
 
 
-CampaignSmsMessageOutputTypeDef = TypedDict(
-    "CampaignSmsMessageOutputTypeDef",
-    {
-        "Body": str,
-        "MessageType": MessageTypeType,
-        "OriginationNumber": str,
-        "SenderId": str,
-        "EntityId": str,
-        "TemplateId": str,
-    },
-    total=False,
-)
-
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
@@ -1343,43 +1198,24 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-ClosedDaysRuleOutputTypeDef = TypedDict(
-    "ClosedDaysRuleOutputTypeDef",
-    {
-        "Name": str,
-        "StartDateTime": str,
-        "EndDateTime": str,
-    },
-    total=False,
-)
-
 ClosedDaysRuleTypeDef = TypedDict(
     "ClosedDaysRuleTypeDef",
     {
         "Name": str,
         "StartDateTime": str,
         "EndDateTime": str,
     },
     total=False,
 )
 
-WaitTimeOutputTypeDef = TypedDict(
-    "WaitTimeOutputTypeDef",
-    {
-        "WaitFor": str,
-        "WaitUntil": str,
-    },
-    total=False,
-)
-
 WaitTimeTypeDef = TypedDict(
     "WaitTimeTypeDef",
     {
         "WaitFor": str,
         "WaitUntil": str,
     },
     total=False,
@@ -1599,56 +1435,22 @@
 
 class CustomDeliveryConfigurationTypeDef(
     _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
 
-JourneyCustomMessageOutputTypeDef = TypedDict(
-    "JourneyCustomMessageOutputTypeDef",
-    {
-        "Data": str,
-    },
-    total=False,
-)
-
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
-_RequiredDefaultButtonConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDefaultButtonConfigurationOutputTypeDef",
-    {
-        "ButtonAction": ButtonActionType,
-        "Text": str,
-    },
-)
-_OptionalDefaultButtonConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDefaultButtonConfigurationOutputTypeDef",
-    {
-        "BackgroundColor": str,
-        "BorderRadius": int,
-        "Link": str,
-        "TextColor": str,
-    },
-    total=False,
-)
-
-
-class DefaultButtonConfigurationOutputTypeDef(
-    _RequiredDefaultButtonConfigurationOutputTypeDef,
-    _OptionalDefaultButtonConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredDefaultButtonConfigurationTypeDef = TypedDict(
     "_RequiredDefaultButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
         "Text": str,
     },
 )
@@ -1689,26 +1491,14 @@
         "Substitutions": Mapping[str, Sequence[str]],
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
-DefaultPushNotificationTemplateOutputTypeDef = TypedDict(
-    "DefaultPushNotificationTemplateOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "Sound": str,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 DefaultPushNotificationTemplateTypeDef = TypedDict(
     "DefaultPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Sound": str,
         "Title": str,
@@ -1890,25 +1680,27 @@
         "ApplicationId": str,
     },
 )
 
 _RequiredGCMChannelResponseTypeDef = TypedDict(
     "_RequiredGCMChannelResponseTypeDef",
     {
-        "Credential": str,
         "Platform": str,
     },
 )
 _OptionalGCMChannelResponseTypeDef = TypedDict(
     "_OptionalGCMChannelResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
+        "Credential": str,
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
         "HasCredential": bool,
+        "HasFcmServiceCredentials": bool,
         "Id": str,
         "IsArchived": bool,
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
@@ -2121,14 +1913,15 @@
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
         "IconReference": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
+        "PreferredAuthenticationMethod": str,
         "Priority": str,
         "RawContent": str,
         "RestrictedPackageName": str,
         "SilentPush": bool,
         "SmallImageIconUrl": str,
         "Sound": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -2187,22 +1980,14 @@
 
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
 
-JourneyEmailMessageOutputTypeDef = TypedDict(
-    "JourneyEmailMessageOutputTypeDef",
-    {
-        "FromAddress": str,
-    },
-    total=False,
-)
-
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
@@ -2280,51 +2065,23 @@
     {
         "UserAttributes": Mapping[str, Sequence[str]],
         "UserId": str,
     },
     total=False,
 )
 
-EndpointDemographicOutputTypeDef = TypedDict(
-    "EndpointDemographicOutputTypeDef",
-    {
-        "AppVersion": str,
-        "Locale": str,
-        "Make": str,
-        "Model": str,
-        "ModelVersion": str,
-        "Platform": str,
-        "PlatformVersion": str,
-        "Timezone": str,
-    },
-    total=False,
-)
-
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
 )
 
-EndpointLocationOutputTypeDef = TypedDict(
-    "EndpointLocationOutputTypeDef",
-    {
-        "City": str,
-        "Country": str,
-        "Latitude": float,
-        "Longitude": float,
-        "PostalCode": str,
-        "Region": str,
-    },
-    total=False,
-)
-
 _RequiredEndpointMessageResultTypeDef = TypedDict(
     "_RequiredEndpointMessageResultTypeDef",
     {
         "DeliveryStatus": DeliveryStatusType,
         "StatusCode": int,
     },
 )
@@ -2363,16 +2120,16 @@
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
+MetricDimensionTypeDef = TypedDict(
+    "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
 
 _RequiredSetDimensionOutputTypeDef = TypedDict(
@@ -2392,22 +2149,14 @@
 
 class SetDimensionOutputTypeDef(
     _RequiredSetDimensionOutputTypeDef, _OptionalSetDimensionOutputTypeDef
 ):
     pass
 
 
-MetricDimensionTypeDef = TypedDict(
-    "MetricDimensionTypeDef",
-    {
-        "ComparisonOperator": str,
-        "Value": float,
-    },
-)
-
 _RequiredSetDimensionTypeDef = TypedDict(
     "_RequiredSetDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalSetDimensionTypeDef = TypedDict(
@@ -2472,43 +2221,25 @@
 
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
 
-_RequiredGCMChannelRequestTypeDef = TypedDict(
-    "_RequiredGCMChannelRequestTypeDef",
+GCMChannelRequestTypeDef = TypedDict(
+    "GCMChannelRequestTypeDef",
     {
         "ApiKey": str,
-    },
-)
-_OptionalGCMChannelRequestTypeDef = TypedDict(
-    "_OptionalGCMChannelRequestTypeDef",
-    {
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
+        "ServiceJson": str,
     },
     total=False,
 )
 
-
-class GCMChannelRequestTypeDef(
-    _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
-):
-    pass
-
-
-GPSCoordinatesOutputTypeDef = TypedDict(
-    "GPSCoordinatesOutputTypeDef",
-    {
-        "Latitude": float,
-        "Longitude": float,
-    },
-)
-
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -3364,54 +3095,23 @@
 
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
 
-InAppMessageBodyConfigOutputTypeDef = TypedDict(
-    "InAppMessageBodyConfigOutputTypeDef",
-    {
-        "Alignment": AlignmentType,
-        "Body": str,
-        "TextColor": str,
-    },
-)
-
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
 )
 
-_RequiredOverrideButtonConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOverrideButtonConfigurationOutputTypeDef",
-    {
-        "ButtonAction": ButtonActionType,
-    },
-)
-_OptionalOverrideButtonConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOverrideButtonConfigurationOutputTypeDef",
-    {
-        "Link": str,
-    },
-    total=False,
-)
-
-
-class OverrideButtonConfigurationOutputTypeDef(
-    _RequiredOverrideButtonConfigurationOutputTypeDef,
-    _OptionalOverrideButtonConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredOverrideButtonConfigurationTypeDef = TypedDict(
     "_RequiredOverrideButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
     },
 )
 _OptionalOverrideButtonConfigurationTypeDef = TypedDict(
@@ -3425,80 +3125,32 @@
 
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
 
-InAppMessageHeaderConfigOutputTypeDef = TypedDict(
-    "InAppMessageHeaderConfigOutputTypeDef",
-    {
-        "Alignment": AlignmentType,
-        "Header": str,
-        "TextColor": str,
-    },
-)
-
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
 )
 
-JourneyChannelSettingsOutputTypeDef = TypedDict(
-    "JourneyChannelSettingsOutputTypeDef",
-    {
-        "ConnectCampaignArn": str,
-        "ConnectCampaignExecutionRoleArn": str,
-    },
-    total=False,
-)
-
 JourneyChannelSettingsTypeDef = TypedDict(
     "JourneyChannelSettingsTypeDef",
     {
         "ConnectCampaignArn": str,
         "ConnectCampaignExecutionRoleArn": str,
     },
     total=False,
 )
 
-JourneyLimitsOutputTypeDef = TypedDict(
-    "JourneyLimitsOutputTypeDef",
-    {
-        "DailyCap": int,
-        "EndpointReentryCap": int,
-        "MessagesPerSecond": int,
-        "EndpointReentryInterval": str,
-    },
-    total=False,
-)
-
-JourneyLimitsTypeDef = TypedDict(
-    "JourneyLimitsTypeDef",
-    {
-        "DailyCap": int,
-        "EndpointReentryCap": int,
-        "MessagesPerSecond": int,
-        "EndpointReentryInterval": str,
-    },
-    total=False,
-)
-
-JourneyPushMessageOutputTypeDef = TypedDict(
-    "JourneyPushMessageOutputTypeDef",
-    {
-        "TimeToLive": str,
-    },
-    total=False,
-)
-
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": str,
     },
     total=False,
 )
@@ -3519,26 +3171,14 @@
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
     },
 )
 
-JourneySMSMessageOutputTypeDef = TypedDict(
-    "JourneySMSMessageOutputTypeDef",
-    {
-        "MessageType": MessageTypeType,
-        "OriginationNumber": str,
-        "SenderId": str,
-        "EntityId": str,
-        "TemplateId": str,
-    },
-    total=False,
-)
-
 JourneySMSMessageTypeDef = TypedDict(
     "JourneySMSMessageTypeDef",
     {
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
         "EntityId": str,
@@ -3632,33 +3272,14 @@
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
     },
     total=False,
 )
 
-MessageOutputTypeDef = TypedDict(
-    "MessageOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "ImageIconUrl": str,
-        "ImageSmallIconUrl": str,
-        "ImageUrl": str,
-        "JsonBody": str,
-        "MediaUrl": str,
-        "RawContent": str,
-        "SilentPush": bool,
-        "TimeToLive": int,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageSmallIconUrl": str,
@@ -3722,23 +3343,14 @@
         "PhoneTypeCode": int,
         "Timezone": str,
         "ZipCode": str,
     },
     total=False,
 )
 
-OpenHoursRuleOutputTypeDef = TypedDict(
-    "OpenHoursRuleOutputTypeDef",
-    {
-        "StartTime": str,
-        "EndTime": str,
-    },
-    total=False,
-)
-
 OpenHoursRuleTypeDef = TypedDict(
     "OpenHoursRuleTypeDef",
     {
         "StartTime": str,
         "EndTime": str,
     },
     total=False,
@@ -3748,49 +3360,23 @@
     "WriteEventStreamTypeDef",
     {
         "DestinationStreamArn": str,
         "RoleArn": str,
     },
 )
 
-QuietTimeTypeDef = TypedDict(
-    "QuietTimeTypeDef",
-    {
-        "End": str,
-        "Start": str,
-    },
-    total=False,
-)
-
-RandomSplitEntryOutputTypeDef = TypedDict(
-    "RandomSplitEntryOutputTypeDef",
-    {
-        "NextActivity": str,
-        "Percentage": int,
-    },
-    total=False,
-)
-
 RandomSplitEntryTypeDef = TypedDict(
     "RandomSplitEntryTypeDef",
     {
         "NextActivity": str,
         "Percentage": int,
     },
     total=False,
 )
 
-RecencyDimensionOutputTypeDef = TypedDict(
-    "RecencyDimensionOutputTypeDef",
-    {
-        "Duration": DurationType,
-        "RecencyType": RecencyTypeType,
-    },
-)
-
 RecencyDimensionTypeDef = TypedDict(
     "RecencyDimensionTypeDef",
     {
         "Duration": DurationType,
         "RecencyType": RecencyTypeType,
     },
 )
@@ -3818,49 +3404,21 @@
         "Enabled": bool,
         "SenderId": str,
         "ShortCode": str,
     },
     total=False,
 )
 
-SegmentConditionOutputTypeDef = TypedDict(
-    "SegmentConditionOutputTypeDef",
-    {
-        "SegmentId": str,
-    },
-)
-
 SegmentConditionTypeDef = TypedDict(
     "SegmentConditionTypeDef",
     {
         "SegmentId": str,
     },
 )
 
-_RequiredSegmentReferenceOutputTypeDef = TypedDict(
-    "_RequiredSegmentReferenceOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalSegmentReferenceOutputTypeDef = TypedDict(
-    "_OptionalSegmentReferenceOutputTypeDef",
-    {
-        "Version": int,
-    },
-    total=False,
-)
-
-
-class SegmentReferenceOutputTypeDef(
-    _RequiredSegmentReferenceOutputTypeDef, _OptionalSegmentReferenceOutputTypeDef
-):
-    pass
-
-
 _RequiredSegmentReferenceTypeDef = TypedDict(
     "_RequiredSegmentReferenceTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalSegmentReferenceTypeDef = TypedDict(
@@ -3951,23 +3509,14 @@
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-TemplateOutputTypeDef = TypedDict(
-    "TemplateOutputTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -4152,38 +3701,37 @@
     {
         "Item": List[ApplicationResponseTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+ApplicationSettingsJourneyLimitsTypeDef = TypedDict(
+    "ApplicationSettingsJourneyLimitsTypeDef",
     {
-        "ApplicationId": str,
+        "DailyCap": int,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
+    total=False,
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+JourneyLimitsTypeDef = TypedDict(
+    "JourneyLimitsTypeDef",
     {
-        "CampaignHook": CampaignHookOutputTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsOutputTypeDef,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "DailyCap": int,
+        "EndpointReentryCap": int,
+        "MessagesPerSecond": int,
+        "EndpointReentryInterval": str,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
     total=False,
 )
 
-
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
-
 UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
     "UpdateBaiduChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
@@ -4194,19 +3742,19 @@
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
 ClosedDaysOutputTypeDef = TypedDict(
     "ClosedDaysOutputTypeDef",
     {
-        "EMAIL": List[ClosedDaysRuleOutputTypeDef],
-        "SMS": List[ClosedDaysRuleOutputTypeDef],
-        "PUSH": List[ClosedDaysRuleOutputTypeDef],
-        "VOICE": List[ClosedDaysRuleOutputTypeDef],
-        "CUSTOM": List[ClosedDaysRuleOutputTypeDef],
+        "EMAIL": List[ClosedDaysRuleTypeDef],
+        "SMS": List[ClosedDaysRuleTypeDef],
+        "PUSH": List[ClosedDaysRuleTypeDef],
+        "VOICE": List[ClosedDaysRuleTypeDef],
+        "CUSTOM": List[ClosedDaysRuleTypeDef],
     },
     total=False,
 )
 
 ClosedDaysTypeDef = TypedDict(
     "ClosedDaysTypeDef",
     {
@@ -4215,23 +3763,14 @@
         "PUSH": Sequence[ClosedDaysRuleTypeDef],
         "VOICE": Sequence[ClosedDaysRuleTypeDef],
         "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
     total=False,
 )
 
-WaitActivityOutputTypeDef = TypedDict(
-    "WaitActivityOutputTypeDef",
-    {
-        "NextActivity": str,
-        "WaitTime": WaitTimeOutputTypeDef,
-    },
-    total=False,
-)
-
 WaitActivityTypeDef = TypedDict(
     "WaitActivityTypeDef",
     {
         "NextActivity": str,
         "WaitTime": WaitTimeTypeDef,
     },
     total=False,
@@ -4640,15 +4179,15 @@
 
 
 CustomMessageActivityOutputTypeDef = TypedDict(
     "CustomMessageActivityOutputTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": List[EndpointTypesElementType],
-        "MessageConfig": JourneyCustomMessageOutputTypeDef,
+        "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
@@ -4661,33 +4200,49 @@
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
+PushNotificationTemplateRequestTypeDef = TypedDict(
+    "PushNotificationTemplateRequestTypeDef",
+    {
+        "ADM": AndroidPushNotificationTemplateTypeDef,
+        "APNS": APNSPushNotificationTemplateTypeDef,
+        "Baidu": AndroidPushNotificationTemplateTypeDef,
+        "Default": DefaultPushNotificationTemplateTypeDef,
+        "DefaultSubstitutions": str,
+        "GCM": AndroidPushNotificationTemplateTypeDef,
+        "RecommenderId": str,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
+
 _RequiredPushNotificationTemplateResponseTypeDef = TypedDict(
     "_RequiredPushNotificationTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalPushNotificationTemplateResponseTypeDef = TypedDict(
     "_OptionalPushNotificationTemplateResponseTypeDef",
     {
-        "ADM": AndroidPushNotificationTemplateOutputTypeDef,
-        "APNS": APNSPushNotificationTemplateOutputTypeDef,
+        "ADM": AndroidPushNotificationTemplateTypeDef,
+        "APNS": APNSPushNotificationTemplateTypeDef,
         "Arn": str,
-        "Baidu": AndroidPushNotificationTemplateOutputTypeDef,
-        "Default": DefaultPushNotificationTemplateOutputTypeDef,
+        "Baidu": AndroidPushNotificationTemplateTypeDef,
+        "Default": DefaultPushNotificationTemplateTypeDef,
         "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateOutputTypeDef,
+        "GCM": AndroidPushNotificationTemplateTypeDef,
         "RecommenderId": str,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
@@ -4696,30 +4251,14 @@
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
 
-PushNotificationTemplateRequestTypeDef = TypedDict(
-    "PushNotificationTemplateRequestTypeDef",
-    {
-        "ADM": AndroidPushNotificationTemplateTypeDef,
-        "APNS": APNSPushNotificationTemplateTypeDef,
-        "Baidu": AndroidPushNotificationTemplateTypeDef,
-        "Default": DefaultPushNotificationTemplateTypeDef,
-        "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateTypeDef,
-        "RecommenderId": str,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
-    },
-    total=False,
-)
-
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4944,25 +4483,14 @@
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EmailChannelRequest": EmailChannelRequestTypeDef,
     },
 )
 
-EmailMessageActivityOutputTypeDef = TypedDict(
-    "EmailMessageActivityOutputTypeDef",
-    {
-        "MessageConfig": JourneyEmailMessageOutputTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 EmailMessageActivityTypeDef = TypedDict(
     "EmailMessageActivityTypeDef",
     {
         "MessageConfig": JourneyEmailMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -5060,33 +4588,33 @@
     {
         "Address": str,
         "ApplicationId": str,
         "Attributes": Dict[str, List[str]],
         "ChannelType": ChannelTypeType,
         "CohortId": str,
         "CreationDate": str,
-        "Demographic": EndpointDemographicOutputTypeDef,
+        "Demographic": EndpointDemographicTypeDef,
         "EffectiveDate": str,
         "EndpointStatus": str,
         "Id": str,
-        "Location": EndpointLocationOutputTypeDef,
+        "Location": EndpointLocationTypeDef,
         "Metrics": Dict[str, float],
         "OptOut": str,
         "RequestId": str,
         "User": EndpointUserOutputTypeDef,
     },
     total=False,
 )
 
 EventDimensionsOutputTypeDef = TypedDict(
     "EventDimensionsOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
         "EventType": SetDimensionOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+        "Metrics": Dict[str, MetricDimensionTypeDef],
     },
     total=False,
 )
 
 SegmentDemographicsOutputTypeDef = TypedDict(
     "SegmentDemographicsOutputTypeDef",
     {
@@ -5195,35 +4723,14 @@
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
 
-_RequiredGPSPointDimensionOutputTypeDef = TypedDict(
-    "_RequiredGPSPointDimensionOutputTypeDef",
-    {
-        "Coordinates": GPSCoordinatesOutputTypeDef,
-    },
-)
-_OptionalGPSPointDimensionOutputTypeDef = TypedDict(
-    "_OptionalGPSPointDimensionOutputTypeDef",
-    {
-        "RangeInKilometers": float,
-    },
-    total=False,
-)
-
-
-class GPSPointDimensionOutputTypeDef(
-    _RequiredGPSPointDimensionOutputTypeDef, _OptionalGPSPointDimensionOutputTypeDef
-):
-    pass
-
-
 _RequiredGPSPointDimensionTypeDef = TypedDict(
     "_RequiredGPSPointDimensionTypeDef",
     {
         "Coordinates": GPSCoordinatesTypeDef,
     },
 )
 _OptionalGPSPointDimensionTypeDef = TypedDict(
@@ -5319,47 +4826,25 @@
 
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
 
-InAppMessageButtonOutputTypeDef = TypedDict(
-    "InAppMessageButtonOutputTypeDef",
-    {
-        "Android": OverrideButtonConfigurationOutputTypeDef,
-        "DefaultConfig": DefaultButtonConfigurationOutputTypeDef,
-        "IOS": OverrideButtonConfigurationOutputTypeDef,
-        "Web": OverrideButtonConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
     },
     total=False,
 )
 
-PushMessageActivityOutputTypeDef = TypedDict(
-    "PushMessageActivityOutputTypeDef",
-    {
-        "MessageConfig": JourneyPushMessageOutputTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 PushMessageActivityTypeDef = TypedDict(
     "PushMessageActivityTypeDef",
     {
         "MessageConfig": JourneyPushMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -5384,25 +4869,14 @@
 
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
 
-SMSMessageActivityOutputTypeDef = TypedDict(
-    "SMSMessageActivityOutputTypeDef",
-    {
-        "MessageConfig": JourneySMSMessageOutputTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -5462,19 +4936,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenHoursOutputTypeDef = TypedDict(
     "OpenHoursOutputTypeDef",
     {
-        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
     },
     total=False,
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
@@ -5491,50 +4965,30 @@
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
 
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
-    {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
-    },
-    total=False,
-)
-
 RandomSplitActivityOutputTypeDef = TypedDict(
     "RandomSplitActivityOutputTypeDef",
     {
-        "Branches": List[RandomSplitEntryOutputTypeDef],
+        "Branches": List[RandomSplitEntryTypeDef],
     },
     total=False,
 )
 
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": Sequence[RandomSplitEntryTypeDef],
     },
     total=False,
 )
 
-SegmentBehaviorsOutputTypeDef = TypedDict(
-    "SegmentBehaviorsOutputTypeDef",
-    {
-        "Recency": RecencyDimensionOutputTypeDef,
-    },
-    total=False,
-)
-
 SegmentBehaviorsTypeDef = TypedDict(
     "SegmentBehaviorsTypeDef",
     {
         "Recency": RecencyDimensionTypeDef,
     },
     total=False,
 )
@@ -5595,32 +5049,22 @@
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
 )
 
-TemplateConfigurationOutputTypeDef = TypedDict(
-    "TemplateConfigurationOutputTypeDef",
-    {
-        "EmailTemplate": TemplateOutputTypeDef,
-        "PushTemplate": TemplateOutputTypeDef,
-        "SMSTemplate": TemplateOutputTypeDef,
-        "VoiceTemplate": TemplateOutputTypeDef,
-    },
-    total=False,
-)
-
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "EmailTemplate": TemplateTypeDef,
         "PushTemplate": TemplateTypeDef,
         "SMSTemplate": TemplateTypeDef,
         "VoiceTemplate": TemplateTypeDef,
+        "InAppTemplate": TemplateTypeDef,
     },
     total=False,
 )
 
 _RequiredTemplatesResponseTypeDef = TypedDict(
     "_RequiredTemplatesResponseTypeDef",
     {
@@ -5709,28 +5153,50 @@
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationSettingsResponseTypeDef = TypedDict(
-    "GetApplicationSettingsResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
+    },
+)
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
+    {
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
-UpdateApplicationSettingsResponseTypeDef = TypedDict(
-    "UpdateApplicationSettingsResponseTypeDef",
+
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5741,22 +5207,14 @@
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPushTemplateResponseTypeDef = TypedDict(
-    "GetPushTemplateResponseTypeDef",
-    {
-        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
         "TemplateName": str,
     },
 )
@@ -5781,14 +5239,22 @@
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+GetPushTemplateResponseTypeDef = TypedDict(
+    "GetPushTemplateResponseTypeDef",
+    {
+        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
     },
 )
 
@@ -5935,15 +5401,15 @@
     },
 )
 
 SegmentLocationOutputTypeDef = TypedDict(
     "SegmentLocationOutputTypeDef",
     {
         "Country": SetDimensionOutputTypeDef,
-        "GPSPoint": GPSPointDimensionOutputTypeDef,
+        "GPSPoint": GPSPointDimensionTypeDef,
     },
     total=False,
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
@@ -5986,27 +5452,14 @@
 
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
 
-InAppMessageContentOutputTypeDef = TypedDict(
-    "InAppMessageContentOutputTypeDef",
-    {
-        "BackgroundColor": str,
-        "BodyConfig": InAppMessageBodyConfigOutputTypeDef,
-        "HeaderConfig": InAppMessageHeaderConfigOutputTypeDef,
-        "ImageUrl": str,
-        "PrimaryBtn": InAppMessageButtonOutputTypeDef,
-        "SecondaryBtn": InAppMessageButtonOutputTypeDef,
-    },
-    total=False,
-)
-
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
         "ImageUrl": str,
@@ -6036,22 +5489,14 @@
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationSettingsRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
-    },
-)
-
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
     },
 )
 
@@ -6081,14 +5526,38 @@
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetApplicationSettingsResponseTypeDef = TypedDict(
+    "GetApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsResponseTypeDef = TypedDict(
+    "UpdateApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationSettingsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+    },
+)
+
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointBatchRequest": EndpointBatchRequestTypeDef,
     },
 )
@@ -6110,15 +5579,15 @@
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
         "EventFilter": CampaignEventFilterOutputTypeDef,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
     total=False,
 )
 
 _RequiredScheduleOutputTypeDef = TypedDict(
     "_RequiredScheduleOutputTypeDef",
     {
@@ -6128,15 +5597,15 @@
 _OptionalScheduleOutputTypeDef = TypedDict(
     "_OptionalScheduleOutputTypeDef",
     {
         "EndTime": str,
         "EventFilter": CampaignEventFilterOutputTypeDef,
         "Frequency": FrequencyType,
         "IsLocalTime": bool,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
 
 class ScheduleOutputTypeDef(_RequiredScheduleOutputTypeDef, _OptionalScheduleOutputTypeDef):
@@ -6216,18 +5685,18 @@
     },
 )
 
 SegmentDimensionsOutputTypeDef = TypedDict(
     "SegmentDimensionsOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
-        "Behavior": SegmentBehaviorsOutputTypeDef,
+        "Behavior": SegmentBehaviorsTypeDef,
         "Demographic": SegmentDemographicsOutputTypeDef,
         "Location": SegmentLocationOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+        "Metrics": Dict[str, MetricDimensionTypeDef],
         "UserAttributes": Dict[str, AttributeDimensionOutputTypeDef],
     },
     total=False,
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
@@ -6258,45 +5727,68 @@
     },
 )
 
 CampaignInAppMessageOutputTypeDef = TypedDict(
     "CampaignInAppMessageOutputTypeDef",
     {
         "Body": str,
-        "Content": List[InAppMessageContentOutputTypeDef],
+        "Content": List[InAppMessageContentTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
+CampaignInAppMessageTypeDef = TypedDict(
+    "CampaignInAppMessageTypeDef",
+    {
+        "Body": str,
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+    },
+    total=False,
+)
+
 InAppMessageTypeDef = TypedDict(
     "InAppMessageTypeDef",
     {
-        "Content": List[InAppMessageContentOutputTypeDef],
+        "Content": List[InAppMessageContentTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
+InAppTemplateRequestTypeDef = TypedDict(
+    "InAppTemplateRequestTypeDef",
+    {
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
+
 _RequiredInAppTemplateResponseTypeDef = TypedDict(
     "_RequiredInAppTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalInAppTemplateResponseTypeDef = TypedDict(
     "_OptionalInAppTemplateResponseTypeDef",
     {
         "Arn": str,
-        "Content": List[InAppMessageContentOutputTypeDef],
+        "Content": List[InAppMessageContentTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
@@ -6305,37 +5797,14 @@
 
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
 
-CampaignInAppMessageTypeDef = TypedDict(
-    "CampaignInAppMessageTypeDef",
-    {
-        "Body": str,
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
-        "Layout": LayoutType,
-    },
-    total=False,
-)
-
-InAppTemplateRequestTypeDef = TypedDict(
-    "InAppTemplateRequestTypeDef",
-    {
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
-        "Layout": LayoutType,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
-    },
-    total=False,
-)
-
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
         "KpiResult": BaseKpiResultTypeDef,
@@ -6426,15 +5895,15 @@
 )
 
 StartConditionOutputTypeDef = TypedDict(
     "StartConditionOutputTypeDef",
     {
         "Description": str,
         "EventStartCondition": EventStartConditionOutputTypeDef,
-        "SegmentStartCondition": SegmentConditionOutputTypeDef,
+        "SegmentStartCondition": SegmentConditionTypeDef,
     },
     total=False,
 )
 
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
@@ -6453,26 +5922,26 @@
     },
 )
 
 SegmentGroupOutputTypeDef = TypedDict(
     "SegmentGroupOutputTypeDef",
     {
         "Dimensions": List[SegmentDimensionsOutputTypeDef],
-        "SourceSegments": List[SegmentReferenceOutputTypeDef],
+        "SourceSegments": List[SegmentReferenceTypeDef],
         "SourceType": SourceTypeType,
         "Type": TypeType,
     },
     total=False,
 )
 
 SimpleConditionOutputTypeDef = TypedDict(
     "SimpleConditionOutputTypeDef",
     {
         "EventCondition": EventConditionOutputTypeDef,
-        "SegmentCondition": SegmentConditionOutputTypeDef,
+        "SegmentCondition": SegmentConditionTypeDef,
         "SegmentDimensions": SegmentDimensionsOutputTypeDef,
     },
     total=False,
 )
 
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
@@ -6494,50 +5963,27 @@
     },
     total=False,
 )
 
 MessageConfigurationOutputTypeDef = TypedDict(
     "MessageConfigurationOutputTypeDef",
     {
-        "ADMMessage": MessageOutputTypeDef,
-        "APNSMessage": MessageOutputTypeDef,
-        "BaiduMessage": MessageOutputTypeDef,
-        "CustomMessage": CampaignCustomMessageOutputTypeDef,
-        "DefaultMessage": MessageOutputTypeDef,
-        "EmailMessage": CampaignEmailMessageOutputTypeDef,
-        "GCMMessage": MessageOutputTypeDef,
-        "SMSMessage": CampaignSmsMessageOutputTypeDef,
+        "ADMMessage": MessageTypeDef,
+        "APNSMessage": MessageTypeDef,
+        "BaiduMessage": MessageTypeDef,
+        "CustomMessage": CampaignCustomMessageTypeDef,
+        "DefaultMessage": MessageTypeDef,
+        "EmailMessage": CampaignEmailMessageTypeDef,
+        "GCMMessage": MessageTypeDef,
+        "SMSMessage": CampaignSmsMessageTypeDef,
         "InAppMessage": CampaignInAppMessageOutputTypeDef,
     },
     total=False,
 )
 
-InAppMessageCampaignTypeDef = TypedDict(
-    "InAppMessageCampaignTypeDef",
-    {
-        "CampaignId": str,
-        "DailyCap": int,
-        "InAppMessage": InAppMessageTypeDef,
-        "Priority": int,
-        "Schedule": InAppCampaignScheduleTypeDef,
-        "SessionCap": int,
-        "TotalCap": int,
-        "TreatmentId": str,
-    },
-    total=False,
-)
-
-GetInAppTemplateResponseTypeDef = TypedDict(
-    "GetInAppTemplateResponseTypeDef",
-    {
-        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MessageConfigurationTypeDef = TypedDict(
     "MessageConfigurationTypeDef",
     {
         "ADMMessage": MessageTypeDef,
         "APNSMessage": MessageTypeDef,
         "BaiduMessage": MessageTypeDef,
         "CustomMessage": CampaignCustomMessageTypeDef,
@@ -6546,14 +5992,29 @@
         "GCMMessage": MessageTypeDef,
         "SMSMessage": CampaignSmsMessageTypeDef,
         "InAppMessage": CampaignInAppMessageTypeDef,
     },
     total=False,
 )
 
+InAppMessageCampaignTypeDef = TypedDict(
+    "InAppMessageCampaignTypeDef",
+    {
+        "CampaignId": str,
+        "DailyCap": int,
+        "InAppMessage": InAppMessageTypeDef,
+        "Priority": int,
+        "Schedule": InAppCampaignScheduleTypeDef,
+        "SessionCap": int,
+        "TotalCap": int,
+        "TreatmentId": str,
+    },
+    total=False,
+)
+
 CreateInAppTemplateRequestRequestTypeDef = TypedDict(
     "CreateInAppTemplateRequestRequestTypeDef",
     {
         "InAppTemplateRequest": InAppTemplateRequestTypeDef,
         "TemplateName": str,
     },
 )
@@ -6578,14 +6039,22 @@
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+GetInAppTemplateResponseTypeDef = TypedDict(
+    "GetInAppTemplateResponseTypeDef",
+    {
+        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6717,36 +6186,28 @@
 _OptionalTreatmentResourceTypeDef = TypedDict(
     "_OptionalTreatmentResourceTypeDef",
     {
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
         "MessageConfiguration": MessageConfigurationOutputTypeDef,
         "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
-        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
+        "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
 
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
 
-InAppMessagesResponseTypeDef = TypedDict(
-    "InAppMessagesResponseTypeDef",
-    {
-        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
-    },
-    total=False,
-)
-
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
 _OptionalWriteTreatmentResourceTypeDef = TypedDict(
@@ -6765,14 +6226,22 @@
 
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
 
+InAppMessagesResponseTypeDef = TypedDict(
+    "InAppMessagesResponseTypeDef",
+    {
+        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
+    },
+    total=False,
+)
+
 SendMessagesRequestRequestTypeDef = TypedDict(
     "SendMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "MessageRequest": MessageRequestTypeDef,
     },
 )
@@ -6814,27 +6283,27 @@
     pass
 
 
 ConditionalSplitActivityOutputTypeDef = TypedDict(
     "ConditionalSplitActivityOutputTypeDef",
     {
         "Condition": ConditionOutputTypeDef,
-        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+        "EvaluationWaitTime": WaitTimeTypeDef,
         "FalseActivity": str,
         "TrueActivity": str,
     },
     total=False,
 )
 
 MultiConditionalSplitActivityOutputTypeDef = TypedDict(
     "MultiConditionalSplitActivityOutputTypeDef",
     {
         "Branches": List[MultiConditionalBranchOutputTypeDef],
         "DefaultActivity": str,
-        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+        "EvaluationWaitTime": WaitTimeTypeDef,
     },
     total=False,
 )
 
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
@@ -6883,44 +6352,36 @@
     "_OptionalCampaignResponseTypeDef",
     {
         "AdditionalTreatments": List[TreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
         "DefaultState": CampaignStateTypeDef,
         "Description": str,
         "HoldoutPercent": int,
-        "Hook": CampaignHookOutputTypeDef,
+        "Hook": CampaignHookTypeDef,
         "IsPaused": bool,
-        "Limits": CampaignLimitsOutputTypeDef,
+        "Limits": CampaignLimitsTypeDef,
         "MessageConfiguration": MessageConfigurationOutputTypeDef,
         "Name": str,
         "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
         "tags": Dict[str, str],
-        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
+        "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
 
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
 
-GetInAppMessagesResponseTypeDef = TypedDict(
-    "GetInAppMessagesResponseTypeDef",
-    {
-        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
         "HoldoutPercent": int,
@@ -6937,14 +6398,22 @@
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Priority": int,
     },
     total=False,
 )
 
+GetInAppMessagesResponseTypeDef = TypedDict(
+    "GetInAppMessagesResponseTypeDef",
+    {
+        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7002,22 +6471,22 @@
 
 ActivityOutputTypeDef = TypedDict(
     "ActivityOutputTypeDef",
     {
         "CUSTOM": CustomMessageActivityOutputTypeDef,
         "ConditionalSplit": ConditionalSplitActivityOutputTypeDef,
         "Description": str,
-        "EMAIL": EmailMessageActivityOutputTypeDef,
-        "Holdout": HoldoutActivityOutputTypeDef,
+        "EMAIL": EmailMessageActivityTypeDef,
+        "Holdout": HoldoutActivityTypeDef,
         "MultiCondition": MultiConditionalSplitActivityOutputTypeDef,
-        "PUSH": PushMessageActivityOutputTypeDef,
+        "PUSH": PushMessageActivityTypeDef,
         "RandomSplit": RandomSplitActivityOutputTypeDef,
-        "SMS": SMSMessageActivityOutputTypeDef,
-        "Wait": WaitActivityOutputTypeDef,
-        "ContactCenter": ContactCenterActivityOutputTypeDef,
+        "SMS": SMSMessageActivityTypeDef,
+        "Wait": WaitActivityTypeDef,
+        "ContactCenter": ContactCenterActivityTypeDef,
     },
     total=False,
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
@@ -7157,26 +6626,26 @@
 )
 _OptionalJourneyResponseTypeDef = TypedDict(
     "_OptionalJourneyResponseTypeDef",
     {
         "Activities": Dict[str, ActivityOutputTypeDef],
         "CreationDate": str,
         "LastModifiedDate": str,
-        "Limits": JourneyLimitsOutputTypeDef,
+        "Limits": JourneyLimitsTypeDef,
         "LocalTime": bool,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "QuietTime": QuietTimeTypeDef,
         "RefreshFrequency": str,
         "Schedule": JourneyScheduleOutputTypeDef,
         "StartActivity": str,
         "StartCondition": StartConditionOutputTypeDef,
         "State": StateType,
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
-        "JourneyChannelSettings": JourneyChannelSettingsOutputTypeDef,
+        "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
         "OpenHours": OpenHoursOutputTypeDef,
         "ClosedDays": ClosedDaysOutputTypeDef,
         "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,74 +56,61 @@
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
-    "APNSPushNotificationTemplateOutputTypeDef",
     "APNSPushNotificationTemplateTypeDef",
     "APNSSandboxChannelRequestTypeDef",
     "APNSSandboxChannelResponseTypeDef",
     "APNSVoipChannelRequestTypeDef",
     "APNSVoipChannelResponseTypeDef",
     "APNSVoipSandboxChannelRequestTypeDef",
     "APNSVoipSandboxChannelResponseTypeDef",
     "ActivityResponseTypeDef",
-    "ContactCenterActivityOutputTypeDef",
-    "HoldoutActivityOutputTypeDef",
     "ContactCenterActivityTypeDef",
     "HoldoutActivityTypeDef",
     "AddressConfigurationTypeDef",
-    "AndroidPushNotificationTemplateOutputTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
-    "CampaignHookOutputTypeDef",
-    "CampaignLimitsOutputTypeDef",
-    "QuietTimeOutputTypeDef",
+    "JourneyTimeframeCapTypeDef",
+    "CampaignHookTypeDef",
+    "CampaignLimitsTypeDef",
+    "QuietTimeTypeDef",
     "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
-    "CampaignCustomMessageOutputTypeDef",
     "CampaignCustomMessageTypeDef",
-    "CampaignEmailMessageOutputTypeDef",
     "CampaignEmailMessageTypeDef",
-    "CampaignHookTypeDef",
-    "CampaignLimitsTypeDef",
     "CampaignStateTypeDef",
     "CustomDeliveryConfigurationOutputTypeDef",
-    "CampaignSmsMessageOutputTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
-    "ClosedDaysRuleOutputTypeDef",
     "ClosedDaysRuleTypeDef",
-    "WaitTimeOutputTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
     "CreateTemplateMessageBodyTypeDef",
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
     "CustomDeliveryConfigurationTypeDef",
-    "JourneyCustomMessageOutputTypeDef",
     "JourneyCustomMessageTypeDef",
-    "DefaultButtonConfigurationOutputTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
-    "DefaultPushNotificationTemplateOutputTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
     "DeleteApnsSandboxChannelRequestRequestTypeDef",
     "DeleteApnsVoipChannelRequestRequestTypeDef",
     "DeleteApnsVoipSandboxChannelRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
@@ -150,36 +137,31 @@
     "DeleteVoiceChannelRequestRequestTypeDef",
     "VoiceChannelResponseTypeDef",
     "DeleteVoiceTemplateRequestRequestTypeDef",
     "GCMMessageTypeDef",
     "SMSMessageTypeDef",
     "VoiceMessageTypeDef",
     "EmailChannelRequestTypeDef",
-    "JourneyEmailMessageOutputTypeDef",
     "JourneyEmailMessageTypeDef",
     "RawEmailTypeDef",
     "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
-    "EndpointDemographicOutputTypeDef",
     "EndpointItemResponseTypeDef",
-    "EndpointLocationOutputTypeDef",
     "EndpointMessageResultTypeDef",
     "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
-    "MetricDimensionOutputTypeDef",
-    "SetDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
+    "SetDimensionOutputTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
-    "GPSCoordinatesOutputTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
     "GetApnsChannelRequestRequestTypeDef",
     "GetApnsSandboxChannelRequestRequestTypeDef",
     "GetApnsVoipChannelRequestRequestTypeDef",
     "GetApnsVoipSandboxChannelRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
@@ -229,63 +211,47 @@
     "GetSmsTemplateRequestRequestTypeDef",
     "SMSTemplateResponseTypeDef",
     "GetUserEndpointsRequestRequestTypeDef",
     "GetVoiceChannelRequestRequestTypeDef",
     "GetVoiceTemplateRequestRequestTypeDef",
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
-    "InAppMessageBodyConfigOutputTypeDef",
     "InAppMessageBodyConfigTypeDef",
-    "OverrideButtonConfigurationOutputTypeDef",
     "OverrideButtonConfigurationTypeDef",
-    "InAppMessageHeaderConfigOutputTypeDef",
     "InAppMessageHeaderConfigTypeDef",
-    "JourneyChannelSettingsOutputTypeDef",
     "JourneyChannelSettingsTypeDef",
-    "JourneyLimitsOutputTypeDef",
-    "JourneyLimitsTypeDef",
-    "JourneyPushMessageOutputTypeDef",
     "JourneyPushMessageTypeDef",
     "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
-    "JourneySMSMessageOutputTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyScheduleTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagsModelOutputTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
-    "MessageOutputTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
-    "OpenHoursRuleOutputTypeDef",
     "OpenHoursRuleTypeDef",
     "WriteEventStreamTypeDef",
-    "QuietTimeTypeDef",
-    "RandomSplitEntryOutputTypeDef",
     "RandomSplitEntryTypeDef",
-    "RecencyDimensionOutputTypeDef",
     "RecencyDimensionTypeDef",
     "UpdateAttributesRequestTypeDef",
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
-    "SegmentConditionOutputTypeDef",
     "SegmentConditionTypeDef",
-    "SegmentReferenceOutputTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
     "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
-    "TemplateOutputTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
     "VerificationResponseTypeDef",
@@ -293,20 +259,20 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "ApplicationSettingsResourceTypeDef",
+    "ApplicationSettingsJourneyLimitsTypeDef",
+    "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
     "ChannelsResponseTypeDef",
     "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
-    "WaitActivityOutputTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
     "DeleteApnsChannelResponseTypeDef",
     "DeleteApnsSandboxChannelResponseTypeDef",
     "DeleteApnsVoipChannelResponseTypeDef",
@@ -345,16 +311,16 @@
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
     "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
-    "PushNotificationTemplateResponseTypeDef",
     "PushNotificationTemplateRequestTypeDef",
+    "PushNotificationTemplateResponseTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
     "DeleteInAppTemplateResponseTypeDef",
     "DeletePushTemplateResponseTypeDef",
     "DeleteSmsTemplateResponseTypeDef",
@@ -376,15 +342,14 @@
     "DeleteSmsChannelResponseTypeDef",
     "GetSmsChannelResponseTypeDef",
     "UpdateSmsChannelResponseTypeDef",
     "DeleteVoiceChannelResponseTypeDef",
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
-    "EmailMessageActivityOutputTypeDef",
     "EmailMessageActivityTypeDef",
     "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
     "EndpointResponseTypeDef",
@@ -392,67 +357,60 @@
     "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
-    "GPSPointDimensionOutputTypeDef",
     "GPSPointDimensionTypeDef",
     "GetJourneyExecutionActivityMetricsResponseTypeDef",
     "GetJourneyExecutionMetricsResponseTypeDef",
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     "GetSmsTemplateResponseTypeDef",
     "GetVoiceTemplateResponseTypeDef",
     "ImportJobResponseTypeDef",
-    "InAppMessageButtonOutputTypeDef",
     "InAppMessageButtonTypeDef",
-    "PushMessageActivityOutputTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
-    "SMSMessageActivityOutputTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
     "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
-    "WriteApplicationSettingsRequestTypeDef",
     "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
-    "SegmentBehaviorsOutputTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
-    "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
-    "GetApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsResponseTypeDef",
+    "ApplicationSettingsResourceTypeDef",
+    "WriteApplicationSettingsRequestTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
-    "GetPushTemplateResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
+    "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
     "CampaignEventFilterOutputTypeDef",
@@ -467,24 +425,25 @@
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
     "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
-    "InAppMessageContentOutputTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
-    "UpdateApplicationSettingsRequestRequestTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
+    "GetApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsRequestRequestTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
     "ScheduleOutputTypeDef",
     "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
@@ -494,60 +453,60 @@
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
     "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
     "CampaignInAppMessageOutputTypeDef",
-    "InAppMessageTypeDef",
-    "InAppTemplateResponseTypeDef",
     "CampaignInAppMessageTypeDef",
+    "InAppMessageTypeDef",
     "InAppTemplateRequestTypeDef",
+    "InAppTemplateResponseTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
     "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
     "SegmentGroupOutputTypeDef",
     "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
     "MessageConfigurationOutputTypeDef",
-    "InAppMessageCampaignTypeDef",
-    "GetInAppTemplateResponseTypeDef",
     "MessageConfigurationTypeDef",
+    "InAppMessageCampaignTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
+    "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
     "SegmentGroupListOutputTypeDef",
     "ConditionOutputTypeDef",
     "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
-    "InAppMessagesResponseTypeDef",
     "WriteTreatmentResourceTypeDef",
+    "InAppMessagesResponseTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
     "ConditionalSplitActivityOutputTypeDef",
     "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
-    "GetInAppMessagesResponseTypeDef",
     "WriteCampaignRequestTypeDef",
+    "GetInAppMessagesResponseTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
     "ActivityOutputTypeDef",
@@ -714,28 +673,14 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
-APNSPushNotificationTemplateOutputTypeDef = TypedDict(
-    "APNSPushNotificationTemplateOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "MediaUrl": str,
-        "RawContent": str,
-        "Sound": str,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 APNSPushNotificationTemplateTypeDef = TypedDict(
     "APNSPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "MediaUrl": str,
         "RawContent": str,
@@ -903,41 +848,14 @@
     },
     total=False,
 )
 
 class ActivityResponseTypeDef(_RequiredActivityResponseTypeDef, _OptionalActivityResponseTypeDef):
     pass
 
-ContactCenterActivityOutputTypeDef = TypedDict(
-    "ContactCenterActivityOutputTypeDef",
-    {
-        "NextActivity": str,
-    },
-    total=False,
-)
-
-_RequiredHoldoutActivityOutputTypeDef = TypedDict(
-    "_RequiredHoldoutActivityOutputTypeDef",
-    {
-        "Percentage": int,
-    },
-)
-_OptionalHoldoutActivityOutputTypeDef = TypedDict(
-    "_OptionalHoldoutActivityOutputTypeDef",
-    {
-        "NextActivity": str,
-    },
-    total=False,
-)
-
-class HoldoutActivityOutputTypeDef(
-    _RequiredHoldoutActivityOutputTypeDef, _OptionalHoldoutActivityOutputTypeDef
-):
-    pass
-
 ContactCenterActivityTypeDef = TypedDict(
     "ContactCenterActivityTypeDef",
     {
         "NextActivity": str,
     },
     total=False,
 )
@@ -968,30 +886,14 @@
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
-AndroidPushNotificationTemplateOutputTypeDef = TypedDict(
-    "AndroidPushNotificationTemplateOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "ImageIconUrl": str,
-        "ImageUrl": str,
-        "RawContent": str,
-        "SmallImageIconUrl": str,
-        "Sound": str,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 AndroidPushNotificationTemplateTypeDef = TypedDict(
     "AndroidPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
@@ -1022,38 +924,47 @@
 )
 
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
-CampaignHookOutputTypeDef = TypedDict(
-    "CampaignHookOutputTypeDef",
+JourneyTimeframeCapTypeDef = TypedDict(
+    "JourneyTimeframeCapTypeDef",
+    {
+        "Cap": int,
+        "Days": int,
+    },
+    total=False,
+)
+
+CampaignHookTypeDef = TypedDict(
+    "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
     total=False,
 )
 
-CampaignLimitsOutputTypeDef = TypedDict(
-    "CampaignLimitsOutputTypeDef",
+CampaignLimitsTypeDef = TypedDict(
+    "CampaignLimitsTypeDef",
     {
         "Daily": int,
         "MaximumDuration": int,
         "MessagesPerSecond": int,
         "Total": int,
         "Session": int,
     },
     total=False,
 )
 
-QuietTimeOutputTypeDef = TypedDict(
-    "QuietTimeOutputTypeDef",
+QuietTimeTypeDef = TypedDict(
+    "QuietTimeTypeDef",
     {
         "End": str,
         "Start": str,
     },
     total=False,
 )
 
@@ -1180,74 +1091,33 @@
         "TimeToLive": int,
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
-CampaignCustomMessageOutputTypeDef = TypedDict(
-    "CampaignCustomMessageOutputTypeDef",
-    {
-        "Data": str,
-    },
-    total=False,
-)
-
 CampaignCustomMessageTypeDef = TypedDict(
     "CampaignCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
-CampaignEmailMessageOutputTypeDef = TypedDict(
-    "CampaignEmailMessageOutputTypeDef",
-    {
-        "Body": str,
-        "FromAddress": str,
-        "HtmlBody": str,
-        "Title": str,
-    },
-    total=False,
-)
-
 CampaignEmailMessageTypeDef = TypedDict(
     "CampaignEmailMessageTypeDef",
     {
         "Body": str,
         "FromAddress": str,
         "HtmlBody": str,
         "Title": str,
     },
     total=False,
 )
 
-CampaignHookTypeDef = TypedDict(
-    "CampaignHookTypeDef",
-    {
-        "LambdaFunctionName": str,
-        "Mode": ModeType,
-        "WebUrl": str,
-    },
-    total=False,
-)
-
-CampaignLimitsTypeDef = TypedDict(
-    "CampaignLimitsTypeDef",
-    {
-        "Daily": int,
-        "MaximumDuration": int,
-        "MessagesPerSecond": int,
-        "Total": int,
-        "Session": int,
-    },
-    total=False,
-)
-
 CampaignStateTypeDef = TypedDict(
     "CampaignStateTypeDef",
     {
         "CampaignStatus": CampaignStatusType,
     },
     total=False,
 )
@@ -1268,27 +1138,14 @@
 
 class CustomDeliveryConfigurationOutputTypeDef(
     _RequiredCustomDeliveryConfigurationOutputTypeDef,
     _OptionalCustomDeliveryConfigurationOutputTypeDef,
 ):
     pass
 
-CampaignSmsMessageOutputTypeDef = TypedDict(
-    "CampaignSmsMessageOutputTypeDef",
-    {
-        "Body": str,
-        "MessageType": MessageTypeType,
-        "OriginationNumber": str,
-        "SenderId": str,
-        "EntityId": str,
-        "TemplateId": str,
-    },
-    total=False,
-)
-
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
@@ -1310,43 +1167,24 @@
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
 )
 
-ClosedDaysRuleOutputTypeDef = TypedDict(
-    "ClosedDaysRuleOutputTypeDef",
-    {
-        "Name": str,
-        "StartDateTime": str,
-        "EndDateTime": str,
-    },
-    total=False,
-)
-
 ClosedDaysRuleTypeDef = TypedDict(
     "ClosedDaysRuleTypeDef",
     {
         "Name": str,
         "StartDateTime": str,
         "EndDateTime": str,
     },
     total=False,
 )
 
-WaitTimeOutputTypeDef = TypedDict(
-    "WaitTimeOutputTypeDef",
-    {
-        "WaitFor": str,
-        "WaitUntil": str,
-    },
-    total=False,
-)
-
 WaitTimeTypeDef = TypedDict(
     "WaitTimeTypeDef",
     {
         "WaitFor": str,
         "WaitUntil": str,
     },
     total=False,
@@ -1554,54 +1392,22 @@
 )
 
 class CustomDeliveryConfigurationTypeDef(
     _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
-JourneyCustomMessageOutputTypeDef = TypedDict(
-    "JourneyCustomMessageOutputTypeDef",
-    {
-        "Data": str,
-    },
-    total=False,
-)
-
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
-_RequiredDefaultButtonConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDefaultButtonConfigurationOutputTypeDef",
-    {
-        "ButtonAction": ButtonActionType,
-        "Text": str,
-    },
-)
-_OptionalDefaultButtonConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDefaultButtonConfigurationOutputTypeDef",
-    {
-        "BackgroundColor": str,
-        "BorderRadius": int,
-        "Link": str,
-        "TextColor": str,
-    },
-    total=False,
-)
-
-class DefaultButtonConfigurationOutputTypeDef(
-    _RequiredDefaultButtonConfigurationOutputTypeDef,
-    _OptionalDefaultButtonConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredDefaultButtonConfigurationTypeDef = TypedDict(
     "_RequiredDefaultButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
         "Text": str,
     },
 )
@@ -1640,26 +1446,14 @@
         "Substitutions": Mapping[str, Sequence[str]],
         "Title": str,
         "Url": str,
     },
     total=False,
 )
 
-DefaultPushNotificationTemplateOutputTypeDef = TypedDict(
-    "DefaultPushNotificationTemplateOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "Sound": str,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 DefaultPushNotificationTemplateTypeDef = TypedDict(
     "DefaultPushNotificationTemplateTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "Sound": str,
         "Title": str,
@@ -1835,25 +1629,27 @@
         "ApplicationId": str,
     },
 )
 
 _RequiredGCMChannelResponseTypeDef = TypedDict(
     "_RequiredGCMChannelResponseTypeDef",
     {
-        "Credential": str,
         "Platform": str,
     },
 )
 _OptionalGCMChannelResponseTypeDef = TypedDict(
     "_OptionalGCMChannelResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
+        "Credential": str,
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
         "HasCredential": bool,
+        "HasFcmServiceCredentials": bool,
         "Id": str,
         "IsArchived": bool,
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
@@ -2052,14 +1848,15 @@
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
         "IconReference": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
+        "PreferredAuthenticationMethod": str,
         "Priority": str,
         "RawContent": str,
         "RestrictedPackageName": str,
         "SilentPush": bool,
         "SmallImageIconUrl": str,
         "Sound": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -2116,22 +1913,14 @@
 )
 
 class EmailChannelRequestTypeDef(
     _RequiredEmailChannelRequestTypeDef, _OptionalEmailChannelRequestTypeDef
 ):
     pass
 
-JourneyEmailMessageOutputTypeDef = TypedDict(
-    "JourneyEmailMessageOutputTypeDef",
-    {
-        "FromAddress": str,
-    },
-    total=False,
-)
-
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": str,
     },
     total=False,
 )
@@ -2207,51 +1996,23 @@
     {
         "UserAttributes": Mapping[str, Sequence[str]],
         "UserId": str,
     },
     total=False,
 )
 
-EndpointDemographicOutputTypeDef = TypedDict(
-    "EndpointDemographicOutputTypeDef",
-    {
-        "AppVersion": str,
-        "Locale": str,
-        "Make": str,
-        "Model": str,
-        "ModelVersion": str,
-        "Platform": str,
-        "PlatformVersion": str,
-        "Timezone": str,
-    },
-    total=False,
-)
-
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
     {
         "Message": str,
         "StatusCode": int,
     },
     total=False,
 )
 
-EndpointLocationOutputTypeDef = TypedDict(
-    "EndpointLocationOutputTypeDef",
-    {
-        "City": str,
-        "Country": str,
-        "Latitude": float,
-        "Longitude": float,
-        "PostalCode": str,
-        "Region": str,
-    },
-    total=False,
-)
-
 _RequiredEndpointMessageResultTypeDef = TypedDict(
     "_RequiredEndpointMessageResultTypeDef",
     {
         "DeliveryStatus": DeliveryStatusType,
         "StatusCode": int,
     },
 )
@@ -2288,16 +2049,16 @@
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
         "TitleOverride": str,
     },
     total=False,
 )
 
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
+MetricDimensionTypeDef = TypedDict(
+    "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
 
 _RequiredSetDimensionOutputTypeDef = TypedDict(
@@ -2315,22 +2076,14 @@
 )
 
 class SetDimensionOutputTypeDef(
     _RequiredSetDimensionOutputTypeDef, _OptionalSetDimensionOutputTypeDef
 ):
     pass
 
-MetricDimensionTypeDef = TypedDict(
-    "MetricDimensionTypeDef",
-    {
-        "ComparisonOperator": str,
-        "Value": float,
-    },
-)
-
 _RequiredSetDimensionTypeDef = TypedDict(
     "_RequiredSetDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalSetDimensionTypeDef = TypedDict(
@@ -2389,41 +2142,25 @@
 )
 
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
-_RequiredGCMChannelRequestTypeDef = TypedDict(
-    "_RequiredGCMChannelRequestTypeDef",
+GCMChannelRequestTypeDef = TypedDict(
+    "GCMChannelRequestTypeDef",
     {
         "ApiKey": str,
-    },
-)
-_OptionalGCMChannelRequestTypeDef = TypedDict(
-    "_OptionalGCMChannelRequestTypeDef",
-    {
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
+        "ServiceJson": str,
     },
     total=False,
 )
 
-class GCMChannelRequestTypeDef(
-    _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
-):
-    pass
-
-GPSCoordinatesOutputTypeDef = TypedDict(
-    "GPSCoordinatesOutputTypeDef",
-    {
-        "Latitude": float,
-        "Longitude": float,
-    },
-)
-
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -3229,52 +2966,23 @@
 )
 
 class ImportJobResourceTypeDef(
     _RequiredImportJobResourceTypeDef, _OptionalImportJobResourceTypeDef
 ):
     pass
 
-InAppMessageBodyConfigOutputTypeDef = TypedDict(
-    "InAppMessageBodyConfigOutputTypeDef",
-    {
-        "Alignment": AlignmentType,
-        "Body": str,
-        "TextColor": str,
-    },
-)
-
 InAppMessageBodyConfigTypeDef = TypedDict(
     "InAppMessageBodyConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Body": str,
         "TextColor": str,
     },
 )
 
-_RequiredOverrideButtonConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOverrideButtonConfigurationOutputTypeDef",
-    {
-        "ButtonAction": ButtonActionType,
-    },
-)
-_OptionalOverrideButtonConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOverrideButtonConfigurationOutputTypeDef",
-    {
-        "Link": str,
-    },
-    total=False,
-)
-
-class OverrideButtonConfigurationOutputTypeDef(
-    _RequiredOverrideButtonConfigurationOutputTypeDef,
-    _OptionalOverrideButtonConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredOverrideButtonConfigurationTypeDef = TypedDict(
     "_RequiredOverrideButtonConfigurationTypeDef",
     {
         "ButtonAction": ButtonActionType,
     },
 )
 _OptionalOverrideButtonConfigurationTypeDef = TypedDict(
@@ -3286,80 +2994,32 @@
 )
 
 class OverrideButtonConfigurationTypeDef(
     _RequiredOverrideButtonConfigurationTypeDef, _OptionalOverrideButtonConfigurationTypeDef
 ):
     pass
 
-InAppMessageHeaderConfigOutputTypeDef = TypedDict(
-    "InAppMessageHeaderConfigOutputTypeDef",
-    {
-        "Alignment": AlignmentType,
-        "Header": str,
-        "TextColor": str,
-    },
-)
-
 InAppMessageHeaderConfigTypeDef = TypedDict(
     "InAppMessageHeaderConfigTypeDef",
     {
         "Alignment": AlignmentType,
         "Header": str,
         "TextColor": str,
     },
 )
 
-JourneyChannelSettingsOutputTypeDef = TypedDict(
-    "JourneyChannelSettingsOutputTypeDef",
-    {
-        "ConnectCampaignArn": str,
-        "ConnectCampaignExecutionRoleArn": str,
-    },
-    total=False,
-)
-
 JourneyChannelSettingsTypeDef = TypedDict(
     "JourneyChannelSettingsTypeDef",
     {
         "ConnectCampaignArn": str,
         "ConnectCampaignExecutionRoleArn": str,
     },
     total=False,
 )
 
-JourneyLimitsOutputTypeDef = TypedDict(
-    "JourneyLimitsOutputTypeDef",
-    {
-        "DailyCap": int,
-        "EndpointReentryCap": int,
-        "MessagesPerSecond": int,
-        "EndpointReentryInterval": str,
-    },
-    total=False,
-)
-
-JourneyLimitsTypeDef = TypedDict(
-    "JourneyLimitsTypeDef",
-    {
-        "DailyCap": int,
-        "EndpointReentryCap": int,
-        "MessagesPerSecond": int,
-        "EndpointReentryInterval": str,
-    },
-    total=False,
-)
-
-JourneyPushMessageOutputTypeDef = TypedDict(
-    "JourneyPushMessageOutputTypeDef",
-    {
-        "TimeToLive": str,
-    },
-    total=False,
-)
-
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": str,
     },
     total=False,
 )
@@ -3380,26 +3040,14 @@
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
     },
 )
 
-JourneySMSMessageOutputTypeDef = TypedDict(
-    "JourneySMSMessageOutputTypeDef",
-    {
-        "MessageType": MessageTypeType,
-        "OriginationNumber": str,
-        "SenderId": str,
-        "EntityId": str,
-        "TemplateId": str,
-    },
-    total=False,
-)
-
 JourneySMSMessageTypeDef = TypedDict(
     "JourneySMSMessageTypeDef",
     {
         "MessageType": MessageTypeType,
         "OriginationNumber": str,
         "SenderId": str,
         "EntityId": str,
@@ -3489,33 +3137,14 @@
         "PageSize": str,
         "Prefix": str,
         "TemplateType": str,
     },
     total=False,
 )
 
-MessageOutputTypeDef = TypedDict(
-    "MessageOutputTypeDef",
-    {
-        "Action": ActionType,
-        "Body": str,
-        "ImageIconUrl": str,
-        "ImageSmallIconUrl": str,
-        "ImageUrl": str,
-        "JsonBody": str,
-        "MediaUrl": str,
-        "RawContent": str,
-        "SilentPush": bool,
-        "TimeToLive": int,
-        "Title": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Action": ActionType,
         "Body": str,
         "ImageIconUrl": str,
         "ImageSmallIconUrl": str,
@@ -3577,23 +3206,14 @@
         "PhoneTypeCode": int,
         "Timezone": str,
         "ZipCode": str,
     },
     total=False,
 )
 
-OpenHoursRuleOutputTypeDef = TypedDict(
-    "OpenHoursRuleOutputTypeDef",
-    {
-        "StartTime": str,
-        "EndTime": str,
-    },
-    total=False,
-)
-
 OpenHoursRuleTypeDef = TypedDict(
     "OpenHoursRuleTypeDef",
     {
         "StartTime": str,
         "EndTime": str,
     },
     total=False,
@@ -3603,49 +3223,23 @@
     "WriteEventStreamTypeDef",
     {
         "DestinationStreamArn": str,
         "RoleArn": str,
     },
 )
 
-QuietTimeTypeDef = TypedDict(
-    "QuietTimeTypeDef",
-    {
-        "End": str,
-        "Start": str,
-    },
-    total=False,
-)
-
-RandomSplitEntryOutputTypeDef = TypedDict(
-    "RandomSplitEntryOutputTypeDef",
-    {
-        "NextActivity": str,
-        "Percentage": int,
-    },
-    total=False,
-)
-
 RandomSplitEntryTypeDef = TypedDict(
     "RandomSplitEntryTypeDef",
     {
         "NextActivity": str,
         "Percentage": int,
     },
     total=False,
 )
 
-RecencyDimensionOutputTypeDef = TypedDict(
-    "RecencyDimensionOutputTypeDef",
-    {
-        "Duration": DurationType,
-        "RecencyType": RecencyTypeType,
-    },
-)
-
 RecencyDimensionTypeDef = TypedDict(
     "RecencyDimensionTypeDef",
     {
         "Duration": DurationType,
         "RecencyType": RecencyTypeType,
     },
 )
@@ -3673,47 +3267,21 @@
         "Enabled": bool,
         "SenderId": str,
         "ShortCode": str,
     },
     total=False,
 )
 
-SegmentConditionOutputTypeDef = TypedDict(
-    "SegmentConditionOutputTypeDef",
-    {
-        "SegmentId": str,
-    },
-)
-
 SegmentConditionTypeDef = TypedDict(
     "SegmentConditionTypeDef",
     {
         "SegmentId": str,
     },
 )
 
-_RequiredSegmentReferenceOutputTypeDef = TypedDict(
-    "_RequiredSegmentReferenceOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalSegmentReferenceOutputTypeDef = TypedDict(
-    "_OptionalSegmentReferenceOutputTypeDef",
-    {
-        "Version": int,
-    },
-    total=False,
-)
-
-class SegmentReferenceOutputTypeDef(
-    _RequiredSegmentReferenceOutputTypeDef, _OptionalSegmentReferenceOutputTypeDef
-):
-    pass
-
 _RequiredSegmentReferenceTypeDef = TypedDict(
     "_RequiredSegmentReferenceTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalSegmentReferenceTypeDef = TypedDict(
@@ -3798,23 +3366,14 @@
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-TemplateOutputTypeDef = TypedDict(
-    "TemplateOutputTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -3991,36 +3550,37 @@
     {
         "Item": List[ApplicationResponseTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
+ApplicationSettingsJourneyLimitsTypeDef = TypedDict(
+    "ApplicationSettingsJourneyLimitsTypeDef",
     {
-        "ApplicationId": str,
+        "DailyCap": int,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
+    total=False,
 )
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+
+JourneyLimitsTypeDef = TypedDict(
+    "JourneyLimitsTypeDef",
     {
-        "CampaignHook": CampaignHookOutputTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsOutputTypeDef,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "DailyCap": int,
+        "EndpointReentryCap": int,
+        "MessagesPerSecond": int,
+        "EndpointReentryInterval": str,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
     total=False,
 )
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
 UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
     "UpdateBaiduChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "BaiduChannelRequest": BaiduChannelRequestTypeDef,
     },
 )
@@ -4031,19 +3591,19 @@
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
 ClosedDaysOutputTypeDef = TypedDict(
     "ClosedDaysOutputTypeDef",
     {
-        "EMAIL": List[ClosedDaysRuleOutputTypeDef],
-        "SMS": List[ClosedDaysRuleOutputTypeDef],
-        "PUSH": List[ClosedDaysRuleOutputTypeDef],
-        "VOICE": List[ClosedDaysRuleOutputTypeDef],
-        "CUSTOM": List[ClosedDaysRuleOutputTypeDef],
+        "EMAIL": List[ClosedDaysRuleTypeDef],
+        "SMS": List[ClosedDaysRuleTypeDef],
+        "PUSH": List[ClosedDaysRuleTypeDef],
+        "VOICE": List[ClosedDaysRuleTypeDef],
+        "CUSTOM": List[ClosedDaysRuleTypeDef],
     },
     total=False,
 )
 
 ClosedDaysTypeDef = TypedDict(
     "ClosedDaysTypeDef",
     {
@@ -4052,23 +3612,14 @@
         "PUSH": Sequence[ClosedDaysRuleTypeDef],
         "VOICE": Sequence[ClosedDaysRuleTypeDef],
         "CUSTOM": Sequence[ClosedDaysRuleTypeDef],
     },
     total=False,
 )
 
-WaitActivityOutputTypeDef = TypedDict(
-    "WaitActivityOutputTypeDef",
-    {
-        "NextActivity": str,
-        "WaitTime": WaitTimeOutputTypeDef,
-    },
-    total=False,
-)
-
 WaitActivityTypeDef = TypedDict(
     "WaitActivityTypeDef",
     {
         "NextActivity": str,
         "WaitTime": WaitTimeTypeDef,
     },
     total=False,
@@ -4469,15 +4020,15 @@
     pass
 
 CustomMessageActivityOutputTypeDef = TypedDict(
     "CustomMessageActivityOutputTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": List[EndpointTypesElementType],
-        "MessageConfig": JourneyCustomMessageOutputTypeDef,
+        "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
@@ -4490,63 +4041,63 @@
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
     },
     total=False,
 )
 
+PushNotificationTemplateRequestTypeDef = TypedDict(
+    "PushNotificationTemplateRequestTypeDef",
+    {
+        "ADM": AndroidPushNotificationTemplateTypeDef,
+        "APNS": APNSPushNotificationTemplateTypeDef,
+        "Baidu": AndroidPushNotificationTemplateTypeDef,
+        "Default": DefaultPushNotificationTemplateTypeDef,
+        "DefaultSubstitutions": str,
+        "GCM": AndroidPushNotificationTemplateTypeDef,
+        "RecommenderId": str,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
+
 _RequiredPushNotificationTemplateResponseTypeDef = TypedDict(
     "_RequiredPushNotificationTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalPushNotificationTemplateResponseTypeDef = TypedDict(
     "_OptionalPushNotificationTemplateResponseTypeDef",
     {
-        "ADM": AndroidPushNotificationTemplateOutputTypeDef,
-        "APNS": APNSPushNotificationTemplateOutputTypeDef,
+        "ADM": AndroidPushNotificationTemplateTypeDef,
+        "APNS": APNSPushNotificationTemplateTypeDef,
         "Arn": str,
-        "Baidu": AndroidPushNotificationTemplateOutputTypeDef,
-        "Default": DefaultPushNotificationTemplateOutputTypeDef,
+        "Baidu": AndroidPushNotificationTemplateTypeDef,
+        "Default": DefaultPushNotificationTemplateTypeDef,
         "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateOutputTypeDef,
+        "GCM": AndroidPushNotificationTemplateTypeDef,
         "RecommenderId": str,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
 class PushNotificationTemplateResponseTypeDef(
     _RequiredPushNotificationTemplateResponseTypeDef,
     _OptionalPushNotificationTemplateResponseTypeDef,
 ):
     pass
 
-PushNotificationTemplateRequestTypeDef = TypedDict(
-    "PushNotificationTemplateRequestTypeDef",
-    {
-        "ADM": AndroidPushNotificationTemplateTypeDef,
-        "APNS": APNSPushNotificationTemplateTypeDef,
-        "Baidu": AndroidPushNotificationTemplateTypeDef,
-        "Default": DefaultPushNotificationTemplateTypeDef,
-        "DefaultSubstitutions": str,
-        "GCM": AndroidPushNotificationTemplateTypeDef,
-        "RecommenderId": str,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
-    },
-    total=False,
-)
-
 DeleteEmailChannelResponseTypeDef = TypedDict(
     "DeleteEmailChannelResponseTypeDef",
     {
         "EmailChannelResponse": EmailChannelResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4771,25 +4322,14 @@
     "UpdateEmailChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EmailChannelRequest": EmailChannelRequestTypeDef,
     },
 )
 
-EmailMessageActivityOutputTypeDef = TypedDict(
-    "EmailMessageActivityOutputTypeDef",
-    {
-        "MessageConfig": JourneyEmailMessageOutputTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 EmailMessageActivityTypeDef = TypedDict(
     "EmailMessageActivityTypeDef",
     {
         "MessageConfig": JourneyEmailMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -4885,33 +4425,33 @@
     {
         "Address": str,
         "ApplicationId": str,
         "Attributes": Dict[str, List[str]],
         "ChannelType": ChannelTypeType,
         "CohortId": str,
         "CreationDate": str,
-        "Demographic": EndpointDemographicOutputTypeDef,
+        "Demographic": EndpointDemographicTypeDef,
         "EffectiveDate": str,
         "EndpointStatus": str,
         "Id": str,
-        "Location": EndpointLocationOutputTypeDef,
+        "Location": EndpointLocationTypeDef,
         "Metrics": Dict[str, float],
         "OptOut": str,
         "RequestId": str,
         "User": EndpointUserOutputTypeDef,
     },
     total=False,
 )
 
 EventDimensionsOutputTypeDef = TypedDict(
     "EventDimensionsOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
         "EventType": SetDimensionOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+        "Metrics": Dict[str, MetricDimensionTypeDef],
     },
     total=False,
 )
 
 SegmentDemographicsOutputTypeDef = TypedDict(
     "SegmentDemographicsOutputTypeDef",
     {
@@ -5016,33 +4556,14 @@
     "UpdateGcmChannelRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "GCMChannelRequest": GCMChannelRequestTypeDef,
     },
 )
 
-_RequiredGPSPointDimensionOutputTypeDef = TypedDict(
-    "_RequiredGPSPointDimensionOutputTypeDef",
-    {
-        "Coordinates": GPSCoordinatesOutputTypeDef,
-    },
-)
-_OptionalGPSPointDimensionOutputTypeDef = TypedDict(
-    "_OptionalGPSPointDimensionOutputTypeDef",
-    {
-        "RangeInKilometers": float,
-    },
-    total=False,
-)
-
-class GPSPointDimensionOutputTypeDef(
-    _RequiredGPSPointDimensionOutputTypeDef, _OptionalGPSPointDimensionOutputTypeDef
-):
-    pass
-
 _RequiredGPSPointDimensionTypeDef = TypedDict(
     "_RequiredGPSPointDimensionTypeDef",
     {
         "Coordinates": GPSCoordinatesTypeDef,
     },
 )
 _OptionalGPSPointDimensionTypeDef = TypedDict(
@@ -5134,47 +4655,25 @@
 )
 
 class ImportJobResponseTypeDef(
     _RequiredImportJobResponseTypeDef, _OptionalImportJobResponseTypeDef
 ):
     pass
 
-InAppMessageButtonOutputTypeDef = TypedDict(
-    "InAppMessageButtonOutputTypeDef",
-    {
-        "Android": OverrideButtonConfigurationOutputTypeDef,
-        "DefaultConfig": DefaultButtonConfigurationOutputTypeDef,
-        "IOS": OverrideButtonConfigurationOutputTypeDef,
-        "Web": OverrideButtonConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 InAppMessageButtonTypeDef = TypedDict(
     "InAppMessageButtonTypeDef",
     {
         "Android": OverrideButtonConfigurationTypeDef,
         "DefaultConfig": DefaultButtonConfigurationTypeDef,
         "IOS": OverrideButtonConfigurationTypeDef,
         "Web": OverrideButtonConfigurationTypeDef,
     },
     total=False,
 )
 
-PushMessageActivityOutputTypeDef = TypedDict(
-    "PushMessageActivityOutputTypeDef",
-    {
-        "MessageConfig": JourneyPushMessageOutputTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 PushMessageActivityTypeDef = TypedDict(
     "PushMessageActivityTypeDef",
     {
         "MessageConfig": JourneyPushMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -5197,25 +4696,14 @@
 )
 
 class JourneyRunsResponseTypeDef(
     _RequiredJourneyRunsResponseTypeDef, _OptionalJourneyRunsResponseTypeDef
 ):
     pass
 
-SMSMessageActivityOutputTypeDef = TypedDict(
-    "SMSMessageActivityOutputTypeDef",
-    {
-        "MessageConfig": JourneySMSMessageOutputTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 SMSMessageActivityTypeDef = TypedDict(
     "SMSMessageActivityTypeDef",
     {
         "MessageConfig": JourneySMSMessageTypeDef,
         "NextActivity": str,
         "TemplateName": str,
         "TemplateVersion": str,
@@ -5273,19 +4761,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenHoursOutputTypeDef = TypedDict(
     "OpenHoursOutputTypeDef",
     {
-        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
-        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleOutputTypeDef]],
+        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
+        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
     },
     total=False,
 )
 
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
@@ -5302,50 +4790,30 @@
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
 
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
-    {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
-    },
-    total=False,
-)
-
 RandomSplitActivityOutputTypeDef = TypedDict(
     "RandomSplitActivityOutputTypeDef",
     {
-        "Branches": List[RandomSplitEntryOutputTypeDef],
+        "Branches": List[RandomSplitEntryTypeDef],
     },
     total=False,
 )
 
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": Sequence[RandomSplitEntryTypeDef],
     },
     total=False,
 )
 
-SegmentBehaviorsOutputTypeDef = TypedDict(
-    "SegmentBehaviorsOutputTypeDef",
-    {
-        "Recency": RecencyDimensionOutputTypeDef,
-    },
-    total=False,
-)
-
 SegmentBehaviorsTypeDef = TypedDict(
     "SegmentBehaviorsTypeDef",
     {
         "Recency": RecencyDimensionTypeDef,
     },
     total=False,
 )
@@ -5406,32 +4874,22 @@
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
 )
 
-TemplateConfigurationOutputTypeDef = TypedDict(
-    "TemplateConfigurationOutputTypeDef",
-    {
-        "EmailTemplate": TemplateOutputTypeDef,
-        "PushTemplate": TemplateOutputTypeDef,
-        "SMSTemplate": TemplateOutputTypeDef,
-        "VoiceTemplate": TemplateOutputTypeDef,
-    },
-    total=False,
-)
-
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "EmailTemplate": TemplateTypeDef,
         "PushTemplate": TemplateTypeDef,
         "SMSTemplate": TemplateTypeDef,
         "VoiceTemplate": TemplateTypeDef,
+        "InAppTemplate": TemplateTypeDef,
     },
     total=False,
 )
 
 _RequiredTemplatesResponseTypeDef = TypedDict(
     "_RequiredTemplatesResponseTypeDef",
     {
@@ -5516,28 +4974,48 @@
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationSettingsResponseTypeDef = TypedDict(
-    "GetApplicationSettingsResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
+    },
+)
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
+    {
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
-UpdateApplicationSettingsResponseTypeDef = TypedDict(
-    "UpdateApplicationSettingsResponseTypeDef",
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5548,22 +5026,14 @@
     "GetRecommenderConfigurationsResponseTypeDef",
     {
         "ListRecommenderConfigurationsResponse": ListRecommenderConfigurationsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPushTemplateResponseTypeDef = TypedDict(
-    "GetPushTemplateResponseTypeDef",
-    {
-        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreatePushTemplateRequestRequestTypeDef = TypedDict(
     "CreatePushTemplateRequestRequestTypeDef",
     {
         "PushNotificationTemplateRequest": PushNotificationTemplateRequestTypeDef,
         "TemplateName": str,
     },
 )
@@ -5586,14 +5056,22 @@
 
 class UpdatePushTemplateRequestRequestTypeDef(
     _RequiredUpdatePushTemplateRequestRequestTypeDef,
     _OptionalUpdatePushTemplateRequestRequestTypeDef,
 ):
     pass
 
+GetPushTemplateResponseTypeDef = TypedDict(
+    "GetPushTemplateResponseTypeDef",
+    {
+        "PushNotificationTemplateResponse": PushNotificationTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EndpointBatchRequestTypeDef = TypedDict(
     "EndpointBatchRequestTypeDef",
     {
         "Item": Sequence[EndpointBatchItemTypeDef],
     },
 )
 
@@ -5738,15 +5216,15 @@
     },
 )
 
 SegmentLocationOutputTypeDef = TypedDict(
     "SegmentLocationOutputTypeDef",
     {
         "Country": SetDimensionOutputTypeDef,
-        "GPSPoint": GPSPointDimensionOutputTypeDef,
+        "GPSPoint": GPSPointDimensionTypeDef,
     },
     total=False,
 )
 
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
@@ -5787,27 +5265,14 @@
 )
 
 class ImportJobsResponseTypeDef(
     _RequiredImportJobsResponseTypeDef, _OptionalImportJobsResponseTypeDef
 ):
     pass
 
-InAppMessageContentOutputTypeDef = TypedDict(
-    "InAppMessageContentOutputTypeDef",
-    {
-        "BackgroundColor": str,
-        "BodyConfig": InAppMessageBodyConfigOutputTypeDef,
-        "HeaderConfig": InAppMessageHeaderConfigOutputTypeDef,
-        "ImageUrl": str,
-        "PrimaryBtn": InAppMessageButtonOutputTypeDef,
-        "SecondaryBtn": InAppMessageButtonOutputTypeDef,
-    },
-    total=False,
-)
-
 InAppMessageContentTypeDef = TypedDict(
     "InAppMessageContentTypeDef",
     {
         "BackgroundColor": str,
         "BodyConfig": InAppMessageBodyConfigTypeDef,
         "HeaderConfig": InAppMessageHeaderConfigTypeDef,
         "ImageUrl": str,
@@ -5837,22 +5302,14 @@
     "SendOTPMessageResponseTypeDef",
     {
         "MessageResponse": MessageResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationSettingsRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
-    },
-)
-
 BaseKpiResultTypeDef = TypedDict(
     "BaseKpiResultTypeDef",
     {
         "Rows": List[ResultRowTypeDef],
     },
 )
 
@@ -5882,14 +5339,38 @@
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetApplicationSettingsResponseTypeDef = TypedDict(
+    "GetApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsResponseTypeDef = TypedDict(
+    "UpdateApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationSettingsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+    },
+)
+
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointBatchRequest": EndpointBatchRequestTypeDef,
     },
 )
@@ -5911,15 +5392,15 @@
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
         "EventFilter": CampaignEventFilterOutputTypeDef,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "QuietTime": QuietTimeTypeDef,
     },
     total=False,
 )
 
 _RequiredScheduleOutputTypeDef = TypedDict(
     "_RequiredScheduleOutputTypeDef",
     {
@@ -5929,15 +5410,15 @@
 _OptionalScheduleOutputTypeDef = TypedDict(
     "_OptionalScheduleOutputTypeDef",
     {
         "EndTime": str,
         "EventFilter": CampaignEventFilterOutputTypeDef,
         "Frequency": FrequencyType,
         "IsLocalTime": bool,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "QuietTime": QuietTimeTypeDef,
         "Timezone": str,
     },
     total=False,
 )
 
 class ScheduleOutputTypeDef(_RequiredScheduleOutputTypeDef, _OptionalScheduleOutputTypeDef):
     pass
@@ -6013,18 +5494,18 @@
     },
 )
 
 SegmentDimensionsOutputTypeDef = TypedDict(
     "SegmentDimensionsOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
-        "Behavior": SegmentBehaviorsOutputTypeDef,
+        "Behavior": SegmentBehaviorsTypeDef,
         "Demographic": SegmentDemographicsOutputTypeDef,
         "Location": SegmentLocationOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionOutputTypeDef],
+        "Metrics": Dict[str, MetricDimensionTypeDef],
         "UserAttributes": Dict[str, AttributeDimensionOutputTypeDef],
     },
     total=False,
 )
 
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
@@ -6055,82 +5536,82 @@
     },
 )
 
 CampaignInAppMessageOutputTypeDef = TypedDict(
     "CampaignInAppMessageOutputTypeDef",
     {
         "Body": str,
-        "Content": List[InAppMessageContentOutputTypeDef],
+        "Content": List[InAppMessageContentTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
+CampaignInAppMessageTypeDef = TypedDict(
+    "CampaignInAppMessageTypeDef",
+    {
+        "Body": str,
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+    },
+    total=False,
+)
+
 InAppMessageTypeDef = TypedDict(
     "InAppMessageTypeDef",
     {
-        "Content": List[InAppMessageContentOutputTypeDef],
+        "Content": List[InAppMessageContentTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
     },
     total=False,
 )
 
+InAppTemplateRequestTypeDef = TypedDict(
+    "InAppTemplateRequestTypeDef",
+    {
+        "Content": Sequence[InAppMessageContentTypeDef],
+        "CustomConfig": Mapping[str, str],
+        "Layout": LayoutType,
+        "tags": Mapping[str, str],
+        "TemplateDescription": str,
+    },
+    total=False,
+)
+
 _RequiredInAppTemplateResponseTypeDef = TypedDict(
     "_RequiredInAppTemplateResponseTypeDef",
     {
         "CreationDate": str,
         "LastModifiedDate": str,
         "TemplateName": str,
         "TemplateType": TemplateTypeType,
     },
 )
 _OptionalInAppTemplateResponseTypeDef = TypedDict(
     "_OptionalInAppTemplateResponseTypeDef",
     {
         "Arn": str,
-        "Content": List[InAppMessageContentOutputTypeDef],
+        "Content": List[InAppMessageContentTypeDef],
         "CustomConfig": Dict[str, str],
         "Layout": LayoutType,
         "tags": Dict[str, str],
         "TemplateDescription": str,
         "Version": str,
     },
     total=False,
 )
 
 class InAppTemplateResponseTypeDef(
     _RequiredInAppTemplateResponseTypeDef, _OptionalInAppTemplateResponseTypeDef
 ):
     pass
 
-CampaignInAppMessageTypeDef = TypedDict(
-    "CampaignInAppMessageTypeDef",
-    {
-        "Body": str,
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
-        "Layout": LayoutType,
-    },
-    total=False,
-)
-
-InAppTemplateRequestTypeDef = TypedDict(
-    "InAppTemplateRequestTypeDef",
-    {
-        "Content": Sequence[InAppMessageContentTypeDef],
-        "CustomConfig": Mapping[str, str],
-        "Layout": LayoutType,
-        "tags": Mapping[str, str],
-        "TemplateDescription": str,
-    },
-    total=False,
-)
-
 _RequiredApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "_RequiredApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationId": str,
         "EndTime": datetime,
         "KpiName": str,
         "KpiResult": BaseKpiResultTypeDef,
@@ -6215,15 +5696,15 @@
 )
 
 StartConditionOutputTypeDef = TypedDict(
     "StartConditionOutputTypeDef",
     {
         "Description": str,
         "EventStartCondition": EventStartConditionOutputTypeDef,
-        "SegmentStartCondition": SegmentConditionOutputTypeDef,
+        "SegmentStartCondition": SegmentConditionTypeDef,
     },
     total=False,
 )
 
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
@@ -6242,26 +5723,26 @@
     },
 )
 
 SegmentGroupOutputTypeDef = TypedDict(
     "SegmentGroupOutputTypeDef",
     {
         "Dimensions": List[SegmentDimensionsOutputTypeDef],
-        "SourceSegments": List[SegmentReferenceOutputTypeDef],
+        "SourceSegments": List[SegmentReferenceTypeDef],
         "SourceType": SourceTypeType,
         "Type": TypeType,
     },
     total=False,
 )
 
 SimpleConditionOutputTypeDef = TypedDict(
     "SimpleConditionOutputTypeDef",
     {
         "EventCondition": EventConditionOutputTypeDef,
-        "SegmentCondition": SegmentConditionOutputTypeDef,
+        "SegmentCondition": SegmentConditionTypeDef,
         "SegmentDimensions": SegmentDimensionsOutputTypeDef,
     },
     total=False,
 )
 
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
@@ -6283,50 +5764,27 @@
     },
     total=False,
 )
 
 MessageConfigurationOutputTypeDef = TypedDict(
     "MessageConfigurationOutputTypeDef",
     {
-        "ADMMessage": MessageOutputTypeDef,
-        "APNSMessage": MessageOutputTypeDef,
-        "BaiduMessage": MessageOutputTypeDef,
-        "CustomMessage": CampaignCustomMessageOutputTypeDef,
-        "DefaultMessage": MessageOutputTypeDef,
-        "EmailMessage": CampaignEmailMessageOutputTypeDef,
-        "GCMMessage": MessageOutputTypeDef,
-        "SMSMessage": CampaignSmsMessageOutputTypeDef,
+        "ADMMessage": MessageTypeDef,
+        "APNSMessage": MessageTypeDef,
+        "BaiduMessage": MessageTypeDef,
+        "CustomMessage": CampaignCustomMessageTypeDef,
+        "DefaultMessage": MessageTypeDef,
+        "EmailMessage": CampaignEmailMessageTypeDef,
+        "GCMMessage": MessageTypeDef,
+        "SMSMessage": CampaignSmsMessageTypeDef,
         "InAppMessage": CampaignInAppMessageOutputTypeDef,
     },
     total=False,
 )
 
-InAppMessageCampaignTypeDef = TypedDict(
-    "InAppMessageCampaignTypeDef",
-    {
-        "CampaignId": str,
-        "DailyCap": int,
-        "InAppMessage": InAppMessageTypeDef,
-        "Priority": int,
-        "Schedule": InAppCampaignScheduleTypeDef,
-        "SessionCap": int,
-        "TotalCap": int,
-        "TreatmentId": str,
-    },
-    total=False,
-)
-
-GetInAppTemplateResponseTypeDef = TypedDict(
-    "GetInAppTemplateResponseTypeDef",
-    {
-        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MessageConfigurationTypeDef = TypedDict(
     "MessageConfigurationTypeDef",
     {
         "ADMMessage": MessageTypeDef,
         "APNSMessage": MessageTypeDef,
         "BaiduMessage": MessageTypeDef,
         "CustomMessage": CampaignCustomMessageTypeDef,
@@ -6335,14 +5793,29 @@
         "GCMMessage": MessageTypeDef,
         "SMSMessage": CampaignSmsMessageTypeDef,
         "InAppMessage": CampaignInAppMessageTypeDef,
     },
     total=False,
 )
 
+InAppMessageCampaignTypeDef = TypedDict(
+    "InAppMessageCampaignTypeDef",
+    {
+        "CampaignId": str,
+        "DailyCap": int,
+        "InAppMessage": InAppMessageTypeDef,
+        "Priority": int,
+        "Schedule": InAppCampaignScheduleTypeDef,
+        "SessionCap": int,
+        "TotalCap": int,
+        "TreatmentId": str,
+    },
+    total=False,
+)
+
 CreateInAppTemplateRequestRequestTypeDef = TypedDict(
     "CreateInAppTemplateRequestRequestTypeDef",
     {
         "InAppTemplateRequest": InAppTemplateRequestTypeDef,
         "TemplateName": str,
     },
 )
@@ -6365,14 +5838,22 @@
 
 class UpdateInAppTemplateRequestRequestTypeDef(
     _RequiredUpdateInAppTemplateRequestRequestTypeDef,
     _OptionalUpdateInAppTemplateRequestRequestTypeDef,
 ):
     pass
 
+GetInAppTemplateResponseTypeDef = TypedDict(
+    "GetInAppTemplateResponseTypeDef",
+    {
+        "InAppTemplateResponse": InAppTemplateResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetApplicationDateRangeKpiResponseTypeDef = TypedDict(
     "GetApplicationDateRangeKpiResponseTypeDef",
     {
         "ApplicationDateRangeKpiResponse": ApplicationDateRangeKpiResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6500,34 +5981,26 @@
 _OptionalTreatmentResourceTypeDef = TypedDict(
     "_OptionalTreatmentResourceTypeDef",
     {
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
         "MessageConfiguration": MessageConfigurationOutputTypeDef,
         "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
-        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
+        "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
 
 class TreatmentResourceTypeDef(
     _RequiredTreatmentResourceTypeDef, _OptionalTreatmentResourceTypeDef
 ):
     pass
 
-InAppMessagesResponseTypeDef = TypedDict(
-    "InAppMessagesResponseTypeDef",
-    {
-        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
-    },
-    total=False,
-)
-
 _RequiredWriteTreatmentResourceTypeDef = TypedDict(
     "_RequiredWriteTreatmentResourceTypeDef",
     {
         "SizePercent": int,
     },
 )
 _OptionalWriteTreatmentResourceTypeDef = TypedDict(
@@ -6544,14 +6017,22 @@
 )
 
 class WriteTreatmentResourceTypeDef(
     _RequiredWriteTreatmentResourceTypeDef, _OptionalWriteTreatmentResourceTypeDef
 ):
     pass
 
+InAppMessagesResponseTypeDef = TypedDict(
+    "InAppMessagesResponseTypeDef",
+    {
+        "InAppMessageCampaigns": List[InAppMessageCampaignTypeDef],
+    },
+    total=False,
+)
+
 SendMessagesRequestRequestTypeDef = TypedDict(
     "SendMessagesRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "MessageRequest": MessageRequestTypeDef,
     },
 )
@@ -6591,27 +6072,27 @@
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
 ConditionalSplitActivityOutputTypeDef = TypedDict(
     "ConditionalSplitActivityOutputTypeDef",
     {
         "Condition": ConditionOutputTypeDef,
-        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+        "EvaluationWaitTime": WaitTimeTypeDef,
         "FalseActivity": str,
         "TrueActivity": str,
     },
     total=False,
 )
 
 MultiConditionalSplitActivityOutputTypeDef = TypedDict(
     "MultiConditionalSplitActivityOutputTypeDef",
     {
         "Branches": List[MultiConditionalBranchOutputTypeDef],
         "DefaultActivity": str,
-        "EvaluationWaitTime": WaitTimeOutputTypeDef,
+        "EvaluationWaitTime": WaitTimeTypeDef,
     },
     total=False,
 )
 
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
@@ -6660,42 +6141,34 @@
     "_OptionalCampaignResponseTypeDef",
     {
         "AdditionalTreatments": List[TreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
         "DefaultState": CampaignStateTypeDef,
         "Description": str,
         "HoldoutPercent": int,
-        "Hook": CampaignHookOutputTypeDef,
+        "Hook": CampaignHookTypeDef,
         "IsPaused": bool,
-        "Limits": CampaignLimitsOutputTypeDef,
+        "Limits": CampaignLimitsTypeDef,
         "MessageConfiguration": MessageConfigurationOutputTypeDef,
         "Name": str,
         "Schedule": ScheduleOutputTypeDef,
         "State": CampaignStateTypeDef,
         "tags": Dict[str, str],
-        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
+        "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
     },
     total=False,
 )
 
 class CampaignResponseTypeDef(_RequiredCampaignResponseTypeDef, _OptionalCampaignResponseTypeDef):
     pass
 
-GetInAppMessagesResponseTypeDef = TypedDict(
-    "GetInAppMessagesResponseTypeDef",
-    {
-        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 WriteCampaignRequestTypeDef = TypedDict(
     "WriteCampaignRequestTypeDef",
     {
         "AdditionalTreatments": Sequence[WriteTreatmentResourceTypeDef],
         "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "Description": str,
         "HoldoutPercent": int,
@@ -6712,14 +6185,22 @@
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Priority": int,
     },
     total=False,
 )
 
+GetInAppMessagesResponseTypeDef = TypedDict(
+    "GetInAppMessagesResponseTypeDef",
+    {
+        "InAppMessagesResponse": InAppMessagesResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6775,22 +6256,22 @@
 
 ActivityOutputTypeDef = TypedDict(
     "ActivityOutputTypeDef",
     {
         "CUSTOM": CustomMessageActivityOutputTypeDef,
         "ConditionalSplit": ConditionalSplitActivityOutputTypeDef,
         "Description": str,
-        "EMAIL": EmailMessageActivityOutputTypeDef,
-        "Holdout": HoldoutActivityOutputTypeDef,
+        "EMAIL": EmailMessageActivityTypeDef,
+        "Holdout": HoldoutActivityTypeDef,
         "MultiCondition": MultiConditionalSplitActivityOutputTypeDef,
-        "PUSH": PushMessageActivityOutputTypeDef,
+        "PUSH": PushMessageActivityTypeDef,
         "RandomSplit": RandomSplitActivityOutputTypeDef,
-        "SMS": SMSMessageActivityOutputTypeDef,
-        "Wait": WaitActivityOutputTypeDef,
-        "ContactCenter": ContactCenterActivityOutputTypeDef,
+        "SMS": SMSMessageActivityTypeDef,
+        "Wait": WaitActivityTypeDef,
+        "ContactCenter": ContactCenterActivityTypeDef,
     },
     total=False,
 )
 
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
@@ -6928,26 +6409,26 @@
 )
 _OptionalJourneyResponseTypeDef = TypedDict(
     "_OptionalJourneyResponseTypeDef",
     {
         "Activities": Dict[str, ActivityOutputTypeDef],
         "CreationDate": str,
         "LastModifiedDate": str,
-        "Limits": JourneyLimitsOutputTypeDef,
+        "Limits": JourneyLimitsTypeDef,
         "LocalTime": bool,
-        "QuietTime": QuietTimeOutputTypeDef,
+        "QuietTime": QuietTimeTypeDef,
         "RefreshFrequency": str,
         "Schedule": JourneyScheduleOutputTypeDef,
         "StartActivity": str,
         "StartCondition": StartConditionOutputTypeDef,
         "State": StateType,
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
-        "JourneyChannelSettings": JourneyChannelSettingsOutputTypeDef,
+        "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
         "OpenHours": OpenHoursOutputTypeDef,
         "ClosedDays": ClosedDaysOutputTypeDef,
         "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.28.12
-Summary: Type annotations for boto3.Pinpoint 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
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
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,74 +329,61 @@
 from mypy_boto3_pinpoint.type_defs import (
     ADMChannelRequestTypeDef,
     ADMChannelResponseTypeDef,
     ADMMessageTypeDef,
     APNSChannelRequestTypeDef,
     APNSChannelResponseTypeDef,
     APNSMessageTypeDef,
-    APNSPushNotificationTemplateOutputTypeDef,
     APNSPushNotificationTemplateTypeDef,
     APNSSandboxChannelRequestTypeDef,
     APNSSandboxChannelResponseTypeDef,
     APNSVoipChannelRequestTypeDef,
     APNSVoipChannelResponseTypeDef,
     APNSVoipSandboxChannelRequestTypeDef,
     APNSVoipSandboxChannelResponseTypeDef,
     ActivityResponseTypeDef,
-    ContactCenterActivityOutputTypeDef,
-    HoldoutActivityOutputTypeDef,
     ContactCenterActivityTypeDef,
     HoldoutActivityTypeDef,
     AddressConfigurationTypeDef,
-    AndroidPushNotificationTemplateOutputTypeDef,
     AndroidPushNotificationTemplateTypeDef,
     ApplicationResponseTypeDef,
-    CampaignHookOutputTypeDef,
-    CampaignLimitsOutputTypeDef,
-    QuietTimeOutputTypeDef,
+    JourneyTimeframeCapTypeDef,
+    CampaignHookTypeDef,
+    CampaignLimitsTypeDef,
+    QuietTimeTypeDef,
     AttributeDimensionOutputTypeDef,
     AttributeDimensionTypeDef,
     AttributesResourceTypeDef,
     BaiduChannelRequestTypeDef,
     BaiduChannelResponseTypeDef,
     BaiduMessageTypeDef,
-    CampaignCustomMessageOutputTypeDef,
     CampaignCustomMessageTypeDef,
-    CampaignEmailMessageOutputTypeDef,
     CampaignEmailMessageTypeDef,
-    CampaignHookTypeDef,
-    CampaignLimitsTypeDef,
     CampaignStateTypeDef,
     CustomDeliveryConfigurationOutputTypeDef,
-    CampaignSmsMessageOutputTypeDef,
     CampaignSmsMessageTypeDef,
     ChannelResponseTypeDef,
-    ClosedDaysRuleOutputTypeDef,
     ClosedDaysRuleTypeDef,
-    WaitTimeOutputTypeDef,
     WaitTimeTypeDef,
     CreateApplicationRequestTypeDef,
     ResponseMetadataTypeDef,
     EmailTemplateRequestTypeDef,
     CreateTemplateMessageBodyTypeDef,
     ExportJobRequestTypeDef,
     ImportJobRequestTypeDef,
     TemplateCreateMessageBodyTypeDef,
     CreateRecommenderConfigurationTypeDef,
     RecommenderConfigurationResponseTypeDef,
     SMSTemplateRequestTypeDef,
     VoiceTemplateRequestTypeDef,
     CustomDeliveryConfigurationTypeDef,
-    JourneyCustomMessageOutputTypeDef,
     JourneyCustomMessageTypeDef,
-    DefaultButtonConfigurationOutputTypeDef,
     DefaultButtonConfigurationTypeDef,
     DefaultMessageTypeDef,
     DefaultPushNotificationMessageTypeDef,
-    DefaultPushNotificationTemplateOutputTypeDef,
     DefaultPushNotificationTemplateTypeDef,
     DeleteAdmChannelRequestRequestTypeDef,
     DeleteApnsChannelRequestRequestTypeDef,
     DeleteApnsSandboxChannelRequestRequestTypeDef,
     DeleteApnsVoipChannelRequestRequestTypeDef,
     DeleteApnsVoipSandboxChannelRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
@@ -423,36 +410,31 @@
     DeleteVoiceChannelRequestRequestTypeDef,
     VoiceChannelResponseTypeDef,
     DeleteVoiceTemplateRequestRequestTypeDef,
     GCMMessageTypeDef,
     SMSMessageTypeDef,
     VoiceMessageTypeDef,
     EmailChannelRequestTypeDef,
-    JourneyEmailMessageOutputTypeDef,
     JourneyEmailMessageTypeDef,
     RawEmailTypeDef,
     EmailTemplateResponseTypeDef,
     EndpointDemographicTypeDef,
     EndpointLocationTypeDef,
     EndpointUserTypeDef,
-    EndpointDemographicOutputTypeDef,
     EndpointItemResponseTypeDef,
-    EndpointLocationOutputTypeDef,
     EndpointMessageResultTypeDef,
     EndpointUserOutputTypeDef,
     EndpointSendConfigurationTypeDef,
-    MetricDimensionOutputTypeDef,
-    SetDimensionOutputTypeDef,
     MetricDimensionTypeDef,
+    SetDimensionOutputTypeDef,
     SetDimensionTypeDef,
     EventItemResponseTypeDef,
     SessionTypeDef,
     ExportJobResourceTypeDef,
     GCMChannelRequestTypeDef,
-    GPSCoordinatesOutputTypeDef,
     GPSCoordinatesTypeDef,
     GetAdmChannelRequestRequestTypeDef,
     GetApnsChannelRequestRequestTypeDef,
     GetApnsSandboxChannelRequestRequestTypeDef,
     GetApnsVoipChannelRequestRequestTypeDef,
     GetApnsVoipSandboxChannelRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
@@ -502,63 +484,47 @@
     GetSmsTemplateRequestRequestTypeDef,
     SMSTemplateResponseTypeDef,
     GetUserEndpointsRequestRequestTypeDef,
     GetVoiceChannelRequestRequestTypeDef,
     GetVoiceTemplateRequestRequestTypeDef,
     VoiceTemplateResponseTypeDef,
     ImportJobResourceTypeDef,
-    InAppMessageBodyConfigOutputTypeDef,
     InAppMessageBodyConfigTypeDef,
-    OverrideButtonConfigurationOutputTypeDef,
     OverrideButtonConfigurationTypeDef,
-    InAppMessageHeaderConfigOutputTypeDef,
     InAppMessageHeaderConfigTypeDef,
-    JourneyChannelSettingsOutputTypeDef,
     JourneyChannelSettingsTypeDef,
-    JourneyLimitsOutputTypeDef,
-    JourneyLimitsTypeDef,
-    JourneyPushMessageOutputTypeDef,
     JourneyPushMessageTypeDef,
     JourneyScheduleOutputTypeDef,
     JourneyRunResponseTypeDef,
-    JourneySMSMessageOutputTypeDef,
     JourneySMSMessageTypeDef,
     JourneyScheduleTypeDef,
     JourneyStateRequestTypeDef,
     ListJourneysRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagsModelOutputTypeDef,
     ListTemplateVersionsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
-    MessageOutputTypeDef,
     MessageTypeDef,
     MessageResultTypeDef,
     NumberValidateRequestTypeDef,
     NumberValidateResponseTypeDef,
-    OpenHoursRuleOutputTypeDef,
     OpenHoursRuleTypeDef,
     WriteEventStreamTypeDef,
-    QuietTimeTypeDef,
-    RandomSplitEntryOutputTypeDef,
     RandomSplitEntryTypeDef,
-    RecencyDimensionOutputTypeDef,
     RecencyDimensionTypeDef,
     UpdateAttributesRequestTypeDef,
     ResultRowValueTypeDef,
     SMSChannelRequestTypeDef,
-    SegmentConditionOutputTypeDef,
     SegmentConditionTypeDef,
-    SegmentReferenceOutputTypeDef,
     SegmentReferenceTypeDef,
     SegmentImportResourceTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SimpleEmailPartTypeDef,
     TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
-    TemplateOutputTypeDef,
     TemplateTypeDef,
     TemplateResponseTypeDef,
     TemplateVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRecommenderConfigurationTypeDef,
     VoiceChannelRequestTypeDef,
     VerificationResponseTypeDef,
@@ -566,20 +532,20 @@
     UpdateAdmChannelRequestRequestTypeDef,
     UpdateApnsChannelRequestRequestTypeDef,
     UpdateApnsSandboxChannelRequestRequestTypeDef,
     UpdateApnsVoipChannelRequestRequestTypeDef,
     UpdateApnsVoipSandboxChannelRequestRequestTypeDef,
     ActivitiesResponseTypeDef,
     ApplicationsResponseTypeDef,
-    ApplicationSettingsResourceTypeDef,
+    ApplicationSettingsJourneyLimitsTypeDef,
+    JourneyLimitsTypeDef,
     UpdateBaiduChannelRequestRequestTypeDef,
     ChannelsResponseTypeDef,
     ClosedDaysOutputTypeDef,
     ClosedDaysTypeDef,
-    WaitActivityOutputTypeDef,
     WaitActivityTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppResponseTypeDef,
     DeleteAdmChannelResponseTypeDef,
     DeleteApnsChannelResponseTypeDef,
     DeleteApnsSandboxChannelResponseTypeDef,
     DeleteApnsVoipChannelResponseTypeDef,
@@ -618,16 +584,16 @@
     UpdateRecommenderConfigurationResponseTypeDef,
     CreateSmsTemplateRequestRequestTypeDef,
     UpdateSmsTemplateRequestRequestTypeDef,
     CreateVoiceTemplateRequestRequestTypeDef,
     UpdateVoiceTemplateRequestRequestTypeDef,
     CustomMessageActivityOutputTypeDef,
     CustomMessageActivityTypeDef,
-    PushNotificationTemplateResponseTypeDef,
     PushNotificationTemplateRequestTypeDef,
+    PushNotificationTemplateResponseTypeDef,
     DeleteEmailChannelResponseTypeDef,
     GetEmailChannelResponseTypeDef,
     UpdateEmailChannelResponseTypeDef,
     DeleteEmailTemplateResponseTypeDef,
     DeleteInAppTemplateResponseTypeDef,
     DeletePushTemplateResponseTypeDef,
     DeleteSmsTemplateResponseTypeDef,
@@ -649,15 +615,14 @@
     DeleteSmsChannelResponseTypeDef,
     GetSmsChannelResponseTypeDef,
     UpdateSmsChannelResponseTypeDef,
     DeleteVoiceChannelResponseTypeDef,
     GetVoiceChannelResponseTypeDef,
     UpdateVoiceChannelResponseTypeDef,
     UpdateEmailChannelRequestRequestTypeDef,
-    EmailMessageActivityOutputTypeDef,
     EmailMessageActivityTypeDef,
     GetEmailTemplateResponseTypeDef,
     EndpointBatchItemTypeDef,
     EndpointRequestTypeDef,
     PublicEndpointTypeDef,
     SendUsersMessageResponseTypeDef,
     EndpointResponseTypeDef,
@@ -665,67 +630,60 @@
     SegmentDemographicsOutputTypeDef,
     EventDimensionsTypeDef,
     SegmentDemographicsTypeDef,
     ItemResponseTypeDef,
     EventTypeDef,
     ExportJobResponseTypeDef,
     UpdateGcmChannelRequestRequestTypeDef,
-    GPSPointDimensionOutputTypeDef,
     GPSPointDimensionTypeDef,
     GetJourneyExecutionActivityMetricsResponseTypeDef,
     GetJourneyExecutionMetricsResponseTypeDef,
     GetJourneyRunExecutionActivityMetricsResponseTypeDef,
     GetJourneyRunExecutionMetricsResponseTypeDef,
     GetSmsTemplateResponseTypeDef,
     GetVoiceTemplateResponseTypeDef,
     ImportJobResponseTypeDef,
-    InAppMessageButtonOutputTypeDef,
     InAppMessageButtonTypeDef,
-    PushMessageActivityOutputTypeDef,
     PushMessageActivityTypeDef,
     JourneyRunsResponseTypeDef,
-    SMSMessageActivityOutputTypeDef,
     SMSMessageActivityTypeDef,
     UpdateJourneyStateRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageResponseTypeDef,
     PhoneNumberValidateRequestRequestTypeDef,
     PhoneNumberValidateResponseTypeDef,
     OpenHoursOutputTypeDef,
     OpenHoursTypeDef,
     PutEventStreamRequestRequestTypeDef,
-    WriteApplicationSettingsRequestTypeDef,
     RandomSplitActivityOutputTypeDef,
     RandomSplitActivityTypeDef,
-    SegmentBehaviorsOutputTypeDef,
     SegmentBehaviorsTypeDef,
     RemoveAttributesRequestRequestTypeDef,
     ResultRowTypeDef,
     UpdateSmsChannelRequestRequestTypeDef,
     SendOTPMessageRequestRequestTypeDef,
     SimpleEmailTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateTemplateActiveVersionRequestRequestTypeDef,
-    TemplateConfigurationOutputTypeDef,
     TemplateConfigurationTypeDef,
     TemplatesResponseTypeDef,
     TemplateVersionsResponseTypeDef,
     UpdateRecommenderConfigurationRequestRequestTypeDef,
     UpdateVoiceChannelRequestRequestTypeDef,
     VerifyOTPMessageResponseTypeDef,
     VerifyOTPMessageRequestRequestTypeDef,
     GetCampaignActivitiesResponseTypeDef,
     GetAppsResponseTypeDef,
-    GetApplicationSettingsResponseTypeDef,
-    UpdateApplicationSettingsResponseTypeDef,
+    ApplicationSettingsResourceTypeDef,
+    WriteApplicationSettingsRequestTypeDef,
     GetChannelsResponseTypeDef,
     GetRecommenderConfigurationsResponseTypeDef,
-    GetPushTemplateResponseTypeDef,
     CreatePushTemplateRequestRequestTypeDef,
     UpdatePushTemplateRequestRequestTypeDef,
+    GetPushTemplateResponseTypeDef,
     EndpointBatchRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     EndpointsResponseTypeDef,
     GetEndpointResponseTypeDef,
     CampaignEventFilterOutputTypeDef,
@@ -740,24 +698,25 @@
     ExportJobsResponseTypeDef,
     GetExportJobResponseTypeDef,
     SegmentLocationOutputTypeDef,
     SegmentLocationTypeDef,
     CreateImportJobResponseTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobsResponseTypeDef,
-    InAppMessageContentOutputTypeDef,
     InAppMessageContentTypeDef,
     GetJourneyRunsResponseTypeDef,
     SendMessagesResponseTypeDef,
     SendOTPMessageResponseTypeDef,
-    UpdateApplicationSettingsRequestRequestTypeDef,
     BaseKpiResultTypeDef,
     EmailMessageTypeDef,
     ListTemplatesResponseTypeDef,
     ListTemplateVersionsResponseTypeDef,
+    GetApplicationSettingsResponseTypeDef,
+    UpdateApplicationSettingsResponseTypeDef,
+    UpdateApplicationSettingsRequestRequestTypeDef,
     UpdateEndpointsBatchRequestRequestTypeDef,
     DeleteUserEndpointsResponseTypeDef,
     GetUserEndpointsResponseTypeDef,
     InAppCampaignScheduleTypeDef,
     ScheduleOutputTypeDef,
     EventStartConditionOutputTypeDef,
     ScheduleTypeDef,
@@ -767,60 +726,60 @@
     GetExportJobsResponseTypeDef,
     GetSegmentExportJobsResponseTypeDef,
     SegmentDimensionsOutputTypeDef,
     SegmentDimensionsTypeDef,
     GetImportJobsResponseTypeDef,
     GetSegmentImportJobsResponseTypeDef,
     CampaignInAppMessageOutputTypeDef,
-    InAppMessageTypeDef,
-    InAppTemplateResponseTypeDef,
     CampaignInAppMessageTypeDef,
+    InAppMessageTypeDef,
     InAppTemplateRequestTypeDef,
+    InAppTemplateResponseTypeDef,
     ApplicationDateRangeKpiResponseTypeDef,
     CampaignDateRangeKpiResponseTypeDef,
     JourneyDateRangeKpiResponseTypeDef,
     DirectMessageConfigurationTypeDef,
     StartConditionOutputTypeDef,
     StartConditionTypeDef,
     PutEventsRequestRequestTypeDef,
     SegmentGroupOutputTypeDef,
     SimpleConditionOutputTypeDef,
     SegmentGroupTypeDef,
     SimpleConditionTypeDef,
     MessageConfigurationOutputTypeDef,
-    InAppMessageCampaignTypeDef,
-    GetInAppTemplateResponseTypeDef,
     MessageConfigurationTypeDef,
+    InAppMessageCampaignTypeDef,
     CreateInAppTemplateRequestRequestTypeDef,
     UpdateInAppTemplateRequestRequestTypeDef,
+    GetInAppTemplateResponseTypeDef,
     GetApplicationDateRangeKpiResponseTypeDef,
     GetCampaignDateRangeKpiResponseTypeDef,
     GetJourneyDateRangeKpiResponseTypeDef,
     MessageRequestTypeDef,
     SendUsersMessageRequestTypeDef,
     SegmentGroupListOutputTypeDef,
     ConditionOutputTypeDef,
     MultiConditionalBranchOutputTypeDef,
     SegmentGroupListTypeDef,
     ConditionTypeDef,
     MultiConditionalBranchTypeDef,
     TreatmentResourceTypeDef,
-    InAppMessagesResponseTypeDef,
     WriteTreatmentResourceTypeDef,
+    InAppMessagesResponseTypeDef,
     SendMessagesRequestRequestTypeDef,
     SendUsersMessagesRequestRequestTypeDef,
     SegmentResponseTypeDef,
     ConditionalSplitActivityOutputTypeDef,
     MultiConditionalSplitActivityOutputTypeDef,
     WriteSegmentRequestTypeDef,
     ConditionalSplitActivityTypeDef,
     MultiConditionalSplitActivityTypeDef,
     CampaignResponseTypeDef,
-    GetInAppMessagesResponseTypeDef,
     WriteCampaignRequestTypeDef,
+    GetInAppMessagesResponseTypeDef,
     CreateSegmentResponseTypeDef,
     DeleteSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     GetSegmentVersionResponseTypeDef,
     SegmentsResponseTypeDef,
     UpdateSegmentResponseTypeDef,
     ActivityOutputTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.28.12/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.28.15/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.28.12/setup.py` & `mypy-boto3-pinpoint-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pinpoint 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Pinpoint 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

