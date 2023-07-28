# Comparing `tmp/mypy-boto3-chime-1.28.12.tar.gz` & `tmp/mypy-boto3-chime-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
```

## Comparing `mypy-boto3-chime-1.28.12.tar` & `mypy-boto3-chime-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33946 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32467 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/mypy_boto3_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-27 05:18:09.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   154447 2023-07-27 05:18:13.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   154280 2023-07-27 05:18:11.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33946 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:22.000000 mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.808567 mypy-boto3-chime-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:18:08.000000 mypy-boto3-chime-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32817 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/mypy_boto3_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-07-28 20:20:26.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-28 20:20:27.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   146654 2023-07-28 20:20:32.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146493 2023-07-28 20:20:30.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32817 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:42:22.000000 mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.352738 mypy-boto3-chime-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:20:25.000000 mypy-boto3-chime-1.28.15/setup.py
```

### Comparing `mypy-boto3-chime-1.28.12/LICENSE` & `mypy-boto3-chime-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/PKG-INFO` & `mypy-boto3-chime-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.28.12
-Summary: Type annotations for boto3.Chime 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,71 +370,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
-    AccountSettingsOutputTypeDef,
     AccountSettingsTypeDef,
-    SigninDelegateGroupOutputTypeDef,
+    SigninDelegateGroupTypeDef,
     AddressTypeDef,
-    AlexaForBusinessMetadataOutputTypeDef,
     AlexaForBusinessMetadataTypeDef,
     IdentityTypeDef,
-    ChannelRetentionSettingsOutputTypeDef,
     ChannelRetentionSettingsTypeDef,
-    AppInstanceStreamingConfigurationOutputTypeDef,
     AppInstanceStreamingConfigurationTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     AppInstanceUserMembershipSummaryTypeDef,
     AppInstanceUserSummaryTypeDef,
     AppInstanceUserTypeDef,
-    AudioArtifactsConfigurationOutputTypeDef,
-    ContentArtifactsConfigurationOutputTypeDef,
-    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
-    SigninDelegateGroupTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     BatchSuspendUserRequestRequestTypeDef,
     UserErrorTypeDef,
     BatchUnsuspendUserRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     BotTypeDef,
-    BusinessCallingSettingsOutputTypeDef,
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
-    ConversationRetentionSettingsOutputTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -442,15 +429,14 @@
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     CreateUserRequestRequestTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     CredentialTypeDef,
-    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeleteAccountRequestRequestTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
@@ -485,65 +471,61 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
-    GeoMatchParamsOutputTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetEventsConfigurationRequestRequestTypeDef,
-    VoiceConnectorSettingsOutputTypeDef,
+    VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationOutputTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
     GetUserSettingsRequestRequestTypeDef,
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
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
@@ -558,123 +540,114 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
-    LoggingConfigurationTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
-    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
-    RoomRetentionSettingsOutputTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
-    SendChannelMessageResponseTypeDef,
-    SipMediaApplicationEndpointOutputTypeDef,
-    SipRuleTargetApplicationOutputTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
-    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
-    TelephonySettingsOutputTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
-    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
-    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    VoiceConnectorItemOutputTypeDef,
-    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
-    UserTypeDef,
+    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
+    UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
-    AppInstanceRetentionSettingsOutputTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
-    ArtifactsConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSettingsResponseTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SendChannelMessageResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
+    UpdateChannelMessageResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -691,110 +664,122 @@
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
+    ListAttendeeTagsResponseTypeDef,
+    ListMeetingTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagAttendeeRequestRequestTypeDef,
     TagMeetingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     ListRoomsResponseTypeDef,
     UpdateRoomResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
+    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
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
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
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
     InviteUsersResponseTypeDef,
-    ListAttendeeTagsResponseTypeDef,
-    ListMeetingTagsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
-    RetentionSettingsOutputTypeDef,
     RetentionSettingsTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
-    SipMediaApplicationTypeDef,
-    SipRuleTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
-    UserSettingsOutputTypeDef,
     UserSettingsTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
+    BatchUpdateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     ResetPersonalPINResponseTypeDef,
     UpdateUserResponseTypeDef,
-    BatchUpdateUserRequestRequestTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
-    PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
+    PutAppInstanceRetentionSettingsResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
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
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
@@ -813,44 +798,32 @@
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     GetRetentionSettingsResponseTypeDef,
-    PutRetentionSettingsResponseTypeDef,
     PutRetentionSettingsRequestRequestTypeDef,
+    PutRetentionSettingsResponseTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
     MediaCapturePipelineTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsOutputTypeDef:
+def get_structure() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.12/README.md` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-chime
+Version: 1.28.15
+Summary: Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,71 +370,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
-    AccountSettingsOutputTypeDef,
     AccountSettingsTypeDef,
-    SigninDelegateGroupOutputTypeDef,
+    SigninDelegateGroupTypeDef,
     AddressTypeDef,
-    AlexaForBusinessMetadataOutputTypeDef,
     AlexaForBusinessMetadataTypeDef,
     IdentityTypeDef,
-    ChannelRetentionSettingsOutputTypeDef,
     ChannelRetentionSettingsTypeDef,
-    AppInstanceStreamingConfigurationOutputTypeDef,
     AppInstanceStreamingConfigurationTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     AppInstanceUserMembershipSummaryTypeDef,
     AppInstanceUserSummaryTypeDef,
     AppInstanceUserTypeDef,
-    AudioArtifactsConfigurationOutputTypeDef,
-    ContentArtifactsConfigurationOutputTypeDef,
-    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
-    SigninDelegateGroupTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     BatchSuspendUserRequestRequestTypeDef,
     UserErrorTypeDef,
     BatchUnsuspendUserRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     BotTypeDef,
-    BusinessCallingSettingsOutputTypeDef,
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
-    ConversationRetentionSettingsOutputTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -410,15 +429,14 @@
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     CreateUserRequestRequestTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     CredentialTypeDef,
-    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeleteAccountRequestRequestTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
@@ -453,65 +471,61 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
-    GeoMatchParamsOutputTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetEventsConfigurationRequestRequestTypeDef,
-    VoiceConnectorSettingsOutputTypeDef,
+    VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationOutputTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
     GetUserSettingsRequestRequestTypeDef,
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
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
@@ -526,123 +540,114 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
-    LoggingConfigurationTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
-    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
-    RoomRetentionSettingsOutputTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
-    SendChannelMessageResponseTypeDef,
-    SipMediaApplicationEndpointOutputTypeDef,
-    SipRuleTargetApplicationOutputTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
-    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
-    TelephonySettingsOutputTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
-    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
-    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    VoiceConnectorItemOutputTypeDef,
-    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
-    UserTypeDef,
+    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
+    UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
-    AppInstanceRetentionSettingsOutputTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
-    ArtifactsConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSettingsResponseTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SendChannelMessageResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
+    UpdateChannelMessageResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -659,110 +664,122 @@
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
+    ListAttendeeTagsResponseTypeDef,
+    ListMeetingTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagAttendeeRequestRequestTypeDef,
     TagMeetingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     ListRoomsResponseTypeDef,
     UpdateRoomResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
+    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
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
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
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
     InviteUsersResponseTypeDef,
-    ListAttendeeTagsResponseTypeDef,
-    ListMeetingTagsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
-    RetentionSettingsOutputTypeDef,
     RetentionSettingsTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
-    SipMediaApplicationTypeDef,
-    SipRuleTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
-    UserSettingsOutputTypeDef,
     UserSettingsTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
+    BatchUpdateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     ResetPersonalPINResponseTypeDef,
     UpdateUserResponseTypeDef,
-    BatchUpdateUserRequestRequestTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
-    PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
+    PutAppInstanceRetentionSettingsResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
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
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
@@ -781,44 +798,32 @@
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     GetRetentionSettingsResponseTypeDef,
-    PutRetentionSettingsResponseTypeDef,
     PutRetentionSettingsRequestRequestTypeDef,
+    PutRetentionSettingsResponseTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
     MediaCapturePipelineTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsOutputTypeDef:
+def get_structure() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.py` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/__init__.pyi` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/__main__.py` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Chime 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Chime 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
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

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.py` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/client.pyi` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.py` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/literals.pyi` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.py` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listaccountspaginator)
         """
 
 
@@ -68,13 +68,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/paginator.pyi` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listaccountspaginator)
         """
 
 class ListUsersPaginator(Paginator):
@@ -64,13 +64,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.py` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime.type_defs import AccountSettingsOutputTypeDef
+    from mypy_boto3_chime.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsOutputTypeDef = {...}
+    data: AccountSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -67,71 +67,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccountSettingsOutputTypeDef",
     "AccountSettingsTypeDef",
-    "SigninDelegateGroupOutputTypeDef",
+    "SigninDelegateGroupTypeDef",
     "AddressTypeDef",
-    "AlexaForBusinessMetadataOutputTypeDef",
     "AlexaForBusinessMetadataTypeDef",
     "IdentityTypeDef",
-    "ChannelRetentionSettingsOutputTypeDef",
     "ChannelRetentionSettingsTypeDef",
-    "AppInstanceStreamingConfigurationOutputTypeDef",
     "AppInstanceStreamingConfigurationTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "AppInstanceUserMembershipSummaryTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "AppInstanceUserTypeDef",
-    "AudioArtifactsConfigurationOutputTypeDef",
-    "ContentArtifactsConfigurationOutputTypeDef",
-    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
-    "SigninDelegateGroupTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "BatchSuspendUserRequestRequestTypeDef",
     "UserErrorTypeDef",
     "BatchUnsuspendUserRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "BotTypeDef",
-    "BusinessCallingSettingsOutputTypeDef",
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
-    "ConversationRetentionSettingsOutputTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "CreateMeetingDialOutRequestRequestTypeDef",
-    "CreateMeetingDialOutResponseTypeDef",
     "MeetingNotificationConfigurationTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateRoomMembershipRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
@@ -139,15 +126,14 @@
     "SipMediaApplicationEndpointTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "CreateUserRequestRequestTypeDef",
     "VoiceConnectorItemTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
     "CredentialTypeDef",
-    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeleteAccountRequestRequestTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
@@ -182,65 +168,61 @@
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociatePhoneNumberFromUserRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
-    "GeoMatchParamsOutputTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetEventsConfigurationRequestRequestTypeDef",
-    "VoiceConnectorSettingsOutputTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetUserRequestRequestTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
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
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
@@ -255,123 +237,114 @@
     "ListRoomMembershipsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
-    "LoggingConfigurationTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
-    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
-    "RoomRetentionSettingsOutputTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
-    "SendChannelMessageResponseTypeDef",
-    "SipMediaApplicationEndpointOutputTypeDef",
-    "SipRuleTargetApplicationOutputTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
-    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
-    "TelephonySettingsOutputTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
-    "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
-    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
-    "VoiceConnectorItemOutputTypeDef",
-    "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
-    "UserTypeDef",
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateChannelBanResponseTypeDef",
-    "CreateChannelMembershipResponseTypeDef",
-    "CreateChannelModeratorResponseTypeDef",
-    "AppInstanceRetentionSettingsOutputTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "DescribeAppInstanceUserResponseTypeDef",
-    "ArtifactsConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
+    "CreateChannelBanResponseTypeDef",
+    "CreateChannelMembershipResponseTypeDef",
+    "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "CreateMeetingDialOutResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "DescribeAppInstanceUserResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSettingsResponseTypeDef",
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SendChannelMessageResponseTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
+    "UpdateChannelMessageResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -388,110 +361,122 @@
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "ListAttendeeTagsResponseTypeDef",
+    "ListMeetingTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagAttendeeRequestRequestTypeDef",
     "TagMeetingRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "ListRoomsResponseTypeDef",
     "UpdateRoomResponseTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
+    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
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
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
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
     "InviteUsersResponseTypeDef",
-    "ListAttendeeTagsResponseTypeDef",
-    "ListMeetingTagsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
-    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    "RetentionSettingsOutputTypeDef",
     "RetentionSettingsTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
-    "SipMediaApplicationTypeDef",
-    "SipRuleTypeDef",
     "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
-    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    "VoiceConnectorGroupTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
+    "BatchUpdateUserRequestRequestTypeDef",
     "CreateUserResponseTypeDef",
     "GetUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ResetPersonalPINResponseTypeDef",
     "UpdateUserResponseTypeDef",
-    "BatchUpdateUserRequestRequestTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
-    "PutAppInstanceRetentionSettingsResponseTypeDef",
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
+    "PutAppInstanceRetentionSettingsResponseTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
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
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
@@ -510,62 +495,41 @@
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "GetRetentionSettingsResponseTypeDef",
-    "PutRetentionSettingsResponseTypeDef",
     "PutRetentionSettingsRequestRequestTypeDef",
+    "PutRetentionSettingsResponseTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
-    "CreateSipMediaApplicationResponseTypeDef",
-    "GetSipMediaApplicationResponseTypeDef",
-    "ListSipMediaApplicationsResponseTypeDef",
-    "UpdateSipMediaApplicationResponseTypeDef",
-    "CreateSipRuleResponseTypeDef",
-    "GetSipRuleResponseTypeDef",
-    "ListSipRulesResponseTypeDef",
-    "UpdateSipRuleResponseTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    "GetVoiceConnectorGroupResponseTypeDef",
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    "UpdateVoiceConnectorGroupResponseTypeDef",
     "MediaCapturePipelineTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
-AccountSettingsOutputTypeDef = TypedDict(
-    "AccountSettingsOutputTypeDef",
-    {
-        "DisableRemoteControl": bool,
-        "EnableDialOut": bool,
-    },
-    total=False,
-)
-
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "DisableRemoteControl": bool,
         "EnableDialOut": bool,
     },
     total=False,
 )
 
-SigninDelegateGroupOutputTypeDef = TypedDict(
-    "SigninDelegateGroupOutputTypeDef",
+SigninDelegateGroupTypeDef = TypedDict(
+    "SigninDelegateGroupTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
 AddressTypeDef = TypedDict(
@@ -581,23 +545,14 @@
         "postalCode": str,
         "postalCodePlus4": str,
         "country": str,
     },
     total=False,
 )
 
-AlexaForBusinessMetadataOutputTypeDef = TypedDict(
-    "AlexaForBusinessMetadataOutputTypeDef",
-    {
-        "IsAlexaForBusinessEnabled": bool,
-        "AlexaForBusinessRoomArn": str,
-    },
-    total=False,
-)
-
 AlexaForBusinessMetadataTypeDef = TypedDict(
     "AlexaForBusinessMetadataTypeDef",
     {
         "IsAlexaForBusinessEnabled": bool,
         "AlexaForBusinessRoomArn": str,
     },
     total=False,
@@ -608,38 +563,22 @@
     {
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
-ChannelRetentionSettingsOutputTypeDef = TypedDict(
-    "ChannelRetentionSettingsOutputTypeDef",
-    {
-        "RetentionDays": int,
-    },
-    total=False,
-)
-
 ChannelRetentionSettingsTypeDef = TypedDict(
     "ChannelRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
 
-AppInstanceStreamingConfigurationOutputTypeDef = TypedDict(
-    "AppInstanceStreamingConfigurationOutputTypeDef",
-    {
-        "AppInstanceDataType": AppInstanceDataTypeType,
-        "ResourceArn": str,
-    },
-)
-
 AppInstanceStreamingConfigurationTypeDef = TypedDict(
     "AppInstanceStreamingConfigurationTypeDef",
     {
         "AppInstanceDataType": AppInstanceDataTypeType,
         "ResourceArn": str,
     },
 )
@@ -693,65 +632,14 @@
         "CreatedTimestamp": datetime,
         "Metadata": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-AudioArtifactsConfigurationOutputTypeDef = TypedDict(
-    "AudioArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": AudioMuxTypeType,
-    },
-)
-
-_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredContentArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalContentArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["ContentOnly"],
-    },
-    total=False,
-)
-
-
-class ContentArtifactsConfigurationOutputTypeDef(
-    _RequiredContentArtifactsConfigurationOutputTypeDef,
-    _OptionalContentArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
-
-_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["VideoOnly"],
-    },
-    total=False,
-)
-
-
-class VideoArtifactsConfigurationOutputTypeDef(
-    _RequiredVideoArtifactsConfigurationOutputTypeDef,
-    _OptionalVideoArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
-
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -835,14 +723,25 @@
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
@@ -858,22 +757,14 @@
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
 
-SigninDelegateGroupTypeDef = TypedDict(
-    "SigninDelegateGroupTypeDef",
-    {
-        "GroupName": str,
-    },
-    total=False,
-)
-
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
     },
@@ -1010,22 +901,14 @@
         "UpdatedTimestamp": datetime,
         "BotEmail": str,
         "SecurityToken": str,
     },
     total=False,
 )
 
-BusinessCallingSettingsOutputTypeDef = TypedDict(
-    "BusinessCallingSettingsOutputTypeDef",
-    {
-        "CdrBucket": str,
-    },
-    total=False,
-)
-
 BusinessCallingSettingsTypeDef = TypedDict(
     "BusinessCallingSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
@@ -1053,22 +936,14 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
-ConversationRetentionSettingsOutputTypeDef = TypedDict(
-    "ConversationRetentionSettingsOutputTypeDef",
-    {
-        "RetentionDays": int,
-    },
-    total=False,
-)
-
 ConversationRetentionSettingsTypeDef = TypedDict(
     "ConversationRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -1092,30 +967,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "DisplayName": str,
     },
 )
@@ -1199,40 +1058,24 @@
 class CreateChannelModeratorRequestRequestTypeDef(
     _RequiredCreateChannelModeratorRequestRequestTypeDef,
     _OptionalCreateChannelModeratorRequestRequestTypeDef,
 ):
     pass
 
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMeetingDialOutRequestRequestTypeDef = TypedDict(
     "CreateMeetingDialOutRequestRequestTypeDef",
     {
         "MeetingId": str,
         "FromPhoneNumber": str,
         "ToPhoneNumber": str,
         "JoinToken": str,
     },
 )
 
-CreateMeetingDialOutResponseTypeDef = TypedDict(
-    "CreateMeetingDialOutResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MeetingNotificationConfigurationTypeDef = TypedDict(
     "MeetingNotificationConfigurationTypeDef",
     {
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
     total=False,
@@ -1437,37 +1280,14 @@
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
@@ -1954,21 +1774,14 @@
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     {
         "AccountId": str,
         "GroupNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -2019,22 +1832,14 @@
         "BotId": str,
         "OutboundEventsHTTPSEndpoint": str,
         "LambdaFunctionArn": str,
     },
     total=False,
 )
 
-GeoMatchParamsOutputTypeDef = TypedDict(
-    "GeoMatchParamsOutputTypeDef",
-    {
-        "Country": str,
-        "AreaCode": str,
-    },
-)
-
 GetAccountRequestRequestTypeDef = TypedDict(
     "GetAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -2101,16 +1906,16 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
 
-VoiceConnectorSettingsOutputTypeDef = TypedDict(
-    "VoiceConnectorSettingsOutputTypeDef",
+VoiceConnectorSettingsTypeDef = TypedDict(
+    "VoiceConnectorSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
@@ -2145,23 +1950,14 @@
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
@@ -2184,16 +1980,16 @@
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
@@ -2243,16 +2039,16 @@
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
 
@@ -2359,20 +2155,20 @@
 
 class InviteUsersRequestRequestTypeDef(
     _RequiredInviteUsersRequestRequestTypeDef, _OptionalInviteUsersRequestRequestTypeDef
 ):
     pass
 
 
-ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Name": str,
-        "UserEmail": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountsRequestRequestTypeDef = TypedDict(
     "ListAccountsRequestRequestTypeDef",
     {
@@ -2443,22 +2239,14 @@
     "ListAttendeeTagsRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
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
 _RequiredListAttendeesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttendeesRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 _OptionalListAttendeesRequestRequestTypeDef = TypedDict(
@@ -2799,38 +2587,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserEmail": str,
-        "UserType": UserTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -2863,40 +2627,23 @@
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
 LogoutUserRequestRequestTypeDef = TypedDict(
     "LogoutUserRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
     },
 )
@@ -2933,48 +2680,26 @@
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
@@ -3023,22 +2748,14 @@
 class PutEventsConfigurationRequestRequestTypeDef(
     _RequiredPutEventsConfigurationRequestRequestTypeDef,
     _OptionalPutEventsConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
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
@@ -3091,23 +2808,14 @@
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedactConversationMessageRequestRequestTypeDef = TypedDict(
     "RedactConversationMessageRequestRequestTypeDef",
     {
         "AccountId": str,
         "ConversationId": str,
         "MessageId": str,
     },
@@ -3134,40 +2842,21 @@
     "ResetPersonalPINRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-RoomRetentionSettingsOutputTypeDef = TypedDict(
-    "RoomRetentionSettingsOutputTypeDef",
-    {
-        "RetentionDays": int,
-    },
-    total=False,
-)
-
 RoomRetentionSettingsTypeDef = TypedDict(
     "RoomRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -3183,23 +2872,14 @@
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
 SelectedVideoStreamsOutputTypeDef = TypedDict(
     "SelectedVideoStreamsOutputTypeDef",
     {
         "AttendeeIds": List[str],
         "ExternalUserIds": List[str],
     },
     total=False,
@@ -3237,71 +2917,28 @@
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
     _OptionalSendChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
-StreamingNotificationTargetOutputTypeDef = TypedDict(
-    "StreamingNotificationTargetOutputTypeDef",
-    {
-        "NotificationTarget": NotificationTargetType,
-    },
-)
-
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
 )
 
-TelephonySettingsOutputTypeDef = TypedDict(
-    "TelephonySettingsOutputTypeDef",
-    {
-        "InboundCalling": bool,
-        "OutboundCalling": bool,
-        "SMS": bool,
-    },
-)
-
 TelephonySettingsTypeDef = TypedDict(
     "TelephonySettingsTypeDef",
     {
         "InboundCalling": bool,
         "OutboundCalling": bool,
         "SMS": bool,
     },
@@ -3372,22 +3009,14 @@
 
 class UpdateAppInstanceRequestRequestTypeDef(
     _RequiredUpdateAppInstanceRequestRequestTypeDef, _OptionalUpdateAppInstanceRequestRequestTypeDef
 ):
     pass
 
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
     },
 )
@@ -3403,22 +3032,14 @@
 class UpdateAppInstanceUserRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
@@ -3458,23 +3079,14 @@
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
@@ -3489,22 +3101,14 @@
 class UpdateChannelReadMarkerRequestRequestTypeDef(
     _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
     _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Mode": ChannelModeType,
     },
@@ -3521,30 +3125,14 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
@@ -3667,30 +3255,14 @@
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
-GetAccountSettingsResponseTypeDef = TypedDict(
-    "GetAccountSettingsResponseTypeDef",
-    {
-        "AccountSettings": AccountSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "AccountSettings": AccountSettingsTypeDef,
     },
 )
@@ -3707,54 +3279,32 @@
     "_OptionalAccountTypeDef",
     {
         "AccountType": AccountTypeType,
         "CreatedTimestamp": datetime,
         "DefaultLicense": LicenseType,
         "SupportedLicenses": List[LicenseType],
         "AccountStatus": AccountStatusType,
-        "SigninDelegateGroups": List[SigninDelegateGroupOutputTypeDef],
+        "SigninDelegateGroups": List[SigninDelegateGroupTypeDef],
     },
     total=False,
 )
 
 
 class AccountTypeDef(_RequiredAccountTypeDef, _OptionalAccountTypeDef):
     pass
 
 
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
+AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     {
         "AccountId": str,
-        "PrimaryEmail": str,
-        "PrimaryProvisionedNumber": str,
-        "DisplayName": str,
-        "LicenseType": LicenseType,
-        "UserType": UserTypeType,
-        "UserRegistrationStatus": RegistrationStatusType,
-        "UserInvitationStatus": InviteStatusType,
-        "RegisteredOn": datetime,
-        "InvitedOn": datetime,
-        "AlexaForBusinessMetadata": AlexaForBusinessMetadataOutputTypeDef,
-        "PersonalPIN": str,
+        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
     },
-    total=False,
 )
 
-
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
-
 _RequiredUpdateUserRequestItemTypeDef = TypedDict(
     "_RequiredUpdateUserRequestItemTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalUpdateUserRequestItemTypeDef = TypedDict(
@@ -3794,14 +3344,44 @@
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredUserTypeDef = TypedDict(
+    "_RequiredUserTypeDef",
+    {
+        "UserId": str,
+    },
+)
+_OptionalUserTypeDef = TypedDict(
+    "_OptionalUserTypeDef",
+    {
+        "AccountId": str,
+        "PrimaryEmail": str,
+        "PrimaryProvisionedNumber": str,
+        "DisplayName": str,
+        "LicenseType": LicenseType,
+        "UserType": UserTypeType,
+        "UserRegistrationStatus": RegistrationStatusType,
+        "UserInvitationStatus": InviteStatusType,
+        "RegisteredOn": datetime,
+        "InvitedOn": datetime,
+        "AlexaForBusinessMetadata": AlexaForBusinessMetadataTypeDef,
+        "PersonalPIN": str,
+    },
+    total=False,
+)
+
+
+class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
+    pass
+
+
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -3932,230 +3512,337 @@
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+AppInstanceRetentionSettingsTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsTypeDef",
+    {
+        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+    },
+    total=False,
+)
+
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+    },
+)
+
+ArtifactsConfigurationTypeDef = TypedDict(
+    "ArtifactsConfigurationTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDeletePhoneNumberResponseTypeDef = TypedDict(
+    "BatchDeletePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
+    "BatchUpdatePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelModeratorResponseTypeDef = TypedDict(
     "CreateChannelModeratorResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AppInstanceRetentionSettingsOutputTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsOutputTypeDef",
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
     {
-        "ChannelRetentionSettings": ChannelRetentionSettingsOutputTypeDef,
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-AppInstanceRetentionSettingsTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsTypeDef",
+CreateMeetingDialOutResponseTypeDef = TypedDict(
+    "CreateMeetingDialOutResponseTypeDef",
     {
-        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+DescribeAppInstanceUserResponseTypeDef = TypedDict(
+    "DescribeAppInstanceUserResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceUser": AppInstanceUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppInstancesResponseTypeDef = TypedDict(
-    "ListAppInstancesResponseTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
-        "AppInstances": List[AppInstanceSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSettingsResponseTypeDef = TypedDict(
+    "GetAccountSettingsResponseTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+    {
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
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
     },
 )
 
 ListAppInstanceUsersResponseTypeDef = TypedDict(
     "ListAppInstanceUsersResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceUserResponseTypeDef = TypedDict(
-    "DescribeAppInstanceUserResponseTypeDef",
+ListAppInstancesResponseTypeDef = TypedDict(
+    "ListAppInstancesResponseTypeDef",
     {
-        "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstances": List[AppInstanceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ArtifactsConfigurationOutputTypeDef = TypedDict(
-    "ArtifactsConfigurationOutputTypeDef",
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationOutputTypeDef,
-        "Video": VideoArtifactsConfigurationOutputTypeDef,
-        "Content": ContentArtifactsConfigurationOutputTypeDef,
+        "Usernames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ArtifactsConfigurationTypeDef = TypedDict(
-    "ArtifactsConfigurationTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeletePhoneNumberResponseTypeDef = TypedDict(
-    "BatchDeletePhoneNumberResponseTypeDef",
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
-    "BatchUpdatePhoneNumberResponseTypeDef",
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
     {
-        "AccountId": str,
-        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateRoomMembershipRequestRequestTypeDef = TypedDict(
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -4164,98 +3851,98 @@
     },
 )
 
 BatchCreateRoomMembershipResponseTypeDef = TypedDict(
     "BatchCreateRoomMembershipResponseTypeDef",
     {
         "Errors": List[MemberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchSuspendUserResponseTypeDef = TypedDict(
     "BatchSuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUnsuspendUserResponseTypeDef = TypedDict(
     "BatchUnsuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateUserResponseTypeDef = TypedDict(
     "BatchUpdateUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "Bots": List[BotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegenerateSecurityTokenResponseTypeDef = TypedDict(
     "RegenerateSecurityTokenResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -4273,15 +3960,15 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -4396,14 +4083,38 @@
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
 
+ListAttendeeTagsResponseTypeDef = TypedDict(
+    "ListAttendeeTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListMeetingTagsResponseTypeDef = TypedDict(
+    "ListMeetingTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -4478,68 +4189,81 @@
     pass
 
 
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "Rooms": List[RoomTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "CreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
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
@@ -4579,14 +4303,29 @@
 
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
+
 _RequiredUpdateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
     },
 )
@@ -4633,44 +4372,57 @@
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
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4691,15 +4443,15 @@
 ):
     pass
 
 
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
@@ -4717,164 +4469,201 @@
     total=False,
 )
 
 GetEventsConfigurationResponseTypeDef = TypedDict(
     "GetEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventsConfigurationResponseTypeDef = TypedDict(
     "PutEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "BusinessCalling": BusinessCallingSettingsOutputTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BusinessCalling": BusinessCallingSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    {
+        "BusinessCalling": BusinessCallingSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
     },
+    total=False,
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
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
     },
 )
 
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
+    },
+    total=False,
+)
+
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
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAttendeeTagsResponseTypeDef = TypedDict(
-    "ListAttendeeTagsResponseTypeDef",
+ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "UserEmail": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListMeetingTagsResponseTypeDef = TypedDict(
-    "ListMeetingTagsResponseTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UserEmail": str,
+        "UserType": UserTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
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
 
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
@@ -4909,15 +4698,15 @@
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
@@ -4939,15 +4728,15 @@
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
@@ -4964,53 +4753,22 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
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
 
-RetentionSettingsOutputTypeDef = TypedDict(
-    "RetentionSettingsOutputTypeDef",
-    {
-        "RoomRetentionSettings": RoomRetentionSettingsOutputTypeDef,
-        "ConversationRetentionSettings": ConversationRetentionSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
@@ -5028,53 +4786,25 @@
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
-SipMediaApplicationTypeDef = TypedDict(
-    "SipMediaApplicationTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
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
 _RequiredStreamingConfigurationOutputTypeDef = TypedDict(
     "_RequiredStreamingConfigurationOutputTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationOutputTypeDef = TypedDict(
     "_OptionalStreamingConfigurationOutputTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 
 class StreamingConfigurationOutputTypeDef(
     _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
@@ -5100,296 +4830,267 @@
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
 
-UserSettingsOutputTypeDef = TypedDict(
-    "UserSettingsOutputTypeDef",
-    {
-        "Telephony": TelephonySettingsOutputTypeDef,
-    },
-)
-
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "Telephony": TelephonySettingsTypeDef,
     },
 )
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    {
-        "BusinessCalling": BusinessCallingSettingsTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
-    },
-    total=False,
-)
-
-VoiceConnectorGroupTypeDef = TypedDict(
-    "VoiceConnectorGroupTypeDef",
-    {
-        "VoiceConnectorGroupId": str,
-        "Name": str,
-        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "VoiceConnectorGroupArn": str,
-    },
-    total=False,
-)
-
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "Accounts": List[AccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountResponseTypeDef = TypedDict(
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateUserRequestRequestTypeDef = TypedDict(
+    "BatchUpdateUserRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetPersonalPINResponseTypeDef = TypedDict(
     "ResetPersonalPINResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchUpdateUserRequestRequestTypeDef = TypedDict(
-    "BatchUpdateUserRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelBansResponseTypeDef = TypedDict(
     "ListChannelBansResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelBans": List[ChannelBanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelBanResponseTypeDef = TypedDict(
     "DescribeChannelBanResponseTypeDef",
     {
         "ChannelBan": ChannelBanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsResponseTypeDef = TypedDict(
     "ListChannelMembershipsResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelMemberships": List[ChannelMembershipSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipResponseTypeDef = TypedDict(
     "DescribeChannelMembershipResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelMessageResponseTypeDef = TypedDict(
     "GetChannelMessageResponseTypeDef",
     {
         "ChannelMessage": ChannelMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelModeratorsResponseTypeDef = TypedDict(
     "ListChannelModeratorsResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelModerators": List[ChannelModeratorSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratorResponseTypeDef = TypedDict(
     "DescribeChannelModeratorResponseTypeDef",
     {
         "ChannelModerator": ChannelModeratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsResponseTypeDef",
+PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
     },
 )
 
-PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
+PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceArn": str,
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsForAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     {
         "ChannelMemberships": List[ChannelMembershipForAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channel": ChannelModeratedByAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channels": List[ChannelModeratedByAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5420,27 +5121,126 @@
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
 
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
+    {
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
@@ -5456,108 +5256,108 @@
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMeetingsResponseTypeDef = TypedDict(
     "ListMeetingsResponseTypeDef",
     {
         "Meetings": List[MeetingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRoomMembershipResponseTypeDef = TypedDict(
     "CreateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomMembershipsResponseTypeDef = TypedDict(
     "ListRoomMembershipsResponseTypeDef",
     {
         "RoomMemberships": List[RoomMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomMembershipResponseTypeDef = TypedDict(
     "UpdateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
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
@@ -5565,260 +5365,161 @@
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
-        "RetentionSettings": RetentionSettingsOutputTypeDef,
+        "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRetentionSettingsResponseTypeDef = TypedDict(
-    "PutRetentionSettingsResponseTypeDef",
+PutRetentionSettingsRequestRequestTypeDef = TypedDict(
+    "PutRetentionSettingsRequestRequestTypeDef",
     {
-        "RetentionSettings": RetentionSettingsOutputTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
+        "RetentionSettings": RetentionSettingsTypeDef,
     },
 )
 
-PutRetentionSettingsRequestRequestTypeDef = TypedDict(
-    "PutRetentionSettingsRequestRequestTypeDef",
+PutRetentionSettingsResponseTypeDef = TypedDict(
+    "PutRetentionSettingsResponseTypeDef",
     {
-        "AccountId": str,
         "RetentionSettings": RetentionSettingsTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
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
-    },
-)
-
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
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
-        "UserSettings": UserSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UserSettings": UserSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
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
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "Status": MediaPipelineStatusType,
@@ -5857,27 +5558,27 @@
     pass
 
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime/type_defs.pyi` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime.type_defs import AccountSettingsOutputTypeDef
+    from mypy_boto3_chime.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsOutputTypeDef = {...}
+    data: AccountSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -66,71 +66,58 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccountSettingsOutputTypeDef",
     "AccountSettingsTypeDef",
-    "SigninDelegateGroupOutputTypeDef",
+    "SigninDelegateGroupTypeDef",
     "AddressTypeDef",
-    "AlexaForBusinessMetadataOutputTypeDef",
     "AlexaForBusinessMetadataTypeDef",
     "IdentityTypeDef",
-    "ChannelRetentionSettingsOutputTypeDef",
     "ChannelRetentionSettingsTypeDef",
-    "AppInstanceStreamingConfigurationOutputTypeDef",
     "AppInstanceStreamingConfigurationTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "AppInstanceUserMembershipSummaryTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "AppInstanceUserTypeDef",
-    "AudioArtifactsConfigurationOutputTypeDef",
-    "ContentArtifactsConfigurationOutputTypeDef",
-    "VideoArtifactsConfigurationOutputTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
-    "SigninDelegateGroupTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "BatchSuspendUserRequestRequestTypeDef",
     "UserErrorTypeDef",
     "BatchUnsuspendUserRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "BotTypeDef",
-    "BusinessCallingSettingsOutputTypeDef",
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
-    "ConversationRetentionSettingsOutputTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "CreateMeetingDialOutRequestRequestTypeDef",
-    "CreateMeetingDialOutResponseTypeDef",
     "MeetingNotificationConfigurationTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateRoomMembershipRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
@@ -138,15 +125,14 @@
     "SipMediaApplicationEndpointTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "CreateUserRequestRequestTypeDef",
     "VoiceConnectorItemTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
     "CredentialTypeDef",
-    "DNISEmergencyCallingConfigurationOutputTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeleteAccountRequestRequestTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
@@ -181,65 +167,61 @@
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociatePhoneNumberFromUserRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
-    "GeoMatchParamsOutputTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetEventsConfigurationRequestRequestTypeDef",
-    "VoiceConnectorSettingsOutputTypeDef",
+    "VoiceConnectorSettingsTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationOutputTypeDef",
+    "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetUserRequestRequestTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
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
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
@@ -254,123 +236,114 @@
     "ListRoomMembershipsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
-    "LoggingConfigurationTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
-    "OriginationRouteOutputTypeDef",
     "OriginationRouteTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationLoggingConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
-    "RoomRetentionSettingsOutputTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
-    "SendChannelMessageResponseTypeDef",
-    "SipMediaApplicationEndpointOutputTypeDef",
-    "SipRuleTargetApplicationOutputTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
-    "StreamingNotificationTargetOutputTypeDef",
     "StreamingNotificationTargetTypeDef",
-    "TelephonySettingsOutputTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
-    "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
-    "VoiceConnectorSettingsTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
-    "VoiceConnectorItemOutputTypeDef",
-    "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
-    "UserTypeDef",
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateChannelBanResponseTypeDef",
-    "CreateChannelMembershipResponseTypeDef",
-    "CreateChannelModeratorResponseTypeDef",
-    "AppInstanceRetentionSettingsOutputTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "DescribeAppInstanceUserResponseTypeDef",
-    "ArtifactsConfigurationOutputTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
+    "CreateChannelBanResponseTypeDef",
+    "CreateChannelMembershipResponseTypeDef",
+    "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "CreateMeetingDialOutResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "DescribeAppInstanceUserResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSettingsResponseTypeDef",
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SendChannelMessageResponseTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
+    "UpdateChannelMessageResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -387,110 +360,122 @@
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "ListAttendeeTagsResponseTypeDef",
+    "ListMeetingTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagAttendeeRequestRequestTypeDef",
     "TagMeetingRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "ListRoomsResponseTypeDef",
     "UpdateRoomResponseTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
+    "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
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
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
+    "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
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
     "InviteUsersResponseTypeDef",
-    "ListAttendeeTagsResponseTypeDef",
-    "ListMeetingTagsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
-    "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
-    "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    "RetentionSettingsOutputTypeDef",
     "RetentionSettingsTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
-    "SipMediaApplicationTypeDef",
-    "SipRuleTypeDef",
     "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
-    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    "VoiceConnectorGroupTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
+    "BatchUpdateUserRequestRequestTypeDef",
     "CreateUserResponseTypeDef",
     "GetUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ResetPersonalPINResponseTypeDef",
     "UpdateUserResponseTypeDef",
-    "BatchUpdateUserRequestRequestTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
-    "PutAppInstanceRetentionSettingsResponseTypeDef",
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
+    "PutAppInstanceRetentionSettingsResponseTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
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
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
@@ -509,62 +494,41 @@
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "GetRetentionSettingsResponseTypeDef",
-    "PutRetentionSettingsResponseTypeDef",
     "PutRetentionSettingsRequestRequestTypeDef",
+    "PutRetentionSettingsResponseTypeDef",
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
-    "CreateSipMediaApplicationResponseTypeDef",
-    "GetSipMediaApplicationResponseTypeDef",
-    "ListSipMediaApplicationsResponseTypeDef",
-    "UpdateSipMediaApplicationResponseTypeDef",
-    "CreateSipRuleResponseTypeDef",
-    "GetSipRuleResponseTypeDef",
-    "ListSipRulesResponseTypeDef",
-    "UpdateSipRuleResponseTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "CreateVoiceConnectorGroupResponseTypeDef",
-    "GetVoiceConnectorGroupResponseTypeDef",
-    "ListVoiceConnectorGroupsResponseTypeDef",
-    "UpdateVoiceConnectorGroupResponseTypeDef",
     "MediaCapturePipelineTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
-AccountSettingsOutputTypeDef = TypedDict(
-    "AccountSettingsOutputTypeDef",
-    {
-        "DisableRemoteControl": bool,
-        "EnableDialOut": bool,
-    },
-    total=False,
-)
-
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "DisableRemoteControl": bool,
         "EnableDialOut": bool,
     },
     total=False,
 )
 
-SigninDelegateGroupOutputTypeDef = TypedDict(
-    "SigninDelegateGroupOutputTypeDef",
+SigninDelegateGroupTypeDef = TypedDict(
+    "SigninDelegateGroupTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
 AddressTypeDef = TypedDict(
@@ -580,23 +544,14 @@
         "postalCode": str,
         "postalCodePlus4": str,
         "country": str,
     },
     total=False,
 )
 
-AlexaForBusinessMetadataOutputTypeDef = TypedDict(
-    "AlexaForBusinessMetadataOutputTypeDef",
-    {
-        "IsAlexaForBusinessEnabled": bool,
-        "AlexaForBusinessRoomArn": str,
-    },
-    total=False,
-)
-
 AlexaForBusinessMetadataTypeDef = TypedDict(
     "AlexaForBusinessMetadataTypeDef",
     {
         "IsAlexaForBusinessEnabled": bool,
         "AlexaForBusinessRoomArn": str,
     },
     total=False,
@@ -607,38 +562,22 @@
     {
         "Arn": str,
         "Name": str,
     },
     total=False,
 )
 
-ChannelRetentionSettingsOutputTypeDef = TypedDict(
-    "ChannelRetentionSettingsOutputTypeDef",
-    {
-        "RetentionDays": int,
-    },
-    total=False,
-)
-
 ChannelRetentionSettingsTypeDef = TypedDict(
     "ChannelRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
 
-AppInstanceStreamingConfigurationOutputTypeDef = TypedDict(
-    "AppInstanceStreamingConfigurationOutputTypeDef",
-    {
-        "AppInstanceDataType": AppInstanceDataTypeType,
-        "ResourceArn": str,
-    },
-)
-
 AppInstanceStreamingConfigurationTypeDef = TypedDict(
     "AppInstanceStreamingConfigurationTypeDef",
     {
         "AppInstanceDataType": AppInstanceDataTypeType,
         "ResourceArn": str,
     },
 )
@@ -692,61 +631,14 @@
         "CreatedTimestamp": datetime,
         "Metadata": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-AudioArtifactsConfigurationOutputTypeDef = TypedDict(
-    "AudioArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": AudioMuxTypeType,
-    },
-)
-
-_RequiredContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredContentArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalContentArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalContentArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["ContentOnly"],
-    },
-    total=False,
-)
-
-class ContentArtifactsConfigurationOutputTypeDef(
-    _RequiredContentArtifactsConfigurationOutputTypeDef,
-    _OptionalContentArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
-_RequiredVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "State": ArtifactsStateType,
-    },
-)
-_OptionalVideoArtifactsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVideoArtifactsConfigurationOutputTypeDef",
-    {
-        "MuxType": Literal["VideoOnly"],
-    },
-    total=False,
-)
-
-class VideoArtifactsConfigurationOutputTypeDef(
-    _RequiredVideoArtifactsConfigurationOutputTypeDef,
-    _OptionalVideoArtifactsConfigurationOutputTypeDef,
-):
-    pass
-
 AudioArtifactsConfigurationTypeDef = TypedDict(
     "AudioArtifactsConfigurationTypeDef",
     {
         "MuxType": AudioMuxTypeType,
     },
 )
 
@@ -824,14 +716,25 @@
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
@@ -845,22 +748,14 @@
 
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
-SigninDelegateGroupTypeDef = TypedDict(
-    "SigninDelegateGroupTypeDef",
-    {
-        "GroupName": str,
-    },
-    total=False,
-)
-
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
     },
@@ -993,22 +888,14 @@
         "UpdatedTimestamp": datetime,
         "BotEmail": str,
         "SecurityToken": str,
     },
     total=False,
 )
 
-BusinessCallingSettingsOutputTypeDef = TypedDict(
-    "BusinessCallingSettingsOutputTypeDef",
-    {
-        "CdrBucket": str,
-    },
-    total=False,
-)
-
 BusinessCallingSettingsTypeDef = TypedDict(
     "BusinessCallingSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
@@ -1036,22 +923,14 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
-ConversationRetentionSettingsOutputTypeDef = TypedDict(
-    "ConversationRetentionSettingsOutputTypeDef",
-    {
-        "RetentionDays": int,
-    },
-    total=False,
-)
-
 ConversationRetentionSettingsTypeDef = TypedDict(
     "ConversationRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -1075,30 +954,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "DisplayName": str,
     },
 )
@@ -1174,40 +1037,24 @@
 
 class CreateChannelModeratorRequestRequestTypeDef(
     _RequiredCreateChannelModeratorRequestRequestTypeDef,
     _OptionalCreateChannelModeratorRequestRequestTypeDef,
 ):
     pass
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMeetingDialOutRequestRequestTypeDef = TypedDict(
     "CreateMeetingDialOutRequestRequestTypeDef",
     {
         "MeetingId": str,
         "FromPhoneNumber": str,
         "ToPhoneNumber": str,
         "JoinToken": str,
     },
 )
 
-CreateMeetingDialOutResponseTypeDef = TypedDict(
-    "CreateMeetingDialOutResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MeetingNotificationConfigurationTypeDef = TypedDict(
     "MeetingNotificationConfigurationTypeDef",
     {
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
     total=False,
@@ -1402,35 +1249,14 @@
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
@@ -1893,21 +1719,14 @@
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     {
         "AccountId": str,
         "GroupNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -1956,22 +1775,14 @@
         "BotId": str,
         "OutboundEventsHTTPSEndpoint": str,
         "LambdaFunctionArn": str,
     },
     total=False,
 )
 
-GeoMatchParamsOutputTypeDef = TypedDict(
-    "GeoMatchParamsOutputTypeDef",
-    {
-        "Country": str,
-        "AreaCode": str,
-    },
-)
-
 GetAccountRequestRequestTypeDef = TypedDict(
     "GetAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -2036,16 +1847,16 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
 
-VoiceConnectorSettingsOutputTypeDef = TypedDict(
-    "VoiceConnectorSettingsOutputTypeDef",
+VoiceConnectorSettingsTypeDef = TypedDict(
+    "VoiceConnectorSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
 
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
@@ -2080,23 +1891,14 @@
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
@@ -2119,16 +1921,16 @@
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
@@ -2178,16 +1980,16 @@
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
 
@@ -2292,20 +2094,20 @@
 )
 
 class InviteUsersRequestRequestTypeDef(
     _RequiredInviteUsersRequestRequestTypeDef, _OptionalInviteUsersRequestRequestTypeDef
 ):
     pass
 
-ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Name": str,
-        "UserEmail": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountsRequestRequestTypeDef = TypedDict(
     "ListAccountsRequestRequestTypeDef",
     {
@@ -2372,22 +2174,14 @@
     "ListAttendeeTagsRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
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
 _RequiredListAttendeesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttendeesRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 _OptionalListAttendeesRequestRequestTypeDef = TypedDict(
@@ -2708,36 +2502,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserEmail": str,
-        "UserType": UserTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -2768,40 +2540,23 @@
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
 LogoutUserRequestRequestTypeDef = TypedDict(
     "LogoutUserRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
     },
 )
@@ -2838,48 +2593,26 @@
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
@@ -2926,22 +2659,14 @@
 
 class PutEventsConfigurationRequestRequestTypeDef(
     _RequiredPutEventsConfigurationRequestRequestTypeDef,
     _OptionalPutEventsConfigurationRequestRequestTypeDef,
 ):
     pass
 
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
@@ -2990,23 +2715,14 @@
 
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedactConversationMessageRequestRequestTypeDef = TypedDict(
     "RedactConversationMessageRequestRequestTypeDef",
     {
         "AccountId": str,
         "ConversationId": str,
         "MessageId": str,
     },
@@ -3033,40 +2749,21 @@
     "ResetPersonalPINRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-RoomRetentionSettingsOutputTypeDef = TypedDict(
-    "RoomRetentionSettingsOutputTypeDef",
-    {
-        "RetentionDays": int,
-    },
-    total=False,
-)
-
 RoomRetentionSettingsTypeDef = TypedDict(
     "RoomRetentionSettingsTypeDef",
     {
         "RetentionDays": int,
     },
     total=False,
 )
@@ -3082,23 +2779,14 @@
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
 SelectedVideoStreamsOutputTypeDef = TypedDict(
     "SelectedVideoStreamsOutputTypeDef",
     {
         "AttendeeIds": List[str],
         "ExternalUserIds": List[str],
     },
     total=False,
@@ -3134,71 +2822,28 @@
 
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
     _OptionalSendChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
-StreamingNotificationTargetOutputTypeDef = TypedDict(
-    "StreamingNotificationTargetOutputTypeDef",
-    {
-        "NotificationTarget": NotificationTargetType,
-    },
-)
-
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
 )
 
-TelephonySettingsOutputTypeDef = TypedDict(
-    "TelephonySettingsOutputTypeDef",
-    {
-        "InboundCalling": bool,
-        "OutboundCalling": bool,
-        "SMS": bool,
-    },
-)
-
 TelephonySettingsTypeDef = TypedDict(
     "TelephonySettingsTypeDef",
     {
         "InboundCalling": bool,
         "OutboundCalling": bool,
         "SMS": bool,
     },
@@ -3265,22 +2910,14 @@
 )
 
 class UpdateAppInstanceRequestRequestTypeDef(
     _RequiredUpdateAppInstanceRequestRequestTypeDef, _OptionalUpdateAppInstanceRequestRequestTypeDef
 ):
     pass
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
     },
 )
@@ -3294,22 +2931,14 @@
 
 class UpdateAppInstanceUserRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
@@ -3345,23 +2974,14 @@
 
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
@@ -3374,22 +2994,14 @@
 
 class UpdateChannelReadMarkerRequestRequestTypeDef(
     _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
     _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
 ):
     pass
 
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Mode": ChannelModeType,
     },
@@ -3404,30 +3016,14 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
@@ -3542,30 +3138,14 @@
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
-GetAccountSettingsResponseTypeDef = TypedDict(
-    "GetAccountSettingsResponseTypeDef",
-    {
-        "AccountSettings": AccountSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "AccountSettings": AccountSettingsTypeDef,
     },
 )
@@ -3582,50 +3162,30 @@
     "_OptionalAccountTypeDef",
     {
         "AccountType": AccountTypeType,
         "CreatedTimestamp": datetime,
         "DefaultLicense": LicenseType,
         "SupportedLicenses": List[LicenseType],
         "AccountStatus": AccountStatusType,
-        "SigninDelegateGroups": List[SigninDelegateGroupOutputTypeDef],
+        "SigninDelegateGroups": List[SigninDelegateGroupTypeDef],
     },
     total=False,
 )
 
 class AccountTypeDef(_RequiredAccountTypeDef, _OptionalAccountTypeDef):
     pass
 
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
-    {
-        "UserId": str,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
+AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
+    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     {
         "AccountId": str,
-        "PrimaryEmail": str,
-        "PrimaryProvisionedNumber": str,
-        "DisplayName": str,
-        "LicenseType": LicenseType,
-        "UserType": UserTypeType,
-        "UserRegistrationStatus": RegistrationStatusType,
-        "UserInvitationStatus": InviteStatusType,
-        "RegisteredOn": datetime,
-        "InvitedOn": datetime,
-        "AlexaForBusinessMetadata": AlexaForBusinessMetadataOutputTypeDef,
-        "PersonalPIN": str,
+        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
     },
-    total=False,
 )
 
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
 _RequiredUpdateUserRequestItemTypeDef = TypedDict(
     "_RequiredUpdateUserRequestItemTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalUpdateUserRequestItemTypeDef = TypedDict(
@@ -3661,14 +3221,42 @@
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
+_RequiredUserTypeDef = TypedDict(
+    "_RequiredUserTypeDef",
+    {
+        "UserId": str,
+    },
+)
+_OptionalUserTypeDef = TypedDict(
+    "_OptionalUserTypeDef",
+    {
+        "AccountId": str,
+        "PrimaryEmail": str,
+        "PrimaryProvisionedNumber": str,
+        "DisplayName": str,
+        "LicenseType": LicenseType,
+        "UserType": UserTypeType,
+        "UserRegistrationStatus": RegistrationStatusType,
+        "UserInvitationStatus": InviteStatusType,
+        "RegisteredOn": datetime,
+        "InvitedOn": datetime,
+        "AlexaForBusinessMetadata": AlexaForBusinessMetadataTypeDef,
+        "PersonalPIN": str,
+    },
+    total=False,
+)
+
+class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
+    pass
+
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -3799,230 +3387,337 @@
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+AppInstanceRetentionSettingsTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsTypeDef",
+    {
+        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+    },
+    total=False,
+)
+
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+    },
+)
+
+ArtifactsConfigurationTypeDef = TypedDict(
+    "ArtifactsConfigurationTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDeletePhoneNumberResponseTypeDef = TypedDict(
+    "BatchDeletePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
+    "BatchUpdatePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelModeratorResponseTypeDef = TypedDict(
     "CreateChannelModeratorResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AppInstanceRetentionSettingsOutputTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsOutputTypeDef",
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
     {
-        "ChannelRetentionSettings": ChannelRetentionSettingsOutputTypeDef,
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-AppInstanceRetentionSettingsTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsTypeDef",
+CreateMeetingDialOutResponseTypeDef = TypedDict(
+    "CreateMeetingDialOutResponseTypeDef",
     {
-        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+DescribeAppInstanceUserResponseTypeDef = TypedDict(
+    "DescribeAppInstanceUserResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceUser": AppInstanceUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppInstancesResponseTypeDef = TypedDict(
-    "ListAppInstancesResponseTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
-        "AppInstances": List[AppInstanceSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSettingsResponseTypeDef = TypedDict(
+    "GetAccountSettingsResponseTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+    {
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
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
     },
 )
 
 ListAppInstanceUsersResponseTypeDef = TypedDict(
     "ListAppInstanceUsersResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceUserResponseTypeDef = TypedDict(
-    "DescribeAppInstanceUserResponseTypeDef",
+ListAppInstancesResponseTypeDef = TypedDict(
+    "ListAppInstancesResponseTypeDef",
     {
-        "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstances": List[AppInstanceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ArtifactsConfigurationOutputTypeDef = TypedDict(
-    "ArtifactsConfigurationOutputTypeDef",
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationOutputTypeDef,
-        "Video": VideoArtifactsConfigurationOutputTypeDef,
-        "Content": ContentArtifactsConfigurationOutputTypeDef,
+        "Usernames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ArtifactsConfigurationTypeDef = TypedDict(
-    "ArtifactsConfigurationTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeletePhoneNumberResponseTypeDef = TypedDict(
-    "BatchDeletePhoneNumberResponseTypeDef",
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
-    "BatchUpdatePhoneNumberResponseTypeDef",
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef = TypedDict(
-    "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
     {
-        "AccountId": str,
-        "SigninDelegateGroups": Sequence[SigninDelegateGroupTypeDef],
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateRoomMembershipRequestRequestTypeDef = TypedDict(
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -4031,98 +3726,98 @@
     },
 )
 
 BatchCreateRoomMembershipResponseTypeDef = TypedDict(
     "BatchCreateRoomMembershipResponseTypeDef",
     {
         "Errors": List[MemberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchSuspendUserResponseTypeDef = TypedDict(
     "BatchSuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUnsuspendUserResponseTypeDef = TypedDict(
     "BatchUnsuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateUserResponseTypeDef = TypedDict(
     "BatchUpdateUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "Bots": List[BotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegenerateSecurityTokenResponseTypeDef = TypedDict(
     "RegenerateSecurityTokenResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -4140,15 +3835,15 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -4253,14 +3948,38 @@
 )
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+ListAttendeeTagsResponseTypeDef = TypedDict(
+    "ListAttendeeTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListMeetingTagsResponseTypeDef = TypedDict(
+    "ListMeetingTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "AttendeeId": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -4331,68 +4050,81 @@
 ):
     pass
 
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "Rooms": List[RoomTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "CreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
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
@@ -4428,14 +4160,29 @@
 )
 
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
+
 _RequiredUpdateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
     },
 )
@@ -4478,44 +4225,57 @@
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
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4534,15 +4294,15 @@
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
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
@@ -4560,164 +4320,197 @@
     total=False,
 )
 
 GetEventsConfigurationResponseTypeDef = TypedDict(
     "GetEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventsConfigurationResponseTypeDef = TypedDict(
     "PutEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
-        "BusinessCalling": BusinessCallingSettingsOutputTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BusinessCalling": BusinessCallingSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateGlobalSettingsRequestRequestTypeDef",
+    {
+        "BusinessCalling": BusinessCallingSettingsTypeDef,
+        "VoiceConnector": VoiceConnectorSettingsTypeDef,
     },
+    total=False,
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
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
     },
 )
 
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
+    },
+    total=False,
+)
+
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
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAttendeeTagsResponseTypeDef = TypedDict(
-    "ListAttendeeTagsResponseTypeDef",
+ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "UserEmail": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListMeetingTagsResponseTypeDef = TypedDict(
-    "ListMeetingTagsResponseTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UserEmail": str,
+        "UserType": UserTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
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
 
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
@@ -4752,15 +4545,15 @@
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
@@ -4782,15 +4575,15 @@
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
@@ -4807,51 +4600,22 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
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
-
 PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Termination": TerminationTypeDef,
     },
 )
 
-RetentionSettingsOutputTypeDef = TypedDict(
-    "RetentionSettingsOutputTypeDef",
-    {
-        "RoomRetentionSettings": RoomRetentionSettingsOutputTypeDef,
-        "ConversationRetentionSettings": ConversationRetentionSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
@@ -4869,53 +4633,25 @@
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
-SipMediaApplicationTypeDef = TypedDict(
-    "SipMediaApplicationTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": List[SipMediaApplicationEndpointOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
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
 _RequiredStreamingConfigurationOutputTypeDef = TypedDict(
     "_RequiredStreamingConfigurationOutputTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationOutputTypeDef = TypedDict(
     "_OptionalStreamingConfigurationOutputTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetOutputTypeDef],
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 class StreamingConfigurationOutputTypeDef(
     _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
 ):
@@ -4937,296 +4673,267 @@
 )
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
-UserSettingsOutputTypeDef = TypedDict(
-    "UserSettingsOutputTypeDef",
-    {
-        "Telephony": TelephonySettingsOutputTypeDef,
-    },
-)
-
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "Telephony": TelephonySettingsTypeDef,
     },
 )
 
-UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateGlobalSettingsRequestRequestTypeDef",
-    {
-        "BusinessCalling": BusinessCallingSettingsTypeDef,
-        "VoiceConnector": VoiceConnectorSettingsTypeDef,
-    },
-    total=False,
-)
-
-VoiceConnectorGroupTypeDef = TypedDict(
-    "VoiceConnectorGroupTypeDef",
-    {
-        "VoiceConnectorGroupId": str,
-        "Name": str,
-        "VoiceConnectorItems": List[VoiceConnectorItemOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "VoiceConnectorGroupArn": str,
-    },
-    total=False,
-)
-
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "Accounts": List[AccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountResponseTypeDef = TypedDict(
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateUserRequestRequestTypeDef = TypedDict(
+    "BatchUpdateUserRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetPersonalPINResponseTypeDef = TypedDict(
     "ResetPersonalPINResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchUpdateUserRequestRequestTypeDef = TypedDict(
-    "BatchUpdateUserRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "UpdateUserRequestItems": Sequence[UpdateUserRequestItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelBansResponseTypeDef = TypedDict(
     "ListChannelBansResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelBans": List[ChannelBanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelBanResponseTypeDef = TypedDict(
     "DescribeChannelBanResponseTypeDef",
     {
         "ChannelBan": ChannelBanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsResponseTypeDef = TypedDict(
     "ListChannelMembershipsResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelMemberships": List[ChannelMembershipSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipResponseTypeDef = TypedDict(
     "DescribeChannelMembershipResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelMessageResponseTypeDef = TypedDict(
     "GetChannelMessageResponseTypeDef",
     {
         "ChannelMessage": ChannelMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelModeratorsResponseTypeDef = TypedDict(
     "ListChannelModeratorsResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelModerators": List[ChannelModeratorSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratorResponseTypeDef = TypedDict(
     "DescribeChannelModeratorResponseTypeDef",
     {
         "ChannelModerator": ChannelModeratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsResponseTypeDef",
+PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
-        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsOutputTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
     },
 )
 
-PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
+PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
+    "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
-        "AppInstanceArn": str,
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsForAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     {
         "ChannelMemberships": List[ChannelMembershipForAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channel": ChannelModeratedByAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channels": List[ChannelModeratedByAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5255,27 +4962,126 @@
 
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
+CreateSipMediaApplicationResponseTypeDef = TypedDict(
+    "CreateSipMediaApplicationResponseTypeDef",
+    {
+        "SipMediaApplication": SipMediaApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSipMediaApplicationResponseTypeDef = TypedDict(
+    "GetSipMediaApplicationResponseTypeDef",
+    {
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
@@ -5291,108 +5097,108 @@
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMeetingsResponseTypeDef = TypedDict(
     "ListMeetingsResponseTypeDef",
     {
         "Meetings": List[MeetingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRoomMembershipResponseTypeDef = TypedDict(
     "CreateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomMembershipsResponseTypeDef = TypedDict(
     "ListRoomMembershipsResponseTypeDef",
     {
         "RoomMemberships": List[RoomMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomMembershipResponseTypeDef = TypedDict(
     "UpdateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
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
@@ -5400,260 +5206,161 @@
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
-        "RetentionSettings": RetentionSettingsOutputTypeDef,
+        "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRetentionSettingsResponseTypeDef = TypedDict(
-    "PutRetentionSettingsResponseTypeDef",
+PutRetentionSettingsRequestRequestTypeDef = TypedDict(
+    "PutRetentionSettingsRequestRequestTypeDef",
     {
-        "RetentionSettings": RetentionSettingsOutputTypeDef,
-        "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountId": str,
+        "RetentionSettings": RetentionSettingsTypeDef,
     },
 )
 
-PutRetentionSettingsRequestRequestTypeDef = TypedDict(
-    "PutRetentionSettingsRequestRequestTypeDef",
+PutRetentionSettingsResponseTypeDef = TypedDict(
+    "PutRetentionSettingsResponseTypeDef",
     {
-        "AccountId": str,
         "RetentionSettings": RetentionSettingsTypeDef,
+        "InitiateDeletionTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationOutputTypeDef",
     {
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
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
-    },
-)
-
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
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
-        "UserSettings": UserSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UserSettings": UserSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
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
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "Status": MediaPipelineStatusType,
@@ -5690,27 +5397,27 @@
 ):
     pass
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/PKG-INFO` & `mypy-boto3-chime-1.28.15/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-chime
-Version: 1.28.12
-Summary: Type annotations for boto3.Chime 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 chime type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-chime"></a>
 
 # mypy-boto3-chime
 
 [![PyPI - mypy-boto3-chime](https://img.shields.io/pypi/v/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime)](https://pepy.tech/project/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [mypy-boto3-chime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -370,71 +338,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime.type_defs import (
-    AccountSettingsOutputTypeDef,
     AccountSettingsTypeDef,
-    SigninDelegateGroupOutputTypeDef,
+    SigninDelegateGroupTypeDef,
     AddressTypeDef,
-    AlexaForBusinessMetadataOutputTypeDef,
     AlexaForBusinessMetadataTypeDef,
     IdentityTypeDef,
-    ChannelRetentionSettingsOutputTypeDef,
     ChannelRetentionSettingsTypeDef,
-    AppInstanceStreamingConfigurationOutputTypeDef,
     AppInstanceStreamingConfigurationTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     AppInstanceUserMembershipSummaryTypeDef,
     AppInstanceUserSummaryTypeDef,
     AppInstanceUserTypeDef,
-    AudioArtifactsConfigurationOutputTypeDef,
-    ContentArtifactsConfigurationOutputTypeDef,
-    VideoArtifactsConfigurationOutputTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
-    SigninDelegateGroupTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     BatchSuspendUserRequestRequestTypeDef,
     UserErrorTypeDef,
     BatchUnsuspendUserRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     BotTypeDef,
-    BusinessCallingSettingsOutputTypeDef,
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
-    ConversationRetentionSettingsOutputTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -442,15 +397,14 @@
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     CreateUserRequestRequestTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     CredentialTypeDef,
-    DNISEmergencyCallingConfigurationOutputTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeleteAccountRequestRequestTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
@@ -485,65 +439,61 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
-    GeoMatchParamsOutputTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetEventsConfigurationRequestRequestTypeDef,
-    VoiceConnectorSettingsOutputTypeDef,
+    VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationOutputTypeDef,
+    SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
     GetUserSettingsRequestRequestTypeDef,
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
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
@@ -558,123 +508,114 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
-    LoggingConfigurationTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
-    OriginationRouteOutputTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
-    SipMediaApplicationLoggingConfigurationTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
-    RoomRetentionSettingsOutputTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
     SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
-    SendChannelMessageResponseTypeDef,
-    SipMediaApplicationEndpointOutputTypeDef,
-    SipRuleTargetApplicationOutputTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
-    StreamingNotificationTargetOutputTypeDef,
     StreamingNotificationTargetTypeDef,
-    TelephonySettingsOutputTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
-    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
-    VoiceConnectorSettingsTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    VoiceConnectorItemOutputTypeDef,
-    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
-    UserTypeDef,
+    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
+    UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
-    AppInstanceRetentionSettingsOutputTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
-    ArtifactsConfigurationOutputTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSettingsResponseTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SendChannelMessageResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
+    UpdateChannelMessageResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -691,110 +632,122 @@
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
+    ListAttendeeTagsResponseTypeDef,
+    ListMeetingTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagAttendeeRequestRequestTypeDef,
     TagMeetingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     ListRoomsResponseTypeDef,
     UpdateRoomResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
+    SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
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
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
+    UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
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
     InviteUsersResponseTypeDef,
-    ListAttendeeTagsResponseTypeDef,
-    ListMeetingTagsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
-    PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
-    PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
-    RetentionSettingsOutputTypeDef,
     RetentionSettingsTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
-    SipMediaApplicationTypeDef,
-    SipRuleTypeDef,
     StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
-    UserSettingsOutputTypeDef,
     UserSettingsTypeDef,
-    UpdateGlobalSettingsRequestRequestTypeDef,
-    VoiceConnectorGroupTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
+    BatchUpdateUserRequestRequestTypeDef,
     CreateUserResponseTypeDef,
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     ResetPersonalPINResponseTypeDef,
     UpdateUserResponseTypeDef,
-    BatchUpdateUserRequestRequestTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
-    PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
+    PutAppInstanceRetentionSettingsResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
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
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
@@ -813,44 +766,32 @@
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     GetRetentionSettingsResponseTypeDef,
-    PutRetentionSettingsResponseTypeDef,
     PutRetentionSettingsRequestRequestTypeDef,
+    PutRetentionSettingsResponseTypeDef,
     ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
-    CreateSipMediaApplicationResponseTypeDef,
-    GetSipMediaApplicationResponseTypeDef,
-    ListSipMediaApplicationsResponseTypeDef,
-    UpdateSipMediaApplicationResponseTypeDef,
-    CreateSipRuleResponseTypeDef,
-    GetSipRuleResponseTypeDef,
-    ListSipRulesResponseTypeDef,
-    UpdateSipRuleResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateVoiceConnectorGroupResponseTypeDef,
-    GetVoiceConnectorGroupResponseTypeDef,
-    ListVoiceConnectorGroupsResponseTypeDef,
-    UpdateVoiceConnectorGroupResponseTypeDef,
     MediaCapturePipelineTypeDef,
     CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsOutputTypeDef:
+def get_structure() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-1.28.12/mypy_boto3_chime.egg-info/SOURCES.txt` & `mypy-boto3-chime-1.28.15/mypy_boto3_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.28.12/setup.py` & `mypy-boto3-chime-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Chime 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Chime 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

