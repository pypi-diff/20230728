# Comparing `tmp/mypy-boto3-chime-sdk-messaging-1.28.12.tar.gz` & `tmp/mypy-boto3-chime-sdk-messaging-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.28.12.tar", last modified: Thu Jul 27 05:34:23 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-messaging-1.28.12.tar` & `mypy-boto3-chime-sdk-messaging-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.944565 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-27 05:18:18.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50483 2023-07-27 05:18:19.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50424 2023-07-27 05:18:19.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:34:23.000000 mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:23.948565 mypy-boto3-chime-sdk-messaging-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-messaging-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.180777 mypy-boto3-chime-sdk-messaging-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-07-28 20:42:25.176777 mypy-boto3-chime-sdk-messaging-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16833 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.176777 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-07-28 20:20:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-28 20:20:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-28 20:20:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47771 2023-07-28 20:20:41.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47714 2023-07-28 20:20:40.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:39.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.176777 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-07-28 20:42:24.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 20:42:24.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:24.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:24.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:24.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:42:24.000000 mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.180777 mypy-boto3-chime-sdk-messaging-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-28 20:20:38.000000 mypy-boto3-chime-sdk-messaging-1.28.15/setup.py
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/LICENSE` & `mypy-boto3-chime-sdk-messaging-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,34 +318,29 @@
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
-    PushNotificationPreferencesOutputTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
     MessageAttributeValueOutputTypeDef,
-    TargetOutputTypeDef,
-    ElasticChannelConfigurationOutputTypeDef,
-    ExpirationSettingsOutputTypeDef,
+    TargetTypeDef,
+    ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    ElasticChannelConfigurationTypeDef,
-    ExpirationSettingsTypeDef,
-    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -353,106 +348,101 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
-    StreamingConfigurationOutputTypeDef,
-    LambdaConfigurationOutputTypeDef,
+    StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    StreamingConfigurationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
-    TargetTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    UpdateChannelFlowResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
-    ChannelMembershipPreferencesOutputTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
-    PutChannelExpirationSettingsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
+    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
-    ProcessorConfigurationOutputTypeDef,
     ProcessorConfigurationTypeDef,
     ListSubChannelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     SearchChannelsRequestRequestTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
-    PutChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
+    PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
-    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/README.md` & `mypy-boto3-chime-sdk-messaging-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,34 +286,29 @@
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
-    PushNotificationPreferencesOutputTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
     MessageAttributeValueOutputTypeDef,
-    TargetOutputTypeDef,
-    ElasticChannelConfigurationOutputTypeDef,
-    ExpirationSettingsOutputTypeDef,
+    TargetTypeDef,
+    ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    ElasticChannelConfigurationTypeDef,
-    ExpirationSettingsTypeDef,
-    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -321,106 +316,101 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
-    StreamingConfigurationOutputTypeDef,
-    LambdaConfigurationOutputTypeDef,
+    StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    StreamingConfigurationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
-    TargetTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    UpdateChannelFlowResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
-    ChannelMembershipPreferencesOutputTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
-    PutChannelExpirationSettingsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
+    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
-    ProcessorConfigurationOutputTypeDef,
     ProcessorConfigurationTypeDef,
     ListSubChannelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     SearchChannelsRequestRequestTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
-    PutChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
+    PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
-    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/__main__.py` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMessaging 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMessaging 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.py` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/client.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.py` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/literals.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.py` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,34 +44,29 @@
 
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
-    "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
-    "PushNotificationPreferencesOutputTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
     "MessageAttributeValueOutputTypeDef",
-    "TargetOutputTypeDef",
-    "ElasticChannelConfigurationOutputTypeDef",
-    "ExpirationSettingsOutputTypeDef",
+    "TargetTypeDef",
+    "ElasticChannelConfigurationTypeDef",
+    "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "ElasticChannelConfigurationTypeDef",
-    "ExpirationSettingsTypeDef",
-    "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
@@ -79,106 +74,101 @@
     "DescribeChannelFlowRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelMembershipRequestRequestTypeDef",
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociateChannelFlowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
-    "StreamingConfigurationOutputTypeDef",
-    "LambdaConfigurationOutputTypeDef",
+    "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "StreamingConfigurationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
-    "TargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
+    "ChannelFlowCallbackResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
+    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "UpdateChannelFlowResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
-    "ChannelMembershipPreferencesOutputTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
+    "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateChannelRequestRequestTypeDef",
-    "PutChannelExpirationSettingsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
-    "ProcessorConfigurationOutputTypeDef",
     "ProcessorConfigurationTypeDef",
     "ListSubChannelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "SearchChannelsRequestRequestTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
-    "PutChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
+    "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
-    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
     "UpdateChannelFlowRequestRequestTypeDef",
     "ListChannelFlowsResponseTypeDef",
     "DescribeChannelFlowResponseTypeDef",
@@ -243,70 +233,50 @@
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
 
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
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
     },
     total=False,
 )
 
-ChannelFlowCallbackResponseTypeDef = TypedDict(
-    "ChannelFlowCallbackResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "CallbackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredPushNotificationPreferencesOutputTypeDef = TypedDict(
-    "_RequiredPushNotificationPreferencesOutputTypeDef",
-    {
-        "AllowNotifications": AllowNotificationsType,
-    },
-)
-_OptionalPushNotificationPreferencesOutputTypeDef = TypedDict(
-    "_OptionalPushNotificationPreferencesOutputTypeDef",
-    {
-        "FilterRule": str,
-    },
-    total=False,
-)
-
-
-class PushNotificationPreferencesOutputTypeDef(
-    _RequiredPushNotificationPreferencesOutputTypeDef,
-    _OptionalPushNotificationPreferencesOutputTypeDef,
-):
-    pass
-
-
 _RequiredPushNotificationPreferencesTypeDef = TypedDict(
     "_RequiredPushNotificationPreferencesTypeDef",
     {
         "AllowNotifications": AllowNotificationsType,
     },
 )
 _OptionalPushNotificationPreferencesTypeDef = TypedDict(
@@ -355,33 +325,33 @@
     "MessageAttributeValueOutputTypeDef",
     {
         "StringValues": List[str],
     },
     total=False,
 )
 
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
 
-ElasticChannelConfigurationOutputTypeDef = TypedDict(
-    "ElasticChannelConfigurationOutputTypeDef",
+ElasticChannelConfigurationTypeDef = TypedDict(
+    "ElasticChannelConfigurationTypeDef",
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
 )
 
-ExpirationSettingsOutputTypeDef = TypedDict(
-    "ExpirationSettingsOutputTypeDef",
+ExpirationSettingsTypeDef = TypedDict(
+    "ExpirationSettingsTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": ExpirationCriterionType,
     },
 )
 
 CreateChannelBanRequestRequestTypeDef = TypedDict(
@@ -397,22 +367,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChannelFlowResponseTypeDef = TypedDict(
-    "CreateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateChannelMembershipRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelMembershipRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "Type": ChannelMembershipTypeType,
         "ChimeBearer": str,
@@ -439,39 +401,14 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
-ElasticChannelConfigurationTypeDef = TypedDict(
-    "ElasticChannelConfigurationTypeDef",
-    {
-        "MaximumSubChannels": int,
-        "TargetMembershipsPerSubChannel": int,
-        "MinimumMembershipPercentage": int,
-    },
-)
-
-ExpirationSettingsTypeDef = TypedDict(
-    "ExpirationSettingsTypeDef",
-    {
-        "ExpirationDays": int,
-        "ExpirationCriterion": ExpirationCriterionType,
-    },
-)
-
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChannelBanRequestRequestTypeDef = TypedDict(
     "DeleteChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -636,21 +573,14 @@
     {
         "ChannelArn": str,
         "ChannelFlowArn": str,
         "ChimeBearer": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -714,30 +644,22 @@
 GetMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
-StreamingConfigurationOutputTypeDef = TypedDict(
-    "StreamingConfigurationOutputTypeDef",
+StreamingConfigurationTypeDef = TypedDict(
+    "StreamingConfigurationTypeDef",
     {
         "DataType": MessagingDataTypeType,
         "ResourceArn": str,
     },
 )
 
-LambdaConfigurationOutputTypeDef = TypedDict(
-    "LambdaConfigurationOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "InvocationType": Literal["ASYNC"],
-    },
-)
-
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "ResourceArn": str,
         "InvocationType": Literal["ASYNC"],
     },
 )
@@ -995,30 +917,14 @@
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
-StreamingConfigurationTypeDef = TypedDict(
-    "StreamingConfigurationTypeDef",
-    {
-        "DataType": MessagingDataTypeType,
-        "ResourceArn": str,
-    },
-)
-
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -1035,68 +941,31 @@
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
-        "SubChannelId": str,
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
 SearchFieldTypeDef = TypedDict(
     "SearchFieldTypeDef",
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
 )
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
-    {
-        "MemberArn": str,
-    },
-    total=False,
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateChannelFlowResponseTypeDef = TypedDict(
-    "UpdateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Content": str,
         "ChimeBearer": str,
@@ -1124,22 +993,14 @@
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
 
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
         "ChimeBearer": str,
     },
 )
@@ -1156,22 +1017,14 @@
 
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
 BatchChannelMembershipsTypeDef = TypedDict(
     "BatchChannelMembershipsTypeDef",
     {
         "InvitedBy": IdentityTypeDef,
         "Type": ChannelMembershipTypeType,
         "Members": List[IdentityTypeDef],
         "ChannelArn": str,
@@ -1236,48 +1089,114 @@
         "ChannelArn": str,
         "CreatedTimestamp": datetime,
         "CreatedBy": IdentityTypeDef,
     },
     total=False,
 )
 
+ChannelFlowCallbackResponseTypeDef = TypedDict(
+    "ChannelFlowCallbackResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "CallbackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChannelFlowResponseTypeDef = TypedDict(
+    "CreateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "SubChannelId": str,
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
+    },
+)
+
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
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
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "SubChannelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelFlowResponseTypeDef = TypedDict(
+    "UpdateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
+    {
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
 
 ListChannelsAssociatedWithChannelFlowResponseTypeDef = TypedDict(
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     {
         "Channels": List[ChannelAssociatedWithFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -1295,33 +1214,25 @@
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
 
 SearchChannelsResponseTypeDef = TypedDict(
     "SearchChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ChannelMembershipPreferencesOutputTypeDef = TypedDict(
-    "ChannelMembershipPreferencesOutputTypeDef",
-    {
-        "PushNotifications": PushNotificationPreferencesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
     },
@@ -1354,37 +1265,37 @@
     pass
 
 
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
         "Status": ChannelMessageStatusStructureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendChannelMessageResponseTypeDef = TypedDict(
     "SendChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelMessageResponseTypeDef = TypedDict(
     "UpdateChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
@@ -1395,15 +1306,15 @@
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "ContentType": str,
-        "Target": List[TargetOutputTypeDef],
+        "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1418,52 +1329,99 @@
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "SubChannelId": str,
         "ContentType": str,
-        "Target": List[TargetOutputTypeDef],
+        "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "CreatedBy": IdentityTypeDef,
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ChannelFlowArn": str,
-        "ElasticChannelConfiguration": ElasticChannelConfigurationOutputTypeDef,
-        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
+        "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
-PutChannelExpirationSettingsResponseTypeDef = TypedDict(
-    "PutChannelExpirationSettingsResponseTypeDef",
+_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
+    {
+        "ChimeBearer": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+    },
+    total=False,
+)
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+
+class PutChannelExpirationSettingsRequestRequestTypeDef(
+    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
+    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
+):
+    pass
+
+
+PutChannelExpirationSettingsResponseTypeDef = TypedDict(
+    "PutChannelExpirationSettingsResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ChannelArn": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1491,65 +1449,59 @@
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ChannelArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ChimeBearer": str,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-
-class PutChannelExpirationSettingsRequestRequestTypeDef(
-    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
-    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
-):
-    pass
-
-
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsResponseTypeDef",
+PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
     },
 )
 
-ProcessorConfigurationOutputTypeDef = TypedDict(
-    "ProcessorConfigurationOutputTypeDef",
+PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "Lambda": LambdaConfigurationOutputTypeDef,
+        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
@@ -1558,31 +1510,15 @@
 
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
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
-    },
-)
-
-PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
-    {
-        "AppInstanceArn": str,
-        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
@@ -1601,170 +1537,138 @@
 
 class SearchChannelsRequestRequestTypeDef(
     _RequiredSearchChannelsRequestRequestTypeDef, _OptionalSearchChannelsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
-
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
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Preferences": ChannelMembershipPreferencesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesResponseTypeDef",
+PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "Member": IdentityTypeDef,
-        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MemberArn": str,
+        "ChimeBearer": str,
+        "Preferences": ChannelMembershipPreferencesTypeDef,
     },
 )
 
-PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesRequestRequestTypeDef",
+PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
-        "MemberArn": str,
-        "ChimeBearer": str,
+        "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1791,41 +1695,31 @@
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
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
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProcessorOutputTypeDef = TypedDict(
-    "ProcessorOutputTypeDef",
-    {
-        "Name": str,
-        "Configuration": ProcessorConfigurationOutputTypeDef,
-        "ExecutionOrder": int,
-        "FallbackAction": FallbackActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
@@ -1836,24 +1730,24 @@
 )
 
 ChannelFlowSummaryTypeDef = TypedDict(
     "ChannelFlowSummaryTypeDef",
     {
         "ChannelFlowArn": str,
         "Name": str,
-        "Processors": List[ProcessorOutputTypeDef],
+        "Processors": List[ProcessorTypeDef],
     },
     total=False,
 )
 
 ChannelFlowTypeDef = TypedDict(
     "ChannelFlowTypeDef",
     {
         "ChannelFlowArn": str,
-        "Processors": List[ProcessorOutputTypeDef],
+        "Processors": List[ProcessorTypeDef],
         "Name": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
@@ -1891,18 +1785,18 @@
 )
 
 ListChannelFlowsResponseTypeDef = TypedDict(
     "ListChannelFlowsResponseTypeDef",
     {
         "ChannelFlows": List[ChannelFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelFlowResponseTypeDef = TypedDict(
     "DescribeChannelFlowResponseTypeDef",
     {
         "ChannelFlow": ChannelFlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging/type_defs.pyi` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -43,34 +43,29 @@
 
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
-    "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
-    "PushNotificationPreferencesOutputTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
     "MessageAttributeValueOutputTypeDef",
-    "TargetOutputTypeDef",
-    "ElasticChannelConfigurationOutputTypeDef",
-    "ExpirationSettingsOutputTypeDef",
+    "TargetTypeDef",
+    "ElasticChannelConfigurationTypeDef",
+    "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "ElasticChannelConfigurationTypeDef",
-    "ExpirationSettingsTypeDef",
-    "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
@@ -78,106 +73,101 @@
     "DescribeChannelFlowRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelMembershipRequestRequestTypeDef",
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociateChannelFlowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
-    "StreamingConfigurationOutputTypeDef",
-    "LambdaConfigurationOutputTypeDef",
+    "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "StreamingConfigurationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
-    "TargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
+    "ChannelFlowCallbackResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
+    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "UpdateChannelFlowResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
-    "ChannelMembershipPreferencesOutputTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
+    "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateChannelRequestRequestTypeDef",
-    "PutChannelExpirationSettingsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
-    "ProcessorConfigurationOutputTypeDef",
     "ProcessorConfigurationTypeDef",
     "ListSubChannelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "SearchChannelsRequestRequestTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
     "ListChannelModeratorsResponseTypeDef",
     "DescribeChannelModeratorResponseTypeDef",
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
-    "PutChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
+    "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
-    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
     "UpdateChannelFlowRequestRequestTypeDef",
     "ListChannelFlowsResponseTypeDef",
     "DescribeChannelFlowResponseTypeDef",
@@ -240,68 +230,50 @@
 
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
 ):
     pass
 
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
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
     },
     total=False,
 )
 
-ChannelFlowCallbackResponseTypeDef = TypedDict(
-    "ChannelFlowCallbackResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "CallbackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "LastMessageTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredPushNotificationPreferencesOutputTypeDef = TypedDict(
-    "_RequiredPushNotificationPreferencesOutputTypeDef",
-    {
-        "AllowNotifications": AllowNotificationsType,
-    },
-)
-_OptionalPushNotificationPreferencesOutputTypeDef = TypedDict(
-    "_OptionalPushNotificationPreferencesOutputTypeDef",
-    {
-        "FilterRule": str,
-    },
-    total=False,
-)
-
-class PushNotificationPreferencesOutputTypeDef(
-    _RequiredPushNotificationPreferencesOutputTypeDef,
-    _OptionalPushNotificationPreferencesOutputTypeDef,
-):
-    pass
-
 _RequiredPushNotificationPreferencesTypeDef = TypedDict(
     "_RequiredPushNotificationPreferencesTypeDef",
     {
         "AllowNotifications": AllowNotificationsType,
     },
 )
 _OptionalPushNotificationPreferencesTypeDef = TypedDict(
@@ -348,33 +320,33 @@
     "MessageAttributeValueOutputTypeDef",
     {
         "StringValues": List[str],
     },
     total=False,
 )
 
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
 
-ElasticChannelConfigurationOutputTypeDef = TypedDict(
-    "ElasticChannelConfigurationOutputTypeDef",
+ElasticChannelConfigurationTypeDef = TypedDict(
+    "ElasticChannelConfigurationTypeDef",
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
 )
 
-ExpirationSettingsOutputTypeDef = TypedDict(
-    "ExpirationSettingsOutputTypeDef",
+ExpirationSettingsTypeDef = TypedDict(
+    "ExpirationSettingsTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": ExpirationCriterionType,
     },
 )
 
 CreateChannelBanRequestRequestTypeDef = TypedDict(
@@ -390,22 +362,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChannelFlowResponseTypeDef = TypedDict(
-    "CreateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateChannelMembershipRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelMembershipRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "Type": ChannelMembershipTypeType,
         "ChimeBearer": str,
@@ -430,39 +394,14 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
-ElasticChannelConfigurationTypeDef = TypedDict(
-    "ElasticChannelConfigurationTypeDef",
-    {
-        "MaximumSubChannels": int,
-        "TargetMembershipsPerSubChannel": int,
-        "MinimumMembershipPercentage": int,
-    },
-)
-
-ExpirationSettingsTypeDef = TypedDict(
-    "ExpirationSettingsTypeDef",
-    {
-        "ExpirationDays": int,
-        "ExpirationCriterion": ExpirationCriterionType,
-    },
-)
-
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChannelBanRequestRequestTypeDef = TypedDict(
     "DeleteChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -621,21 +560,14 @@
     {
         "ChannelArn": str,
         "ChannelFlowArn": str,
         "ChimeBearer": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -695,30 +627,22 @@
 GetMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
-StreamingConfigurationOutputTypeDef = TypedDict(
-    "StreamingConfigurationOutputTypeDef",
+StreamingConfigurationTypeDef = TypedDict(
+    "StreamingConfigurationTypeDef",
     {
         "DataType": MessagingDataTypeType,
         "ResourceArn": str,
     },
 )
 
-LambdaConfigurationOutputTypeDef = TypedDict(
-    "LambdaConfigurationOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "InvocationType": Literal["ASYNC"],
-    },
-)
-
 LambdaConfigurationTypeDef = TypedDict(
     "LambdaConfigurationTypeDef",
     {
         "ResourceArn": str,
         "InvocationType": Literal["ASYNC"],
     },
 )
@@ -956,30 +880,14 @@
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
-StreamingConfigurationTypeDef = TypedDict(
-    "StreamingConfigurationTypeDef",
-    {
-        "DataType": MessagingDataTypeType,
-        "ResourceArn": str,
-    },
-)
-
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "ChimeBearer": str,
     },
@@ -994,68 +902,31 @@
 
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
-        "SubChannelId": str,
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
 SearchFieldTypeDef = TypedDict(
     "SearchFieldTypeDef",
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
 )
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
-    {
-        "MemberArn": str,
-    },
-    total=False,
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateChannelFlowResponseTypeDef = TypedDict(
-    "UpdateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Content": str,
         "ChimeBearer": str,
@@ -1081,22 +952,14 @@
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
 
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
         "ChimeBearer": str,
     },
 )
@@ -1111,22 +974,14 @@
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
 BatchChannelMembershipsTypeDef = TypedDict(
     "BatchChannelMembershipsTypeDef",
     {
         "InvitedBy": IdentityTypeDef,
         "Type": ChannelMembershipTypeType,
         "Members": List[IdentityTypeDef],
         "ChannelArn": str,
@@ -1191,48 +1046,114 @@
         "ChannelArn": str,
         "CreatedTimestamp": datetime,
         "CreatedBy": IdentityTypeDef,
     },
     total=False,
 )
 
+ChannelFlowCallbackResponseTypeDef = TypedDict(
+    "ChannelFlowCallbackResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "CallbackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChannelFlowResponseTypeDef = TypedDict(
+    "CreateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "SubChannelId": str,
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
+    },
+)
+
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
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
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "SubChannelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelFlowResponseTypeDef = TypedDict(
+    "UpdateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
+    {
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
 
 ListChannelsAssociatedWithChannelFlowResponseTypeDef = TypedDict(
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     {
         "Channels": List[ChannelAssociatedWithFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -1250,33 +1171,25 @@
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
 
 SearchChannelsResponseTypeDef = TypedDict(
     "SearchChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ChannelMembershipPreferencesOutputTypeDef = TypedDict(
-    "ChannelMembershipPreferencesOutputTypeDef",
-    {
-        "PushNotifications": PushNotificationPreferencesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
     },
@@ -1307,37 +1220,37 @@
 ):
     pass
 
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
         "Status": ChannelMessageStatusStructureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendChannelMessageResponseTypeDef = TypedDict(
     "SendChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelMessageResponseTypeDef = TypedDict(
     "UpdateChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
@@ -1348,15 +1261,15 @@
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "ContentType": str,
-        "Target": List[TargetOutputTypeDef],
+        "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1371,52 +1284,95 @@
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "SubChannelId": str,
         "ContentType": str,
-        "Target": List[TargetOutputTypeDef],
+        "Target": List[TargetTypeDef],
+    },
+    total=False,
+)
+
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
     },
     total=False,
 )
 
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "CreatedBy": IdentityTypeDef,
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ChannelFlowArn": str,
-        "ElasticChannelConfiguration": ElasticChannelConfigurationOutputTypeDef,
-        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
+        "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
-PutChannelExpirationSettingsResponseTypeDef = TypedDict(
-    "PutChannelExpirationSettingsResponseTypeDef",
+_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "ExpirationSettings": ExpirationSettingsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
+    {
+        "ChimeBearer": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+    },
+    total=False,
+)
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+class PutChannelExpirationSettingsRequestRequestTypeDef(
+    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
+    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
+):
+    pass
+
+PutChannelExpirationSettingsResponseTypeDef = TypedDict(
+    "PutChannelExpirationSettingsResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ChannelArn": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1442,63 +1398,59 @@
 )
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ChannelArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ChimeBearer": str,
-        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-class PutChannelExpirationSettingsRequestRequestTypeDef(
-    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
-    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
-):
-    pass
-
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsResponseTypeDef",
+PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
-        "StreamingConfigurations": List[StreamingConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
     },
 )
 
-ProcessorConfigurationOutputTypeDef = TypedDict(
-    "ProcessorConfigurationOutputTypeDef",
+PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
-        "Lambda": LambdaConfigurationOutputTypeDef,
+        "StreamingConfigurations": List[StreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
@@ -1507,31 +1459,15 @@
 
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
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
-    },
-)
-
-PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
-    {
-        "AppInstanceArn": str,
-        "StreamingConfigurations": Sequence[StreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
@@ -1548,168 +1484,138 @@
 )
 
 class SearchChannelsRequestRequestTypeDef(
     _RequiredSearchChannelsRequestRequestTypeDef, _OptionalSearchChannelsRequestRequestTypeDef
 ):
     pass
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
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
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Preferences": ChannelMembershipPreferencesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesResponseTypeDef",
+PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "Member": IdentityTypeDef,
-        "Preferences": ChannelMembershipPreferencesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MemberArn": str,
+        "ChimeBearer": str,
+        "Preferences": ChannelMembershipPreferencesTypeDef,
     },
 )
 
-PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
-    "PutChannelMembershipPreferencesRequestRequestTypeDef",
+PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
+    "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
-        "MemberArn": str,
-        "ChimeBearer": str,
+        "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1734,41 +1640,31 @@
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
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
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProcessorOutputTypeDef = TypedDict(
-    "ProcessorOutputTypeDef",
-    {
-        "Name": str,
-        "Configuration": ProcessorConfigurationOutputTypeDef,
-        "ExecutionOrder": int,
-        "FallbackAction": FallbackActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
@@ -1779,24 +1675,24 @@
 )
 
 ChannelFlowSummaryTypeDef = TypedDict(
     "ChannelFlowSummaryTypeDef",
     {
         "ChannelFlowArn": str,
         "Name": str,
-        "Processors": List[ProcessorOutputTypeDef],
+        "Processors": List[ProcessorTypeDef],
     },
     total=False,
 )
 
 ChannelFlowTypeDef = TypedDict(
     "ChannelFlowTypeDef",
     {
         "ChannelFlowArn": str,
-        "Processors": List[ProcessorOutputTypeDef],
+        "Processors": List[ProcessorTypeDef],
         "Name": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
@@ -1832,18 +1728,18 @@
 )
 
 ListChannelFlowsResponseTypeDef = TypedDict(
     "ListChannelFlowsResponseTypeDef",
     {
         "ChannelFlows": List[ChannelFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelFlowResponseTypeDef = TypedDict(
     "DescribeChannelFlowResponseTypeDef",
     {
         "ChannelFlow": ChannelFlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-messaging)](https://pepy.tech/project/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,34 +318,29 @@
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
-    PushNotificationPreferencesOutputTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
     MessageAttributeValueOutputTypeDef,
-    TargetOutputTypeDef,
-    ElasticChannelConfigurationOutputTypeDef,
-    ExpirationSettingsOutputTypeDef,
+    TargetTypeDef,
+    ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    ElasticChannelConfigurationTypeDef,
-    ExpirationSettingsTypeDef,
-    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -353,106 +348,101 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
-    StreamingConfigurationOutputTypeDef,
-    LambdaConfigurationOutputTypeDef,
+    StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
     ListChannelMessagesRequestRequestTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    StreamingConfigurationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
-    TargetTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    UpdateChannelFlowResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
-    ChannelMembershipPreferencesOutputTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateChannelRequestRequestTypeDef,
-    PutChannelExpirationSettingsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
+    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
-    ProcessorConfigurationOutputTypeDef,
     ProcessorConfigurationTypeDef,
     ListSubChannelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     SearchChannelsRequestRequestTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
-    PutChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
+    PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
-    ProcessorOutputTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-messaging-1.28.15/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.28.12/setup.py` & `mypy-boto3-chime-sdk-messaging-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-messaging",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMessaging 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ChimeSDKMessaging 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

