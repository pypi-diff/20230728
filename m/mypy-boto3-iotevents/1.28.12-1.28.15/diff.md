# Comparing `tmp/mypy-boto3-iotevents-1.28.12.tar.gz` & `tmp/mypy-boto3-iotevents-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
+gzip compressed data, was "mypy-boto3-iotevents-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iotevents-1.28.12.tar` & `mypy-boto3-iotevents-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53782 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53679 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.461257 mypy-boto3-iotevents-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-07-28 20:42:59.453257 mypy-boto3-iotevents-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.445257 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-28 20:28:23.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-28 20:28:23.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42731 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42652 2023-07-28 20:28:23.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.453257 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.461257 mypy-boto3-iotevents-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:28:22.000000 mypy-boto3-iotevents-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotevents-1.28.12/LICENSE` & `mypy-boto3-iotevents-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.12/PKG-INFO` & `mypy-boto3-iotevents-1.28.15/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iotevents
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTEvents 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotevents type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotevents"></a>
 
 # mypy-boto3-iotevents
 
 [![PyPI - mypy-boto3-iotevents](https://img.shields.io/pypi/v/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,154 +272,123 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
-    AcknowledgeFlowOutputTypeDef,
     AcknowledgeFlowTypeDef,
-    ClearTimerActionOutputTypeDef,
-    ResetTimerActionOutputTypeDef,
-    SetTimerActionOutputTypeDef,
-    SetVariableActionOutputTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
     SetVariableActionTypeDef,
-    InitializationConfigurationOutputTypeDef,
     InitializationConfigurationTypeDef,
     AlarmModelSummaryTypeDef,
     AlarmModelVersionSummaryTypeDef,
-    SimpleRuleOutputTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
-    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
-    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    CreateAlarmModelResponseTypeDef,
+    ResponseMetadataTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
-    DetectorDebugOptionOutputTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
-    PayloadOutputTypeDef,
     PayloadTypeDef,
-    EmailContentOutputTypeDef,
     EmailContentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    SSOIdentityOutputTypeDef,
     SSOIdentityTypeDef,
-    ResponseMetadataTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlarmModelResponseTypeDef,
-    AlarmCapabilitiesOutputTypeDef,
     AlarmCapabilitiesTypeDef,
-    ListAlarmModelsResponseTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
-    AlarmRuleOutputTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
-    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
     InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAlarmModelResponseTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
     LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
-    DynamoDBActionOutputTypeDef,
-    DynamoDBv2ActionOutputTypeDef,
-    FirehoseActionOutputTypeDef,
-    IotEventsActionOutputTypeDef,
-    IotTopicPublishActionOutputTypeDef,
-    LambdaActionOutputTypeDef,
-    SNSTopicPublishActionOutputTypeDef,
-    SqsActionOutputTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
     IotTopicPublishActionTypeDef,
     LambdaActionTypeDef,
     SNSTopicPublishActionTypeDef,
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RecipientDetailOutputTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     InputTypeDef,
     CreateInputRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    NotificationTargetActionsOutputTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
     EmailRecipientsOutputTypeDef,
-    SMSConfigurationOutputTypeDef,
     EmailRecipientsTypeDef,
+    SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
-    ActionOutputTypeDef,
-    AlarmActionOutputTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
     EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
     EventOutputTypeDef,
-    TransitionEventOutputTypeDef,
-    AlarmEventActionsOutputTypeDef,
     EventTypeDef,
+    TransitionEventOutputTypeDef,
     TransitionEventTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
     NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
     OnEnterLifecycleOutputTypeDef,
     OnExitLifecycleOutputTypeDef,
-    OnInputLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
     AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     StateOutputTypeDef,
     StateTypeDef,
     DescribeAlarmModelResponseTypeDef,
     CreateAlarmModelRequestRequestTypeDef,
@@ -462,15 +399,15 @@
     CreateDetectorModelRequestRequestTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowOutputTypeDef:
+def get_structure() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.12/README.md` & `mypy-boto3-iotevents-1.28.15/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iotevents
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iotevents type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotevents"></a>
 
 # mypy-boto3-iotevents
 
 [![PyPI - mypy-boto3-iotevents](https://img.shields.io/pypi/v/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,154 +304,123 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
-    AcknowledgeFlowOutputTypeDef,
     AcknowledgeFlowTypeDef,
-    ClearTimerActionOutputTypeDef,
-    ResetTimerActionOutputTypeDef,
-    SetTimerActionOutputTypeDef,
-    SetVariableActionOutputTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
     SetVariableActionTypeDef,
-    InitializationConfigurationOutputTypeDef,
     InitializationConfigurationTypeDef,
     AlarmModelSummaryTypeDef,
     AlarmModelVersionSummaryTypeDef,
-    SimpleRuleOutputTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
-    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
-    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    CreateAlarmModelResponseTypeDef,
+    ResponseMetadataTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
-    DetectorDebugOptionOutputTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
-    PayloadOutputTypeDef,
     PayloadTypeDef,
-    EmailContentOutputTypeDef,
     EmailContentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    SSOIdentityOutputTypeDef,
     SSOIdentityTypeDef,
-    ResponseMetadataTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlarmModelResponseTypeDef,
-    AlarmCapabilitiesOutputTypeDef,
     AlarmCapabilitiesTypeDef,
-    ListAlarmModelsResponseTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
-    AlarmRuleOutputTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
-    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
     InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAlarmModelResponseTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
     LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
-    DynamoDBActionOutputTypeDef,
-    DynamoDBv2ActionOutputTypeDef,
-    FirehoseActionOutputTypeDef,
-    IotEventsActionOutputTypeDef,
-    IotTopicPublishActionOutputTypeDef,
-    LambdaActionOutputTypeDef,
-    SNSTopicPublishActionOutputTypeDef,
-    SqsActionOutputTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
     IotTopicPublishActionTypeDef,
     LambdaActionTypeDef,
     SNSTopicPublishActionTypeDef,
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RecipientDetailOutputTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     InputTypeDef,
     CreateInputRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    NotificationTargetActionsOutputTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
     EmailRecipientsOutputTypeDef,
-    SMSConfigurationOutputTypeDef,
     EmailRecipientsTypeDef,
+    SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
-    ActionOutputTypeDef,
-    AlarmActionOutputTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
     EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
     EventOutputTypeDef,
-    TransitionEventOutputTypeDef,
-    AlarmEventActionsOutputTypeDef,
     EventTypeDef,
+    TransitionEventOutputTypeDef,
     TransitionEventTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
     NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
     OnEnterLifecycleOutputTypeDef,
     OnExitLifecycleOutputTypeDef,
-    OnInputLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
     AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     StateOutputTypeDef,
     StateTypeDef,
     DescribeAlarmModelResponseTypeDef,
     CreateAlarmModelRequestRequestTypeDef,
@@ -430,15 +431,15 @@
     CreateDetectorModelRequestRequestTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowOutputTypeDef:
+def get_structure() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__main__.py` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTEvents 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTEvents 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.py` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.pyi` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.py` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.pyi` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/type_defs.py` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotevents service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotevents.type_defs import AcknowledgeFlowOutputTypeDef
+    from mypy_boto3_iotevents.type_defs import AcknowledgeFlowTypeDef
 
-    data: AcknowledgeFlowOutputTypeDef = {...}
+    data: AcknowledgeFlowTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -30,154 +30,123 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AcknowledgeFlowOutputTypeDef",
     "AcknowledgeFlowTypeDef",
-    "ClearTimerActionOutputTypeDef",
-    "ResetTimerActionOutputTypeDef",
-    "SetTimerActionOutputTypeDef",
-    "SetVariableActionOutputTypeDef",
     "ClearTimerActionTypeDef",
     "ResetTimerActionTypeDef",
     "SetTimerActionTypeDef",
     "SetVariableActionTypeDef",
-    "InitializationConfigurationOutputTypeDef",
     "InitializationConfigurationTypeDef",
     "AlarmModelSummaryTypeDef",
     "AlarmModelVersionSummaryTypeDef",
-    "SimpleRuleOutputTypeDef",
     "SimpleRuleTypeDef",
     "AnalysisResultLocationTypeDef",
-    "AssetPropertyTimestampOutputTypeDef",
     "AssetPropertyTimestampTypeDef",
-    "AssetPropertyVariantOutputTypeDef",
     "AssetPropertyVariantTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "TagTypeDef",
-    "CreateAlarmModelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DetectorModelConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "DeleteAlarmModelRequestRequestTypeDef",
     "DeleteDetectorModelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DescribeAlarmModelRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
-    "DescribeDetectorModelAnalysisResponseTypeDef",
     "DescribeDetectorModelRequestRequestTypeDef",
     "DescribeInputRequestRequestTypeDef",
-    "DetectorDebugOptionOutputTypeDef",
     "DetectorDebugOptionTypeDef",
     "DetectorModelSummaryTypeDef",
     "DetectorModelVersionSummaryTypeDef",
-    "PayloadOutputTypeDef",
     "PayloadTypeDef",
-    "EmailContentOutputTypeDef",
     "EmailContentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetDetectorModelAnalysisResultsRequestRequestTypeDef",
     "IotEventsInputIdentifierTypeDef",
     "InputSummaryTypeDef",
     "IotSiteWiseAssetModelPropertyIdentifierTypeDef",
     "ListAlarmModelVersionsRequestRequestTypeDef",
     "ListAlarmModelsRequestRequestTypeDef",
     "ListDetectorModelVersionsRequestRequestTypeDef",
     "ListDetectorModelsRequestRequestTypeDef",
     "RoutedResourceTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "SSOIdentityOutputTypeDef",
     "SSOIdentityTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDetectorModelAnalysisResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlarmModelResponseTypeDef",
-    "AlarmCapabilitiesOutputTypeDef",
     "AlarmCapabilitiesTypeDef",
-    "ListAlarmModelsResponseTypeDef",
-    "ListAlarmModelVersionsResponseTypeDef",
-    "AlarmRuleOutputTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
-    "AssetPropertyValueOutputTypeDef",
     "AssetPropertyValueTypeDef",
     "InputDefinitionOutputTypeDef",
     "InputDefinitionTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateAlarmModelResponseTypeDef",
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAlarmModelVersionsResponseTypeDef",
+    "ListAlarmModelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDetectorModelAnalysisResponseTypeDef",
+    "UpdateAlarmModelResponseTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "LoggingOptionsOutputTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
-    "DynamoDBActionOutputTypeDef",
-    "DynamoDBv2ActionOutputTypeDef",
-    "FirehoseActionOutputTypeDef",
-    "IotEventsActionOutputTypeDef",
-    "IotTopicPublishActionOutputTypeDef",
-    "LambdaActionOutputTypeDef",
-    "SNSTopicPublishActionOutputTypeDef",
-    "SqsActionOutputTypeDef",
     "DynamoDBActionTypeDef",
     "DynamoDBv2ActionTypeDef",
     "FirehoseActionTypeDef",
     "IotEventsActionTypeDef",
     "IotTopicPublishActionTypeDef",
     "LambdaActionTypeDef",
     "SNSTopicPublishActionTypeDef",
     "SqsActionTypeDef",
     "ListInputsResponseTypeDef",
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RecipientDetailOutputTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
-    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "InputTypeDef",
     "CreateInputRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
-    "NotificationTargetActionsOutputTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
     "EmailRecipientsOutputTypeDef",
-    "SMSConfigurationOutputTypeDef",
     "EmailRecipientsTypeDef",
+    "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
-    "ActionOutputTypeDef",
-    "AlarmActionOutputTypeDef",
     "ActionTypeDef",
     "AlarmActionTypeDef",
     "DescribeInputResponseTypeDef",
     "ListInputRoutingsRequestRequestTypeDef",
     "EmailConfigurationOutputTypeDef",
     "EmailConfigurationTypeDef",
     "EventOutputTypeDef",
-    "TransitionEventOutputTypeDef",
-    "AlarmEventActionsOutputTypeDef",
     "EventTypeDef",
+    "TransitionEventOutputTypeDef",
     "TransitionEventTypeDef",
+    "AlarmEventActionsOutputTypeDef",
     "AlarmEventActionsTypeDef",
     "NotificationActionOutputTypeDef",
     "NotificationActionTypeDef",
     "OnEnterLifecycleOutputTypeDef",
     "OnExitLifecycleOutputTypeDef",
-    "OnInputLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
+    "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
     "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
     "StateOutputTypeDef",
     "StateTypeDef",
     "DescribeAlarmModelResponseTypeDef",
     "CreateAlarmModelRequestRequestTypeDef",
@@ -187,72 +156,21 @@
     "DetectorModelTypeDef",
     "CreateDetectorModelRequestRequestTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
-AcknowledgeFlowOutputTypeDef = TypedDict(
-    "AcknowledgeFlowOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
     {
         "enabled": bool,
     },
 )
 
-ClearTimerActionOutputTypeDef = TypedDict(
-    "ClearTimerActionOutputTypeDef",
-    {
-        "timerName": str,
-    },
-)
-
-ResetTimerActionOutputTypeDef = TypedDict(
-    "ResetTimerActionOutputTypeDef",
-    {
-        "timerName": str,
-    },
-)
-
-_RequiredSetTimerActionOutputTypeDef = TypedDict(
-    "_RequiredSetTimerActionOutputTypeDef",
-    {
-        "timerName": str,
-    },
-)
-_OptionalSetTimerActionOutputTypeDef = TypedDict(
-    "_OptionalSetTimerActionOutputTypeDef",
-    {
-        "seconds": int,
-        "durationExpression": str,
-    },
-    total=False,
-)
-
-
-class SetTimerActionOutputTypeDef(
-    _RequiredSetTimerActionOutputTypeDef, _OptionalSetTimerActionOutputTypeDef
-):
-    pass
-
-
-SetVariableActionOutputTypeDef = TypedDict(
-    "SetVariableActionOutputTypeDef",
-    {
-        "variableName": str,
-        "value": str,
-    },
-)
-
 ClearTimerActionTypeDef = TypedDict(
     "ClearTimerActionTypeDef",
     {
         "timerName": str,
     },
 )
 
@@ -287,21 +205,14 @@
     "SetVariableActionTypeDef",
     {
         "variableName": str,
         "value": str,
     },
 )
 
-InitializationConfigurationOutputTypeDef = TypedDict(
-    "InitializationConfigurationOutputTypeDef",
-    {
-        "disabledOnInitialization": bool,
-    },
-)
-
 InitializationConfigurationTypeDef = TypedDict(
     "InitializationConfigurationTypeDef",
     {
         "disabledOnInitialization": bool,
     },
 )
 
@@ -326,23 +237,14 @@
         "lastUpdateTime": datetime,
         "status": AlarmModelVersionStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-SimpleRuleOutputTypeDef = TypedDict(
-    "SimpleRuleOutputTypeDef",
-    {
-        "inputProperty": str,
-        "comparisonOperator": ComparisonOperatorType,
-        "threshold": str,
-    },
-)
-
 SimpleRuleTypeDef = TypedDict(
     "SimpleRuleTypeDef",
     {
         "inputProperty": str,
         "comparisonOperator": ComparisonOperatorType,
         "threshold": str,
     },
@@ -352,35 +254,14 @@
     "AnalysisResultLocationTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
-_RequiredAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyTimestampOutputTypeDef",
-    {
-        "timeInSeconds": str,
-    },
-)
-_OptionalAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyTimestampOutputTypeDef",
-    {
-        "offsetInNanos": str,
-    },
-    total=False,
-)
-
-
-class AssetPropertyTimestampOutputTypeDef(
-    _RequiredAssetPropertyTimestampOutputTypeDef, _OptionalAssetPropertyTimestampOutputTypeDef
-):
-    pass
-
-
 _RequiredAssetPropertyTimestampTypeDef = TypedDict(
     "_RequiredAssetPropertyTimestampTypeDef",
     {
         "timeInSeconds": str,
     },
 )
 _OptionalAssetPropertyTimestampTypeDef = TypedDict(
@@ -394,43 +275,25 @@
 
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
 
-AssetPropertyVariantOutputTypeDef = TypedDict(
-    "AssetPropertyVariantOutputTypeDef",
-    {
-        "stringValue": str,
-        "integerValue": str,
-        "doubleValue": str,
-        "booleanValue": str,
-    },
-    total=False,
-)
-
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
     },
     total=False,
 )
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
-    {
-        "jsonPath": str,
-    },
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "jsonPath": str,
     },
 )
 
@@ -438,23 +301,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreateAlarmModelResponseTypeDef = TypedDict(
-    "CreateAlarmModelResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DetectorModelConfigurationTypeDef = TypedDict(
     "DetectorModelConfigurationTypeDef",
     {
         "detectorModelName": str,
@@ -542,22 +404,14 @@
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
-DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    {
-        "status": AnalysisStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDescribeDetectorModelRequestRequestTypeDef = TypedDict(
@@ -579,35 +433,14 @@
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "inputName": str,
     },
 )
 
-_RequiredDetectorDebugOptionOutputTypeDef = TypedDict(
-    "_RequiredDetectorDebugOptionOutputTypeDef",
-    {
-        "detectorModelName": str,
-    },
-)
-_OptionalDetectorDebugOptionOutputTypeDef = TypedDict(
-    "_OptionalDetectorDebugOptionOutputTypeDef",
-    {
-        "keyValue": str,
-    },
-    total=False,
-)
-
-
-class DetectorDebugOptionOutputTypeDef(
-    _RequiredDetectorDebugOptionOutputTypeDef, _OptionalDetectorDebugOptionOutputTypeDef
-):
-    pass
-
-
 _RequiredDetectorDebugOptionTypeDef = TypedDict(
     "_RequiredDetectorDebugOptionTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDetectorDebugOptionTypeDef = TypedDict(
@@ -646,55 +479,31 @@
         "lastUpdateTime": datetime,
         "status": DetectorModelVersionStatusType,
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
-PayloadOutputTypeDef = TypedDict(
-    "PayloadOutputTypeDef",
-    {
-        "contentExpression": str,
-        "type": PayloadTypeType,
-    },
-)
-
 PayloadTypeDef = TypedDict(
     "PayloadTypeDef",
     {
         "contentExpression": str,
         "type": PayloadTypeType,
     },
 )
 
-EmailContentOutputTypeDef = TypedDict(
-    "EmailContentOutputTypeDef",
-    {
-        "subject": str,
-        "additionalMessage": str,
-    },
-    total=False,
-)
-
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "subject": str,
         "additionalMessage": str,
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
 _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
@@ -827,43 +636,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
-_RequiredSSOIdentityOutputTypeDef = TypedDict(
-    "_RequiredSSOIdentityOutputTypeDef",
-    {
-        "identityStoreId": str,
-    },
-)
-_OptionalSSOIdentityOutputTypeDef = TypedDict(
-    "_OptionalSSOIdentityOutputTypeDef",
-    {
-        "userId": str,
-    },
-    total=False,
-)
-
-
-class SSOIdentityOutputTypeDef(
-    _RequiredSSOIdentityOutputTypeDef, _OptionalSSOIdentityOutputTypeDef
-):
-    pass
-
-
 _RequiredSSOIdentityTypeDef = TypedDict(
     "_RequiredSSOIdentityTypeDef",
     {
         "identityStoreId": str,
     },
 )
 _OptionalSSOIdentityTypeDef = TypedDict(
@@ -875,97 +655,31 @@
 )
 
 
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
     pass
 
 
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
-StartDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "StartDetectorModelAnalysisResponseTypeDef",
-    {
-        "analysisId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAlarmModelResponseTypeDef = TypedDict(
-    "UpdateAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AlarmCapabilitiesOutputTypeDef = TypedDict(
-    "AlarmCapabilitiesOutputTypeDef",
-    {
-        "initializationConfiguration": InitializationConfigurationOutputTypeDef,
-        "acknowledgeFlow": AcknowledgeFlowOutputTypeDef,
-    },
-    total=False,
-)
-
 AlarmCapabilitiesTypeDef = TypedDict(
     "AlarmCapabilitiesTypeDef",
     {
         "initializationConfiguration": InitializationConfigurationTypeDef,
         "acknowledgeFlow": AcknowledgeFlowTypeDef,
     },
     total=False,
 )
 
-ListAlarmModelsResponseTypeDef = TypedDict(
-    "ListAlarmModelsResponseTypeDef",
-    {
-        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAlarmModelVersionsResponseTypeDef = TypedDict(
-    "ListAlarmModelVersionsResponseTypeDef",
-    {
-        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AlarmRuleOutputTypeDef = TypedDict(
-    "AlarmRuleOutputTypeDef",
-    {
-        "simpleRule": SimpleRuleOutputTypeDef,
-    },
-    total=False,
-)
-
 AlarmRuleTypeDef = TypedDict(
     "AlarmRuleTypeDef",
     {
         "simpleRule": SimpleRuleTypeDef,
     },
     total=False,
 )
@@ -977,38 +691,28 @@
         "level": AnalysisResultLevelType,
         "message": str,
         "locations": List[AnalysisResultLocationTypeDef],
     },
     total=False,
 )
 
-AssetPropertyValueOutputTypeDef = TypedDict(
-    "AssetPropertyValueOutputTypeDef",
-    {
-        "value": AssetPropertyVariantOutputTypeDef,
-        "timestamp": AssetPropertyTimestampOutputTypeDef,
-        "quality": str,
-    },
-    total=False,
-)
-
 AssetPropertyValueTypeDef = TypedDict(
     "AssetPropertyValueTypeDef",
     {
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
         "quality": str,
     },
     total=False,
 )
 
 InputDefinitionOutputTypeDef = TypedDict(
     "InputDefinitionOutputTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
     },
 )
 
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
@@ -1019,58 +723,131 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+CreateAlarmModelResponseTypeDef = TypedDict(
+    "CreateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    {
+        "status": AnalysisStatusType,
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
+ListAlarmModelVersionsResponseTypeDef = TypedDict(
+    "ListAlarmModelVersionsResponseTypeDef",
+    {
+        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlarmModelsResponseTypeDef = TypedDict(
+    "ListAlarmModelsResponseTypeDef",
+    {
+        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "StartDetectorModelAnalysisResponseTypeDef",
+    {
+        "analysisId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlarmModelResponseTypeDef = TypedDict(
+    "UpdateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDetectorModelResponseTypeDef = TypedDict(
     "CreateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDetectorModelResponseTypeDef = TypedDict(
     "UpdateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredLoggingOptionsOutputTypeDef = TypedDict(
     "_RequiredLoggingOptionsOutputTypeDef",
     {
         "roleArn": str,
         "level": LoggingLevelType,
         "enabled": bool,
     },
 )
 _OptionalLoggingOptionsOutputTypeDef = TypedDict(
     "_OptionalLoggingOptionsOutputTypeDef",
     {
-        "detectorDebugOptions": List[DetectorDebugOptionOutputTypeDef],
+        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
     },
     total=False,
 )
 
 
 class LoggingOptionsOutputTypeDef(
     _RequiredLoggingOptionsOutputTypeDef, _OptionalLoggingOptionsOutputTypeDef
@@ -1100,202 +877,26 @@
 
 
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectorModelVersionsResponseTypeDef = TypedDict(
     "ListDetectorModelVersionsResponseTypeDef",
     {
         "detectorModelVersionSummaries": List[DetectorModelVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDynamoDBActionOutputTypeDef = TypedDict(
-    "_RequiredDynamoDBActionOutputTypeDef",
-    {
-        "hashKeyField": str,
-        "hashKeyValue": str,
-        "tableName": str,
-    },
-)
-_OptionalDynamoDBActionOutputTypeDef = TypedDict(
-    "_OptionalDynamoDBActionOutputTypeDef",
-    {
-        "hashKeyType": str,
-        "rangeKeyType": str,
-        "rangeKeyField": str,
-        "rangeKeyValue": str,
-        "operation": str,
-        "payloadField": str,
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DynamoDBActionOutputTypeDef(
-    _RequiredDynamoDBActionOutputTypeDef, _OptionalDynamoDBActionOutputTypeDef
-):
-    pass
-
-
-_RequiredDynamoDBv2ActionOutputTypeDef = TypedDict(
-    "_RequiredDynamoDBv2ActionOutputTypeDef",
-    {
-        "tableName": str,
-    },
-)
-_OptionalDynamoDBv2ActionOutputTypeDef = TypedDict(
-    "_OptionalDynamoDBv2ActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DynamoDBv2ActionOutputTypeDef(
-    _RequiredDynamoDBv2ActionOutputTypeDef, _OptionalDynamoDBv2ActionOutputTypeDef
-):
-    pass
-
-
-_RequiredFirehoseActionOutputTypeDef = TypedDict(
-    "_RequiredFirehoseActionOutputTypeDef",
-    {
-        "deliveryStreamName": str,
-    },
-)
-_OptionalFirehoseActionOutputTypeDef = TypedDict(
-    "_OptionalFirehoseActionOutputTypeDef",
-    {
-        "separator": str,
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FirehoseActionOutputTypeDef(
-    _RequiredFirehoseActionOutputTypeDef, _OptionalFirehoseActionOutputTypeDef
-):
-    pass
-
-
-_RequiredIotEventsActionOutputTypeDef = TypedDict(
-    "_RequiredIotEventsActionOutputTypeDef",
-    {
-        "inputName": str,
-    },
-)
-_OptionalIotEventsActionOutputTypeDef = TypedDict(
-    "_OptionalIotEventsActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class IotEventsActionOutputTypeDef(
-    _RequiredIotEventsActionOutputTypeDef, _OptionalIotEventsActionOutputTypeDef
-):
-    pass
-
-
-_RequiredIotTopicPublishActionOutputTypeDef = TypedDict(
-    "_RequiredIotTopicPublishActionOutputTypeDef",
-    {
-        "mqttTopic": str,
-    },
-)
-_OptionalIotTopicPublishActionOutputTypeDef = TypedDict(
-    "_OptionalIotTopicPublishActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class IotTopicPublishActionOutputTypeDef(
-    _RequiredIotTopicPublishActionOutputTypeDef, _OptionalIotTopicPublishActionOutputTypeDef
-):
-    pass
-
-
-_RequiredLambdaActionOutputTypeDef = TypedDict(
-    "_RequiredLambdaActionOutputTypeDef",
-    {
-        "functionArn": str,
-    },
-)
-_OptionalLambdaActionOutputTypeDef = TypedDict(
-    "_OptionalLambdaActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class LambdaActionOutputTypeDef(
-    _RequiredLambdaActionOutputTypeDef, _OptionalLambdaActionOutputTypeDef
-):
-    pass
-
-
-_RequiredSNSTopicPublishActionOutputTypeDef = TypedDict(
-    "_RequiredSNSTopicPublishActionOutputTypeDef",
-    {
-        "targetArn": str,
-    },
-)
-_OptionalSNSTopicPublishActionOutputTypeDef = TypedDict(
-    "_OptionalSNSTopicPublishActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SNSTopicPublishActionOutputTypeDef(
-    _RequiredSNSTopicPublishActionOutputTypeDef, _OptionalSNSTopicPublishActionOutputTypeDef
-):
-    pass
-
-
-_RequiredSqsActionOutputTypeDef = TypedDict(
-    "_RequiredSqsActionOutputTypeDef",
-    {
-        "queueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSqsActionOutputTypeDef = TypedDict(
-    "_OptionalSqsActionOutputTypeDef",
-    {
-        "useBase64": bool,
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SqsActionOutputTypeDef(_RequiredSqsActionOutputTypeDef, _OptionalSqsActionOutputTypeDef):
-    pass
-
 
 _RequiredDynamoDBActionTypeDef = TypedDict(
     "_RequiredDynamoDBActionTypeDef",
     {
         "hashKeyField": str,
         "hashKeyValue": str,
         "tableName": str,
@@ -1460,15 +1061,15 @@
 
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IotSiteWiseInputIdentifierTypeDef = TypedDict(
     "IotSiteWiseInputIdentifierTypeDef",
     {
         "iotSiteWiseAssetModelPropertyIdentifier": IotSiteWiseAssetModelPropertyIdentifierTypeDef,
@@ -1477,61 +1078,33 @@
 )
 
 ListInputRoutingsResponseTypeDef = TypedDict(
     "ListInputRoutingsResponseTypeDef",
     {
         "routedResources": List[RoutedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RecipientDetailOutputTypeDef = TypedDict(
-    "RecipientDetailOutputTypeDef",
-    {
-        "ssoIdentity": SSOIdentityOutputTypeDef,
-    },
-    total=False,
-)
-
 RecipientDetailTypeDef = TypedDict(
     "RecipientDetailTypeDef",
     {
         "ssoIdentity": SSOIdentityTypeDef,
     },
     total=False,
 )
 
 GetDetectorModelAnalysisResultsResponseTypeDef = TypedDict(
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     {
         "analysisResults": List[AnalysisResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IotSiteWiseActionOutputTypeDef = TypedDict(
-    "IotSiteWiseActionOutputTypeDef",
-    {
-        "entryId": str,
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "propertyValue": AssetPropertyValueOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "entryId": str,
         "assetId": str,
@@ -1596,33 +1169,25 @@
     pass
 
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
-NotificationTargetActionsOutputTypeDef = TypedDict(
-    "NotificationTargetActionsOutputTypeDef",
-    {
-        "lambdaAction": LambdaActionOutputTypeDef,
-    },
-    total=False,
-)
-
 NotificationTargetActionsTypeDef = TypedDict(
     "NotificationTargetActionsTypeDef",
     {
         "lambdaAction": LambdaActionTypeDef,
     },
     total=False,
 )
@@ -1635,23 +1200,31 @@
     },
     total=False,
 )
 
 EmailRecipientsOutputTypeDef = TypedDict(
     "EmailRecipientsOutputTypeDef",
     {
-        "to": List[RecipientDetailOutputTypeDef],
+        "to": List[RecipientDetailTypeDef],
+    },
+    total=False,
+)
+
+EmailRecipientsTypeDef = TypedDict(
+    "EmailRecipientsTypeDef",
+    {
+        "to": Sequence[RecipientDetailTypeDef],
     },
     total=False,
 )
 
 _RequiredSMSConfigurationOutputTypeDef = TypedDict(
     "_RequiredSMSConfigurationOutputTypeDef",
     {
-        "recipients": List[RecipientDetailOutputTypeDef],
+        "recipients": List[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationOutputTypeDef = TypedDict(
     "_OptionalSMSConfigurationOutputTypeDef",
     {
         "senderId": str,
         "additionalMessage": str,
@@ -1662,22 +1235,14 @@
 
 class SMSConfigurationOutputTypeDef(
     _RequiredSMSConfigurationOutputTypeDef, _OptionalSMSConfigurationOutputTypeDef
 ):
     pass
 
 
-EmailRecipientsTypeDef = TypedDict(
-    "EmailRecipientsTypeDef",
-    {
-        "to": Sequence[RecipientDetailTypeDef],
-    },
-    total=False,
-)
-
 _RequiredSMSConfigurationTypeDef = TypedDict(
     "_RequiredSMSConfigurationTypeDef",
     {
         "recipients": Sequence[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationTypeDef = TypedDict(
@@ -1690,50 +1255,14 @@
 )
 
 
 class SMSConfigurationTypeDef(_RequiredSMSConfigurationTypeDef, _OptionalSMSConfigurationTypeDef):
     pass
 
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "setVariable": SetVariableActionOutputTypeDef,
-        "sns": SNSTopicPublishActionOutputTypeDef,
-        "iotTopicPublish": IotTopicPublishActionOutputTypeDef,
-        "setTimer": SetTimerActionOutputTypeDef,
-        "clearTimer": ClearTimerActionOutputTypeDef,
-        "resetTimer": ResetTimerActionOutputTypeDef,
-        "lambda": LambdaActionOutputTypeDef,
-        "iotEvents": IotEventsActionOutputTypeDef,
-        "sqs": SqsActionOutputTypeDef,
-        "firehose": FirehoseActionOutputTypeDef,
-        "dynamoDB": DynamoDBActionOutputTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
-        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-    },
-    total=False,
-)
-
-AlarmActionOutputTypeDef = TypedDict(
-    "AlarmActionOutputTypeDef",
-    {
-        "sns": SNSTopicPublishActionOutputTypeDef,
-        "iotTopicPublish": IotTopicPublishActionOutputTypeDef,
-        "lambda": LambdaActionOutputTypeDef,
-        "iotEvents": IotEventsActionOutputTypeDef,
-        "sqs": SqsActionOutputTypeDef,
-        "firehose": FirehoseActionOutputTypeDef,
-        "dynamoDB": DynamoDBActionOutputTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
-        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "setVariable": SetVariableActionTypeDef,
         "sns": SNSTopicPublishActionTypeDef,
         "iotTopicPublish": IotTopicPublishActionTypeDef,
         "setTimer": SetTimerActionTypeDef,
@@ -1766,15 +1295,15 @@
     total=False,
 )
 
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListInputRoutingsRequestRequestTypeDef = TypedDict(
     "_RequiredListInputRoutingsRequestRequestTypeDef",
     {
         "inputIdentifier": InputIdentifierTypeDef,
@@ -1802,15 +1331,15 @@
         "from": str,
         "recipients": EmailRecipientsOutputTypeDef,
     },
 )
 _OptionalEmailConfigurationOutputTypeDef = TypedDict(
     "_OptionalEmailConfigurationOutputTypeDef",
     {
-        "content": EmailContentOutputTypeDef,
+        "content": EmailContentTypeDef,
     },
     total=False,
 )
 
 
 class EmailConfigurationOutputTypeDef(
     _RequiredEmailConfigurationOutputTypeDef, _OptionalEmailConfigurationOutputTypeDef
@@ -1846,72 +1375,64 @@
         "eventName": str,
     },
 )
 _OptionalEventOutputTypeDef = TypedDict(
     "_OptionalEventOutputTypeDef",
     {
         "condition": str,
-        "actions": List[ActionOutputTypeDef],
+        "actions": List[ActionTypeDef],
     },
     total=False,
 )
 
 
 class EventOutputTypeDef(_RequiredEventOutputTypeDef, _OptionalEventOutputTypeDef):
     pass
 
 
-_RequiredTransitionEventOutputTypeDef = TypedDict(
-    "_RequiredTransitionEventOutputTypeDef",
+_RequiredEventTypeDef = TypedDict(
+    "_RequiredEventTypeDef",
     {
         "eventName": str,
-        "condition": str,
-        "nextState": str,
     },
 )
-_OptionalTransitionEventOutputTypeDef = TypedDict(
-    "_OptionalTransitionEventOutputTypeDef",
+_OptionalEventTypeDef = TypedDict(
+    "_OptionalEventTypeDef",
     {
-        "actions": List[ActionOutputTypeDef],
+        "condition": str,
+        "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
 
-class TransitionEventOutputTypeDef(
-    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
-):
+class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
 
-AlarmEventActionsOutputTypeDef = TypedDict(
-    "AlarmEventActionsOutputTypeDef",
-    {
-        "alarmActions": List[AlarmActionOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredEventTypeDef = TypedDict(
-    "_RequiredEventTypeDef",
+_RequiredTransitionEventOutputTypeDef = TypedDict(
+    "_RequiredTransitionEventOutputTypeDef",
     {
         "eventName": str,
+        "condition": str,
+        "nextState": str,
     },
 )
-_OptionalEventTypeDef = TypedDict(
-    "_OptionalEventTypeDef",
+_OptionalTransitionEventOutputTypeDef = TypedDict(
+    "_OptionalTransitionEventOutputTypeDef",
     {
-        "condition": str,
-        "actions": Sequence[ActionTypeDef],
+        "actions": List[ActionTypeDef],
     },
     total=False,
 )
 
 
-class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
+class TransitionEventOutputTypeDef(
+    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
+):
     pass
 
 
 _RequiredTransitionEventTypeDef = TypedDict(
     "_RequiredTransitionEventTypeDef",
     {
         "eventName": str,
@@ -1928,26 +1449,34 @@
 )
 
 
 class TransitionEventTypeDef(_RequiredTransitionEventTypeDef, _OptionalTransitionEventTypeDef):
     pass
 
 
+AlarmEventActionsOutputTypeDef = TypedDict(
+    "AlarmEventActionsOutputTypeDef",
+    {
+        "alarmActions": List[AlarmActionTypeDef],
+    },
+    total=False,
+)
+
 AlarmEventActionsTypeDef = TypedDict(
     "AlarmEventActionsTypeDef",
     {
         "alarmActions": Sequence[AlarmActionTypeDef],
     },
     total=False,
 )
 
 _RequiredNotificationActionOutputTypeDef = TypedDict(
     "_RequiredNotificationActionOutputTypeDef",
     {
-        "action": NotificationTargetActionsOutputTypeDef,
+        "action": NotificationTargetActionsTypeDef,
     },
 )
 _OptionalNotificationActionOutputTypeDef = TypedDict(
     "_OptionalNotificationActionOutputTypeDef",
     {
         "smsConfigurations": List[SMSConfigurationOutputTypeDef],
         "emailConfigurations": List[EmailConfigurationOutputTypeDef],
@@ -1996,23 +1525,14 @@
     "OnExitLifecycleOutputTypeDef",
     {
         "events": List[EventOutputTypeDef],
     },
     total=False,
 )
 
-OnInputLifecycleOutputTypeDef = TypedDict(
-    "OnInputLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-        "transitionEvents": List[TransitionEventOutputTypeDef],
-    },
-    total=False,
-)
-
 OnEnterLifecycleTypeDef = TypedDict(
     "OnEnterLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
@@ -2021,14 +1541,23 @@
     "OnExitLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
 
+OnInputLifecycleOutputTypeDef = TypedDict(
+    "OnInputLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+        "transitionEvents": List[TransitionEventOutputTypeDef],
+    },
+    total=False,
+)
+
 OnInputLifecycleTypeDef = TypedDict(
     "OnInputLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
@@ -2102,19 +1631,19 @@
         "status": AlarmModelVersionStatusType,
         "statusMessage": str,
         "alarmModelName": str,
         "alarmModelDescription": str,
         "roleArn": str,
         "key": str,
         "severity": int,
-        "alarmRule": AlarmRuleOutputTypeDef,
+        "alarmRule": AlarmRuleTypeDef,
         "alarmNotification": AlarmNotificationOutputTypeDef,
         "alarmEventActions": AlarmEventActionsOutputTypeDef,
-        "alarmCapabilities": AlarmCapabilitiesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "alarmCapabilities": AlarmCapabilitiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
@@ -2254,10 +1783,10 @@
     pass
 
 
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/type_defs.pyi` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotevents service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotevents.type_defs import AcknowledgeFlowOutputTypeDef
+    from mypy_boto3_iotevents.type_defs import AcknowledgeFlowTypeDef
 
-    data: AcknowledgeFlowOutputTypeDef = {...}
+    data: AcknowledgeFlowTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -29,154 +29,123 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AcknowledgeFlowOutputTypeDef",
     "AcknowledgeFlowTypeDef",
-    "ClearTimerActionOutputTypeDef",
-    "ResetTimerActionOutputTypeDef",
-    "SetTimerActionOutputTypeDef",
-    "SetVariableActionOutputTypeDef",
     "ClearTimerActionTypeDef",
     "ResetTimerActionTypeDef",
     "SetTimerActionTypeDef",
     "SetVariableActionTypeDef",
-    "InitializationConfigurationOutputTypeDef",
     "InitializationConfigurationTypeDef",
     "AlarmModelSummaryTypeDef",
     "AlarmModelVersionSummaryTypeDef",
-    "SimpleRuleOutputTypeDef",
     "SimpleRuleTypeDef",
     "AnalysisResultLocationTypeDef",
-    "AssetPropertyTimestampOutputTypeDef",
     "AssetPropertyTimestampTypeDef",
-    "AssetPropertyVariantOutputTypeDef",
     "AssetPropertyVariantTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "TagTypeDef",
-    "CreateAlarmModelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DetectorModelConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "DeleteAlarmModelRequestRequestTypeDef",
     "DeleteDetectorModelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DescribeAlarmModelRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
-    "DescribeDetectorModelAnalysisResponseTypeDef",
     "DescribeDetectorModelRequestRequestTypeDef",
     "DescribeInputRequestRequestTypeDef",
-    "DetectorDebugOptionOutputTypeDef",
     "DetectorDebugOptionTypeDef",
     "DetectorModelSummaryTypeDef",
     "DetectorModelVersionSummaryTypeDef",
-    "PayloadOutputTypeDef",
     "PayloadTypeDef",
-    "EmailContentOutputTypeDef",
     "EmailContentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetDetectorModelAnalysisResultsRequestRequestTypeDef",
     "IotEventsInputIdentifierTypeDef",
     "InputSummaryTypeDef",
     "IotSiteWiseAssetModelPropertyIdentifierTypeDef",
     "ListAlarmModelVersionsRequestRequestTypeDef",
     "ListAlarmModelsRequestRequestTypeDef",
     "ListDetectorModelVersionsRequestRequestTypeDef",
     "ListDetectorModelsRequestRequestTypeDef",
     "RoutedResourceTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "SSOIdentityOutputTypeDef",
     "SSOIdentityTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDetectorModelAnalysisResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlarmModelResponseTypeDef",
-    "AlarmCapabilitiesOutputTypeDef",
     "AlarmCapabilitiesTypeDef",
-    "ListAlarmModelsResponseTypeDef",
-    "ListAlarmModelVersionsResponseTypeDef",
-    "AlarmRuleOutputTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
-    "AssetPropertyValueOutputTypeDef",
     "AssetPropertyValueTypeDef",
     "InputDefinitionOutputTypeDef",
     "InputDefinitionTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateAlarmModelResponseTypeDef",
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAlarmModelVersionsResponseTypeDef",
+    "ListAlarmModelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDetectorModelAnalysisResponseTypeDef",
+    "UpdateAlarmModelResponseTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "LoggingOptionsOutputTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
-    "DynamoDBActionOutputTypeDef",
-    "DynamoDBv2ActionOutputTypeDef",
-    "FirehoseActionOutputTypeDef",
-    "IotEventsActionOutputTypeDef",
-    "IotTopicPublishActionOutputTypeDef",
-    "LambdaActionOutputTypeDef",
-    "SNSTopicPublishActionOutputTypeDef",
-    "SqsActionOutputTypeDef",
     "DynamoDBActionTypeDef",
     "DynamoDBv2ActionTypeDef",
     "FirehoseActionTypeDef",
     "IotEventsActionTypeDef",
     "IotTopicPublishActionTypeDef",
     "LambdaActionTypeDef",
     "SNSTopicPublishActionTypeDef",
     "SqsActionTypeDef",
     "ListInputsResponseTypeDef",
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RecipientDetailOutputTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
-    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "InputTypeDef",
     "CreateInputRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
-    "NotificationTargetActionsOutputTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
     "EmailRecipientsOutputTypeDef",
-    "SMSConfigurationOutputTypeDef",
     "EmailRecipientsTypeDef",
+    "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
-    "ActionOutputTypeDef",
-    "AlarmActionOutputTypeDef",
     "ActionTypeDef",
     "AlarmActionTypeDef",
     "DescribeInputResponseTypeDef",
     "ListInputRoutingsRequestRequestTypeDef",
     "EmailConfigurationOutputTypeDef",
     "EmailConfigurationTypeDef",
     "EventOutputTypeDef",
-    "TransitionEventOutputTypeDef",
-    "AlarmEventActionsOutputTypeDef",
     "EventTypeDef",
+    "TransitionEventOutputTypeDef",
     "TransitionEventTypeDef",
+    "AlarmEventActionsOutputTypeDef",
     "AlarmEventActionsTypeDef",
     "NotificationActionOutputTypeDef",
     "NotificationActionTypeDef",
     "OnEnterLifecycleOutputTypeDef",
     "OnExitLifecycleOutputTypeDef",
-    "OnInputLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
+    "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
     "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
     "StateOutputTypeDef",
     "StateTypeDef",
     "DescribeAlarmModelResponseTypeDef",
     "CreateAlarmModelRequestRequestTypeDef",
@@ -186,70 +155,21 @@
     "DetectorModelTypeDef",
     "CreateDetectorModelRequestRequestTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
-AcknowledgeFlowOutputTypeDef = TypedDict(
-    "AcknowledgeFlowOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
     {
         "enabled": bool,
     },
 )
 
-ClearTimerActionOutputTypeDef = TypedDict(
-    "ClearTimerActionOutputTypeDef",
-    {
-        "timerName": str,
-    },
-)
-
-ResetTimerActionOutputTypeDef = TypedDict(
-    "ResetTimerActionOutputTypeDef",
-    {
-        "timerName": str,
-    },
-)
-
-_RequiredSetTimerActionOutputTypeDef = TypedDict(
-    "_RequiredSetTimerActionOutputTypeDef",
-    {
-        "timerName": str,
-    },
-)
-_OptionalSetTimerActionOutputTypeDef = TypedDict(
-    "_OptionalSetTimerActionOutputTypeDef",
-    {
-        "seconds": int,
-        "durationExpression": str,
-    },
-    total=False,
-)
-
-class SetTimerActionOutputTypeDef(
-    _RequiredSetTimerActionOutputTypeDef, _OptionalSetTimerActionOutputTypeDef
-):
-    pass
-
-SetVariableActionOutputTypeDef = TypedDict(
-    "SetVariableActionOutputTypeDef",
-    {
-        "variableName": str,
-        "value": str,
-    },
-)
-
 ClearTimerActionTypeDef = TypedDict(
     "ClearTimerActionTypeDef",
     {
         "timerName": str,
     },
 )
 
@@ -282,21 +202,14 @@
     "SetVariableActionTypeDef",
     {
         "variableName": str,
         "value": str,
     },
 )
 
-InitializationConfigurationOutputTypeDef = TypedDict(
-    "InitializationConfigurationOutputTypeDef",
-    {
-        "disabledOnInitialization": bool,
-    },
-)
-
 InitializationConfigurationTypeDef = TypedDict(
     "InitializationConfigurationTypeDef",
     {
         "disabledOnInitialization": bool,
     },
 )
 
@@ -321,23 +234,14 @@
         "lastUpdateTime": datetime,
         "status": AlarmModelVersionStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-SimpleRuleOutputTypeDef = TypedDict(
-    "SimpleRuleOutputTypeDef",
-    {
-        "inputProperty": str,
-        "comparisonOperator": ComparisonOperatorType,
-        "threshold": str,
-    },
-)
-
 SimpleRuleTypeDef = TypedDict(
     "SimpleRuleTypeDef",
     {
         "inputProperty": str,
         "comparisonOperator": ComparisonOperatorType,
         "threshold": str,
     },
@@ -347,33 +251,14 @@
     "AnalysisResultLocationTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
-_RequiredAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyTimestampOutputTypeDef",
-    {
-        "timeInSeconds": str,
-    },
-)
-_OptionalAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyTimestampOutputTypeDef",
-    {
-        "offsetInNanos": str,
-    },
-    total=False,
-)
-
-class AssetPropertyTimestampOutputTypeDef(
-    _RequiredAssetPropertyTimestampOutputTypeDef, _OptionalAssetPropertyTimestampOutputTypeDef
-):
-    pass
-
 _RequiredAssetPropertyTimestampTypeDef = TypedDict(
     "_RequiredAssetPropertyTimestampTypeDef",
     {
         "timeInSeconds": str,
     },
 )
 _OptionalAssetPropertyTimestampTypeDef = TypedDict(
@@ -385,43 +270,25 @@
 )
 
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
-AssetPropertyVariantOutputTypeDef = TypedDict(
-    "AssetPropertyVariantOutputTypeDef",
-    {
-        "stringValue": str,
-        "integerValue": str,
-        "doubleValue": str,
-        "booleanValue": str,
-    },
-    total=False,
-)
-
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
     },
     total=False,
 )
 
-AttributeOutputTypeDef = TypedDict(
-    "AttributeOutputTypeDef",
-    {
-        "jsonPath": str,
-    },
-)
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "jsonPath": str,
     },
 )
 
@@ -429,23 +296,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreateAlarmModelResponseTypeDef = TypedDict(
-    "CreateAlarmModelResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DetectorModelConfigurationTypeDef = TypedDict(
     "DetectorModelConfigurationTypeDef",
     {
         "detectorModelName": str,
@@ -529,22 +395,14 @@
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
-DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    {
-        "status": AnalysisStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDescribeDetectorModelRequestRequestTypeDef = TypedDict(
@@ -564,33 +422,14 @@
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "inputName": str,
     },
 )
 
-_RequiredDetectorDebugOptionOutputTypeDef = TypedDict(
-    "_RequiredDetectorDebugOptionOutputTypeDef",
-    {
-        "detectorModelName": str,
-    },
-)
-_OptionalDetectorDebugOptionOutputTypeDef = TypedDict(
-    "_OptionalDetectorDebugOptionOutputTypeDef",
-    {
-        "keyValue": str,
-    },
-    total=False,
-)
-
-class DetectorDebugOptionOutputTypeDef(
-    _RequiredDetectorDebugOptionOutputTypeDef, _OptionalDetectorDebugOptionOutputTypeDef
-):
-    pass
-
 _RequiredDetectorDebugOptionTypeDef = TypedDict(
     "_RequiredDetectorDebugOptionTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDetectorDebugOptionTypeDef = TypedDict(
@@ -627,55 +466,31 @@
         "lastUpdateTime": datetime,
         "status": DetectorModelVersionStatusType,
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
-PayloadOutputTypeDef = TypedDict(
-    "PayloadOutputTypeDef",
-    {
-        "contentExpression": str,
-        "type": PayloadTypeType,
-    },
-)
-
 PayloadTypeDef = TypedDict(
     "PayloadTypeDef",
     {
         "contentExpression": str,
         "type": PayloadTypeType,
     },
 )
 
-EmailContentOutputTypeDef = TypedDict(
-    "EmailContentOutputTypeDef",
-    {
-        "subject": str,
-        "additionalMessage": str,
-    },
-    total=False,
-)
-
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "subject": str,
         "additionalMessage": str,
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
 _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
@@ -802,41 +617,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
-_RequiredSSOIdentityOutputTypeDef = TypedDict(
-    "_RequiredSSOIdentityOutputTypeDef",
-    {
-        "identityStoreId": str,
-    },
-)
-_OptionalSSOIdentityOutputTypeDef = TypedDict(
-    "_OptionalSSOIdentityOutputTypeDef",
-    {
-        "userId": str,
-    },
-    total=False,
-)
-
-class SSOIdentityOutputTypeDef(
-    _RequiredSSOIdentityOutputTypeDef, _OptionalSSOIdentityOutputTypeDef
-):
-    pass
-
 _RequiredSSOIdentityTypeDef = TypedDict(
     "_RequiredSSOIdentityTypeDef",
     {
         "identityStoreId": str,
     },
 )
 _OptionalSSOIdentityTypeDef = TypedDict(
@@ -846,97 +634,31 @@
     },
     total=False,
 )
 
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
     pass
 
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
-StartDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "StartDetectorModelAnalysisResponseTypeDef",
-    {
-        "analysisId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAlarmModelResponseTypeDef = TypedDict(
-    "UpdateAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AlarmCapabilitiesOutputTypeDef = TypedDict(
-    "AlarmCapabilitiesOutputTypeDef",
-    {
-        "initializationConfiguration": InitializationConfigurationOutputTypeDef,
-        "acknowledgeFlow": AcknowledgeFlowOutputTypeDef,
-    },
-    total=False,
-)
-
 AlarmCapabilitiesTypeDef = TypedDict(
     "AlarmCapabilitiesTypeDef",
     {
         "initializationConfiguration": InitializationConfigurationTypeDef,
         "acknowledgeFlow": AcknowledgeFlowTypeDef,
     },
     total=False,
 )
 
-ListAlarmModelsResponseTypeDef = TypedDict(
-    "ListAlarmModelsResponseTypeDef",
-    {
-        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAlarmModelVersionsResponseTypeDef = TypedDict(
-    "ListAlarmModelVersionsResponseTypeDef",
-    {
-        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AlarmRuleOutputTypeDef = TypedDict(
-    "AlarmRuleOutputTypeDef",
-    {
-        "simpleRule": SimpleRuleOutputTypeDef,
-    },
-    total=False,
-)
-
 AlarmRuleTypeDef = TypedDict(
     "AlarmRuleTypeDef",
     {
         "simpleRule": SimpleRuleTypeDef,
     },
     total=False,
 )
@@ -948,38 +670,28 @@
         "level": AnalysisResultLevelType,
         "message": str,
         "locations": List[AnalysisResultLocationTypeDef],
     },
     total=False,
 )
 
-AssetPropertyValueOutputTypeDef = TypedDict(
-    "AssetPropertyValueOutputTypeDef",
-    {
-        "value": AssetPropertyVariantOutputTypeDef,
-        "timestamp": AssetPropertyTimestampOutputTypeDef,
-        "quality": str,
-    },
-    total=False,
-)
-
 AssetPropertyValueTypeDef = TypedDict(
     "AssetPropertyValueTypeDef",
     {
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
         "quality": str,
     },
     total=False,
 )
 
 InputDefinitionOutputTypeDef = TypedDict(
     "InputDefinitionOutputTypeDef",
     {
-        "attributes": List[AttributeOutputTypeDef],
+        "attributes": List[AttributeTypeDef],
     },
 )
 
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
@@ -990,58 +702,131 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+CreateAlarmModelResponseTypeDef = TypedDict(
+    "CreateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    {
+        "status": AnalysisStatusType,
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
+ListAlarmModelVersionsResponseTypeDef = TypedDict(
+    "ListAlarmModelVersionsResponseTypeDef",
+    {
+        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlarmModelsResponseTypeDef = TypedDict(
+    "ListAlarmModelsResponseTypeDef",
+    {
+        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "StartDetectorModelAnalysisResponseTypeDef",
+    {
+        "analysisId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlarmModelResponseTypeDef = TypedDict(
+    "UpdateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDetectorModelResponseTypeDef = TypedDict(
     "CreateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDetectorModelResponseTypeDef = TypedDict(
     "UpdateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredLoggingOptionsOutputTypeDef = TypedDict(
     "_RequiredLoggingOptionsOutputTypeDef",
     {
         "roleArn": str,
         "level": LoggingLevelType,
         "enabled": bool,
     },
 )
 _OptionalLoggingOptionsOutputTypeDef = TypedDict(
     "_OptionalLoggingOptionsOutputTypeDef",
     {
-        "detectorDebugOptions": List[DetectorDebugOptionOutputTypeDef],
+        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
     },
     total=False,
 )
 
 class LoggingOptionsOutputTypeDef(
     _RequiredLoggingOptionsOutputTypeDef, _OptionalLoggingOptionsOutputTypeDef
 ):
@@ -1067,186 +852,26 @@
     pass
 
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectorModelVersionsResponseTypeDef = TypedDict(
     "ListDetectorModelVersionsResponseTypeDef",
     {
         "detectorModelVersionSummaries": List[DetectorModelVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDynamoDBActionOutputTypeDef = TypedDict(
-    "_RequiredDynamoDBActionOutputTypeDef",
-    {
-        "hashKeyField": str,
-        "hashKeyValue": str,
-        "tableName": str,
-    },
-)
-_OptionalDynamoDBActionOutputTypeDef = TypedDict(
-    "_OptionalDynamoDBActionOutputTypeDef",
-    {
-        "hashKeyType": str,
-        "rangeKeyType": str,
-        "rangeKeyField": str,
-        "rangeKeyValue": str,
-        "operation": str,
-        "payloadField": str,
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class DynamoDBActionOutputTypeDef(
-    _RequiredDynamoDBActionOutputTypeDef, _OptionalDynamoDBActionOutputTypeDef
-):
-    pass
-
-_RequiredDynamoDBv2ActionOutputTypeDef = TypedDict(
-    "_RequiredDynamoDBv2ActionOutputTypeDef",
-    {
-        "tableName": str,
-    },
-)
-_OptionalDynamoDBv2ActionOutputTypeDef = TypedDict(
-    "_OptionalDynamoDBv2ActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class DynamoDBv2ActionOutputTypeDef(
-    _RequiredDynamoDBv2ActionOutputTypeDef, _OptionalDynamoDBv2ActionOutputTypeDef
-):
-    pass
-
-_RequiredFirehoseActionOutputTypeDef = TypedDict(
-    "_RequiredFirehoseActionOutputTypeDef",
-    {
-        "deliveryStreamName": str,
-    },
-)
-_OptionalFirehoseActionOutputTypeDef = TypedDict(
-    "_OptionalFirehoseActionOutputTypeDef",
-    {
-        "separator": str,
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class FirehoseActionOutputTypeDef(
-    _RequiredFirehoseActionOutputTypeDef, _OptionalFirehoseActionOutputTypeDef
-):
-    pass
-
-_RequiredIotEventsActionOutputTypeDef = TypedDict(
-    "_RequiredIotEventsActionOutputTypeDef",
-    {
-        "inputName": str,
-    },
-)
-_OptionalIotEventsActionOutputTypeDef = TypedDict(
-    "_OptionalIotEventsActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class IotEventsActionOutputTypeDef(
-    _RequiredIotEventsActionOutputTypeDef, _OptionalIotEventsActionOutputTypeDef
-):
-    pass
-
-_RequiredIotTopicPublishActionOutputTypeDef = TypedDict(
-    "_RequiredIotTopicPublishActionOutputTypeDef",
-    {
-        "mqttTopic": str,
-    },
-)
-_OptionalIotTopicPublishActionOutputTypeDef = TypedDict(
-    "_OptionalIotTopicPublishActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class IotTopicPublishActionOutputTypeDef(
-    _RequiredIotTopicPublishActionOutputTypeDef, _OptionalIotTopicPublishActionOutputTypeDef
-):
-    pass
-
-_RequiredLambdaActionOutputTypeDef = TypedDict(
-    "_RequiredLambdaActionOutputTypeDef",
-    {
-        "functionArn": str,
-    },
-)
-_OptionalLambdaActionOutputTypeDef = TypedDict(
-    "_OptionalLambdaActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class LambdaActionOutputTypeDef(
-    _RequiredLambdaActionOutputTypeDef, _OptionalLambdaActionOutputTypeDef
-):
-    pass
-
-_RequiredSNSTopicPublishActionOutputTypeDef = TypedDict(
-    "_RequiredSNSTopicPublishActionOutputTypeDef",
-    {
-        "targetArn": str,
-    },
-)
-_OptionalSNSTopicPublishActionOutputTypeDef = TypedDict(
-    "_OptionalSNSTopicPublishActionOutputTypeDef",
-    {
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class SNSTopicPublishActionOutputTypeDef(
-    _RequiredSNSTopicPublishActionOutputTypeDef, _OptionalSNSTopicPublishActionOutputTypeDef
-):
-    pass
-
-_RequiredSqsActionOutputTypeDef = TypedDict(
-    "_RequiredSqsActionOutputTypeDef",
-    {
-        "queueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSqsActionOutputTypeDef = TypedDict(
-    "_OptionalSqsActionOutputTypeDef",
-    {
-        "useBase64": bool,
-        "payload": PayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-class SqsActionOutputTypeDef(_RequiredSqsActionOutputTypeDef, _OptionalSqsActionOutputTypeDef):
-    pass
 
 _RequiredDynamoDBActionTypeDef = TypedDict(
     "_RequiredDynamoDBActionTypeDef",
     {
         "hashKeyField": str,
         "hashKeyValue": str,
         "tableName": str,
@@ -1395,15 +1020,15 @@
     pass
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IotSiteWiseInputIdentifierTypeDef = TypedDict(
     "IotSiteWiseInputIdentifierTypeDef",
     {
         "iotSiteWiseAssetModelPropertyIdentifier": IotSiteWiseAssetModelPropertyIdentifierTypeDef,
@@ -1412,61 +1037,33 @@
 )
 
 ListInputRoutingsResponseTypeDef = TypedDict(
     "ListInputRoutingsResponseTypeDef",
     {
         "routedResources": List[RoutedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RecipientDetailOutputTypeDef = TypedDict(
-    "RecipientDetailOutputTypeDef",
-    {
-        "ssoIdentity": SSOIdentityOutputTypeDef,
-    },
-    total=False,
-)
-
 RecipientDetailTypeDef = TypedDict(
     "RecipientDetailTypeDef",
     {
         "ssoIdentity": SSOIdentityTypeDef,
     },
     total=False,
 )
 
 GetDetectorModelAnalysisResultsResponseTypeDef = TypedDict(
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     {
         "analysisResults": List[AnalysisResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IotSiteWiseActionOutputTypeDef = TypedDict(
-    "IotSiteWiseActionOutputTypeDef",
-    {
-        "entryId": str,
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-        "propertyValue": AssetPropertyValueOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "entryId": str,
         "assetId": str,
@@ -1527,33 +1124,25 @@
 ):
     pass
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
-NotificationTargetActionsOutputTypeDef = TypedDict(
-    "NotificationTargetActionsOutputTypeDef",
-    {
-        "lambdaAction": LambdaActionOutputTypeDef,
-    },
-    total=False,
-)
-
 NotificationTargetActionsTypeDef = TypedDict(
     "NotificationTargetActionsTypeDef",
     {
         "lambdaAction": LambdaActionTypeDef,
     },
     total=False,
 )
@@ -1566,23 +1155,31 @@
     },
     total=False,
 )
 
 EmailRecipientsOutputTypeDef = TypedDict(
     "EmailRecipientsOutputTypeDef",
     {
-        "to": List[RecipientDetailOutputTypeDef],
+        "to": List[RecipientDetailTypeDef],
+    },
+    total=False,
+)
+
+EmailRecipientsTypeDef = TypedDict(
+    "EmailRecipientsTypeDef",
+    {
+        "to": Sequence[RecipientDetailTypeDef],
     },
     total=False,
 )
 
 _RequiredSMSConfigurationOutputTypeDef = TypedDict(
     "_RequiredSMSConfigurationOutputTypeDef",
     {
-        "recipients": List[RecipientDetailOutputTypeDef],
+        "recipients": List[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationOutputTypeDef = TypedDict(
     "_OptionalSMSConfigurationOutputTypeDef",
     {
         "senderId": str,
         "additionalMessage": str,
@@ -1591,22 +1188,14 @@
 )
 
 class SMSConfigurationOutputTypeDef(
     _RequiredSMSConfigurationOutputTypeDef, _OptionalSMSConfigurationOutputTypeDef
 ):
     pass
 
-EmailRecipientsTypeDef = TypedDict(
-    "EmailRecipientsTypeDef",
-    {
-        "to": Sequence[RecipientDetailTypeDef],
-    },
-    total=False,
-)
-
 _RequiredSMSConfigurationTypeDef = TypedDict(
     "_RequiredSMSConfigurationTypeDef",
     {
         "recipients": Sequence[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationTypeDef = TypedDict(
@@ -1617,50 +1206,14 @@
     },
     total=False,
 )
 
 class SMSConfigurationTypeDef(_RequiredSMSConfigurationTypeDef, _OptionalSMSConfigurationTypeDef):
     pass
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "setVariable": SetVariableActionOutputTypeDef,
-        "sns": SNSTopicPublishActionOutputTypeDef,
-        "iotTopicPublish": IotTopicPublishActionOutputTypeDef,
-        "setTimer": SetTimerActionOutputTypeDef,
-        "clearTimer": ClearTimerActionOutputTypeDef,
-        "resetTimer": ResetTimerActionOutputTypeDef,
-        "lambda": LambdaActionOutputTypeDef,
-        "iotEvents": IotEventsActionOutputTypeDef,
-        "sqs": SqsActionOutputTypeDef,
-        "firehose": FirehoseActionOutputTypeDef,
-        "dynamoDB": DynamoDBActionOutputTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
-        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-    },
-    total=False,
-)
-
-AlarmActionOutputTypeDef = TypedDict(
-    "AlarmActionOutputTypeDef",
-    {
-        "sns": SNSTopicPublishActionOutputTypeDef,
-        "iotTopicPublish": IotTopicPublishActionOutputTypeDef,
-        "lambda": LambdaActionOutputTypeDef,
-        "iotEvents": IotEventsActionOutputTypeDef,
-        "sqs": SqsActionOutputTypeDef,
-        "firehose": FirehoseActionOutputTypeDef,
-        "dynamoDB": DynamoDBActionOutputTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
-        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "setVariable": SetVariableActionTypeDef,
         "sns": SNSTopicPublishActionTypeDef,
         "iotTopicPublish": IotTopicPublishActionTypeDef,
         "setTimer": SetTimerActionTypeDef,
@@ -1693,15 +1246,15 @@
     total=False,
 )
 
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListInputRoutingsRequestRequestTypeDef = TypedDict(
     "_RequiredListInputRoutingsRequestRequestTypeDef",
     {
         "inputIdentifier": InputIdentifierTypeDef,
@@ -1727,15 +1280,15 @@
         "from": str,
         "recipients": EmailRecipientsOutputTypeDef,
     },
 )
 _OptionalEmailConfigurationOutputTypeDef = TypedDict(
     "_OptionalEmailConfigurationOutputTypeDef",
     {
-        "content": EmailContentOutputTypeDef,
+        "content": EmailContentTypeDef,
     },
     total=False,
 )
 
 class EmailConfigurationOutputTypeDef(
     _RequiredEmailConfigurationOutputTypeDef, _OptionalEmailConfigurationOutputTypeDef
 ):
@@ -1767,67 +1320,59 @@
         "eventName": str,
     },
 )
 _OptionalEventOutputTypeDef = TypedDict(
     "_OptionalEventOutputTypeDef",
     {
         "condition": str,
-        "actions": List[ActionOutputTypeDef],
+        "actions": List[ActionTypeDef],
     },
     total=False,
 )
 
 class EventOutputTypeDef(_RequiredEventOutputTypeDef, _OptionalEventOutputTypeDef):
     pass
 
-_RequiredTransitionEventOutputTypeDef = TypedDict(
-    "_RequiredTransitionEventOutputTypeDef",
+_RequiredEventTypeDef = TypedDict(
+    "_RequiredEventTypeDef",
     {
         "eventName": str,
-        "condition": str,
-        "nextState": str,
     },
 )
-_OptionalTransitionEventOutputTypeDef = TypedDict(
-    "_OptionalTransitionEventOutputTypeDef",
+_OptionalEventTypeDef = TypedDict(
+    "_OptionalEventTypeDef",
     {
-        "actions": List[ActionOutputTypeDef],
+        "condition": str,
+        "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
-class TransitionEventOutputTypeDef(
-    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
-):
+class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-AlarmEventActionsOutputTypeDef = TypedDict(
-    "AlarmEventActionsOutputTypeDef",
-    {
-        "alarmActions": List[AlarmActionOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredEventTypeDef = TypedDict(
-    "_RequiredEventTypeDef",
+_RequiredTransitionEventOutputTypeDef = TypedDict(
+    "_RequiredTransitionEventOutputTypeDef",
     {
         "eventName": str,
+        "condition": str,
+        "nextState": str,
     },
 )
-_OptionalEventTypeDef = TypedDict(
-    "_OptionalEventTypeDef",
+_OptionalTransitionEventOutputTypeDef = TypedDict(
+    "_OptionalTransitionEventOutputTypeDef",
     {
-        "condition": str,
-        "actions": Sequence[ActionTypeDef],
+        "actions": List[ActionTypeDef],
     },
     total=False,
 )
 
-class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
+class TransitionEventOutputTypeDef(
+    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
+):
     pass
 
 _RequiredTransitionEventTypeDef = TypedDict(
     "_RequiredTransitionEventTypeDef",
     {
         "eventName": str,
         "condition": str,
@@ -1841,26 +1386,34 @@
     },
     total=False,
 )
 
 class TransitionEventTypeDef(_RequiredTransitionEventTypeDef, _OptionalTransitionEventTypeDef):
     pass
 
+AlarmEventActionsOutputTypeDef = TypedDict(
+    "AlarmEventActionsOutputTypeDef",
+    {
+        "alarmActions": List[AlarmActionTypeDef],
+    },
+    total=False,
+)
+
 AlarmEventActionsTypeDef = TypedDict(
     "AlarmEventActionsTypeDef",
     {
         "alarmActions": Sequence[AlarmActionTypeDef],
     },
     total=False,
 )
 
 _RequiredNotificationActionOutputTypeDef = TypedDict(
     "_RequiredNotificationActionOutputTypeDef",
     {
-        "action": NotificationTargetActionsOutputTypeDef,
+        "action": NotificationTargetActionsTypeDef,
     },
 )
 _OptionalNotificationActionOutputTypeDef = TypedDict(
     "_OptionalNotificationActionOutputTypeDef",
     {
         "smsConfigurations": List[SMSConfigurationOutputTypeDef],
         "emailConfigurations": List[EmailConfigurationOutputTypeDef],
@@ -1905,23 +1458,14 @@
     "OnExitLifecycleOutputTypeDef",
     {
         "events": List[EventOutputTypeDef],
     },
     total=False,
 )
 
-OnInputLifecycleOutputTypeDef = TypedDict(
-    "OnInputLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-        "transitionEvents": List[TransitionEventOutputTypeDef],
-    },
-    total=False,
-)
-
 OnEnterLifecycleTypeDef = TypedDict(
     "OnEnterLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
@@ -1930,14 +1474,23 @@
     "OnExitLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
 
+OnInputLifecycleOutputTypeDef = TypedDict(
+    "OnInputLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+        "transitionEvents": List[TransitionEventOutputTypeDef],
+    },
+    total=False,
+)
+
 OnInputLifecycleTypeDef = TypedDict(
     "OnInputLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
@@ -2007,19 +1560,19 @@
         "status": AlarmModelVersionStatusType,
         "statusMessage": str,
         "alarmModelName": str,
         "alarmModelDescription": str,
         "roleArn": str,
         "key": str,
         "severity": int,
-        "alarmRule": AlarmRuleOutputTypeDef,
+        "alarmRule": AlarmRuleTypeDef,
         "alarmNotification": AlarmNotificationOutputTypeDef,
         "alarmEventActions": AlarmEventActionsOutputTypeDef,
-        "alarmCapabilities": AlarmCapabilitiesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "alarmCapabilities": AlarmCapabilitiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
@@ -2151,10 +1704,10 @@
 ):
     pass
 
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/PKG-INFO` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTEvents 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,154 +304,123 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
-    AcknowledgeFlowOutputTypeDef,
     AcknowledgeFlowTypeDef,
-    ClearTimerActionOutputTypeDef,
-    ResetTimerActionOutputTypeDef,
-    SetTimerActionOutputTypeDef,
-    SetVariableActionOutputTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
     SetVariableActionTypeDef,
-    InitializationConfigurationOutputTypeDef,
     InitializationConfigurationTypeDef,
     AlarmModelSummaryTypeDef,
     AlarmModelVersionSummaryTypeDef,
-    SimpleRuleOutputTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
-    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
-    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
-    AttributeOutputTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    CreateAlarmModelResponseTypeDef,
+    ResponseMetadataTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
-    DetectorDebugOptionOutputTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
-    PayloadOutputTypeDef,
     PayloadTypeDef,
-    EmailContentOutputTypeDef,
     EmailContentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    SSOIdentityOutputTypeDef,
     SSOIdentityTypeDef,
-    ResponseMetadataTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlarmModelResponseTypeDef,
-    AlarmCapabilitiesOutputTypeDef,
     AlarmCapabilitiesTypeDef,
-    ListAlarmModelsResponseTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
-    AlarmRuleOutputTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
-    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
     InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAlarmModelResponseTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
     LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
-    DynamoDBActionOutputTypeDef,
-    DynamoDBv2ActionOutputTypeDef,
-    FirehoseActionOutputTypeDef,
-    IotEventsActionOutputTypeDef,
-    IotTopicPublishActionOutputTypeDef,
-    LambdaActionOutputTypeDef,
-    SNSTopicPublishActionOutputTypeDef,
-    SqsActionOutputTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
     IotTopicPublishActionTypeDef,
     LambdaActionTypeDef,
     SNSTopicPublishActionTypeDef,
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RecipientDetailOutputTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     InputTypeDef,
     CreateInputRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
-    NotificationTargetActionsOutputTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
     EmailRecipientsOutputTypeDef,
-    SMSConfigurationOutputTypeDef,
     EmailRecipientsTypeDef,
+    SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
-    ActionOutputTypeDef,
-    AlarmActionOutputTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
     EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
     EventOutputTypeDef,
-    TransitionEventOutputTypeDef,
-    AlarmEventActionsOutputTypeDef,
     EventTypeDef,
+    TransitionEventOutputTypeDef,
     TransitionEventTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
     NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
     OnEnterLifecycleOutputTypeDef,
     OnExitLifecycleOutputTypeDef,
-    OnInputLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
     AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
     StateOutputTypeDef,
     StateTypeDef,
     DescribeAlarmModelResponseTypeDef,
     CreateAlarmModelRequestRequestTypeDef,
@@ -462,15 +431,15 @@
     CreateDetectorModelRequestRequestTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowOutputTypeDef:
+def get_structure() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-1.28.15/mypy_boto3_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.12/setup.py` & `mypy-boto3-iotevents-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTEvents 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTEvents 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

