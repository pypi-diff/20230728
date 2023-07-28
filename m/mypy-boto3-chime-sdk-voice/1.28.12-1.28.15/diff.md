# Comparing `tmp/mypy-boto3-chime-sdk-voice-1.28.12.tar.gz` & `tmp/mypy-boto3-chime-sdk-voice-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-voice-1.28.12.tar` & `mypy-boto3-chime-sdk-voice-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66722 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66620 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75322 2023-07-27 05:18:22.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-07-27 05:18:22.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:24.000000 mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.276564 mypy-boto3-chime-sdk-voice-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-27 05:18:20.000000 mypy-boto3-chime-sdk-voice-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23696 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66722 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66620 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-28 20:20:43.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71721 2023-07-28 20:20:46.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71668 2023-07-28 20:20:44.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23696 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:25.000000 mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.332780 mypy-boto3-chime-sdk-voice-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-28 20:20:42.000000 mypy-boto3-chime-sdk-voice-1.28.15/setup.py
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/LICENSE` & `mypy-boto3-chime-sdk-voice-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKVoice 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,14 +350,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.type_defs import (
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
@@ -368,15 +369,14 @@
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
-    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
@@ -386,169 +386,171 @@
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GeoMatchParamsOutputTypeDef,
-    VoiceConnectorSettingsOutputTypeDef,
+    VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationOutputTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationOutputTypeDef,
+    LoggingConfigurationTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationOutputTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
-    ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
-    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
-    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
-    LoggingConfigurationTypeDef,
-    MediaInsightsConfigurationOutputTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
-    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     TerminationTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
-    SipMediaApplicationEndpointOutputTypeDef,
-    SipRuleTargetApplicationOutputTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
-    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
-    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     UpdateVoiceProfileDomainRequestRequestTypeDef,
     UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    VoiceConnectorItemOutputTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAvailableVoiceConnectorRegionsResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
+    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
+    SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
+    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
+    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
-    VoiceProfileDomainTypeDef,
-    SipMediaApplicationTypeDef,
-    SipRuleTypeDef,
     SpeakerSearchDetailsTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     GetVoiceToneAnalysisTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
@@ -558,33 +560,18 @@
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
-    CreateVoiceProfileDomainResponseTypeDef,
-    GetVoiceProfileDomainResponseTypeDef,
-    UpdateVoiceProfileDomainResponseTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
     SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
     GetSpeakerSearchTaskResponseTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/README.md` & `mypy-boto3-chime-sdk-voice-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,14 +318,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.type_defs import (
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
@@ -336,15 +337,14 @@
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
-    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
@@ -354,169 +354,171 @@
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GeoMatchParamsOutputTypeDef,
-    VoiceConnectorSettingsOutputTypeDef,
+    VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationOutputTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationOutputTypeDef,
+    LoggingConfigurationTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationOutputTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
-    ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
-    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
-    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
-    LoggingConfigurationTypeDef,
-    MediaInsightsConfigurationOutputTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
-    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     TerminationTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
-    SipMediaApplicationEndpointOutputTypeDef,
-    SipRuleTargetApplicationOutputTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
-    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
-    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     UpdateVoiceProfileDomainRequestRequestTypeDef,
     UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    VoiceConnectorItemOutputTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAvailableVoiceConnectorRegionsResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
+    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
+    SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
+    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
+    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
-    VoiceProfileDomainTypeDef,
-    SipMediaApplicationTypeDef,
-    SipRuleTypeDef,
     SpeakerSearchDetailsTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     GetVoiceToneAnalysisTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
@@ -526,33 +528,18 @@
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
-    CreateVoiceProfileDomainResponseTypeDef,
-    GetVoiceProfileDomainResponseTypeDef,
-    UpdateVoiceProfileDomainResponseTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
     SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
     GetSpeakerSearchTaskResponseTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.py` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__init__.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/__main__.py` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKVoice 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKVoice 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice\nOther"
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

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.py` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/client.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.py` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/literals.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.py` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListSipMediaApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSipMediaApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
         """
 
 
 class ListSipRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
     """
 
     def paginate(
-        self, *, SipMediaApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SipMediaApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSipRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
         """
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/paginator.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListSipMediaApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSipMediaApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
         """
 
 class ListSipRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
     """
 
     def paginate(
-        self, *, SipMediaApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SipMediaApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSipRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
         """
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.py` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "CallDetailsTypeDef",
     "CandidateAddressTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
@@ -65,15 +65,14 @@
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
     "VoiceConnectorTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "CreateVoiceProfileRequestRequestTypeDef",
     "VoiceProfileTypeDef",
     "CredentialTypeDef",
-    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
     "DeleteSipRuleRequestRequestTypeDef",
     "DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorGroupRequestRequestTypeDef",
@@ -83,169 +82,171 @@
     "DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     "DeleteVoiceProfileDomainRequestRequestTypeDef",
     "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GeoMatchParamsOutputTypeDef",
-    "VoiceConnectorSettingsOutputTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    "LoggingConfigurationOutputTypeDef",
+    "LoggingConfigurationTypeDef",
     "GetVoiceConnectorOriginationRequestRequestTypeDef",
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationOutputTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "ListVoiceProfileDomainsRequestRequestTypeDef",
     "VoiceProfileDomainSummaryTypeDef",
     "ListVoiceProfilesRequestRequestTypeDef",
     "VoiceProfileSummaryTypeDef",
-    "LoggingConfigurationTypeDef",
-    "MediaInsightsConfigurationOutputTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
-    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "TerminationTypeDef",
-    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    "SipMediaApplicationEndpointOutputTypeDef",
-    "SipRuleTargetApplicationOutputTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
-    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "UpdateVoiceProfileDomainRequestRequestTypeDef",
     "UpdateVoiceProfileRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
-    "VoiceConnectorItemOutputTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
+    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSipRuleRequestRequestTypeDef",
+    "SipRuleTypeDef",
     "UpdateSipRuleRequestRequestTypeDef",
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
+    "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
+    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
+    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    "VoiceProfileDomainTypeDef",
-    "SipMediaApplicationTypeDef",
-    "SipRuleTypeDef",
     "SpeakerSearchDetailsTypeDef",
     "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    "VoiceConnectorGroupTypeDef",
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     "StartVoiceToneAnalysisTaskResponseTypeDef",
+    "CreateSipMediaApplicationResponseTypeDef",
+    "GetSipMediaApplicationResponseTypeDef",
+    "ListSipMediaApplicationsResponseTypeDef",
+    "UpdateSipMediaApplicationResponseTypeDef",
+    "CreateSipRuleResponseTypeDef",
+    "GetSipRuleResponseTypeDef",
+    "ListSipRulesResponseTypeDef",
+    "UpdateSipRuleResponseTypeDef",
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    "GetVoiceConnectorGroupResponseTypeDef",
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    "UpdateVoiceConnectorGroupResponseTypeDef",
+    "CreateVoiceProfileDomainResponseTypeDef",
+    "GetVoiceProfileDomainResponseTypeDef",
+    "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
@@ -255,33 +256,18 @@
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
-    "CreateVoiceProfileDomainResponseTypeDef",
-    "GetVoiceProfileDomainResponseTypeDef",
-    "UpdateVoiceProfileDomainResponseTypeDef",
-    "CreateSipMediaApplicationResponseTypeDef",
-    "GetSipMediaApplicationResponseTypeDef",
-    "ListSipMediaApplicationsResponseTypeDef",
-    "UpdateSipMediaApplicationResponseTypeDef",
-    "CreateSipRuleResponseTypeDef",
-    "GetSipRuleResponseTypeDef",
-    "ListSipRulesResponseTypeDef",
-    "UpdateSipRuleResponseTypeDef",
     "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    "GetVoiceConnectorGroupResponseTypeDef",
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetSpeakerSearchTaskResponseTypeDef",
     "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
@@ -310,32 +296,41 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
-
 class AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
-
 PhoneNumberErrorTypeDef = TypedDict(
     "PhoneNumberErrorTypeDef",
     {
         "PhoneNumberId": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
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
 _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -343,22 +338,20 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
-
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
-
 BatchDeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
     },
 )
 
@@ -373,21 +366,19 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
-
 class UpdatePhoneNumberRequestItemTypeDef(
     _RequiredUpdatePhoneNumberRequestItemTypeDef, _OptionalUpdatePhoneNumberRequestItemTypeDef
 ):
     pass
 
-
 CallDetailsTypeDef = TypedDict(
     "CallDetailsTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "IsCaller": bool,
     },
@@ -437,22 +428,20 @@
     {
         "SipHeaders": Mapping[str, str],
         "ArgumentsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSipMediaApplicationCallRequestRequestTypeDef(
     _RequiredCreateSipMediaApplicationCallRequestRequestTypeDef,
     _OptionalCreateSipMediaApplicationCallRequestRequestTypeDef,
 ):
     pass
 
-
 SipMediaApplicationCallTypeDef = TypedDict(
     "SipMediaApplicationCallTypeDef",
     {
         "TransactionId": str,
     },
     total=False,
 )
@@ -538,37 +527,14 @@
     {
         "Username": str,
         "Password": str,
     },
     total=False,
 )
 
-_RequiredDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDNISEmergencyCallingConfigurationOutputTypeDef",
-    {
-        "EmergencyPhoneNumber": str,
-        "CallingCountry": str,
-    },
-)
-_OptionalDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDNISEmergencyCallingConfigurationOutputTypeDef",
-    {
-        "TestPhoneNumber": str,
-    },
-    total=False,
-)
-
-
-class DNISEmergencyCallingConfigurationOutputTypeDef(
-    _RequiredDNISEmergencyCallingConfigurationOutputTypeDef,
-    _OptionalDNISEmergencyCallingConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredDNISEmergencyCallingConfigurationTypeDef = TypedDict(
     "_RequiredDNISEmergencyCallingConfigurationTypeDef",
     {
         "EmergencyPhoneNumber": str,
         "CallingCountry": str,
     },
 )
@@ -576,22 +542,20 @@
     "_OptionalDNISEmergencyCallingConfigurationTypeDef",
     {
         "TestPhoneNumber": str,
     },
     total=False,
 )
 
-
 class DNISEmergencyCallingConfigurationTypeDef(
     _RequiredDNISEmergencyCallingConfigurationTypeDef,
     _OptionalDNISEmergencyCallingConfigurationTypeDef,
 ):
     pass
 
-
 DeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "DeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -700,31 +664,16 @@
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GeoMatchParamsOutputTypeDef = TypedDict(
-    "GeoMatchParamsOutputTypeDef",
-    {
-        "Country": str,
-        "AreaCode": str,
-    },
-)
-
-VoiceConnectorSettingsOutputTypeDef = TypedDict(
-    "VoiceConnectorSettingsOutputTypeDef",
+VoiceConnectorSettingsTypeDef = TypedDict(
+    "VoiceConnectorSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetPhoneNumberOrderRequestRequestTypeDef = TypedDict(
@@ -737,23 +686,14 @@
 GetPhoneNumberRequestRequestTypeDef = TypedDict(
     "GetPhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
-    {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProxySessionRequestRequestTypeDef = TypedDict(
     "GetProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "ProxySessionId": str,
     },
 )
@@ -776,16 +716,16 @@
 GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 
-SipMediaApplicationLoggingConfigurationOutputTypeDef = TypedDict(
-    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
+SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     {
         "EnableSipMediaApplicationMessageLogs": bool,
     },
     total=False,
 )
 
 GetSipMediaApplicationRequestRequestTypeDef = TypedDict(
@@ -827,16 +767,16 @@
 GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-LoggingConfigurationOutputTypeDef = TypedDict(
-    "LoggingConfigurationOutputTypeDef",
+LoggingConfigurationTypeDef = TypedDict(
+    "LoggingConfigurationTypeDef",
     {
         "EnableSIPLogs": bool,
         "EnableMediaMetricLogs": bool,
     },
     total=False,
 )
 
@@ -933,22 +873,14 @@
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
         "IsCaller": bool,
     },
 )
 
-ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
-    {
-        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPhoneNumberOrdersRequestRequestTypeDef = TypedDict(
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -979,47 +911,38 @@
         "Status": ProxySessionStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListProxySessionsRequestRequestTypeDef(
     _RequiredListProxySessionsRequestRequestTypeDef, _OptionalListProxySessionsRequestRequestTypeDef
 ):
     pass
 
-
-ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
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
 
 ListSipMediaApplicationsRequestRequestTypeDef = TypedDict(
     "ListSipMediaApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSipRulesRequestRequestTypeDef = TypedDict(
     "ListSipRulesRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1045,22 +968,14 @@
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
 ListVoiceConnectorGroupsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1069,22 +984,14 @@
 ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    {
-        "Usernames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVoiceConnectorsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1123,52 +1030,32 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListVoiceProfilesRequestRequestTypeDef(
     _RequiredListVoiceProfilesRequestRequestTypeDef, _OptionalListVoiceProfilesRequestRequestTypeDef
 ):
     pass
 
-
 VoiceProfileSummaryTypeDef = TypedDict(
     "VoiceProfileSummaryTypeDef",
     {
         "VoiceProfileId": str,
         "VoiceProfileArn": str,
         "VoiceProfileDomainId": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ExpirationTimestamp": datetime,
     },
     total=False,
 )
 
-LoggingConfigurationTypeDef = TypedDict(
-    "LoggingConfigurationTypeDef",
-    {
-        "EnableSIPLogs": bool,
-        "EnableMediaMetricLogs": bool,
-    },
-    total=False,
-)
-
-MediaInsightsConfigurationOutputTypeDef = TypedDict(
-    "MediaInsightsConfigurationOutputTypeDef",
-    {
-        "Disabled": bool,
-        "ConfigurationArn": str,
-    },
-    total=False,
-)
-
 MediaInsightsConfigurationTypeDef = TypedDict(
     "MediaInsightsConfigurationTypeDef",
     {
         "Disabled": bool,
         "ConfigurationArn": str,
     },
     total=False,
@@ -1179,48 +1066,26 @@
     {
         "E164PhoneNumber": str,
         "Status": OrderedPhoneNumberStatusType,
     },
     total=False,
 )
 
-OriginationRouteOutputTypeDef = TypedDict(
-    "OriginationRouteOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Protocol": OriginationRouteProtocolType,
-        "Priority": int,
-        "Weight": int,
-    },
-    total=False,
-)
-
 OriginationRouteTypeDef = TypedDict(
     "OriginationRouteTypeDef",
     {
         "Host": str,
         "Port": int,
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
         "Weight": int,
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
 ParticipantTypeDef = TypedDict(
     "ParticipantTypeDef",
     {
         "PhoneNumber": str,
         "ProxyPhoneNumber": str,
     },
     total=False,
@@ -1253,22 +1118,14 @@
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     {
         "AlexaSkillStatus": AlexaSkillStatusType,
         "AlexaSkillIds": Sequence[str],
     },
 )
 
-SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationLoggingConfigurationTypeDef",
-    {
-        "EnableSipMediaApplicationMessageLogs": bool,
-    },
-    total=False,
-)
-
 _RequiredPutVoiceConnectorProxyRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorProxyRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "DefaultSessionExpiryMinutes": int,
         "PhoneNumberPoolCountries": Sequence[str],
     },
@@ -1278,45 +1135,32 @@
     {
         "FallBackPhoneNumber": str,
         "Disabled": bool,
     },
     total=False,
 )
 
-
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
-
 TerminationTypeDef = TypedDict(
     "TerminationTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": Sequence[str],
         "CidrAllowedList": Sequence[str],
         "Disabled": bool,
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -1331,48 +1175,14 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-)
-
-SipMediaApplicationEndpointOutputTypeDef = TypedDict(
-    "SipMediaApplicationEndpointOutputTypeDef",
-    {
-        "LambdaArn": str,
-    },
-    total=False,
-)
-
-SipRuleTargetApplicationOutputTypeDef = TypedDict(
-    "SipRuleTargetApplicationOutputTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "Priority": int,
-        "AwsRegion": str,
-    },
-    total=False,
-)
-
 SpeakerSearchResultTypeDef = TypedDict(
     "SpeakerSearchResultTypeDef",
     {
         "ConfidenceScore": float,
         "VoiceProfileId": str,
     },
     total=False,
@@ -1391,22 +1201,20 @@
     {
         "ClientRequestToken": str,
         "CallLeg": CallLegTypeType,
     },
     total=False,
 )
 
-
 class StartSpeakerSearchTaskRequestRequestTypeDef(
     _RequiredStartSpeakerSearchTaskRequestRequestTypeDef,
     _OptionalStartSpeakerSearchTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "LanguageCode": Literal["en-US"],
     },
@@ -1415,22 +1223,20 @@
     "_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class StartVoiceToneAnalysisTaskRequestRequestTypeDef(
     _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef,
     _OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef,
 ):
     pass
 
-
 StopSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1439,22 +1245,14 @@
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
     },
 )
 
-StreamingNotificationTargetOutputTypeDef = TypedDict(
-    "StreamingNotificationTargetOutputTypeDef",
-    {
-        "NotificationTarget": NotificationTargetType,
-    },
-    total=False,
-)
-
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
     total=False,
 )
@@ -1463,22 +1261,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-VoiceConnectorSettingsTypeDef = TypedDict(
-    "VoiceConnectorSettingsTypeDef",
-    {
-        "CdrBucket": str,
-    },
-    total=False,
-)
-
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -1486,21 +1276,19 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
-
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
-
 UpdatePhoneNumberSettingsRequestRequestTypeDef = TypedDict(
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     {
         "CallingName": str,
     },
 )
 
@@ -1516,22 +1304,20 @@
     "_OptionalUpdateProxySessionRequestRequestTypeDef",
     {
         "ExpiryMinutes": int,
     },
     total=False,
 )
 
-
 class UpdateProxySessionRequestRequestTypeDef(
     _RequiredUpdateProxySessionRequestRequestTypeDef,
     _OptionalUpdateProxySessionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateSipMediaApplicationCallRequestRequestTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "TransactionId": str,
         "Arguments": Mapping[str, str],
     },
@@ -1557,22 +1343,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredUpdateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalUpdateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateVoiceProfileRequestRequestTypeDef = TypedDict(
     "UpdateVoiceProfileRequestRequestTypeDef",
     {
         "VoiceProfileId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1586,67 +1370,100 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
-VoiceConnectorItemOutputTypeDef = TypedDict(
-    "VoiceConnectorItemOutputTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Priority": int,
-    },
-)
-
 AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeletePhoneNumberResponseTypeDef = TypedDict(
     "BatchDeletePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
     "BatchUpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
+GetPhoneNumberSettingsResponseTypeDef = TypedDict(
+    "GetPhoneNumberSettingsResponseTypeDef",
+    {
+        "CallingName": str,
+        "CallingNameUpdatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
+    {
+        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    {
+        "Usernames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    {
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
@@ -1670,15 +1487,15 @@
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProxySessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1694,38 +1511,50 @@
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
         "GeoMatchParams": GeoMatchParamsTypeDef,
     },
     total=False,
 )
 
-
 class CreateProxySessionRequestRequestTypeDef(
     _RequiredCreateProxySessionRequestRequestTypeDef,
     _OptionalCreateProxySessionRequestRequestTypeDef,
 ):
     pass
 
-
 CreateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SipMediaApplicationTypeDef = TypedDict(
+    "SipMediaApplicationTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": List[SipMediaApplicationEndpointTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "SipMediaApplicationArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipMediaApplicationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 _OptionalUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
@@ -1733,22 +1562,20 @@
     {
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
     },
     total=False,
 )
 
-
 class UpdateSipMediaApplicationRequestRequestTypeDef(
     _RequiredUpdateSipMediaApplicationRequestRequestTypeDef,
     _OptionalUpdateSipMediaApplicationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
     },
@@ -1757,22 +1584,20 @@
     "_OptionalCreateSipMediaApplicationRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSipMediaApplicationRequestRequestTypeDef(
     _RequiredCreateSipMediaApplicationRequestRequestTypeDef,
     _OptionalCreateSipMediaApplicationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceConnectorRequestRequestTypeDef",
     {
         "Name": str,
         "RequireEncryption": bool,
     },
 )
@@ -1781,21 +1606,27 @@
     {
         "AwsRegion": VoiceConnectorAwsRegionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVoiceConnectorRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorRequestRequestTypeDef,
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
@@ -1814,20 +1645,33 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
-
 class CreateSipRuleRequestRequestTypeDef(
     _RequiredCreateSipRuleRequestRequestTypeDef, _OptionalCreateSipRuleRequestRequestTypeDef
 ):
     pass
 
+SipRuleTypeDef = TypedDict(
+    "SipRuleTypeDef",
+    {
+        "SipRuleId": str,
+        "Name": str,
+        "Disabled": bool,
+        "TriggerType": SipRuleTriggerTypeType,
+        "TriggerValue": str,
+        "TargetApplications": List[SipRuleTargetApplicationTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
 
 _RequiredUpdateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
     },
@@ -1837,82 +1681,91 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateSipRuleRequestRequestTypeDef(
     _RequiredUpdateSipRuleRequestRequestTypeDef, _OptionalUpdateSipRuleRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
     total=False,
 )
 
-
 class CreateVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorGroupId": str,
         "Name": str,
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
 )
 
+VoiceConnectorGroupTypeDef = TypedDict(
+    "VoiceConnectorGroupTypeDef",
+    {
+        "VoiceConnectorGroupId": str,
+        "Name": str,
+        "VoiceConnectorItems": List[VoiceConnectorItemTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "VoiceConnectorGroupArn": str,
+    },
+    total=False,
+)
+
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorResponseTypeDef = TypedDict(
     "GetVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceProfileDomainRequestRequestTypeDef",
     {
         "Name": str,
@@ -1925,43 +1778,55 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
 
 CreateVoiceProfileResponseTypeDef = TypedDict(
     "CreateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceProfileResponseTypeDef = TypedDict(
     "GetVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceProfileResponseTypeDef = TypedDict(
     "UpdateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1971,26 +1836,24 @@
     "_OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "Credentials": Sequence[CredentialTypeDef],
     },
     total=False,
 )
 
-
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
-
 EmergencyCallingConfigurationOutputTypeDef = TypedDict(
     "EmergencyCallingConfigurationOutputTypeDef",
     {
-        "DNIS": List[DNISEmergencyCallingConfigurationOutputTypeDef],
+        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
@@ -1998,154 +1861,187 @@
     },
     total=False,
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    {
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
     },
+    total=False,
 )
 
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": (
-            SipMediaApplicationLoggingConfigurationOutputTypeDef
-        ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationId": str,
+    },
+)
+_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
     },
+    total=False,
 )
 
+class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": (
-            SipMediaApplicationLoggingConfigurationOutputTypeDef
-        ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorProxyResponseTypeDef = TypedDict(
     "PutVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationHealthResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     {
         "TerminationHealth": TerminationHealthTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
-    "ListSupportedPhoneNumberCountriesResponseTypeDef",
+ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     {
-        "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
+    "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceProfilesResponseTypeDef = TypedDict(
     "ListVoiceProfilesResponseTypeDef",
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
@@ -2158,15 +2054,15 @@
     },
     total=False,
 )
 
 OriginationOutputTypeDef = TypedDict(
     "OriginationOutputTypeDef",
     {
-        "Routes": List[OriginationRouteOutputTypeDef],
+        "Routes": List[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
@@ -2188,15 +2084,15 @@
         "Capabilities": List[CapabilityType],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "EndedTimestamp": datetime,
         "Participants": List[ParticipantTypeDef],
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
-        "GeoMatchParams": GeoMatchParamsOutputTypeDef,
+        "GeoMatchParams": GeoMatchParamsTypeDef,
     },
     total=False,
 )
 
 PhoneNumberTypeDef = TypedDict(
     "PhoneNumberTypeDef",
     {
@@ -2230,95 +2126,28 @@
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
     },
     total=False,
 )
 
-
 class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
     _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-    },
-)
-_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
-    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Termination": TerminationTypeDef,
     },
 )
 
-VoiceProfileDomainTypeDef = TypedDict(
-    "VoiceProfileDomainTypeDef",
-    {
-        "VoiceProfileDomainId": str,
-        "VoiceProfileDomainArn": str,
-        "Name": str,
-        "Description": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
-SipMediaApplicationTypeDef = TypedDict(
-    "SipMediaApplicationTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "SipMediaApplicationArn": str,
-    },
-    total=False,
-)
-
-SipRuleTypeDef = TypedDict(
-    "SipRuleTypeDef",
-    {
-        "SipRuleId": str,
-        "Name": str,
-        "Disabled": bool,
-        "TriggerType": SipRuleTriggerTypeType,
-        "TriggerValue": str,
-        "TargetApplications": List[SipRuleTargetApplicationOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 SpeakerSearchDetailsTypeDef = TypedDict(
     "SpeakerSearchDetailsTypeDef",
     {
         "Results": List[SpeakerSearchResultTypeDef],
         "VoiceprintGenerationStatus": str,
     },
     total=False,
@@ -2330,27 +2159,25 @@
         "DataRetentionInHours": int,
         "Disabled": bool,
     },
 )
 _OptionalStreamingConfigurationOutputTypeDef = TypedDict(
     "_OptionalStreamingConfigurationOutputTypeDef",
     {
-        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
-        "MediaInsightsConfiguration": MediaInsightsConfigurationOutputTypeDef,
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StreamingConfigurationOutputTypeDef(
     _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
         "Disabled": bool,
     },
 )
@@ -2359,71 +2186,171 @@
     {
         "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
         "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
+GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
+    {
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
+StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
     {
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VoiceConnectorGroupTypeDef = TypedDict(
-    "VoiceConnectorGroupTypeDef",
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
     {
-        "VoiceConnectorGroupId": str,
-        "Name": str,
-        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "VoiceConnectorGroupArn": str,
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "GetVoiceToneAnalysisTaskResponseTypeDef",
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "StartVoiceToneAnalysisTaskResponseTypeDef",
+ListSipMediaApplicationsResponseTypeDef = TypedDict(
+    "ListSipMediaApplicationsResponseTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplications": List[SipMediaApplicationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSipMediaApplicationResponseTypeDef = TypedDict(
+    "UpdateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSipRuleResponseTypeDef = TypedDict(
+    "CreateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSipRuleResponseTypeDef = TypedDict(
+    "GetSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSipRulesResponseTypeDef = TypedDict(
+    "ListSipRulesResponseTypeDef",
+    {
+        "SipRules": List[SipRuleTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSipRuleResponseTypeDef = TypedDict(
+    "UpdateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "GetVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    {
+        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "UpdateVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "CreateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceProfileDomainResponseTypeDef = TypedDict(
+    "GetVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -2431,48 +2358,48 @@
     },
 )
 
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberOrderResponseTypeDef = TypedDict(
     "GetPhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "PutVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -2480,163 +2407,73 @@
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProxySessionResponseTypeDef = TypedDict(
     "GetProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberResponseTypeDef = TypedDict(
     "GetPhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePhoneNumberResponseTypeDef = TypedDict(
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "CreateVoiceProfileDomainResponseTypeDef",
-    {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetVoiceProfileDomainResponseTypeDef = TypedDict(
-    "GetVoiceProfileDomainResponseTypeDef",
-    {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "UpdateVoiceProfileDomainResponseTypeDef",
-    {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSipMediaApplicationResponseTypeDef = TypedDict(
-    "CreateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipMediaApplicationResponseTypeDef = TypedDict(
-    "GetSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipMediaApplicationsResponseTypeDef = TypedDict(
-    "ListSipMediaApplicationsResponseTypeDef",
-    {
-        "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipMediaApplicationResponseTypeDef = TypedDict(
-    "UpdateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSipRuleResponseTypeDef = TypedDict(
-    "CreateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipRuleResponseTypeDef = TypedDict(
-    "GetSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipRulesResponseTypeDef = TypedDict(
-    "ListSipRulesResponseTypeDef",
-    {
-        "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipRuleResponseTypeDef = TypedDict(
-    "UpdateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SpeakerSearchTaskTypeDef = TypedDict(
     "SpeakerSearchTaskTypeDef",
     {
         "SpeakerSearchTaskId": str,
@@ -2651,75 +2488,42 @@
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
-CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "GetVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    {
-        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "UpdateVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeakerSearchTaskResponseTypeDef = TypedDict(
     "StartSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice/type_defs.pyi` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddressTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "CallDetailsTypeDef",
     "CandidateAddressTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
@@ -64,15 +66,14 @@
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
     "VoiceConnectorTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "CreateVoiceProfileRequestRequestTypeDef",
     "VoiceProfileTypeDef",
     "CredentialTypeDef",
-    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
     "DeleteSipRuleRequestRequestTypeDef",
     "DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorGroupRequestRequestTypeDef",
@@ -82,169 +83,171 @@
     "DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     "DeleteVoiceProfileDomainRequestRequestTypeDef",
     "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GeoMatchParamsOutputTypeDef",
-    "VoiceConnectorSettingsOutputTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    "LoggingConfigurationOutputTypeDef",
+    "LoggingConfigurationTypeDef",
     "GetVoiceConnectorOriginationRequestRequestTypeDef",
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationOutputTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "ListVoiceProfileDomainsRequestRequestTypeDef",
     "VoiceProfileDomainSummaryTypeDef",
     "ListVoiceProfilesRequestRequestTypeDef",
     "VoiceProfileSummaryTypeDef",
-    "LoggingConfigurationTypeDef",
-    "MediaInsightsConfigurationOutputTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
-    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "TerminationTypeDef",
-    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    "SipMediaApplicationEndpointOutputTypeDef",
-    "SipRuleTargetApplicationOutputTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
-    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "UpdateVoiceProfileDomainRequestRequestTypeDef",
     "UpdateVoiceProfileRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
-    "VoiceConnectorItemOutputTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
+    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSipRuleRequestRequestTypeDef",
+    "SipRuleTypeDef",
     "UpdateSipRuleRequestRequestTypeDef",
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
+    "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
+    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
+    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    "VoiceProfileDomainTypeDef",
-    "SipMediaApplicationTypeDef",
-    "SipRuleTypeDef",
     "SpeakerSearchDetailsTypeDef",
     "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    "VoiceConnectorGroupTypeDef",
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     "StartVoiceToneAnalysisTaskResponseTypeDef",
+    "CreateSipMediaApplicationResponseTypeDef",
+    "GetSipMediaApplicationResponseTypeDef",
+    "ListSipMediaApplicationsResponseTypeDef",
+    "UpdateSipMediaApplicationResponseTypeDef",
+    "CreateSipRuleResponseTypeDef",
+    "GetSipRuleResponseTypeDef",
+    "ListSipRulesResponseTypeDef",
+    "UpdateSipRuleResponseTypeDef",
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    "GetVoiceConnectorGroupResponseTypeDef",
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    "UpdateVoiceConnectorGroupResponseTypeDef",
+    "CreateVoiceProfileDomainResponseTypeDef",
+    "GetVoiceProfileDomainResponseTypeDef",
+    "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
@@ -254,33 +257,18 @@
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
-    "CreateVoiceProfileDomainResponseTypeDef",
-    "GetVoiceProfileDomainResponseTypeDef",
-    "UpdateVoiceProfileDomainResponseTypeDef",
-    "CreateSipMediaApplicationResponseTypeDef",
-    "GetSipMediaApplicationResponseTypeDef",
-    "ListSipMediaApplicationsResponseTypeDef",
-    "UpdateSipMediaApplicationResponseTypeDef",
-    "CreateSipRuleResponseTypeDef",
-    "GetSipRuleResponseTypeDef",
-    "ListSipRulesResponseTypeDef",
-    "UpdateSipRuleResponseTypeDef",
     "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    "GetVoiceConnectorGroupResponseTypeDef",
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetSpeakerSearchTaskResponseTypeDef",
     "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
@@ -309,30 +297,43 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
+
 class AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
+
 PhoneNumberErrorTypeDef = TypedDict(
     "PhoneNumberErrorTypeDef",
     {
         "PhoneNumberId": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
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
 _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -340,20 +341,22 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
+
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
+
 BatchDeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
     },
 )
 
@@ -368,19 +371,21 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
+
 class UpdatePhoneNumberRequestItemTypeDef(
     _RequiredUpdatePhoneNumberRequestItemTypeDef, _OptionalUpdatePhoneNumberRequestItemTypeDef
 ):
     pass
 
+
 CallDetailsTypeDef = TypedDict(
     "CallDetailsTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "IsCaller": bool,
     },
@@ -430,20 +435,22 @@
     {
         "SipHeaders": Mapping[str, str],
         "ArgumentsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSipMediaApplicationCallRequestRequestTypeDef(
     _RequiredCreateSipMediaApplicationCallRequestRequestTypeDef,
     _OptionalCreateSipMediaApplicationCallRequestRequestTypeDef,
 ):
     pass
 
+
 SipMediaApplicationCallTypeDef = TypedDict(
     "SipMediaApplicationCallTypeDef",
     {
         "TransactionId": str,
     },
     total=False,
 )
@@ -529,35 +536,14 @@
     {
         "Username": str,
         "Password": str,
     },
     total=False,
 )
 
-_RequiredDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDNISEmergencyCallingConfigurationOutputTypeDef",
-    {
-        "EmergencyPhoneNumber": str,
-        "CallingCountry": str,
-    },
-)
-_OptionalDNISEmergencyCallingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDNISEmergencyCallingConfigurationOutputTypeDef",
-    {
-        "TestPhoneNumber": str,
-    },
-    total=False,
-)
-
-class DNISEmergencyCallingConfigurationOutputTypeDef(
-    _RequiredDNISEmergencyCallingConfigurationOutputTypeDef,
-    _OptionalDNISEmergencyCallingConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredDNISEmergencyCallingConfigurationTypeDef = TypedDict(
     "_RequiredDNISEmergencyCallingConfigurationTypeDef",
     {
         "EmergencyPhoneNumber": str,
         "CallingCountry": str,
     },
 )
@@ -565,20 +551,22 @@
     "_OptionalDNISEmergencyCallingConfigurationTypeDef",
     {
         "TestPhoneNumber": str,
     },
     total=False,
 )
 
+
 class DNISEmergencyCallingConfigurationTypeDef(
     _RequiredDNISEmergencyCallingConfigurationTypeDef,
     _OptionalDNISEmergencyCallingConfigurationTypeDef,
 ):
     pass
 
+
 DeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "DeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -687,31 +675,16 @@
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GeoMatchParamsOutputTypeDef = TypedDict(
-    "GeoMatchParamsOutputTypeDef",
-    {
-        "Country": str,
-        "AreaCode": str,
-    },
-)
-
-VoiceConnectorSettingsOutputTypeDef = TypedDict(
-    "VoiceConnectorSettingsOutputTypeDef",
+VoiceConnectorSettingsTypeDef = TypedDict(
+    "VoiceConnectorSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetPhoneNumberOrderRequestRequestTypeDef = TypedDict(
@@ -724,23 +697,14 @@
 GetPhoneNumberRequestRequestTypeDef = TypedDict(
     "GetPhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
-    {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProxySessionRequestRequestTypeDef = TypedDict(
     "GetProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "ProxySessionId": str,
     },
 )
@@ -763,16 +727,16 @@
 GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
 
-SipMediaApplicationLoggingConfigurationOutputTypeDef = TypedDict(
-    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
+SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     {
         "EnableSipMediaApplicationMessageLogs": bool,
     },
     total=False,
 )
 
 GetSipMediaApplicationRequestRequestTypeDef = TypedDict(
@@ -814,16 +778,16 @@
 GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-LoggingConfigurationOutputTypeDef = TypedDict(
-    "LoggingConfigurationOutputTypeDef",
+LoggingConfigurationTypeDef = TypedDict(
+    "LoggingConfigurationTypeDef",
     {
         "EnableSIPLogs": bool,
         "EnableMediaMetricLogs": bool,
     },
     total=False,
 )
 
@@ -920,22 +884,14 @@
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
         "IsCaller": bool,
     },
 )
 
-ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
-    {
-        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPhoneNumberOrdersRequestRequestTypeDef = TypedDict(
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -966,45 +922,40 @@
         "Status": ProxySessionStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListProxySessionsRequestRequestTypeDef(
     _RequiredListProxySessionsRequestRequestTypeDef, _OptionalListProxySessionsRequestRequestTypeDef
 ):
     pass
 
-ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
+
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
 
 ListSipMediaApplicationsRequestRequestTypeDef = TypedDict(
     "ListSipMediaApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSipRulesRequestRequestTypeDef = TypedDict(
     "ListSipRulesRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1030,22 +981,14 @@
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
 ListVoiceConnectorGroupsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1054,22 +997,14 @@
 ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    {
-        "Usernames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVoiceConnectorsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1108,50 +1043,34 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListVoiceProfilesRequestRequestTypeDef(
     _RequiredListVoiceProfilesRequestRequestTypeDef, _OptionalListVoiceProfilesRequestRequestTypeDef
 ):
     pass
 
+
 VoiceProfileSummaryTypeDef = TypedDict(
     "VoiceProfileSummaryTypeDef",
     {
         "VoiceProfileId": str,
         "VoiceProfileArn": str,
         "VoiceProfileDomainId": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ExpirationTimestamp": datetime,
     },
     total=False,
 )
 
-LoggingConfigurationTypeDef = TypedDict(
-    "LoggingConfigurationTypeDef",
-    {
-        "EnableSIPLogs": bool,
-        "EnableMediaMetricLogs": bool,
-    },
-    total=False,
-)
-
-MediaInsightsConfigurationOutputTypeDef = TypedDict(
-    "MediaInsightsConfigurationOutputTypeDef",
-    {
-        "Disabled": bool,
-        "ConfigurationArn": str,
-    },
-    total=False,
-)
-
 MediaInsightsConfigurationTypeDef = TypedDict(
     "MediaInsightsConfigurationTypeDef",
     {
         "Disabled": bool,
         "ConfigurationArn": str,
     },
     total=False,
@@ -1162,48 +1081,26 @@
     {
         "E164PhoneNumber": str,
         "Status": OrderedPhoneNumberStatusType,
     },
     total=False,
 )
 
-OriginationRouteOutputTypeDef = TypedDict(
-    "OriginationRouteOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Protocol": OriginationRouteProtocolType,
-        "Priority": int,
-        "Weight": int,
-    },
-    total=False,
-)
-
 OriginationRouteTypeDef = TypedDict(
     "OriginationRouteTypeDef",
     {
         "Host": str,
         "Port": int,
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
         "Weight": int,
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
 ParticipantTypeDef = TypedDict(
     "ParticipantTypeDef",
     {
         "PhoneNumber": str,
         "ProxyPhoneNumber": str,
     },
     total=False,
@@ -1236,22 +1133,14 @@
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     {
         "AlexaSkillStatus": AlexaSkillStatusType,
         "AlexaSkillIds": Sequence[str],
     },
 )
 
-SipMediaApplicationLoggingConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationLoggingConfigurationTypeDef",
-    {
-        "EnableSipMediaApplicationMessageLogs": bool,
-    },
-    total=False,
-)
-
 _RequiredPutVoiceConnectorProxyRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorProxyRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "DefaultSessionExpiryMinutes": int,
         "PhoneNumberPoolCountries": Sequence[str],
     },
@@ -1261,43 +1150,34 @@
     {
         "FallBackPhoneNumber": str,
         "Disabled": bool,
     },
     total=False,
 )
 
+
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
+
 TerminationTypeDef = TypedDict(
     "TerminationTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": Sequence[str],
         "CidrAllowedList": Sequence[str],
         "Disabled": bool,
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -1312,48 +1192,14 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-)
-
-SipMediaApplicationEndpointOutputTypeDef = TypedDict(
-    "SipMediaApplicationEndpointOutputTypeDef",
-    {
-        "LambdaArn": str,
-    },
-    total=False,
-)
-
-SipRuleTargetApplicationOutputTypeDef = TypedDict(
-    "SipRuleTargetApplicationOutputTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "Priority": int,
-        "AwsRegion": str,
-    },
-    total=False,
-)
-
 SpeakerSearchResultTypeDef = TypedDict(
     "SpeakerSearchResultTypeDef",
     {
         "ConfidenceScore": float,
         "VoiceProfileId": str,
     },
     total=False,
@@ -1372,20 +1218,22 @@
     {
         "ClientRequestToken": str,
         "CallLeg": CallLegTypeType,
     },
     total=False,
 )
 
+
 class StartSpeakerSearchTaskRequestRequestTypeDef(
     _RequiredStartSpeakerSearchTaskRequestRequestTypeDef,
     _OptionalStartSpeakerSearchTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "LanguageCode": Literal["en-US"],
     },
@@ -1394,20 +1242,22 @@
     "_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class StartVoiceToneAnalysisTaskRequestRequestTypeDef(
     _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef,
     _OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef,
 ):
     pass
 
+
 StopSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1416,22 +1266,14 @@
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
     },
 )
 
-StreamingNotificationTargetOutputTypeDef = TypedDict(
-    "StreamingNotificationTargetOutputTypeDef",
-    {
-        "NotificationTarget": NotificationTargetType,
-    },
-    total=False,
-)
-
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
     total=False,
 )
@@ -1440,22 +1282,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-VoiceConnectorSettingsTypeDef = TypedDict(
-    "VoiceConnectorSettingsTypeDef",
-    {
-        "CdrBucket": str,
-    },
-    total=False,
-)
-
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -1463,19 +1297,21 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
+
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
+
 UpdatePhoneNumberSettingsRequestRequestTypeDef = TypedDict(
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     {
         "CallingName": str,
     },
 )
 
@@ -1491,20 +1327,22 @@
     "_OptionalUpdateProxySessionRequestRequestTypeDef",
     {
         "ExpiryMinutes": int,
     },
     total=False,
 )
 
+
 class UpdateProxySessionRequestRequestTypeDef(
     _RequiredUpdateProxySessionRequestRequestTypeDef,
     _OptionalUpdateProxySessionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateSipMediaApplicationCallRequestRequestTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "TransactionId": str,
         "Arguments": Mapping[str, str],
     },
@@ -1530,20 +1368,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredUpdateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalUpdateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateVoiceProfileRequestRequestTypeDef = TypedDict(
     "UpdateVoiceProfileRequestRequestTypeDef",
     {
         "VoiceProfileId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1557,67 +1397,100 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
-VoiceConnectorItemOutputTypeDef = TypedDict(
-    "VoiceConnectorItemOutputTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Priority": int,
-    },
-)
-
 AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeletePhoneNumberResponseTypeDef = TypedDict(
     "BatchDeletePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
     "BatchUpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
+GetPhoneNumberSettingsResponseTypeDef = TypedDict(
+    "GetPhoneNumberSettingsResponseTypeDef",
+    {
+        "CallingName": str,
+        "CallingNameUpdatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
+    {
+        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    {
+        "Usernames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    {
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
@@ -1641,15 +1514,15 @@
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProxySessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1665,34 +1538,50 @@
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
         "GeoMatchParams": GeoMatchParamsTypeDef,
     },
     total=False,
 )
 
+
 class CreateProxySessionRequestRequestTypeDef(
     _RequiredCreateProxySessionRequestRequestTypeDef,
     _OptionalCreateProxySessionRequestRequestTypeDef,
 ):
     pass
 
+
 CreateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SipMediaApplicationTypeDef = TypedDict(
+    "SipMediaApplicationTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": List[SipMediaApplicationEndpointTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "SipMediaApplicationArn": str,
     },
+    total=False,
 )
 
 _RequiredUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipMediaApplicationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
@@ -1702,20 +1591,22 @@
     {
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
     },
     total=False,
 )
 
+
 class UpdateSipMediaApplicationRequestRequestTypeDef(
     _RequiredUpdateSipMediaApplicationRequestRequestTypeDef,
     _OptionalUpdateSipMediaApplicationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
     },
@@ -1724,20 +1615,22 @@
     "_OptionalCreateSipMediaApplicationRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSipMediaApplicationRequestRequestTypeDef(
     _RequiredCreateSipMediaApplicationRequestRequestTypeDef,
     _OptionalCreateSipMediaApplicationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceConnectorRequestRequestTypeDef",
     {
         "Name": str,
         "RequireEncryption": bool,
     },
 )
@@ -1746,20 +1639,30 @@
     {
         "AwsRegion": VoiceConnectorAwsRegionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVoiceConnectorRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorRequestRequestTypeDef,
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
@@ -1777,19 +1680,36 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
+
 class CreateSipRuleRequestRequestTypeDef(
     _RequiredCreateSipRuleRequestRequestTypeDef, _OptionalCreateSipRuleRequestRequestTypeDef
 ):
     pass
 
+
+SipRuleTypeDef = TypedDict(
+    "SipRuleTypeDef",
+    {
+        "SipRuleId": str,
+        "Name": str,
+        "Disabled": bool,
+        "TriggerType": SipRuleTriggerTypeType,
+        "TriggerValue": str,
+        "TargetApplications": List[SipRuleTargetApplicationTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
     },
 )
@@ -1798,78 +1718,95 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateSipRuleRequestRequestTypeDef(
     _RequiredUpdateSipRuleRequestRequestTypeDef, _OptionalUpdateSipRuleRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
     total=False,
 )
 
+
 class CreateVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorGroupId": str,
         "Name": str,
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
 )
 
+VoiceConnectorGroupTypeDef = TypedDict(
+    "VoiceConnectorGroupTypeDef",
+    {
+        "VoiceConnectorGroupId": str,
+        "Name": str,
+        "VoiceConnectorItems": List[VoiceConnectorItemTypeDef],
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "VoiceConnectorGroupArn": str,
+    },
+    total=False,
+)
+
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorResponseTypeDef = TypedDict(
     "GetVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceProfileDomainRequestRequestTypeDef",
     {
         "Name": str,
@@ -1882,41 +1819,57 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
+
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 CreateVoiceProfileResponseTypeDef = TypedDict(
     "CreateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceProfileResponseTypeDef = TypedDict(
     "GetVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceProfileResponseTypeDef = TypedDict(
     "UpdateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1926,24 +1879,26 @@
     "_OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "Credentials": Sequence[CredentialTypeDef],
     },
     total=False,
 )
 
+
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
+
 EmergencyCallingConfigurationOutputTypeDef = TypedDict(
     "EmergencyCallingConfigurationOutputTypeDef",
     {
-        "DNIS": List[DNISEmergencyCallingConfigurationOutputTypeDef],
+        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
@@ -1951,154 +1906,189 @@
     },
     total=False,
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    {
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
     },
+    total=False,
 )
 
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationOutputTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": (
-            SipMediaApplicationLoggingConfigurationOutputTypeDef
-        ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationId": str,
+    },
+)
+_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
     },
+    total=False,
 )
 
+
+class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
+    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationLoggingConfiguration": (
-            SipMediaApplicationLoggingConfigurationOutputTypeDef
-        ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorProxyResponseTypeDef = TypedDict(
     "PutVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationHealthResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     {
         "TerminationHealth": TerminationHealthTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
-    "ListSupportedPhoneNumberCountriesResponseTypeDef",
+ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     {
-        "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
+    "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceProfilesResponseTypeDef = TypedDict(
     "ListVoiceProfilesResponseTypeDef",
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
@@ -2111,15 +2101,15 @@
     },
     total=False,
 )
 
 OriginationOutputTypeDef = TypedDict(
     "OriginationOutputTypeDef",
     {
-        "Routes": List[OriginationRouteOutputTypeDef],
+        "Routes": List[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
@@ -2141,15 +2131,15 @@
         "Capabilities": List[CapabilityType],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "EndedTimestamp": datetime,
         "Participants": List[ParticipantTypeDef],
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
-        "GeoMatchParams": GeoMatchParamsOutputTypeDef,
+        "GeoMatchParams": GeoMatchParamsTypeDef,
     },
     total=False,
 )
 
 PhoneNumberTypeDef = TypedDict(
     "PhoneNumberTypeDef",
     {
@@ -2183,91 +2173,30 @@
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
     },
     total=False,
 )
 
+
 class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
     _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-    },
-)
-_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
-    _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
 
 PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Termination": TerminationTypeDef,
     },
 )
 
-VoiceProfileDomainTypeDef = TypedDict(
-    "VoiceProfileDomainTypeDef",
-    {
-        "VoiceProfileDomainId": str,
-        "VoiceProfileDomainArn": str,
-        "Name": str,
-        "Description": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
-SipMediaApplicationTypeDef = TypedDict(
-    "SipMediaApplicationTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "SipMediaApplicationArn": str,
-    },
-    total=False,
-)
-
-SipRuleTypeDef = TypedDict(
-    "SipRuleTypeDef",
-    {
-        "SipRuleId": str,
-        "Name": str,
-        "Disabled": bool,
-        "TriggerType": SipRuleTriggerTypeType,
-        "TriggerValue": str,
-        "TargetApplications": List[SipRuleTargetApplicationOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 SpeakerSearchDetailsTypeDef = TypedDict(
     "SpeakerSearchDetailsTypeDef",
     {
         "Results": List[SpeakerSearchResultTypeDef],
         "VoiceprintGenerationStatus": str,
     },
     total=False,
@@ -2279,25 +2208,27 @@
         "DataRetentionInHours": int,
         "Disabled": bool,
     },
 )
 _OptionalStreamingConfigurationOutputTypeDef = TypedDict(
     "_OptionalStreamingConfigurationOutputTypeDef",
     {
-        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
-        "MediaInsightsConfiguration": MediaInsightsConfigurationOutputTypeDef,
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StreamingConfigurationOutputTypeDef(
     _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
         "Disabled": bool,
     },
 )
@@ -2306,69 +2237,173 @@
     {
         "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
         "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
+
+GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
     {
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VoiceConnectorGroupTypeDef = TypedDict(
-    "VoiceConnectorGroupTypeDef",
+StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
     {
-        "VoiceConnectorGroupId": str,
-        "Name": str,
-        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "VoiceConnectorGroupArn": str,
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "GetVoiceToneAnalysisTaskResponseTypeDef",
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
-    "StartVoiceToneAnalysisTaskResponseTypeDef",
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
     {
-        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSipMediaApplicationsResponseTypeDef = TypedDict(
+    "ListSipMediaApplicationsResponseTypeDef",
+    {
+        "SipMediaApplications": List[SipMediaApplicationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSipMediaApplicationResponseTypeDef = TypedDict(
+    "UpdateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSipRuleResponseTypeDef = TypedDict(
+    "CreateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSipRuleResponseTypeDef = TypedDict(
+    "GetSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSipRulesResponseTypeDef = TypedDict(
+    "ListSipRulesResponseTypeDef",
+    {
+        "SipRules": List[SipRuleTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSipRuleResponseTypeDef = TypedDict(
+    "UpdateSipRuleResponseTypeDef",
+    {
+        "SipRule": SipRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "CreateVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "GetVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorGroupsResponseTypeDef",
+    {
+        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "UpdateVoiceConnectorGroupResponseTypeDef",
+    {
+        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "CreateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceProfileDomainResponseTypeDef = TypedDict(
+    "GetVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -2376,48 +2411,48 @@
     },
 )
 
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberOrderResponseTypeDef = TypedDict(
     "GetPhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "PutVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -2425,163 +2460,73 @@
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProxySessionResponseTypeDef = TypedDict(
     "GetProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberResponseTypeDef = TypedDict(
     "GetPhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePhoneNumberResponseTypeDef = TypedDict(
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "CreateVoiceProfileDomainResponseTypeDef",
-    {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetVoiceProfileDomainResponseTypeDef = TypedDict(
-    "GetVoiceProfileDomainResponseTypeDef",
-    {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
-    "UpdateVoiceProfileDomainResponseTypeDef",
-    {
-        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSipMediaApplicationResponseTypeDef = TypedDict(
-    "CreateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipMediaApplicationResponseTypeDef = TypedDict(
-    "GetSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipMediaApplicationsResponseTypeDef = TypedDict(
-    "ListSipMediaApplicationsResponseTypeDef",
-    {
-        "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipMediaApplicationResponseTypeDef = TypedDict(
-    "UpdateSipMediaApplicationResponseTypeDef",
-    {
-        "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSipRuleResponseTypeDef = TypedDict(
-    "CreateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSipRuleResponseTypeDef = TypedDict(
-    "GetSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSipRulesResponseTypeDef = TypedDict(
-    "ListSipRulesResponseTypeDef",
-    {
-        "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSipRuleResponseTypeDef = TypedDict(
-    "UpdateSipRuleResponseTypeDef",
-    {
-        "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SpeakerSearchTaskTypeDef = TypedDict(
     "SpeakerSearchTaskTypeDef",
     {
         "SpeakerSearchTaskId": str,
@@ -2596,75 +2541,42 @@
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
-CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "GetVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    {
-        "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "UpdateVoiceConnectorGroupResponseTypeDef",
-    {
-        "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeakerSearchTaskResponseTypeDef = TypedDict(
     "StartSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKVoice 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,14 +350,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.type_defs import (
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
@@ -368,15 +369,14 @@
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
-    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
@@ -386,169 +386,171 @@
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GeoMatchParamsOutputTypeDef,
-    VoiceConnectorSettingsOutputTypeDef,
+    VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationOutputTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationOutputTypeDef,
+    LoggingConfigurationTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationOutputTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
-    ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
-    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
-    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
-    LoggingConfigurationTypeDef,
-    MediaInsightsConfigurationOutputTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
-    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     TerminationTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
-    SipMediaApplicationEndpointOutputTypeDef,
-    SipRuleTargetApplicationOutputTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
-    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
-    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     UpdateVoiceProfileDomainRequestRequestTypeDef,
     UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    VoiceConnectorItemOutputTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAvailableVoiceConnectorRegionsResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
+    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
+    SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
+    VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
+    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
+    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
+    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
+    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
-    VoiceProfileDomainTypeDef,
-    SipMediaApplicationTypeDef,
-    SipRuleTypeDef,
     SpeakerSearchDetailsTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     GetVoiceToneAnalysisTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
+    CreateSipMediaApplicationResponseTypeDef,
+    GetSipMediaApplicationResponseTypeDef,
+    ListSipMediaApplicationsResponseTypeDef,
+    UpdateSipMediaApplicationResponseTypeDef,
+    CreateSipRuleResponseTypeDef,
+    GetSipRuleResponseTypeDef,
+    ListSipRulesResponseTypeDef,
+    UpdateSipRuleResponseTypeDef,
+    CreateVoiceConnectorGroupResponseTypeDef,
+    GetVoiceConnectorGroupResponseTypeDef,
+    ListVoiceConnectorGroupsResponseTypeDef,
+    UpdateVoiceConnectorGroupResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
@@ -558,33 +560,18 @@
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
-    CreateVoiceProfileDomainResponseTypeDef,
-    GetVoiceProfileDomainResponseTypeDef,
-    UpdateVoiceProfileDomainResponseTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
     SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
     GetSpeakerSearchTaskResponseTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
```

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-voice-1.28.15/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.28.12/setup.py` & `mypy-boto3-chime-sdk-voice-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-voice",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_chime_sdk_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKVoice 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ChimeSDKVoice 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

