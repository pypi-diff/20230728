# Comparing `tmp/mypy-boto3-stepfunctions-1.28.12.tar.gz` & `tmp/mypy-boto3-stepfunctions-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-stepfunctions-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
+gzip compressed data, was "mypy-boto3-stepfunctions-1.28.15.tar", last modified: Fri Jul 28 20:43:50 2023, max compression
```

## Comparing `mypy-boto3-stepfunctions-1.28.12.tar` & `mypy-boto3-stepfunctions-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.077344 mypy-boto3-stepfunctions-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-07-27 11:49:44.073344 mypy-boto3-stepfunctions-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.069344 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-27 11:47:40.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-27 11:47:40.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45195 2023-07-27 11:47:41.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45130 2023-07-27 11:47:40.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.073344 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:43.000000 mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.077344 mypy-boto3-stepfunctions-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:47:39.000000 mypy-boto3-stepfunctions-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44183 2023-07-28 20:40:18.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44118 2023-07-28 20:40:17.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:50.000000 mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:50.521957 mypy-boto3-stepfunctions-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:40:16.000000 mypy-boto3-stepfunctions-1.28.15/setup.py
```

### Comparing `mypy-boto3-stepfunctions-1.28.12/LICENSE` & `mypy-boto3-stepfunctions-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.12
-Summary: Type annotations for boto3.SFN 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,15 +352,14 @@
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
-    CloudWatchLogsLogGroupOutputTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
     TracingConfigurationTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
@@ -368,17 +367,15 @@
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
-    RoutingConfigurationListItemOutputTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
-    TracingConfigurationOutputTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -404,15 +401,14 @@
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
@@ -423,48 +419,47 @@
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    LogDestinationOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateActivityOutputTypeDef,
     CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     ListActivitiesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     ListExecutionsOutputTypeDef,
     GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     ListActivitiesInputListActivitiesPaginateTypeDef,
     ListExecutionsInputListExecutionsPaginateTypeDef,
     ListMapRunsInputListMapRunsPaginateTypeDef,
     ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     CreateStateMachineInputRequestTypeDef,
     UpdateStateMachineInputRequestTypeDef,
```

### Comparing `mypy-boto3-stepfunctions-1.28.12/README.md` & `mypy-boto3-stepfunctions-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,15 +320,14 @@
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
-    CloudWatchLogsLogGroupOutputTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
     TracingConfigurationTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
@@ -336,17 +335,15 @@
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
-    RoutingConfigurationListItemOutputTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
-    TracingConfigurationOutputTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -372,15 +369,14 @@
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
@@ -391,48 +387,47 @@
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    LogDestinationOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateActivityOutputTypeDef,
     CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     ListActivitiesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     ListExecutionsOutputTypeDef,
     GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     ListActivitiesInputListActivitiesPaginateTypeDef,
     ListExecutionsInputListExecutionsPaginateTypeDef,
     ListMapRunsInputListMapRunsPaginateTypeDef,
     ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     CreateStateMachineInputRequestTypeDef,
     UpdateStateMachineInputRequestTypeDef,
```

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.py` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__init__.pyi` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/__main__.py` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SFN 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SFN 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
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

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.py` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/client.pyi` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.py` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/literals.pyi` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.py` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/paginator.pyi` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.py` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
-    "CloudWatchLogsLogGroupOutputTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "RoutingConfigurationListItemTypeDef",
     "TracingConfigurationTypeDef",
     "DeleteActivityInputRequestTypeDef",
     "DeleteStateMachineAliasInputRequestTypeDef",
@@ -52,17 +51,15 @@
     "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
     "DescribeStateMachineAliasInputRequestTypeDef",
-    "RoutingConfigurationListItemOutputTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
-    "TracingConfigurationOutputTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -88,15 +85,14 @@
     "ListStateMachineAliasesInputRequestTypeDef",
     "StateMachineAliasListItemTypeDef",
     "ListStateMachineVersionsInputRequestTypeDef",
     "StateMachineVersionListItemTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
     "PublishStateMachineVersionInputRequestTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
@@ -107,48 +103,47 @@
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
-    "LogDestinationOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateActivityOutputTypeDef",
     "CreateStateMachineAliasOutputTypeDef",
     "CreateStateMachineOutputTypeDef",
     "DescribeActivityOutputTypeDef",
     "DescribeExecutionOutputTypeDef",
     "GetActivityTaskOutputTypeDef",
     "ListActivitiesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "PublishStateMachineVersionOutputTypeDef",
     "StartExecutionOutputTypeDef",
     "StartSyncExecutionOutputTypeDef",
     "StopExecutionOutputTypeDef",
     "UpdateStateMachineAliasOutputTypeDef",
     "UpdateStateMachineOutputTypeDef",
     "CreateStateMachineAliasInputRequestTypeDef",
+    "DescribeStateMachineAliasOutputTypeDef",
     "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
-    "DescribeStateMachineAliasOutputTypeDef",
     "ListExecutionsOutputTypeDef",
     "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
     "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "CreateStateMachineInputRequestTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
@@ -220,22 +215,14 @@
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     {
         "included": bool,
     },
     total=False,
 )
 
-CloudWatchLogsLogGroupOutputTypeDef = TypedDict(
-    "CloudWatchLogsLogGroupOutputTypeDef",
-    {
-        "logGroupArn": str,
-    },
-    total=False,
-)
-
 CloudWatchLogsLogGroupTypeDef = TypedDict(
     "CloudWatchLogsLogGroupTypeDef",
     {
         "logGroupArn": str,
     },
     total=False,
 )
@@ -356,37 +343,21 @@
 DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
     "DescribeStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 
-RoutingConfigurationListItemOutputTypeDef = TypedDict(
-    "RoutingConfigurationListItemOutputTypeDef",
-    {
-        "stateMachineVersionArn": str,
-        "weight": int,
-    },
-)
-
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
-TracingConfigurationOutputTypeDef = TypedDict(
-    "TracingConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-    total=False,
-)
-
 DescribeStateMachineInputRequestTypeDef = TypedDict(
     "DescribeStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
@@ -828,23 +799,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
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
-    total=False,
-)
-
 _RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
     "_RequiredPublishStateMachineVersionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
@@ -1149,22 +1111,14 @@
 
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
 
-LogDestinationOutputTypeDef = TypedDict(
-    "LogDestinationOutputTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupOutputTypeDef,
-    },
-    total=False,
-)
-
 LogDestinationTypeDef = TypedDict(
     "LogDestinationTypeDef",
     {
         "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
@@ -1273,14 +1227,22 @@
     {
         "activities": List[ActivityListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PublishStateMachineVersionOutputTypeDef = TypedDict(
     "PublishStateMachineVersionOutputTypeDef",
     {
         "creationDate": datetime,
         "stateMachineVersionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1361,14 +1323,27 @@
 class CreateStateMachineAliasInputRequestTypeDef(
     _RequiredCreateStateMachineAliasInputRequestTypeDef,
     _OptionalCreateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
 
+DescribeStateMachineAliasOutputTypeDef = TypedDict(
+    "DescribeStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "name": str,
+        "description": str,
+        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
+        "creationDate": datetime,
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 _OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
@@ -1401,27 +1376,14 @@
         "toleratedFailureCount": int,
         "itemCounts": MapRunItemCountsTypeDef,
         "executionCounts": MapRunExecutionCountsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStateMachineAliasOutputTypeDef = TypedDict(
-    "DescribeStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "name": str,
-        "description": str,
-        "routingConfiguration": List[RoutingConfigurationListItemOutputTypeDef],
-        "creationDate": datetime,
-        "updateDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1583,28 +1545,20 @@
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 LoggingConfigurationOutputTypeDef = TypedDict(
     "LoggingConfigurationOutputTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
-        "destinations": List[LogDestinationOutputTypeDef],
+        "destinations": List[LogDestinationTypeDef],
     },
     total=False,
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
@@ -1675,15 +1629,15 @@
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
         "loggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "tracingConfiguration": TracingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1694,15 +1648,15 @@
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
         "loggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "tracingConfiguration": TracingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions/type_defs.pyi` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
-    "CloudWatchLogsLogGroupOutputTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "RoutingConfigurationListItemTypeDef",
     "TracingConfigurationTypeDef",
     "DeleteActivityInputRequestTypeDef",
     "DeleteStateMachineAliasInputRequestTypeDef",
@@ -51,17 +50,15 @@
     "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
     "DescribeStateMachineAliasInputRequestTypeDef",
-    "RoutingConfigurationListItemOutputTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
-    "TracingConfigurationOutputTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -87,15 +84,14 @@
     "ListStateMachineAliasesInputRequestTypeDef",
     "StateMachineAliasListItemTypeDef",
     "ListStateMachineVersionsInputRequestTypeDef",
     "StateMachineVersionListItemTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
     "PublishStateMachineVersionInputRequestTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
@@ -106,48 +102,47 @@
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
-    "LogDestinationOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateActivityOutputTypeDef",
     "CreateStateMachineAliasOutputTypeDef",
     "CreateStateMachineOutputTypeDef",
     "DescribeActivityOutputTypeDef",
     "DescribeExecutionOutputTypeDef",
     "GetActivityTaskOutputTypeDef",
     "ListActivitiesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "PublishStateMachineVersionOutputTypeDef",
     "StartExecutionOutputTypeDef",
     "StartSyncExecutionOutputTypeDef",
     "StopExecutionOutputTypeDef",
     "UpdateStateMachineAliasOutputTypeDef",
     "UpdateStateMachineOutputTypeDef",
     "CreateStateMachineAliasInputRequestTypeDef",
+    "DescribeStateMachineAliasOutputTypeDef",
     "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
-    "DescribeStateMachineAliasOutputTypeDef",
     "ListExecutionsOutputTypeDef",
     "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
     "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "CreateStateMachineInputRequestTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
@@ -219,22 +214,14 @@
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     {
         "included": bool,
     },
     total=False,
 )
 
-CloudWatchLogsLogGroupOutputTypeDef = TypedDict(
-    "CloudWatchLogsLogGroupOutputTypeDef",
-    {
-        "logGroupArn": str,
-    },
-    total=False,
-)
-
 CloudWatchLogsLogGroupTypeDef = TypedDict(
     "CloudWatchLogsLogGroupTypeDef",
     {
         "logGroupArn": str,
     },
     total=False,
 )
@@ -355,37 +342,21 @@
 DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
     "DescribeStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 
-RoutingConfigurationListItemOutputTypeDef = TypedDict(
-    "RoutingConfigurationListItemOutputTypeDef",
-    {
-        "stateMachineVersionArn": str,
-        "weight": int,
-    },
-)
-
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
-TracingConfigurationOutputTypeDef = TypedDict(
-    "TracingConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-    total=False,
-)
-
 DescribeStateMachineInputRequestTypeDef = TypedDict(
     "DescribeStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
@@ -805,23 +776,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
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
-    total=False,
-)
-
 _RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
     "_RequiredPublishStateMachineVersionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
@@ -1104,22 +1066,14 @@
 )
 
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
-LogDestinationOutputTypeDef = TypedDict(
-    "LogDestinationOutputTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupOutputTypeDef,
-    },
-    total=False,
-)
-
 LogDestinationTypeDef = TypedDict(
     "LogDestinationTypeDef",
     {
         "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
@@ -1226,14 +1180,22 @@
     {
         "activities": List[ActivityListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PublishStateMachineVersionOutputTypeDef = TypedDict(
     "PublishStateMachineVersionOutputTypeDef",
     {
         "creationDate": datetime,
         "stateMachineVersionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1312,14 +1274,27 @@
 
 class CreateStateMachineAliasInputRequestTypeDef(
     _RequiredCreateStateMachineAliasInputRequestTypeDef,
     _OptionalCreateStateMachineAliasInputRequestTypeDef,
 ):
     pass
 
+DescribeStateMachineAliasOutputTypeDef = TypedDict(
+    "DescribeStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "name": str,
+        "description": str,
+        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
+        "creationDate": datetime,
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
     },
 )
 _OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
@@ -1350,27 +1325,14 @@
         "toleratedFailureCount": int,
         "itemCounts": MapRunItemCountsTypeDef,
         "executionCounts": MapRunExecutionCountsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStateMachineAliasOutputTypeDef = TypedDict(
-    "DescribeStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "name": str,
-        "description": str,
-        "routingConfiguration": List[RoutingConfigurationListItemOutputTypeDef],
-        "creationDate": datetime,
-        "updateDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1524,28 +1486,20 @@
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 LoggingConfigurationOutputTypeDef = TypedDict(
     "LoggingConfigurationOutputTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
-        "destinations": List[LogDestinationOutputTypeDef],
+        "destinations": List[LogDestinationTypeDef],
     },
     total=False,
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
@@ -1614,15 +1568,15 @@
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
         "loggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "tracingConfiguration": TracingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1633,15 +1587,15 @@
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
         "loggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "tracingConfiguration": TracingConfigurationOutputTypeDef,
+        "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/PKG-INFO` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.28.12
-Summary: Type annotations for boto3.SFN 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,15 +352,14 @@
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
-    CloudWatchLogsLogGroupOutputTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
     TracingConfigurationTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
@@ -368,17 +367,15 @@
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
-    RoutingConfigurationListItemOutputTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
-    TracingConfigurationOutputTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
     PaginatorConfigTypeDef,
@@ -404,15 +401,14 @@
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
@@ -423,48 +419,47 @@
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    LogDestinationOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateActivityOutputTypeDef,
     CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     ListActivitiesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
+    DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     ListExecutionsOutputTypeDef,
     GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     ListActivitiesInputListActivitiesPaginateTypeDef,
     ListExecutionsInputListExecutionsPaginateTypeDef,
     ListMapRunsInputListMapRunsPaginateTypeDef,
     ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     CreateStateMachineInputRequestTypeDef,
     UpdateStateMachineInputRequestTypeDef,
```

### Comparing `mypy-boto3-stepfunctions-1.28.12/mypy_boto3_stepfunctions.egg-info/SOURCES.txt` & `mypy-boto3-stepfunctions-1.28.15/mypy_boto3_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.28.12/setup.py` & `mypy-boto3-stepfunctions-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-stepfunctions",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SFN 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SFN 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

