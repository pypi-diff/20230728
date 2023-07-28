# Comparing `tmp/mypy-boto3-events-1.28.12.tar.gz` & `tmp/mypy-boto3-events-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-events-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
+gzip compressed data, was "mypy-boto3-events-1.28.15.tar", last modified: Fri Jul 28 20:42:47 2023, max compression
```

## Comparing `mypy-boto3-events-1.28.12.tar` & `mypy-boto3-events-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.912513 mypy-boto3-events-1.28.12/mypy_boto3_events/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69913 2023-07-27 05:22:10.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69828 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.117087 mypy-boto3-events-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-07-28 20:42:47.105087 mypy-boto3-events-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18700 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.105087 mypy-boto3-events-1.28.15/mypy_boto3_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-28 20:25:41.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-28 20:25:41.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64838 2023-07-28 20:25:42.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64757 2023-07-28 20:25:42.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/mypy_boto3_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.105087 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:46.000000 mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:47.117087 mypy-boto3-events-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-28 20:25:40.000000 mypy-boto3-events-1.28.15/setup.py
```

### Comparing `mypy-boto3-events-1.28.12/LICENSE` & `mypy-boto3-events-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/PKG-INFO` & `mypy-boto3-events-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.12
-Summary: Type annotations for boto3.EventBridge 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,175 +351,155 @@
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
-    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
-    CancelReplayResponseTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
+    ResponseMetadataTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
-    ConnectionBodyParameterOutputTypeDef,
     ConnectionBodyParameterTypeDef,
-    ConnectionHeaderParameterOutputTypeDef,
     ConnectionHeaderParameterTypeDef,
-    ConnectionQueryStringParameterOutputTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
-    CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
-    CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
-    CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
-    EndpointEventBusOutputTypeDef,
-    ReplicationConfigOutputTypeDef,
     TagTypeDef,
-    CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
-    CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
-    DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
-    DeleteConnectionResponseTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEventBusRequestRequestTypeDef,
     DeletePartnerEventSourceRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DescribeApiDestinationRequestRequestTypeDef,
-    DescribeApiDestinationResponseTypeDef,
     DescribeArchiveRequestRequestTypeDef,
-    DescribeArchiveResponseTypeDef,
     DescribeConnectionRequestRequestTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEventBusRequestRequestTypeDef,
-    DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
-    DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
-    DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
     ReplayDestinationOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
-    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
-    PrimaryOutputTypeDef,
-    SecondaryOutputTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
     HttpParametersOutputTypeDef,
     HttpParametersTypeDef,
     InputTransformerOutputTypeDef,
     InputTransformerTypeDef,
-    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
     ListApiDestinationsRequestRequestTypeDef,
     ListArchivesRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEventBusesRequestRequestTypeDef,
     ListEventSourcesRequestRequestTypeDef,
     ListPartnerEventSourceAccountsRequestRequestTypeDef,
     PartnerEventSourceAccountTypeDef,
     ListPartnerEventSourcesRequestRequestTypeDef,
     PartnerEventSourceTypeDef,
     ListReplaysRequestRequestTypeDef,
     ReplayTypeDef,
-    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
-    ListRuleNamesByTargetResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
-    PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
     ReplayDestinationTypeDef,
-    ResponseMetadataTypeDef,
-    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
     RunCommandTargetOutputTypeDef,
     RunCommandTargetTypeDef,
-    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
-    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
-    StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
-    TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
-    UpdateApiDestinationResponseTypeDef,
     UpdateArchiveRequestRequestTypeDef,
-    UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
-    UpdateConnectionResponseTypeDef,
-    ListApiDestinationsResponseTypeDef,
-    ListArchivesResponseTypeDef,
     NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
-    BatchParametersOutputTypeDef,
     BatchParametersTypeDef,
+    CancelReplayResponseTypeDef,
+    CreateApiDestinationResponseTypeDef,
+    CreateArchiveResponseTypeDef,
+    CreateConnectionResponseTypeDef,
+    CreateEventBusResponseTypeDef,
+    CreatePartnerEventSourceResponseTypeDef,
+    DeauthorizeConnectionResponseTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DescribeApiDestinationResponseTypeDef,
+    DescribeArchiveResponseTypeDef,
+    DescribeEventBusResponseTypeDef,
+    DescribeEventSourceResponseTypeDef,
+    DescribePartnerEventSourceResponseTypeDef,
+    DescribeRuleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListApiDestinationsResponseTypeDef,
+    ListArchivesResponseTypeDef,
+    ListRuleNamesByTargetResponseTypeDef,
+    PutRuleResponseTypeDef,
+    StartReplayResponseTypeDef,
+    TestEventPatternResponseTypeDef,
+    UpdateApiDestinationResponseTypeDef,
+    UpdateArchiveResponseTypeDef,
+    UpdateConnectionResponseTypeDef,
     PutPermissionRequestRequestTypeDef,
     ConnectionHttpParametersOutputTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeReplayResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
-    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
+    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
@@ -529,27 +509,26 @@
     SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
-    RoutingConfigOutputTypeDef,
     RoutingConfigTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
+    CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
-    UpdateEndpointResponseTypeDef,
-    CreateEndpointRequestRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
+    UpdateEndpointResponseTypeDef,
     ListTargetsByRuleResponseTypeDef,
     PutTargetsRequestRequestTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-events-1.28.12/README.md` & `mypy-boto3-events-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,175 +319,155 @@
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
-    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
-    CancelReplayResponseTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
+    ResponseMetadataTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
-    ConnectionBodyParameterOutputTypeDef,
     ConnectionBodyParameterTypeDef,
-    ConnectionHeaderParameterOutputTypeDef,
     ConnectionHeaderParameterTypeDef,
-    ConnectionQueryStringParameterOutputTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
-    CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
-    CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
-    CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
-    EndpointEventBusOutputTypeDef,
-    ReplicationConfigOutputTypeDef,
     TagTypeDef,
-    CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
-    CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
-    DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
-    DeleteConnectionResponseTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEventBusRequestRequestTypeDef,
     DeletePartnerEventSourceRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DescribeApiDestinationRequestRequestTypeDef,
-    DescribeApiDestinationResponseTypeDef,
     DescribeArchiveRequestRequestTypeDef,
-    DescribeArchiveResponseTypeDef,
     DescribeConnectionRequestRequestTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEventBusRequestRequestTypeDef,
-    DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
-    DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
-    DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
     ReplayDestinationOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
-    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
-    PrimaryOutputTypeDef,
-    SecondaryOutputTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
     HttpParametersOutputTypeDef,
     HttpParametersTypeDef,
     InputTransformerOutputTypeDef,
     InputTransformerTypeDef,
-    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
     ListApiDestinationsRequestRequestTypeDef,
     ListArchivesRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEventBusesRequestRequestTypeDef,
     ListEventSourcesRequestRequestTypeDef,
     ListPartnerEventSourceAccountsRequestRequestTypeDef,
     PartnerEventSourceAccountTypeDef,
     ListPartnerEventSourcesRequestRequestTypeDef,
     PartnerEventSourceTypeDef,
     ListReplaysRequestRequestTypeDef,
     ReplayTypeDef,
-    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
-    ListRuleNamesByTargetResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
-    PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
     ReplayDestinationTypeDef,
-    ResponseMetadataTypeDef,
-    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
     RunCommandTargetOutputTypeDef,
     RunCommandTargetTypeDef,
-    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
-    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
-    StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
-    TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
-    UpdateApiDestinationResponseTypeDef,
     UpdateArchiveRequestRequestTypeDef,
-    UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
-    UpdateConnectionResponseTypeDef,
-    ListApiDestinationsResponseTypeDef,
-    ListArchivesResponseTypeDef,
     NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
-    BatchParametersOutputTypeDef,
     BatchParametersTypeDef,
+    CancelReplayResponseTypeDef,
+    CreateApiDestinationResponseTypeDef,
+    CreateArchiveResponseTypeDef,
+    CreateConnectionResponseTypeDef,
+    CreateEventBusResponseTypeDef,
+    CreatePartnerEventSourceResponseTypeDef,
+    DeauthorizeConnectionResponseTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DescribeApiDestinationResponseTypeDef,
+    DescribeArchiveResponseTypeDef,
+    DescribeEventBusResponseTypeDef,
+    DescribeEventSourceResponseTypeDef,
+    DescribePartnerEventSourceResponseTypeDef,
+    DescribeRuleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListApiDestinationsResponseTypeDef,
+    ListArchivesResponseTypeDef,
+    ListRuleNamesByTargetResponseTypeDef,
+    PutRuleResponseTypeDef,
+    StartReplayResponseTypeDef,
+    TestEventPatternResponseTypeDef,
+    UpdateApiDestinationResponseTypeDef,
+    UpdateArchiveResponseTypeDef,
+    UpdateConnectionResponseTypeDef,
     PutPermissionRequestRequestTypeDef,
     ConnectionHttpParametersOutputTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeReplayResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
-    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
+    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
@@ -497,27 +477,26 @@
     SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
-    RoutingConfigOutputTypeDef,
     RoutingConfigTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
+    CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
-    UpdateEndpointResponseTypeDef,
-    CreateEndpointRequestRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
+    UpdateEndpointResponseTypeDef,
     ListTargetsByRuleResponseTypeDef,
     PutTargetsRequestRequestTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.py` & `mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.pyi` & `mypy-boto3-events-1.28.15/mypy_boto3_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/__main__.py` & `mypy-boto3-events-1.28.15/mypy_boto3_events/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridge 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.EventBridge 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
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

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/client.py` & `mypy-boto3-events-1.28.15/mypy_boto3_events/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/client.pyi` & `mypy-boto3-events-1.28.15/mypy_boto3_events/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/literals.py` & `mypy-boto3-events-1.28.15/mypy_boto3_events/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/literals.pyi` & `mypy-boto3-events-1.28.15/mypy_boto3_events/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.py` & `mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         EventBusName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRuleNamesByTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRuleNamesByTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulenamesbytargetpaginator)
         """
 
 
@@ -73,32 +73,28 @@
     """
 
     def paginate(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulespaginator)
         """
 
 
 class ListTargetsByRulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Rule: str,
-        EventBusName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Rule: str, EventBusName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsByRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
         """
```

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.pyi` & `mypy-boto3-events-1.28.15/mypy_boto3_events/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         EventBusName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRuleNamesByTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRuleNamesByTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulenamesbytargetpaginator)
         """
 
 class ListRulesPaginator(Paginator):
@@ -69,31 +69,27 @@
     """
 
     def paginate(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulespaginator)
         """
 
 class ListTargetsByRulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Rule: str,
-        EventBusName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Rule: str, EventBusName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsByRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
         """
```

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.py` & `mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,175 +45,155 @@
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
-    "BatchArrayPropertiesOutputTypeDef",
     "BatchArrayPropertiesTypeDef",
-    "BatchRetryStrategyOutputTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
-    "CancelReplayResponseTypeDef",
-    "CapacityProviderStrategyItemOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
     "ConnectionApiKeyAuthResponseParametersTypeDef",
     "ConnectionBasicAuthResponseParametersTypeDef",
-    "ConnectionBodyParameterOutputTypeDef",
     "ConnectionBodyParameterTypeDef",
-    "ConnectionHeaderParameterOutputTypeDef",
     "ConnectionHeaderParameterTypeDef",
-    "ConnectionQueryStringParameterOutputTypeDef",
     "ConnectionQueryStringParameterTypeDef",
     "ConnectionOAuthClientResponseParametersTypeDef",
     "ConnectionTypeDef",
     "CreateApiDestinationRequestRequestTypeDef",
-    "CreateApiDestinationResponseTypeDef",
     "CreateArchiveRequestRequestTypeDef",
-    "CreateArchiveResponseTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
-    "CreateConnectionResponseTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
-    "EndpointEventBusOutputTypeDef",
-    "ReplicationConfigOutputTypeDef",
     "TagTypeDef",
-    "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
-    "CreatePartnerEventSourceResponseTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
-    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
-    "DeauthorizeConnectionResponseTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
-    "DeleteConnectionResponseTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEventBusRequestRequestTypeDef",
     "DeletePartnerEventSourceRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DescribeApiDestinationRequestRequestTypeDef",
-    "DescribeApiDestinationResponseTypeDef",
     "DescribeArchiveRequestRequestTypeDef",
-    "DescribeArchiveResponseTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
-    "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
-    "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
-    "DescribePartnerEventSourceResponseTypeDef",
     "DescribeReplayRequestRequestTypeDef",
     "ReplayDestinationOutputTypeDef",
     "DescribeRuleRequestRequestTypeDef",
-    "DescribeRuleResponseTypeDef",
     "DisableRuleRequestRequestTypeDef",
-    "PlacementConstraintOutputTypeDef",
-    "PlacementStrategyOutputTypeDef",
-    "TagOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
-    "PrimaryOutputTypeDef",
-    "SecondaryOutputTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
     "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
     "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
-    "KinesisParametersOutputTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
     "ListEventSourcesRequestRequestTypeDef",
     "ListPartnerEventSourceAccountsRequestRequestTypeDef",
     "PartnerEventSourceAccountTypeDef",
     "ListPartnerEventSourcesRequestRequestTypeDef",
     "PartnerEventSourceTypeDef",
     "ListReplaysRequestRequestTypeDef",
     "ReplayTypeDef",
-    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRuleNamesByTargetRequestRequestTypeDef",
-    "ListRuleNamesByTargetResponseTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
-    "PutRuleResponseTypeDef",
     "PutTargetsResultEntryTypeDef",
     "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
     "ReplayDestinationTypeDef",
-    "ResponseMetadataTypeDef",
-    "RetryPolicyOutputTypeDef",
     "RetryPolicyTypeDef",
     "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
-    "SageMakerPipelineParameterOutputTypeDef",
     "SageMakerPipelineParameterTypeDef",
-    "SqsParametersOutputTypeDef",
     "SqsParametersTypeDef",
-    "StartReplayResponseTypeDef",
     "TestEventPatternRequestRequestTypeDef",
-    "TestEventPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
-    "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
-    "UpdateArchiveResponseTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "UpdateConnectionResponseTypeDef",
-    "ListApiDestinationsResponseTypeDef",
-    "ListArchivesResponseTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
-    "BatchParametersOutputTypeDef",
     "BatchParametersTypeDef",
+    "CancelReplayResponseTypeDef",
+    "CreateApiDestinationResponseTypeDef",
+    "CreateArchiveResponseTypeDef",
+    "CreateConnectionResponseTypeDef",
+    "CreateEventBusResponseTypeDef",
+    "CreatePartnerEventSourceResponseTypeDef",
+    "DeauthorizeConnectionResponseTypeDef",
+    "DeleteConnectionResponseTypeDef",
+    "DescribeApiDestinationResponseTypeDef",
+    "DescribeArchiveResponseTypeDef",
+    "DescribeEventBusResponseTypeDef",
+    "DescribeEventSourceResponseTypeDef",
+    "DescribePartnerEventSourceResponseTypeDef",
+    "DescribeRuleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListApiDestinationsResponseTypeDef",
+    "ListArchivesResponseTypeDef",
+    "ListRuleNamesByTargetResponseTypeDef",
+    "PutRuleResponseTypeDef",
+    "StartReplayResponseTypeDef",
+    "TestEventPatternResponseTypeDef",
+    "UpdateApiDestinationResponseTypeDef",
+    "UpdateArchiveResponseTypeDef",
+    "UpdateConnectionResponseTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
-    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
+    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
@@ -223,27 +203,26 @@
     "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
-    "RoutingConfigOutputTypeDef",
     "RoutingConfigTypeDef",
     "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
+    "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
-    "UpdateEndpointResponseTypeDef",
-    "CreateEndpointRequestRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
+    "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
     "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
 )
@@ -326,38 +305,22 @@
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
 
-BatchArrayPropertiesOutputTypeDef = TypedDict(
-    "BatchArrayPropertiesOutputTypeDef",
-    {
-        "Size": int,
-    },
-    total=False,
-)
-
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
-BatchRetryStrategyOutputTypeDef = TypedDict(
-    "BatchRetryStrategyOutputTypeDef",
-    {
-        "Attempts": int,
-    },
-    total=False,
-)
-
 BatchRetryStrategyTypeDef = TypedDict(
     "BatchRetryStrategyTypeDef",
     {
         "Attempts": int,
     },
     total=False,
 )
@@ -365,47 +328,25 @@
 CancelReplayRequestRequestTypeDef = TypedDict(
     "CancelReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-CancelReplayResponseTypeDef = TypedDict(
-    "CancelReplayResponseTypeDef",
-    {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "capacityProvider": str,
-    },
-)
-_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "weight": int,
-        "base": int,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class CapacityProviderStrategyItemOutputTypeDef(
-    _RequiredCapacityProviderStrategyItemOutputTypeDef,
-    _OptionalCapacityProviderStrategyItemOutputTypeDef,
-):
-    pass
-
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -445,64 +386,34 @@
     "ConnectionBasicAuthResponseParametersTypeDef",
     {
         "Username": str,
     },
     total=False,
 )
 
-ConnectionBodyParameterOutputTypeDef = TypedDict(
-    "ConnectionBodyParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "IsValueSecret": bool,
-    },
-    total=False,
-)
-
 ConnectionBodyParameterTypeDef = TypedDict(
     "ConnectionBodyParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
-ConnectionHeaderParameterOutputTypeDef = TypedDict(
-    "ConnectionHeaderParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "IsValueSecret": bool,
-    },
-    total=False,
-)
-
 ConnectionHeaderParameterTypeDef = TypedDict(
     "ConnectionHeaderParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
-ConnectionQueryStringParameterOutputTypeDef = TypedDict(
-    "ConnectionQueryStringParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "IsValueSecret": bool,
-    },
-    total=False,
-)
-
 ConnectionQueryStringParameterTypeDef = TypedDict(
     "ConnectionQueryStringParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
@@ -554,25 +465,14 @@
 class CreateApiDestinationRequestRequestTypeDef(
     _RequiredCreateApiDestinationRequestRequestTypeDef,
     _OptionalCreateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateApiDestinationResponseTypeDef = TypedDict(
-    "CreateApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
         "EventSourceArn": str,
     },
 )
@@ -589,25 +489,14 @@
 
 class CreateArchiveRequestRequestTypeDef(
     _RequiredCreateArchiveRequestRequestTypeDef, _OptionalCreateArchiveRequestRequestTypeDef
 ):
     pass
 
 
-CreateArchiveResponseTypeDef = TypedDict(
-    "CreateArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
 )
@@ -624,25 +513,14 @@
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     {
         "ClientID": str,
         "ClientSecret": str,
     },
 )
 
-CreateConnectionResponseTypeDef = TypedDict(
-    "CreateConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointEventBusTypeDef = TypedDict(
     "EndpointEventBusTypeDef",
     {
         "EventBusArn": str,
     },
 )
 
@@ -650,76 +528,37 @@
     "ReplicationConfigTypeDef",
     {
         "State": ReplicationStateType,
     },
     total=False,
 )
 
-EndpointEventBusOutputTypeDef = TypedDict(
-    "EndpointEventBusOutputTypeDef",
-    {
-        "EventBusArn": str,
-    },
-)
-
-ReplicationConfigOutputTypeDef = TypedDict(
-    "ReplicationConfigOutputTypeDef",
-    {
-        "State": ReplicationStateType,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateEventBusResponseTypeDef = TypedDict(
-    "CreateEventBusResponseTypeDef",
-    {
-        "EventBusArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "CreatePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
         "Account": str,
     },
 )
 
-CreatePartnerEventSourceResponseTypeDef = TypedDict(
-    "CreatePartnerEventSourceResponseTypeDef",
-    {
-        "EventSourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeadLetterConfigOutputTypeDef = TypedDict(
-    "DeadLetterConfigOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -727,26 +566,14 @@
 DeauthorizeConnectionRequestRequestTypeDef = TypedDict(
     "DeauthorizeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeauthorizeConnectionResponseTypeDef = TypedDict(
-    "DeauthorizeConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApiDestinationRequestRequestTypeDef = TypedDict(
     "DeleteApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -760,26 +587,14 @@
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteConnectionResponseTypeDef = TypedDict(
-    "DeleteConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -823,56 +638,21 @@
 DescribeApiDestinationRequestRequestTypeDef = TypedDict(
     "DescribeApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeApiDestinationResponseTypeDef = TypedDict(
-    "DescribeApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "Name": str,
-        "Description": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "ConnectionArn": str,
-        "InvocationEndpoint": str,
-        "HttpMethod": ApiDestinationHttpMethodType,
-        "InvocationRateLimitPerSecond": int,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeArchiveRequestRequestTypeDef = TypedDict(
     "DescribeArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 
-DescribeArchiveResponseTypeDef = TypedDict(
-    "DescribeArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "ArchiveName": str,
-        "EventSourceArn": str,
-        "Description": str,
-        "EventPattern": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "RetentionDays": int,
-        "SizeBytes": int,
-        "EventCount": int,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeConnectionRequestRequestTypeDef = TypedDict(
     "DescribeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -901,60 +681,28 @@
     "DescribeEventBusRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-DescribeEventBusResponseTypeDef = TypedDict(
-    "DescribeEventBusResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEventSourceRequestRequestTypeDef = TypedDict(
     "DescribeEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEventSourceResponseTypeDef = TypedDict(
-    "DescribeEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "CreatedBy": str,
-        "CreationTime": datetime,
-        "ExpirationTime": datetime,
-        "Name": str,
-        "State": EventSourceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "DescribePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribePartnerEventSourceResponseTypeDef = TypedDict(
-    "DescribePartnerEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
@@ -996,31 +744,14 @@
 
 class DescribeRuleRequestRequestTypeDef(
     _RequiredDescribeRuleRequestRequestTypeDef, _OptionalDescribeRuleRequestRequestTypeDef
 ):
     pass
 
 
-DescribeRuleResponseTypeDef = TypedDict(
-    "DescribeRuleResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "EventPattern": str,
-        "ScheduleExpression": str,
-        "State": RuleStateType,
-        "Description": str,
-        "RoleArn": str,
-        "ManagedBy": str,
-        "EventBusName": str,
-        "CreatedBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDisableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDisableRuleRequestRequestTypeDef = TypedDict(
@@ -1034,40 +765,14 @@
 
 class DisableRuleRequestRequestTypeDef(
     _RequiredDisableRuleRequestRequestTypeDef, _OptionalDisableRuleRequestRequestTypeDef
 ):
     pass
 
 
-PlacementConstraintOutputTypeDef = TypedDict(
-    "PlacementConstraintOutputTypeDef",
-    {
-        "type": PlacementConstraintTypeType,
-        "expression": str,
-    },
-    total=False,
-)
-
-PlacementStrategyOutputTypeDef = TypedDict(
-    "PlacementStrategyOutputTypeDef",
-    {
-        "type": PlacementStrategyTypeType,
-        "field": str,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "type": PlacementConstraintTypeType,
         "expression": str,
     },
     total=False,
@@ -1078,21 +783,14 @@
     {
         "type": PlacementStrategyTypeType,
         "field": str,
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
 _RequiredEnableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalEnableRuleRequestRequestTypeDef = TypedDict(
@@ -1129,28 +827,14 @@
         "ExpirationTime": datetime,
         "Name": str,
         "State": EventSourceStateType,
     },
     total=False,
 )
 
-PrimaryOutputTypeDef = TypedDict(
-    "PrimaryOutputTypeDef",
-    {
-        "HealthCheck": str,
-    },
-)
-
-SecondaryOutputTypeDef = TypedDict(
-    "SecondaryOutputTypeDef",
-    {
-        "Route": str,
-    },
-)
-
 PrimaryTypeDef = TypedDict(
     "PrimaryTypeDef",
     {
         "HealthCheck": str,
     },
 )
 
@@ -1217,21 +901,14 @@
 )
 
 
 class InputTransformerTypeDef(_RequiredInputTransformerTypeDef, _OptionalInputTransformerTypeDef):
     pass
 
 
-KinesisParametersOutputTypeDef = TypedDict(
-    "KinesisParametersOutputTypeDef",
-    {
-        "PartitionKeyPath": str,
-    },
-)
-
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKeyPath": str,
     },
 )
 
@@ -1390,37 +1067,24 @@
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
     },
     total=False,
 )
 
-_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    {
-        "TargetArn": str,
-    },
-)
-_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EventBusName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
-    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleNamesByTargetRequestRequestTypeDef",
     {
         "TargetArn": str,
     },
 )
 _OptionalListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
@@ -1437,33 +1101,14 @@
 class ListRuleNamesByTargetRequestRequestTypeDef(
     _RequiredListRuleNamesByTargetRequestRequestTypeDef,
     _OptionalListRuleNamesByTargetRequestRequestTypeDef,
 ):
     pass
 
 
-ListRuleNamesByTargetResponseTypeDef = TypedDict(
-    "ListRuleNamesByTargetResponseTypeDef",
-    {
-        "RuleNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "NamePrefix": str,
-        "EventBusName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NamePrefix": str,
         "EventBusName": str,
         "NextToken": str,
         "Limit": int,
@@ -1490,37 +1135,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "Rule": str,
-    },
-)
-_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "EventBusName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
-    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTargetsByRuleRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsByRuleRequestRequestTypeDef",
     {
         "Rule": str,
     },
 )
 _OptionalListTargetsByRuleRequestRequestTypeDef = TypedDict(
@@ -1536,24 +1158,14 @@
 
 class ListTargetsByRuleRequestRequestTypeDef(
     _RequiredListTargetsByRuleRequestRequestTypeDef, _OptionalListTargetsByRuleRequestRequestTypeDef
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
 PutEventsRequestEntryTypeDef = TypedDict(
     "PutEventsRequestEntryTypeDef",
     {
         "Time": Union[datetime, str],
         "Source": str,
         "Resources": Sequence[str],
         "DetailType": str,
@@ -1592,22 +1204,14 @@
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PutRuleResponseTypeDef = TypedDict(
-    "PutRuleResponseTypeDef",
-    {
-        "RuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutTargetsResultEntryTypeDef = TypedDict(
     "PutTargetsResultEntryTypeDef",
     {
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -1726,34 +1330,14 @@
 
 class ReplayDestinationTypeDef(
     _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
 ):
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
-RetryPolicyOutputTypeDef = TypedDict(
-    "RetryPolicyOutputTypeDef",
-    {
-        "MaximumRetryAttempts": int,
-        "MaximumEventAgeInSeconds": int,
-    },
-    total=False,
-)
-
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
@@ -1771,73 +1355,38 @@
     "RunCommandTargetTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
 
-SageMakerPipelineParameterOutputTypeDef = TypedDict(
-    "SageMakerPipelineParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-SqsParametersOutputTypeDef = TypedDict(
-    "SqsParametersOutputTypeDef",
-    {
-        "MessageGroupId": str,
-    },
-    total=False,
-)
-
 SqsParametersTypeDef = TypedDict(
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
 
-StartReplayResponseTypeDef = TypedDict(
-    "StartReplayResponseTypeDef",
-    {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ReplayStartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TestEventPatternRequestRequestTypeDef = TypedDict(
     "TestEventPatternRequestRequestTypeDef",
     {
         "EventPattern": str,
         "Event": str,
     },
 )
 
-TestEventPatternResponseTypeDef = TypedDict(
-    "TestEventPatternResponseTypeDef",
-    {
-        "Result": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1864,25 +1413,14 @@
 class UpdateApiDestinationRequestRequestTypeDef(
     _RequiredUpdateApiDestinationRequestRequestTypeDef,
     _OptionalUpdateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateApiDestinationResponseTypeDef = TypedDict(
-    "UpdateApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 _OptionalUpdateArchiveRequestRequestTypeDef = TypedDict(
@@ -1898,25 +1436,14 @@
 
 class UpdateArchiveRequestRequestTypeDef(
     _RequiredUpdateArchiveRequestRequestTypeDef, _OptionalUpdateArchiveRequestRequestTypeDef
 ):
     pass
 
 
-UpdateArchiveResponseTypeDef = TypedDict(
-    "UpdateArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
     total=False,
@@ -1936,103 +1463,312 @@
     {
         "ClientID": str,
         "ClientSecret": str,
     },
     total=False,
 )
 
-UpdateConnectionResponseTypeDef = TypedDict(
-    "UpdateConnectionResponseTypeDef",
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+_RequiredBatchParametersTypeDef = TypedDict(
+    "_RequiredBatchParametersTypeDef",
+    {
+        "JobDefinition": str,
+        "JobName": str,
+    },
+)
+_OptionalBatchParametersTypeDef = TypedDict(
+    "_OptionalBatchParametersTypeDef",
+    {
+        "ArrayProperties": BatchArrayPropertiesTypeDef,
+        "RetryStrategy": BatchRetryStrategyTypeDef,
+    },
+    total=False,
+)
+
+
+class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
+    pass
+
+
+CancelReplayResponseTypeDef = TypedDict(
+    "CancelReplayResponseTypeDef",
+    {
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApiDestinationResponseTypeDef = TypedDict(
+    "CreateApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateArchiveResponseTypeDef = TypedDict(
+    "CreateArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectionResponseTypeDef = TypedDict(
+    "CreateConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventBusResponseTypeDef = TypedDict(
+    "CreateEventBusResponseTypeDef",
+    {
+        "EventBusArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePartnerEventSourceResponseTypeDef = TypedDict(
+    "CreatePartnerEventSourceResponseTypeDef",
+    {
+        "EventSourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeauthorizeConnectionResponseTypeDef = TypedDict(
+    "DeauthorizeConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteConnectionResponseTypeDef = TypedDict(
+    "DeleteConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "ConnectionState": ConnectionStateType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApiDestinationResponseTypeDef = TypedDict(
+    "DescribeApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "Name": str,
+        "Description": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "ConnectionArn": str,
+        "InvocationEndpoint": str,
+        "HttpMethod": ApiDestinationHttpMethodType,
+        "InvocationRateLimitPerSecond": int,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeArchiveResponseTypeDef = TypedDict(
+    "DescribeArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "ArchiveName": str,
+        "EventSourceArn": str,
+        "Description": str,
+        "EventPattern": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "RetentionDays": int,
+        "SizeBytes": int,
+        "EventCount": int,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventBusResponseTypeDef = TypedDict(
+    "DescribeEventBusResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventSourceResponseTypeDef = TypedDict(
+    "DescribeEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedBy": str,
+        "CreationTime": datetime,
+        "ExpirationTime": datetime,
+        "Name": str,
+        "State": EventSourceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePartnerEventSourceResponseTypeDef = TypedDict(
+    "DescribePartnerEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRuleResponseTypeDef = TypedDict(
+    "DescribeRuleResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "EventPattern": str,
+        "ScheduleExpression": str,
+        "State": RuleStateType,
+        "Description": str,
+        "RoleArn": str,
+        "ManagedBy": str,
+        "EventBusName": str,
+        "CreatedBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApiDestinationsResponseTypeDef = TypedDict(
     "ListApiDestinationsResponseTypeDef",
     {
         "ApiDestinations": List[ApiDestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListArchivesResponseTypeDef = TypedDict(
     "ListArchivesResponseTypeDef",
     {
         "Archives": List[ArchiveTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
+ListRuleNamesByTargetResponseTypeDef = TypedDict(
+    "ListRuleNamesByTargetResponseTypeDef",
     {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+        "RuleNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
+PutRuleResponseTypeDef = TypedDict(
+    "PutRuleResponseTypeDef",
     {
-        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
+        "RuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredBatchParametersOutputTypeDef = TypedDict(
-    "_RequiredBatchParametersOutputTypeDef",
+StartReplayResponseTypeDef = TypedDict(
+    "StartReplayResponseTypeDef",
     {
-        "JobDefinition": str,
-        "JobName": str,
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ReplayStartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchParametersOutputTypeDef = TypedDict(
-    "_OptionalBatchParametersOutputTypeDef",
+
+TestEventPatternResponseTypeDef = TypedDict(
+    "TestEventPatternResponseTypeDef",
     {
-        "ArrayProperties": BatchArrayPropertiesOutputTypeDef,
-        "RetryStrategy": BatchRetryStrategyOutputTypeDef,
+        "Result": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class BatchParametersOutputTypeDef(
-    _RequiredBatchParametersOutputTypeDef, _OptionalBatchParametersOutputTypeDef
-):
-    pass
-
-
-_RequiredBatchParametersTypeDef = TypedDict(
-    "_RequiredBatchParametersTypeDef",
+UpdateApiDestinationResponseTypeDef = TypedDict(
+    "UpdateApiDestinationResponseTypeDef",
     {
-        "JobDefinition": str,
-        "JobName": str,
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchParametersTypeDef = TypedDict(
-    "_OptionalBatchParametersTypeDef",
+
+UpdateArchiveResponseTypeDef = TypedDict(
+    "UpdateArchiveResponseTypeDef",
     {
-        "ArrayProperties": BatchArrayPropertiesTypeDef,
-        "RetryStrategy": BatchRetryStrategyTypeDef,
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
-    pass
-
+UpdateConnectionResponseTypeDef = TypedDict(
+    "UpdateConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 PutPermissionRequestRequestTypeDef = TypedDict(
     "PutPermissionRequestRequestTypeDef",
     {
         "EventBusName": str,
         "Action": str,
         "Principal": str,
@@ -2042,17 +1778,17 @@
     },
     total=False,
 )
 
 ConnectionHttpParametersOutputTypeDef = TypedDict(
     "ConnectionHttpParametersOutputTypeDef",
     {
-        "HeaderParameters": List[ConnectionHeaderParameterOutputTypeDef],
-        "QueryStringParameters": List[ConnectionQueryStringParameterOutputTypeDef],
-        "BodyParameters": List[ConnectionBodyParameterOutputTypeDef],
+        "HeaderParameters": List[ConnectionHeaderParameterTypeDef],
+        "QueryStringParameters": List[ConnectionQueryStringParameterTypeDef],
+        "BodyParameters": List[ConnectionBodyParameterTypeDef],
     },
     total=False,
 )
 
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
@@ -2064,15 +1800,15 @@
 )
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventBusRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventBusRequestRequestTypeDef",
     {
         "Name": str,
@@ -2090,14 +1826,22 @@
 
 class CreateEventBusRequestRequestTypeDef(
     _RequiredCreateEventBusRequestRequestTypeDef, _OptionalCreateEventBusRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPutRuleRequestRequestTypeDef = TypedDict(
@@ -2140,49 +1884,33 @@
         "EventSourceArn": str,
         "Destination": ReplayDestinationOutputTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
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
 
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSourcesResponseTypeDef = TypedDict(
     "ListEventSourcesResponseTypeDef",
     {
         "EventSources": List[EventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-FailoverConfigOutputTypeDef = TypedDict(
-    "FailoverConfigOutputTypeDef",
-    {
-        "Primary": PrimaryOutputTypeDef,
-        "Secondary": SecondaryOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
@@ -2191,42 +1919,98 @@
 )
 
 ListPartnerEventSourceAccountsResponseTypeDef = TypedDict(
     "ListPartnerEventSourceAccountsResponseTypeDef",
     {
         "PartnerEventSourceAccounts": List[PartnerEventSourceAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartnerEventSourcesResponseTypeDef = TypedDict(
     "ListPartnerEventSourcesResponseTypeDef",
     {
         "PartnerEventSources": List[PartnerEventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReplaysResponseTypeDef = TypedDict(
     "ListReplaysResponseTypeDef",
     {
         "Replays": List[ReplayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    {
+        "TargetArn": str,
+    },
+)
+_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
+    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+):
+    pass
+
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "NamePrefix": str,
+        "EventBusName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "Rule": str,
+    },
+)
+_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
+    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+):
+    pass
+
+
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutEventsRequestEntryTypeDef],
@@ -2248,15 +2032,15 @@
 
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
@@ -2264,33 +2048,33 @@
 )
 
 PutPartnerEventsResponseTypeDef = TypedDict(
     "PutPartnerEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutPartnerEventsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutTargetsResponseTypeDef = TypedDict(
     "PutTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[PutTargetsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveTargetsResponseTypeDef = TypedDict(
     "RemoveTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReplayRequestRequestTypeDef = TypedDict(
     "_RequiredStartReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
@@ -2328,15 +2112,15 @@
         "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
     },
 )
 
 SageMakerPipelineParametersOutputTypeDef = TypedDict(
     "SageMakerPipelineParametersOutputTypeDef",
     {
-        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
+        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
 
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
@@ -2355,22 +2139,22 @@
     "_OptionalEcsParametersOutputTypeDef",
     {
         "TaskCount": int,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
         "PlatformVersion": str,
         "Group": str,
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
-        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
-        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PlacementConstraints": List[PlacementConstraintTypeDef],
+        "PlacementStrategy": List[PlacementStrategyTypeDef],
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 
 class EcsParametersOutputTypeDef(
     _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
@@ -2451,21 +2235,14 @@
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
         "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
-RoutingConfigOutputTypeDef = TypedDict(
-    "RoutingConfigOutputTypeDef",
-    {
-        "FailoverConfig": FailoverConfigOutputTypeDef,
-    },
-)
-
 RoutingConfigTypeDef = TypedDict(
     "RoutingConfigTypeDef",
     {
         "FailoverConfig": FailoverConfigTypeDef,
     },
 )
 
@@ -2479,24 +2256,24 @@
 _OptionalTargetOutputTypeDef = TypedDict(
     "_OptionalTargetOutputTypeDef",
     {
         "RoleArn": str,
         "Input": str,
         "InputPath": str,
         "InputTransformer": InputTransformerOutputTypeDef,
-        "KinesisParameters": KinesisParametersOutputTypeDef,
+        "KinesisParameters": KinesisParametersTypeDef,
         "RunCommandParameters": RunCommandParametersOutputTypeDef,
         "EcsParameters": EcsParametersOutputTypeDef,
-        "BatchParameters": BatchParametersOutputTypeDef,
-        "SqsParameters": SqsParametersOutputTypeDef,
+        "BatchParameters": BatchParametersTypeDef,
+        "SqsParameters": SqsParametersTypeDef,
         "HttpParameters": HttpParametersOutputTypeDef,
         "RedshiftDataParameters": RedshiftDataParametersOutputTypeDef,
         "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
-        "RetryPolicy": RetryPolicyOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "RetryPolicy": RetryPolicyTypeDef,
     },
     total=False,
 )
 
 
 class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
     pass
@@ -2564,109 +2341,93 @@
         "OAuthParameters": UpdateConnectionOAuthRequestParametersTypeDef,
         "ApiKeyAuthParameters": UpdateConnectionApiKeyAuthRequestParametersTypeDef,
         "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEndpointRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoutingConfig": RoutingConfigTypeDef,
+        "EventBuses": Sequence[EndpointEventBusTypeDef],
+    },
+)
+_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEndpointRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "RoleArn": str,
+    },
+    total=False,
+)
+
+
+class CreateEndpointRequestRequestTypeDef(
+    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
+):
+    pass
+
+
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "State": EndpointStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
-        "RoleArn": str,
-        "EndpointId": str,
-        "EndpointUrl": str,
-        "State": EndpointStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEndpointRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "EventBuses": Sequence[EndpointEventBusTypeDef],
-    },
-)
-_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEndpointRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-
-class CreateEndpointRequestRequestTypeDef(
-    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
@@ -2684,20 +2445,36 @@
 
 class UpdateEndpointRequestRequestTypeDef(
     _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
 
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoleArn": str,
+        "EndpointId": str,
+        "EndpointUrl": str,
+        "State": EndpointStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
         "Targets": List[TargetOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
     {
         "Rule": str,
@@ -2729,15 +2506,15 @@
         "StateReason": str,
         "AuthorizationType": ConnectionAuthorizationTypeType,
         "SecretArn": str,
         "AuthParameters": ConnectionAuthResponseParametersTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "Name": str,
@@ -2784,10 +2561,10 @@
 
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.pyi` & `mypy-boto3-events-1.28.15/mypy_boto3_events/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -44,175 +44,155 @@
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
-    "BatchArrayPropertiesOutputTypeDef",
     "BatchArrayPropertiesTypeDef",
-    "BatchRetryStrategyOutputTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
-    "CancelReplayResponseTypeDef",
-    "CapacityProviderStrategyItemOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
     "ConnectionApiKeyAuthResponseParametersTypeDef",
     "ConnectionBasicAuthResponseParametersTypeDef",
-    "ConnectionBodyParameterOutputTypeDef",
     "ConnectionBodyParameterTypeDef",
-    "ConnectionHeaderParameterOutputTypeDef",
     "ConnectionHeaderParameterTypeDef",
-    "ConnectionQueryStringParameterOutputTypeDef",
     "ConnectionQueryStringParameterTypeDef",
     "ConnectionOAuthClientResponseParametersTypeDef",
     "ConnectionTypeDef",
     "CreateApiDestinationRequestRequestTypeDef",
-    "CreateApiDestinationResponseTypeDef",
     "CreateArchiveRequestRequestTypeDef",
-    "CreateArchiveResponseTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
-    "CreateConnectionResponseTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
-    "EndpointEventBusOutputTypeDef",
-    "ReplicationConfigOutputTypeDef",
     "TagTypeDef",
-    "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
-    "CreatePartnerEventSourceResponseTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
-    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
-    "DeauthorizeConnectionResponseTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
-    "DeleteConnectionResponseTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEventBusRequestRequestTypeDef",
     "DeletePartnerEventSourceRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DescribeApiDestinationRequestRequestTypeDef",
-    "DescribeApiDestinationResponseTypeDef",
     "DescribeArchiveRequestRequestTypeDef",
-    "DescribeArchiveResponseTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
-    "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
-    "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
-    "DescribePartnerEventSourceResponseTypeDef",
     "DescribeReplayRequestRequestTypeDef",
     "ReplayDestinationOutputTypeDef",
     "DescribeRuleRequestRequestTypeDef",
-    "DescribeRuleResponseTypeDef",
     "DisableRuleRequestRequestTypeDef",
-    "PlacementConstraintOutputTypeDef",
-    "PlacementStrategyOutputTypeDef",
-    "TagOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
-    "PrimaryOutputTypeDef",
-    "SecondaryOutputTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
     "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
     "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
-    "KinesisParametersOutputTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
     "ListEventSourcesRequestRequestTypeDef",
     "ListPartnerEventSourceAccountsRequestRequestTypeDef",
     "PartnerEventSourceAccountTypeDef",
     "ListPartnerEventSourcesRequestRequestTypeDef",
     "PartnerEventSourceTypeDef",
     "ListReplaysRequestRequestTypeDef",
     "ReplayTypeDef",
-    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRuleNamesByTargetRequestRequestTypeDef",
-    "ListRuleNamesByTargetResponseTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
-    "PutRuleResponseTypeDef",
     "PutTargetsResultEntryTypeDef",
     "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
     "ReplayDestinationTypeDef",
-    "ResponseMetadataTypeDef",
-    "RetryPolicyOutputTypeDef",
     "RetryPolicyTypeDef",
     "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
-    "SageMakerPipelineParameterOutputTypeDef",
     "SageMakerPipelineParameterTypeDef",
-    "SqsParametersOutputTypeDef",
     "SqsParametersTypeDef",
-    "StartReplayResponseTypeDef",
     "TestEventPatternRequestRequestTypeDef",
-    "TestEventPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
-    "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
-    "UpdateArchiveResponseTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "UpdateConnectionResponseTypeDef",
-    "ListApiDestinationsResponseTypeDef",
-    "ListArchivesResponseTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
-    "BatchParametersOutputTypeDef",
     "BatchParametersTypeDef",
+    "CancelReplayResponseTypeDef",
+    "CreateApiDestinationResponseTypeDef",
+    "CreateArchiveResponseTypeDef",
+    "CreateConnectionResponseTypeDef",
+    "CreateEventBusResponseTypeDef",
+    "CreatePartnerEventSourceResponseTypeDef",
+    "DeauthorizeConnectionResponseTypeDef",
+    "DeleteConnectionResponseTypeDef",
+    "DescribeApiDestinationResponseTypeDef",
+    "DescribeArchiveResponseTypeDef",
+    "DescribeEventBusResponseTypeDef",
+    "DescribeEventSourceResponseTypeDef",
+    "DescribePartnerEventSourceResponseTypeDef",
+    "DescribeRuleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListApiDestinationsResponseTypeDef",
+    "ListArchivesResponseTypeDef",
+    "ListRuleNamesByTargetResponseTypeDef",
+    "PutRuleResponseTypeDef",
+    "StartReplayResponseTypeDef",
+    "TestEventPatternResponseTypeDef",
+    "UpdateApiDestinationResponseTypeDef",
+    "UpdateArchiveResponseTypeDef",
+    "UpdateConnectionResponseTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
-    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
+    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
@@ -222,27 +202,26 @@
     "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
-    "RoutingConfigOutputTypeDef",
     "RoutingConfigTypeDef",
     "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
+    "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
-    "UpdateEndpointResponseTypeDef",
-    "CreateEndpointRequestRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
+    "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
     "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
 )
@@ -321,38 +300,22 @@
 )
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
-BatchArrayPropertiesOutputTypeDef = TypedDict(
-    "BatchArrayPropertiesOutputTypeDef",
-    {
-        "Size": int,
-    },
-    total=False,
-)
-
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
-BatchRetryStrategyOutputTypeDef = TypedDict(
-    "BatchRetryStrategyOutputTypeDef",
-    {
-        "Attempts": int,
-    },
-    total=False,
-)
-
 BatchRetryStrategyTypeDef = TypedDict(
     "BatchRetryStrategyTypeDef",
     {
         "Attempts": int,
     },
     total=False,
 )
@@ -360,45 +323,25 @@
 CancelReplayRequestRequestTypeDef = TypedDict(
     "CancelReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-CancelReplayResponseTypeDef = TypedDict(
-    "CancelReplayResponseTypeDef",
-    {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "capacityProvider": str,
-    },
-)
-_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "weight": int,
-        "base": int,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class CapacityProviderStrategyItemOutputTypeDef(
-    _RequiredCapacityProviderStrategyItemOutputTypeDef,
-    _OptionalCapacityProviderStrategyItemOutputTypeDef,
-):
-    pass
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -436,64 +379,34 @@
     "ConnectionBasicAuthResponseParametersTypeDef",
     {
         "Username": str,
     },
     total=False,
 )
 
-ConnectionBodyParameterOutputTypeDef = TypedDict(
-    "ConnectionBodyParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "IsValueSecret": bool,
-    },
-    total=False,
-)
-
 ConnectionBodyParameterTypeDef = TypedDict(
     "ConnectionBodyParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
-ConnectionHeaderParameterOutputTypeDef = TypedDict(
-    "ConnectionHeaderParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "IsValueSecret": bool,
-    },
-    total=False,
-)
-
 ConnectionHeaderParameterTypeDef = TypedDict(
     "ConnectionHeaderParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
-ConnectionQueryStringParameterOutputTypeDef = TypedDict(
-    "ConnectionQueryStringParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "IsValueSecret": bool,
-    },
-    total=False,
-)
-
 ConnectionQueryStringParameterTypeDef = TypedDict(
     "ConnectionQueryStringParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
@@ -543,25 +456,14 @@
 
 class CreateApiDestinationRequestRequestTypeDef(
     _RequiredCreateApiDestinationRequestRequestTypeDef,
     _OptionalCreateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
-CreateApiDestinationResponseTypeDef = TypedDict(
-    "CreateApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
         "EventSourceArn": str,
     },
 )
@@ -576,25 +478,14 @@
 )
 
 class CreateArchiveRequestRequestTypeDef(
     _RequiredCreateArchiveRequestRequestTypeDef, _OptionalCreateArchiveRequestRequestTypeDef
 ):
     pass
 
-CreateArchiveResponseTypeDef = TypedDict(
-    "CreateArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
 )
@@ -611,25 +502,14 @@
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     {
         "ClientID": str,
         "ClientSecret": str,
     },
 )
 
-CreateConnectionResponseTypeDef = TypedDict(
-    "CreateConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointEventBusTypeDef = TypedDict(
     "EndpointEventBusTypeDef",
     {
         "EventBusArn": str,
     },
 )
 
@@ -637,76 +517,37 @@
     "ReplicationConfigTypeDef",
     {
         "State": ReplicationStateType,
     },
     total=False,
 )
 
-EndpointEventBusOutputTypeDef = TypedDict(
-    "EndpointEventBusOutputTypeDef",
-    {
-        "EventBusArn": str,
-    },
-)
-
-ReplicationConfigOutputTypeDef = TypedDict(
-    "ReplicationConfigOutputTypeDef",
-    {
-        "State": ReplicationStateType,
-    },
-    total=False,
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateEventBusResponseTypeDef = TypedDict(
-    "CreateEventBusResponseTypeDef",
-    {
-        "EventBusArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "CreatePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
         "Account": str,
     },
 )
 
-CreatePartnerEventSourceResponseTypeDef = TypedDict(
-    "CreatePartnerEventSourceResponseTypeDef",
-    {
-        "EventSourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeadLetterConfigOutputTypeDef = TypedDict(
-    "DeadLetterConfigOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -714,26 +555,14 @@
 DeauthorizeConnectionRequestRequestTypeDef = TypedDict(
     "DeauthorizeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeauthorizeConnectionResponseTypeDef = TypedDict(
-    "DeauthorizeConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApiDestinationRequestRequestTypeDef = TypedDict(
     "DeleteApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -747,26 +576,14 @@
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteConnectionResponseTypeDef = TypedDict(
-    "DeleteConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -808,56 +625,21 @@
 DescribeApiDestinationRequestRequestTypeDef = TypedDict(
     "DescribeApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeApiDestinationResponseTypeDef = TypedDict(
-    "DescribeApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "Name": str,
-        "Description": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "ConnectionArn": str,
-        "InvocationEndpoint": str,
-        "HttpMethod": ApiDestinationHttpMethodType,
-        "InvocationRateLimitPerSecond": int,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeArchiveRequestRequestTypeDef = TypedDict(
     "DescribeArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 
-DescribeArchiveResponseTypeDef = TypedDict(
-    "DescribeArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "ArchiveName": str,
-        "EventSourceArn": str,
-        "Description": str,
-        "EventPattern": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "RetentionDays": int,
-        "SizeBytes": int,
-        "EventCount": int,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeConnectionRequestRequestTypeDef = TypedDict(
     "DescribeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -884,60 +666,28 @@
     "DescribeEventBusRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-DescribeEventBusResponseTypeDef = TypedDict(
-    "DescribeEventBusResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEventSourceRequestRequestTypeDef = TypedDict(
     "DescribeEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEventSourceResponseTypeDef = TypedDict(
-    "DescribeEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "CreatedBy": str,
-        "CreationTime": datetime,
-        "ExpirationTime": datetime,
-        "Name": str,
-        "State": EventSourceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "DescribePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribePartnerEventSourceResponseTypeDef = TypedDict(
-    "DescribePartnerEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
@@ -975,31 +725,14 @@
 )
 
 class DescribeRuleRequestRequestTypeDef(
     _RequiredDescribeRuleRequestRequestTypeDef, _OptionalDescribeRuleRequestRequestTypeDef
 ):
     pass
 
-DescribeRuleResponseTypeDef = TypedDict(
-    "DescribeRuleResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "EventPattern": str,
-        "ScheduleExpression": str,
-        "State": RuleStateType,
-        "Description": str,
-        "RoleArn": str,
-        "ManagedBy": str,
-        "EventBusName": str,
-        "CreatedBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDisableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDisableRuleRequestRequestTypeDef = TypedDict(
@@ -1011,40 +744,14 @@
 )
 
 class DisableRuleRequestRequestTypeDef(
     _RequiredDisableRuleRequestRequestTypeDef, _OptionalDisableRuleRequestRequestTypeDef
 ):
     pass
 
-PlacementConstraintOutputTypeDef = TypedDict(
-    "PlacementConstraintOutputTypeDef",
-    {
-        "type": PlacementConstraintTypeType,
-        "expression": str,
-    },
-    total=False,
-)
-
-PlacementStrategyOutputTypeDef = TypedDict(
-    "PlacementStrategyOutputTypeDef",
-    {
-        "type": PlacementStrategyTypeType,
-        "field": str,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "type": PlacementConstraintTypeType,
         "expression": str,
     },
     total=False,
@@ -1055,21 +762,14 @@
     {
         "type": PlacementStrategyTypeType,
         "field": str,
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
 _RequiredEnableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalEnableRuleRequestRequestTypeDef = TypedDict(
@@ -1104,28 +804,14 @@
         "ExpirationTime": datetime,
         "Name": str,
         "State": EventSourceStateType,
     },
     total=False,
 )
 
-PrimaryOutputTypeDef = TypedDict(
-    "PrimaryOutputTypeDef",
-    {
-        "HealthCheck": str,
-    },
-)
-
-SecondaryOutputTypeDef = TypedDict(
-    "SecondaryOutputTypeDef",
-    {
-        "Route": str,
-    },
-)
-
 PrimaryTypeDef = TypedDict(
     "PrimaryTypeDef",
     {
         "HealthCheck": str,
     },
 )
 
@@ -1188,21 +874,14 @@
     },
     total=False,
 )
 
 class InputTransformerTypeDef(_RequiredInputTransformerTypeDef, _OptionalInputTransformerTypeDef):
     pass
 
-KinesisParametersOutputTypeDef = TypedDict(
-    "KinesisParametersOutputTypeDef",
-    {
-        "PartitionKeyPath": str,
-    },
-)
-
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKeyPath": str,
     },
 )
 
@@ -1357,35 +1036,24 @@
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
     },
     total=False,
 )
 
-_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    {
-        "TargetArn": str,
-    },
-)
-_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EventBusName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
-    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-):
-    pass
-
 _RequiredListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleNamesByTargetRequestRequestTypeDef",
     {
         "TargetArn": str,
     },
 )
 _OptionalListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
@@ -1400,33 +1068,14 @@
 
 class ListRuleNamesByTargetRequestRequestTypeDef(
     _RequiredListRuleNamesByTargetRequestRequestTypeDef,
     _OptionalListRuleNamesByTargetRequestRequestTypeDef,
 ):
     pass
 
-ListRuleNamesByTargetResponseTypeDef = TypedDict(
-    "ListRuleNamesByTargetResponseTypeDef",
-    {
-        "RuleNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "NamePrefix": str,
-        "EventBusName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NamePrefix": str,
         "EventBusName": str,
         "NextToken": str,
         "Limit": int,
@@ -1453,35 +1102,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "Rule": str,
-    },
-)
-_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "EventBusName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
-    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-):
-    pass
-
 _RequiredListTargetsByRuleRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsByRuleRequestRequestTypeDef",
     {
         "Rule": str,
     },
 )
 _OptionalListTargetsByRuleRequestRequestTypeDef = TypedDict(
@@ -1495,24 +1123,14 @@
 )
 
 class ListTargetsByRuleRequestRequestTypeDef(
     _RequiredListTargetsByRuleRequestRequestTypeDef, _OptionalListTargetsByRuleRequestRequestTypeDef
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
 PutEventsRequestEntryTypeDef = TypedDict(
     "PutEventsRequestEntryTypeDef",
     {
         "Time": Union[datetime, str],
         "Source": str,
         "Resources": Sequence[str],
         "DetailType": str,
@@ -1551,22 +1169,14 @@
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PutRuleResponseTypeDef = TypedDict(
-    "PutRuleResponseTypeDef",
-    {
-        "RuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutTargetsResultEntryTypeDef = TypedDict(
     "PutTargetsResultEntryTypeDef",
     {
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -1677,34 +1287,14 @@
 )
 
 class ReplayDestinationTypeDef(
     _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
 ):
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
-RetryPolicyOutputTypeDef = TypedDict(
-    "RetryPolicyOutputTypeDef",
-    {
-        "MaximumRetryAttempts": int,
-        "MaximumEventAgeInSeconds": int,
-    },
-    total=False,
-)
-
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
@@ -1722,73 +1312,38 @@
     "RunCommandTargetTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
 
-SageMakerPipelineParameterOutputTypeDef = TypedDict(
-    "SageMakerPipelineParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-SqsParametersOutputTypeDef = TypedDict(
-    "SqsParametersOutputTypeDef",
-    {
-        "MessageGroupId": str,
-    },
-    total=False,
-)
-
 SqsParametersTypeDef = TypedDict(
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
 
-StartReplayResponseTypeDef = TypedDict(
-    "StartReplayResponseTypeDef",
-    {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ReplayStartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TestEventPatternRequestRequestTypeDef = TypedDict(
     "TestEventPatternRequestRequestTypeDef",
     {
         "EventPattern": str,
         "Event": str,
     },
 )
 
-TestEventPatternResponseTypeDef = TypedDict(
-    "TestEventPatternResponseTypeDef",
-    {
-        "Result": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1813,25 +1368,14 @@
 
 class UpdateApiDestinationRequestRequestTypeDef(
     _RequiredUpdateApiDestinationRequestRequestTypeDef,
     _OptionalUpdateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
-UpdateApiDestinationResponseTypeDef = TypedDict(
-    "UpdateApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 _OptionalUpdateArchiveRequestRequestTypeDef = TypedDict(
@@ -1845,25 +1389,14 @@
 )
 
 class UpdateArchiveRequestRequestTypeDef(
     _RequiredUpdateArchiveRequestRequestTypeDef, _OptionalUpdateArchiveRequestRequestTypeDef
 ):
     pass
 
-UpdateArchiveResponseTypeDef = TypedDict(
-    "UpdateArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
     total=False,
@@ -1883,99 +1416,310 @@
     {
         "ClientID": str,
         "ClientSecret": str,
     },
     total=False,
 )
 
-UpdateConnectionResponseTypeDef = TypedDict(
-    "UpdateConnectionResponseTypeDef",
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+_RequiredBatchParametersTypeDef = TypedDict(
+    "_RequiredBatchParametersTypeDef",
+    {
+        "JobDefinition": str,
+        "JobName": str,
+    },
+)
+_OptionalBatchParametersTypeDef = TypedDict(
+    "_OptionalBatchParametersTypeDef",
+    {
+        "ArrayProperties": BatchArrayPropertiesTypeDef,
+        "RetryStrategy": BatchRetryStrategyTypeDef,
+    },
+    total=False,
+)
+
+class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
+    pass
+
+CancelReplayResponseTypeDef = TypedDict(
+    "CancelReplayResponseTypeDef",
+    {
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApiDestinationResponseTypeDef = TypedDict(
+    "CreateApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateArchiveResponseTypeDef = TypedDict(
+    "CreateArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectionResponseTypeDef = TypedDict(
+    "CreateConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventBusResponseTypeDef = TypedDict(
+    "CreateEventBusResponseTypeDef",
+    {
+        "EventBusArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePartnerEventSourceResponseTypeDef = TypedDict(
+    "CreatePartnerEventSourceResponseTypeDef",
+    {
+        "EventSourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeauthorizeConnectionResponseTypeDef = TypedDict(
+    "DeauthorizeConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteConnectionResponseTypeDef = TypedDict(
+    "DeleteConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "ConnectionState": ConnectionStateType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApiDestinationResponseTypeDef = TypedDict(
+    "DescribeApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "Name": str,
+        "Description": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "ConnectionArn": str,
+        "InvocationEndpoint": str,
+        "HttpMethod": ApiDestinationHttpMethodType,
+        "InvocationRateLimitPerSecond": int,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeArchiveResponseTypeDef = TypedDict(
+    "DescribeArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "ArchiveName": str,
+        "EventSourceArn": str,
+        "Description": str,
+        "EventPattern": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "RetentionDays": int,
+        "SizeBytes": int,
+        "EventCount": int,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventBusResponseTypeDef = TypedDict(
+    "DescribeEventBusResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventSourceResponseTypeDef = TypedDict(
+    "DescribeEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedBy": str,
+        "CreationTime": datetime,
+        "ExpirationTime": datetime,
+        "Name": str,
+        "State": EventSourceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePartnerEventSourceResponseTypeDef = TypedDict(
+    "DescribePartnerEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRuleResponseTypeDef = TypedDict(
+    "DescribeRuleResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "EventPattern": str,
+        "ScheduleExpression": str,
+        "State": RuleStateType,
+        "Description": str,
+        "RoleArn": str,
+        "ManagedBy": str,
+        "EventBusName": str,
+        "CreatedBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApiDestinationsResponseTypeDef = TypedDict(
     "ListApiDestinationsResponseTypeDef",
     {
         "ApiDestinations": List[ApiDestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListArchivesResponseTypeDef = TypedDict(
     "ListArchivesResponseTypeDef",
     {
         "Archives": List[ArchiveTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
+ListRuleNamesByTargetResponseTypeDef = TypedDict(
+    "ListRuleNamesByTargetResponseTypeDef",
     {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+        "RuleNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
+PutRuleResponseTypeDef = TypedDict(
+    "PutRuleResponseTypeDef",
     {
-        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
+        "RuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredBatchParametersOutputTypeDef = TypedDict(
-    "_RequiredBatchParametersOutputTypeDef",
+StartReplayResponseTypeDef = TypedDict(
+    "StartReplayResponseTypeDef",
     {
-        "JobDefinition": str,
-        "JobName": str,
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ReplayStartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchParametersOutputTypeDef = TypedDict(
-    "_OptionalBatchParametersOutputTypeDef",
+
+TestEventPatternResponseTypeDef = TypedDict(
+    "TestEventPatternResponseTypeDef",
     {
-        "ArrayProperties": BatchArrayPropertiesOutputTypeDef,
-        "RetryStrategy": BatchRetryStrategyOutputTypeDef,
+        "Result": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class BatchParametersOutputTypeDef(
-    _RequiredBatchParametersOutputTypeDef, _OptionalBatchParametersOutputTypeDef
-):
-    pass
-
-_RequiredBatchParametersTypeDef = TypedDict(
-    "_RequiredBatchParametersTypeDef",
+UpdateApiDestinationResponseTypeDef = TypedDict(
+    "UpdateApiDestinationResponseTypeDef",
     {
-        "JobDefinition": str,
-        "JobName": str,
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchParametersTypeDef = TypedDict(
-    "_OptionalBatchParametersTypeDef",
+
+UpdateArchiveResponseTypeDef = TypedDict(
+    "UpdateArchiveResponseTypeDef",
     {
-        "ArrayProperties": BatchArrayPropertiesTypeDef,
-        "RetryStrategy": BatchRetryStrategyTypeDef,
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
-    pass
+UpdateConnectionResponseTypeDef = TypedDict(
+    "UpdateConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 PutPermissionRequestRequestTypeDef = TypedDict(
     "PutPermissionRequestRequestTypeDef",
     {
         "EventBusName": str,
         "Action": str,
         "Principal": str,
@@ -1985,17 +1729,17 @@
     },
     total=False,
 )
 
 ConnectionHttpParametersOutputTypeDef = TypedDict(
     "ConnectionHttpParametersOutputTypeDef",
     {
-        "HeaderParameters": List[ConnectionHeaderParameterOutputTypeDef],
-        "QueryStringParameters": List[ConnectionQueryStringParameterOutputTypeDef],
-        "BodyParameters": List[ConnectionBodyParameterOutputTypeDef],
+        "HeaderParameters": List[ConnectionHeaderParameterTypeDef],
+        "QueryStringParameters": List[ConnectionQueryStringParameterTypeDef],
+        "BodyParameters": List[ConnectionBodyParameterTypeDef],
     },
     total=False,
 )
 
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
@@ -2007,15 +1751,15 @@
 )
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventBusRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventBusRequestRequestTypeDef",
     {
         "Name": str,
@@ -2031,14 +1775,22 @@
 )
 
 class CreateEventBusRequestRequestTypeDef(
     _RequiredCreateEventBusRequestRequestTypeDef, _OptionalCreateEventBusRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPutRuleRequestRequestTypeDef = TypedDict(
@@ -2079,49 +1831,33 @@
         "EventSourceArn": str,
         "Destination": ReplayDestinationOutputTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
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
 
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSourcesResponseTypeDef = TypedDict(
     "ListEventSourcesResponseTypeDef",
     {
         "EventSources": List[EventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-FailoverConfigOutputTypeDef = TypedDict(
-    "FailoverConfigOutputTypeDef",
-    {
-        "Primary": PrimaryOutputTypeDef,
-        "Secondary": SecondaryOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
@@ -2130,42 +1866,94 @@
 )
 
 ListPartnerEventSourceAccountsResponseTypeDef = TypedDict(
     "ListPartnerEventSourceAccountsResponseTypeDef",
     {
         "PartnerEventSourceAccounts": List[PartnerEventSourceAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartnerEventSourcesResponseTypeDef = TypedDict(
     "ListPartnerEventSourcesResponseTypeDef",
     {
         "PartnerEventSources": List[PartnerEventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReplaysResponseTypeDef = TypedDict(
     "ListReplaysResponseTypeDef",
     {
         "Replays": List[ReplayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    {
+        "TargetArn": str,
+    },
+)
+_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
+    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+):
+    pass
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "NamePrefix": str,
+        "EventBusName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "Rule": str,
+    },
+)
+_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
+    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+):
+    pass
+
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutEventsRequestEntryTypeDef],
@@ -2185,15 +1973,15 @@
     pass
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
@@ -2201,33 +1989,33 @@
 )
 
 PutPartnerEventsResponseTypeDef = TypedDict(
     "PutPartnerEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutPartnerEventsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutTargetsResponseTypeDef = TypedDict(
     "PutTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[PutTargetsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveTargetsResponseTypeDef = TypedDict(
     "RemoveTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReplayRequestRequestTypeDef = TypedDict(
     "_RequiredStartReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
@@ -2263,15 +2051,15 @@
         "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
     },
 )
 
 SageMakerPipelineParametersOutputTypeDef = TypedDict(
     "SageMakerPipelineParametersOutputTypeDef",
     {
-        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
+        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
 
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
@@ -2290,22 +2078,22 @@
     "_OptionalEcsParametersOutputTypeDef",
     {
         "TaskCount": int,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
         "PlatformVersion": str,
         "Group": str,
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
-        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
-        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PlacementConstraints": List[PlacementConstraintTypeDef],
+        "PlacementStrategy": List[PlacementStrategyTypeDef],
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 class EcsParametersOutputTypeDef(
     _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
 ):
@@ -2380,21 +2168,14 @@
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
         "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
-RoutingConfigOutputTypeDef = TypedDict(
-    "RoutingConfigOutputTypeDef",
-    {
-        "FailoverConfig": FailoverConfigOutputTypeDef,
-    },
-)
-
 RoutingConfigTypeDef = TypedDict(
     "RoutingConfigTypeDef",
     {
         "FailoverConfig": FailoverConfigTypeDef,
     },
 )
 
@@ -2408,24 +2189,24 @@
 _OptionalTargetOutputTypeDef = TypedDict(
     "_OptionalTargetOutputTypeDef",
     {
         "RoleArn": str,
         "Input": str,
         "InputPath": str,
         "InputTransformer": InputTransformerOutputTypeDef,
-        "KinesisParameters": KinesisParametersOutputTypeDef,
+        "KinesisParameters": KinesisParametersTypeDef,
         "RunCommandParameters": RunCommandParametersOutputTypeDef,
         "EcsParameters": EcsParametersOutputTypeDef,
-        "BatchParameters": BatchParametersOutputTypeDef,
-        "SqsParameters": SqsParametersOutputTypeDef,
+        "BatchParameters": BatchParametersTypeDef,
+        "SqsParameters": SqsParametersTypeDef,
         "HttpParameters": HttpParametersOutputTypeDef,
         "RedshiftDataParameters": RedshiftDataParametersOutputTypeDef,
         "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
-        "RetryPolicy": RetryPolicyOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "RetryPolicy": RetryPolicyTypeDef,
     },
     total=False,
 )
 
 class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
     pass
 
@@ -2489,107 +2270,91 @@
         "OAuthParameters": UpdateConnectionOAuthRequestParametersTypeDef,
         "ApiKeyAuthParameters": UpdateConnectionApiKeyAuthRequestParametersTypeDef,
         "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEndpointRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoutingConfig": RoutingConfigTypeDef,
+        "EventBuses": Sequence[EndpointEventBusTypeDef],
+    },
+)
+_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEndpointRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "RoleArn": str,
+    },
+    total=False,
+)
+
+class CreateEndpointRequestRequestTypeDef(
+    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
+):
+    pass
+
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "State": EndpointStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "RoutingConfig": RoutingConfigOutputTypeDef,
-        "ReplicationConfig": ReplicationConfigOutputTypeDef,
-        "EventBuses": List[EndpointEventBusOutputTypeDef],
-        "RoleArn": str,
-        "EndpointId": str,
-        "EndpointUrl": str,
-        "State": EndpointStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEndpointRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "EventBuses": Sequence[EndpointEventBusTypeDef],
-    },
-)
-_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEndpointRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-class CreateEndpointRequestRequestTypeDef(
-    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
@@ -2605,20 +2370,36 @@
 )
 
 class UpdateEndpointRequestRequestTypeDef(
     _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
 ):
     pass
 
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "RoutingConfig": RoutingConfigTypeDef,
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoleArn": str,
+        "EndpointId": str,
+        "EndpointUrl": str,
+        "State": EndpointStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
         "Targets": List[TargetOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
     {
         "Rule": str,
@@ -2648,15 +2429,15 @@
         "StateReason": str,
         "AuthorizationType": ConnectionAuthorizationTypeType,
         "SecretArn": str,
         "AuthParameters": ConnectionAuthResponseParametersTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "Name": str,
@@ -2699,10 +2480,10 @@
     pass
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/PKG-INFO` & `mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.12
-Summary: Type annotations for boto3.EventBridge 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,175 +351,155 @@
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
-    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
-    CancelReplayResponseTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
+    ResponseMetadataTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
-    ConnectionBodyParameterOutputTypeDef,
     ConnectionBodyParameterTypeDef,
-    ConnectionHeaderParameterOutputTypeDef,
     ConnectionHeaderParameterTypeDef,
-    ConnectionQueryStringParameterOutputTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
-    CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
-    CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
-    CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
-    EndpointEventBusOutputTypeDef,
-    ReplicationConfigOutputTypeDef,
     TagTypeDef,
-    CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
-    CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
-    DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
-    DeleteConnectionResponseTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEventBusRequestRequestTypeDef,
     DeletePartnerEventSourceRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DescribeApiDestinationRequestRequestTypeDef,
-    DescribeApiDestinationResponseTypeDef,
     DescribeArchiveRequestRequestTypeDef,
-    DescribeArchiveResponseTypeDef,
     DescribeConnectionRequestRequestTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEventBusRequestRequestTypeDef,
-    DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
-    DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
-    DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
     ReplayDestinationOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
-    DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
-    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
-    PrimaryOutputTypeDef,
-    SecondaryOutputTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
     HttpParametersOutputTypeDef,
     HttpParametersTypeDef,
     InputTransformerOutputTypeDef,
     InputTransformerTypeDef,
-    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
     ListApiDestinationsRequestRequestTypeDef,
     ListArchivesRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEventBusesRequestRequestTypeDef,
     ListEventSourcesRequestRequestTypeDef,
     ListPartnerEventSourceAccountsRequestRequestTypeDef,
     PartnerEventSourceAccountTypeDef,
     ListPartnerEventSourcesRequestRequestTypeDef,
     PartnerEventSourceTypeDef,
     ListReplaysRequestRequestTypeDef,
     ReplayTypeDef,
-    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
-    ListRuleNamesByTargetResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
-    PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
     ReplayDestinationTypeDef,
-    ResponseMetadataTypeDef,
-    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
     RunCommandTargetOutputTypeDef,
     RunCommandTargetTypeDef,
-    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
-    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
-    StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
-    TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
-    UpdateApiDestinationResponseTypeDef,
     UpdateArchiveRequestRequestTypeDef,
-    UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
-    UpdateConnectionResponseTypeDef,
-    ListApiDestinationsResponseTypeDef,
-    ListArchivesResponseTypeDef,
     NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
-    BatchParametersOutputTypeDef,
     BatchParametersTypeDef,
+    CancelReplayResponseTypeDef,
+    CreateApiDestinationResponseTypeDef,
+    CreateArchiveResponseTypeDef,
+    CreateConnectionResponseTypeDef,
+    CreateEventBusResponseTypeDef,
+    CreatePartnerEventSourceResponseTypeDef,
+    DeauthorizeConnectionResponseTypeDef,
+    DeleteConnectionResponseTypeDef,
+    DescribeApiDestinationResponseTypeDef,
+    DescribeArchiveResponseTypeDef,
+    DescribeEventBusResponseTypeDef,
+    DescribeEventSourceResponseTypeDef,
+    DescribePartnerEventSourceResponseTypeDef,
+    DescribeRuleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListApiDestinationsResponseTypeDef,
+    ListArchivesResponseTypeDef,
+    ListRuleNamesByTargetResponseTypeDef,
+    PutRuleResponseTypeDef,
+    StartReplayResponseTypeDef,
+    TestEventPatternResponseTypeDef,
+    UpdateApiDestinationResponseTypeDef,
+    UpdateArchiveResponseTypeDef,
+    UpdateConnectionResponseTypeDef,
     PutPermissionRequestRequestTypeDef,
     ConnectionHttpParametersOutputTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeReplayResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
-    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
+    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
@@ -529,27 +509,26 @@
     SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
-    RoutingConfigOutputTypeDef,
     RoutingConfigTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
+    CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
-    UpdateEndpointResponseTypeDef,
-    CreateEndpointRequestRequestTypeDef,
     UpdateEndpointRequestRequestTypeDef,
+    UpdateEndpointResponseTypeDef,
     ListTargetsByRuleResponseTypeDef,
     PutTargetsRequestRequestTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/SOURCES.txt` & `mypy-boto3-events-1.28.15/mypy_boto3_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.12/setup.py` & `mypy-boto3-events-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-events",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridge 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

