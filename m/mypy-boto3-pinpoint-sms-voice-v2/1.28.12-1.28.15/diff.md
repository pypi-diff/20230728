# Comparing `tmp/mypy-boto3-pinpoint-sms-voice-v2-1.28.12.tar.gz` & `tmp/mypy-boto3-pinpoint-sms-voice-v2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-sms-voice-v2-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-sms-voice-v2-1.28.15.tar", last modified: Fri Jul 28 20:43:28 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12.tar` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39760 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39699 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-27 11:41:38.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-27 11:41:38.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:37.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47600 2023-07-27 11:41:39.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-07-27 11:41:38.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.893162 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-27 11:41:36.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:28.189651 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20883 2023-07-28 20:43:28.185651 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:28.177651 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39760 2023-07-28 20:33:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39699 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-28 20:33:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-28 20:33:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-28 20:33:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-28 20:33:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46825 2023-07-28 20:33:30.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46778 2023-07-28 20:33:30.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:28.185651 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20883 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:28.189651 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-28 20:33:28.000000 mypy-boto3-pinpoint-sms-voice-v2-1.28.15/setup.py
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/LICENSE` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/PKG-INFO` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.28.12
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,19 +395,17 @@
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
@@ -429,16 +427,14 @@
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutKeywordRequestRequestTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     SendTextMessageRequestRequestTypeDef,
@@ -471,24 +467,25 @@
     SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UpdatePhoneNumberResultTypeDef,
     UpdatePoolResultTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateOptOutListRequestRequestTypeDef,
-    CreatePoolRequestRequestTypeDef,
-    RequestPhoneNumberRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateConfigurationSetResultTypeDef,
+    CreateOptOutListRequestRequestTypeDef,
     CreateOptOutListResultTypeDef,
+    CreatePoolRequestRequestTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
+    RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
+    EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
     DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
     DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
     DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
@@ -504,15 +501,14 @@
     DescribePoolsRequestDescribePoolsPaginateTypeDef,
     DescribePoolsRequestRequestTypeDef,
     DescribePoolsResultTypeDef,
     DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef,
     DescribeSenderIdsRequestRequestTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
-    EventDestinationTypeDef,
     ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
     ListPoolOriginationIdentitiesRequestRequestTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ConfigurationSetInformationTypeDef,
     CreateEventDestinationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteEventDestinationResultTypeDef,
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/README.md` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,19 +363,17 @@
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
@@ -397,16 +395,14 @@
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutKeywordRequestRequestTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     SendTextMessageRequestRequestTypeDef,
@@ -439,24 +435,25 @@
     SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UpdatePhoneNumberResultTypeDef,
     UpdatePoolResultTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateOptOutListRequestRequestTypeDef,
-    CreatePoolRequestRequestTypeDef,
-    RequestPhoneNumberRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateConfigurationSetResultTypeDef,
+    CreateOptOutListRequestRequestTypeDef,
     CreateOptOutListResultTypeDef,
+    CreatePoolRequestRequestTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
+    RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
+    EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
     DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
     DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
     DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
@@ -472,15 +469,14 @@
     DescribePoolsRequestDescribePoolsPaginateTypeDef,
     DescribePoolsRequestRequestTypeDef,
     DescribePoolsResultTypeDef,
     DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef,
     DescribeSenderIdsRequestRequestTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
-    EventDestinationTypeDef,
     ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
     ListPoolOriginationIdentitiesRequestRequestTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ConfigurationSetInformationTypeDef,
     CreateEventDestinationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteEventDestinationResultTypeDef,
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/__main__.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2\nOther"
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/client.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,17 @@
 
 
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "CloudWatchLogsDestinationOutputTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
-    "TagOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
@@ -81,16 +79,14 @@
     "PoolInformationTypeDef",
     "SenderIdAndCountryTypeDef",
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "SnsDestinationOutputTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutKeywordRequestRequestTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "SendTextMessageRequestRequestTypeDef",
@@ -123,24 +119,25 @@
     "SetDefaultSenderIdResultTypeDef",
     "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolResultTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "CreateOptOutListRequestRequestTypeDef",
-    "CreatePoolRequestRequestTypeDef",
-    "RequestPhoneNumberRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetResultTypeDef",
+    "CreateOptOutListRequestRequestTypeDef",
     "CreateOptOutListResultTypeDef",
+    "CreatePoolRequestRequestTypeDef",
     "CreatePoolResultTypeDef",
     "ListTagsForResourceResultTypeDef",
+    "RequestPhoneNumberRequestRequestTypeDef",
     "RequestPhoneNumberResultTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateEventDestinationRequestRequestTypeDef",
+    "EventDestinationTypeDef",
     "UpdateEventDestinationRequestRequestTypeDef",
     "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
     "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
     "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
     "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
     "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
@@ -156,15 +153,14 @@
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     "DescribePoolsRequestRequestTypeDef",
     "DescribePoolsResultTypeDef",
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     "DescribeSenderIdsRequestRequestTypeDef",
     "DescribeSenderIdsResultTypeDef",
     "DescribeSpendLimitsResultTypeDef",
-    "EventDestinationTypeDef",
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     "ListPoolOriginationIdentitiesRequestRequestTypeDef",
     "ListPoolOriginationIdentitiesResultTypeDef",
     "ConfigurationSetInformationTypeDef",
     "CreateEventDestinationResultTypeDef",
     "DeleteConfigurationSetResultTypeDef",
     "DeleteEventDestinationResultTypeDef",
@@ -220,22 +216,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-CloudWatchLogsDestinationOutputTypeDef = TypedDict(
-    "CloudWatchLogsDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "LogGroupArn": str,
-    },
-)
-
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
         "LogGroupArn": str,
     },
 )
@@ -252,22 +240,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IamRoleArn": str,
         "DeliveryStreamArn": str,
     },
 )
@@ -564,29 +544,14 @@
 class DisassociateOriginationIdentityRequestRequestTypeDef(
     _RequiredDisassociateOriginationIdentityRequestRequestTypeDef,
     _OptionalDisassociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "DeliveryStreamArn": str,
-    },
-)
-
-SnsDestinationOutputTypeDef = TypedDict(
-    "SnsDestinationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -1090,14 +1055,25 @@
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
 
+CreateConfigurationSetResultTypeDef = TypedDict(
+    "CreateConfigurationSetResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "Tags": List[TagTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateOptOutListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalCreateOptOutListRequestRequestTypeDef = TypedDict(
@@ -1112,14 +1088,25 @@
 
 class CreateOptOutListRequestRequestTypeDef(
     _RequiredCreateOptOutListRequestRequestTypeDef, _OptionalCreateOptOutListRequestRequestTypeDef
 ):
     pass
 
 
+CreateOptOutListResultTypeDef = TypedDict(
+    "CreateOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "Tags": List[TagTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePoolRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
     },
@@ -1137,14 +1124,42 @@
 
 class CreatePoolRequestRequestTypeDef(
     _RequiredCreatePoolRequestRequestTypeDef, _OptionalCreatePoolRequestRequestTypeDef
 ):
     pass
 
 
+CreatePoolResultTypeDef = TypedDict(
+    "CreatePoolResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
+        "Tags": List[TagTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRequestPhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredRequestPhoneNumberRequestRequestTypeDef",
     {
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
         "NumberCapabilities": Sequence[NumberCapabilityType],
         "NumberType": RequestableNumberTypeType,
@@ -1167,72 +1182,14 @@
 class RequestPhoneNumberRequestRequestTypeDef(
     _RequiredRequestPhoneNumberRequestRequestTypeDef,
     _OptionalRequestPhoneNumberRequestRequestTypeDef,
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
-CreateConfigurationSetResultTypeDef = TypedDict(
-    "CreateConfigurationSetResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "Tags": List[TagOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateOptOutListResultTypeDef = TypedDict(
-    "CreateOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "Tags": List[TagOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePoolResultTypeDef = TypedDict(
-    "CreatePoolResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
-        "Tags": List[TagOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RequestPhoneNumberResultTypeDef = TypedDict(
     "RequestPhoneNumberResultTypeDef",
     {
         "PhoneNumberArn": str,
         "PhoneNumberId": str,
         "PhoneNumber": str,
         "Status": NumberStatusType,
@@ -1243,20 +1200,28 @@
         "MonthlyLeasingPrice": str,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "DeletionProtectionEnabled": bool,
         "PoolId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 _RequiredCreateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
@@ -1276,14 +1241,37 @@
 class CreateEventDestinationRequestRequestTypeDef(
     _RequiredCreateEventDestinationRequestRequestTypeDef,
     _OptionalCreateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredEventDestinationTypeDef = TypedDict(
+    "_RequiredEventDestinationTypeDef",
+    {
+        "EventDestinationName": str,
+        "Enabled": bool,
+        "MatchingEventTypes": List[EventTypeType],
+    },
+)
+_OptionalEventDestinationTypeDef = TypedDict(
+    "_OptionalEventDestinationTypeDef",
+    {
+        "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+    },
+    total=False,
+)
+
+
+class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
+    pass
+
+
 _RequiredUpdateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -1573,37 +1561,14 @@
     {
         "SpendLimits": List[SpendLimitTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventDestinationTypeDef = TypedDict(
-    "_RequiredEventDestinationTypeDef",
-    {
-        "EventDestinationName": str,
-        "Enabled": bool,
-        "MatchingEventTypes": List[EventTypeType],
-    },
-)
-_OptionalEventDestinationTypeDef = TypedDict(
-    "_OptionalEventDestinationTypeDef",
-    {
-        "CloudWatchLogsDestination": CloudWatchLogsDestinationOutputTypeDef,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
-        "SnsDestination": SnsDestinationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
-    pass
-
-
 _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "PoolId": str,
         },
     )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,17 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "CloudWatchLogsDestinationOutputTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
-    "TagOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
@@ -80,16 +78,14 @@
     "PoolInformationTypeDef",
     "SenderIdAndCountryTypeDef",
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "SnsDestinationOutputTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutKeywordRequestRequestTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "SendTextMessageRequestRequestTypeDef",
@@ -122,24 +118,25 @@
     "SetDefaultSenderIdResultTypeDef",
     "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolResultTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "CreateOptOutListRequestRequestTypeDef",
-    "CreatePoolRequestRequestTypeDef",
-    "RequestPhoneNumberRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetResultTypeDef",
+    "CreateOptOutListRequestRequestTypeDef",
     "CreateOptOutListResultTypeDef",
+    "CreatePoolRequestRequestTypeDef",
     "CreatePoolResultTypeDef",
     "ListTagsForResourceResultTypeDef",
+    "RequestPhoneNumberRequestRequestTypeDef",
     "RequestPhoneNumberResultTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateEventDestinationRequestRequestTypeDef",
+    "EventDestinationTypeDef",
     "UpdateEventDestinationRequestRequestTypeDef",
     "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
     "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
     "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
     "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
     "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
@@ -155,15 +152,14 @@
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     "DescribePoolsRequestRequestTypeDef",
     "DescribePoolsResultTypeDef",
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     "DescribeSenderIdsRequestRequestTypeDef",
     "DescribeSenderIdsResultTypeDef",
     "DescribeSpendLimitsResultTypeDef",
-    "EventDestinationTypeDef",
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     "ListPoolOriginationIdentitiesRequestRequestTypeDef",
     "ListPoolOriginationIdentitiesResultTypeDef",
     "ConfigurationSetInformationTypeDef",
     "CreateEventDestinationResultTypeDef",
     "DeleteConfigurationSetResultTypeDef",
     "DeleteEventDestinationResultTypeDef",
@@ -217,22 +213,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-CloudWatchLogsDestinationOutputTypeDef = TypedDict(
-    "CloudWatchLogsDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "LogGroupArn": str,
-    },
-)
-
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
         "LogGroupArn": str,
     },
 )
@@ -249,22 +237,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IamRoleArn": str,
         "DeliveryStreamArn": str,
     },
 )
@@ -555,29 +535,14 @@
 
 class DisassociateOriginationIdentityRequestRequestTypeDef(
     _RequiredDisassociateOriginationIdentityRequestRequestTypeDef,
     _OptionalDisassociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "DeliveryStreamArn": str,
-    },
-)
-
-SnsDestinationOutputTypeDef = TypedDict(
-    "SnsDestinationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -1069,14 +1034,25 @@
 
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+CreateConfigurationSetResultTypeDef = TypedDict(
+    "CreateConfigurationSetResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "Tags": List[TagTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateOptOutListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalCreateOptOutListRequestRequestTypeDef = TypedDict(
@@ -1089,14 +1065,25 @@
 )
 
 class CreateOptOutListRequestRequestTypeDef(
     _RequiredCreateOptOutListRequestRequestTypeDef, _OptionalCreateOptOutListRequestRequestTypeDef
 ):
     pass
 
+CreateOptOutListResultTypeDef = TypedDict(
+    "CreateOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "Tags": List[TagTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePoolRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
     },
@@ -1112,14 +1099,42 @@
 )
 
 class CreatePoolRequestRequestTypeDef(
     _RequiredCreatePoolRequestRequestTypeDef, _OptionalCreatePoolRequestRequestTypeDef
 ):
     pass
 
+CreatePoolResultTypeDef = TypedDict(
+    "CreatePoolResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
+        "Tags": List[TagTypeDef],
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRequestPhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredRequestPhoneNumberRequestRequestTypeDef",
     {
         "IsoCountryCode": str,
         "MessageType": MessageTypeType,
         "NumberCapabilities": Sequence[NumberCapabilityType],
         "NumberType": RequestableNumberTypeType,
@@ -1140,72 +1155,14 @@
 
 class RequestPhoneNumberRequestRequestTypeDef(
     _RequiredRequestPhoneNumberRequestRequestTypeDef,
     _OptionalRequestPhoneNumberRequestRequestTypeDef,
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
-CreateConfigurationSetResultTypeDef = TypedDict(
-    "CreateConfigurationSetResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "Tags": List[TagOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateOptOutListResultTypeDef = TypedDict(
-    "CreateOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "Tags": List[TagOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePoolResultTypeDef = TypedDict(
-    "CreatePoolResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
-        "Tags": List[TagOutputTypeDef],
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RequestPhoneNumberResultTypeDef = TypedDict(
     "RequestPhoneNumberResultTypeDef",
     {
         "PhoneNumberArn": str,
         "PhoneNumberId": str,
         "PhoneNumber": str,
         "Status": NumberStatusType,
@@ -1216,20 +1173,28 @@
         "MonthlyLeasingPrice": str,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "DeletionProtectionEnabled": bool,
         "PoolId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 _RequiredCreateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
@@ -1247,14 +1212,35 @@
 
 class CreateEventDestinationRequestRequestTypeDef(
     _RequiredCreateEventDestinationRequestRequestTypeDef,
     _OptionalCreateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredEventDestinationTypeDef = TypedDict(
+    "_RequiredEventDestinationTypeDef",
+    {
+        "EventDestinationName": str,
+        "Enabled": bool,
+        "MatchingEventTypes": List[EventTypeType],
+    },
+)
+_OptionalEventDestinationTypeDef = TypedDict(
+    "_OptionalEventDestinationTypeDef",
+    {
+        "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+    },
+    total=False,
+)
+
+class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
+    pass
+
 _RequiredUpdateEventDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -1534,35 +1520,14 @@
     {
         "SpendLimits": List[SpendLimitTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventDestinationTypeDef = TypedDict(
-    "_RequiredEventDestinationTypeDef",
-    {
-        "EventDestinationName": str,
-        "Enabled": bool,
-        "MatchingEventTypes": List[EventTypeType],
-    },
-)
-_OptionalEventDestinationTypeDef = TypedDict(
-    "_OptionalEventDestinationTypeDef",
-    {
-        "CloudWatchLogsDestination": CloudWatchLogsDestinationOutputTypeDef,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
-        "SnsDestination": SnsDestinationOutputTypeDef,
-    },
-    total=False,
-)
-
-class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
-    pass
-
 _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "PoolId": str,
         },
     )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.28.12
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,19 +395,17 @@
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    CloudWatchLogsDestinationOutputTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
-    TagOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
@@ -429,16 +427,14 @@
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutKeywordRequestRequestTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
     SendTextMessageRequestRequestTypeDef,
@@ -471,24 +467,25 @@
     SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UpdatePhoneNumberResultTypeDef,
     UpdatePoolResultTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    CreateOptOutListRequestRequestTypeDef,
-    CreatePoolRequestRequestTypeDef,
-    RequestPhoneNumberRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateConfigurationSetResultTypeDef,
+    CreateOptOutListRequestRequestTypeDef,
     CreateOptOutListResultTypeDef,
+    CreatePoolRequestRequestTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
+    RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
+    EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
     DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
     DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
     DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
@@ -504,15 +501,14 @@
     DescribePoolsRequestDescribePoolsPaginateTypeDef,
     DescribePoolsRequestRequestTypeDef,
     DescribePoolsResultTypeDef,
     DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef,
     DescribeSenderIdsRequestRequestTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
-    EventDestinationTypeDef,
     ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
     ListPoolOriginationIdentitiesRequestRequestTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ConfigurationSetInformationTypeDef,
     CreateEventDestinationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteEventDestinationResultTypeDef,
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.28.12/setup.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-sms-voice-v2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_pinpoint_sms_voice_v2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.PinpointSMSVoiceV2 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

