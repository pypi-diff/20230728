# Comparing `tmp/mypy-boto3-swf-1.28.12.tar.gz` & `tmp/mypy-boto3-swf-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-swf-1.28.12.tar", last modified: Thu Jul 27 11:49:45 2023, max compression
+gzip compressed data, was "mypy-boto3-swf-1.28.15.tar", last modified: Fri Jul 28 20:43:52 2023, max compression
```

## Comparing `mypy-boto3-swf-1.28.12.tar` & `mypy-boto3-swf-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:45.769408 mypy-boto3-swf-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-27 11:49:45.765408 mypy-boto3-swf-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:45.765408 mypy-boto3-swf-1.28.12/mypy_boto3_swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30971 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-07-27 11:47:53.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-27 11:47:52.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85198 2023-07-27 11:47:54.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85040 2023-07-27 11:47:53.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:45.765408 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:45.000000 mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:45.769408 mypy-boto3-swf-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:50.000000 mypy-boto3-swf-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.089979 mypy-boto3-swf-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-07-28 20:43:52.089979 mypy-boto3-swf-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.081978 mypy-boto3-swf-1.28.15/mypy_boto3_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30971 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-07-28 20:40:31.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    83888 2023-07-28 20:40:33.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83731 2023-07-28 20:40:32.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.089979 mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-07-28 20:43:51.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:51.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:51.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:51.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:51.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:51.000000 mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:52.089979 mypy-boto3-swf-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:40:30.000000 mypy-boto3-swf-1.28.15/setup.py
```

### Comparing `mypy-boto3-swf-1.28.12/LICENSE` & `mypy-boto3-swf-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/PKG-INFO` & `mypy-boto3-swf-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.28.12
-Summary: Type annotations for boto3.SWF 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SWF 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -379,30 +379,28 @@
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
-    ActivityTypeOutputTypeDef,
-    TaskListOutputTypeDef,
+    ActivityTypeTypeDef,
+    TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
     ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
-    WorkflowExecutionOutputTypeDef,
-    ActivityTypeTypeDef,
+    WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
-    WorkflowTypeOutputTypeDef,
+    WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
-    TaskListTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
     ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
@@ -411,17 +409,15 @@
     RecordMarkerDecisionAttributesTypeDef,
     RequestCancelActivityTaskDecisionAttributesTypeDef,
     RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
-    WorkflowTypeTypeDef,
     DescribeDomainInputRequestTypeDef,
-    WorkflowExecutionTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
     PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
@@ -444,101 +440,100 @@
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
     ListActivityTypesInputRequestTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResourceTagOutputTypeDef,
+    ResourceTagTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
-    ResourceTagTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
+    DeprecateActivityTypeInputRequestTypeDef,
+    DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
+    UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
+    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+    CountPendingActivityTasksInputRequestTypeDef,
+    CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
+    PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputRequestTypeDef,
+    RegisterActivityTypeInputRequestTypeDef,
+    RegisterWorkflowTypeInputRequestTypeDef,
+    ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
     ActivityTaskStatusTypeDef,
     EmptyResponseMetadataTypeDef,
     PendingTaskCountTypeDef,
     RunTypeDef,
     WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
+    DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
+    GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
-    DeprecateActivityTypeInputRequestTypeDef,
-    DescribeActivityTypeInputRequestTypeDef,
-    UndeprecateActivityTypeInputRequestTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
     ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
     ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
+    DeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowTypeInputRequestTypeDef,
+    StartChildWorkflowExecutionDecisionAttributesTypeDef,
     StartChildWorkflowExecutionFailedEventAttributesTypeDef,
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
+    StartWorkflowExecutionInputRequestTypeDef,
+    UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
-    CountPendingActivityTasksInputRequestTypeDef,
-    CountPendingDecisionTasksInputRequestTypeDef,
-    PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputRequestTypeDef,
-    RegisterActivityTypeInputRequestTypeDef,
-    RegisterWorkflowTypeInputRequestTypeDef,
-    ScheduleActivityTaskDecisionAttributesTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
-    DeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowTypeInputRequestTypeDef,
-    StartChildWorkflowExecutionDecisionAttributesTypeDef,
-    StartWorkflowExecutionInputRequestTypeDef,
-    UndeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowExecutionInputRequestTypeDef,
-    GetWorkflowExecutionHistoryInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
     GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListDomainsInputListDomainsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
+    DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
-    DecisionTypeDef,
+    RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
-    RespondDecisionTaskCompletedInputRequestTypeDef,
 )
 
 
 def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-swf-1.28.12/README.md` & `mypy-boto3-swf-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -347,30 +347,28 @@
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
-    ActivityTypeOutputTypeDef,
-    TaskListOutputTypeDef,
+    ActivityTypeTypeDef,
+    TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
     ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
-    WorkflowExecutionOutputTypeDef,
-    ActivityTypeTypeDef,
+    WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
-    WorkflowTypeOutputTypeDef,
+    WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
-    TaskListTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
     ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
@@ -379,17 +377,15 @@
     RecordMarkerDecisionAttributesTypeDef,
     RequestCancelActivityTaskDecisionAttributesTypeDef,
     RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
-    WorkflowTypeTypeDef,
     DescribeDomainInputRequestTypeDef,
-    WorkflowExecutionTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
     PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
@@ -412,101 +408,100 @@
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
     ListActivityTypesInputRequestTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResourceTagOutputTypeDef,
+    ResourceTagTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
-    ResourceTagTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
+    DeprecateActivityTypeInputRequestTypeDef,
+    DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
+    UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
+    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+    CountPendingActivityTasksInputRequestTypeDef,
+    CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
+    PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputRequestTypeDef,
+    RegisterActivityTypeInputRequestTypeDef,
+    RegisterWorkflowTypeInputRequestTypeDef,
+    ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
     ActivityTaskStatusTypeDef,
     EmptyResponseMetadataTypeDef,
     PendingTaskCountTypeDef,
     RunTypeDef,
     WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
+    DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
+    GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
-    DeprecateActivityTypeInputRequestTypeDef,
-    DescribeActivityTypeInputRequestTypeDef,
-    UndeprecateActivityTypeInputRequestTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
     ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
     ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
+    DeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowTypeInputRequestTypeDef,
+    StartChildWorkflowExecutionDecisionAttributesTypeDef,
     StartChildWorkflowExecutionFailedEventAttributesTypeDef,
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
+    StartWorkflowExecutionInputRequestTypeDef,
+    UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
-    CountPendingActivityTasksInputRequestTypeDef,
-    CountPendingDecisionTasksInputRequestTypeDef,
-    PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputRequestTypeDef,
-    RegisterActivityTypeInputRequestTypeDef,
-    RegisterWorkflowTypeInputRequestTypeDef,
-    ScheduleActivityTaskDecisionAttributesTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
-    DeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowTypeInputRequestTypeDef,
-    StartChildWorkflowExecutionDecisionAttributesTypeDef,
-    StartWorkflowExecutionInputRequestTypeDef,
-    UndeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowExecutionInputRequestTypeDef,
-    GetWorkflowExecutionHistoryInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
     GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListDomainsInputListDomainsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
+    DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
-    DecisionTypeDef,
+    RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
-    RespondDecisionTaskCompletedInputRequestTypeDef,
 )
 
 
 def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.py` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/__init__.pyi` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/__main__.py` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SWF 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SWF 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
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

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.py` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/client.pyi` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.py` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/literals.pyi` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.py` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/paginator.pyi` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.py` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,36 +43,33 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
-    "ActivityTypeOutputTypeDef",
-    "TaskListOutputTypeDef",
+    "ActivityTypeTypeDef",
+    "TaskListTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
     "ResponseMetadataTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
-    "WorkflowExecutionOutputTypeDef",
-    "ActivityTypeTypeDef",
+    "WorkflowExecutionTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
-    "WorkflowTypeOutputTypeDef",
+    "WorkflowTypeTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
-    "TaskListTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
@@ -81,17 +78,15 @@
     "RecordMarkerDecisionAttributesTypeDef",
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     "RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef",
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
-    "WorkflowTypeTypeDef",
     "DescribeDomainInputRequestTypeDef",
-    "WorkflowExecutionTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
@@ -114,101 +109,100 @@
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     "ListActivityTypesInputRequestTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResourceTagOutputTypeDef",
+    "ResourceTagTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
-    "ResourceTagTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
+    "DeprecateActivityTypeInputRequestTypeDef",
+    "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
+    "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    "CountPendingActivityTasksInputRequestTypeDef",
+    "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
+    "PollForActivityTaskInputRequestTypeDef",
+    "PollForDecisionTaskInputRequestTypeDef",
+    "RegisterActivityTypeInputRequestTypeDef",
+    "RegisterWorkflowTypeInputRequestTypeDef",
+    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
     "ActivityTaskStatusTypeDef",
     "EmptyResponseMetadataTypeDef",
     "PendingTaskCountTypeDef",
     "RunTypeDef",
     "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
+    "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
+    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
-    "DeprecateActivityTypeInputRequestTypeDef",
-    "DescribeActivityTypeInputRequestTypeDef",
-    "UndeprecateActivityTypeInputRequestTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    "DescribeWorkflowTypeInputRequestTypeDef",
+    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
     "StartChildWorkflowExecutionFailedEventAttributesTypeDef",
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
+    "StartWorkflowExecutionInputRequestTypeDef",
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    "CountPendingActivityTasksInputRequestTypeDef",
-    "CountPendingDecisionTasksInputRequestTypeDef",
-    "PollForActivityTaskInputRequestTypeDef",
-    "PollForDecisionTaskInputRequestTypeDef",
-    "RegisterActivityTypeInputRequestTypeDef",
-    "RegisterWorkflowTypeInputRequestTypeDef",
-    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "CountClosedWorkflowExecutionsInputRequestTypeDef",
     "CountOpenWorkflowExecutionsInputRequestTypeDef",
     "ListClosedWorkflowExecutionsInputRequestTypeDef",
     "ListOpenWorkflowExecutionsInputRequestTypeDef",
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
-    "StartWorkflowExecutionInputRequestTypeDef",
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
-    "DescribeWorkflowExecutionInputRequestTypeDef",
-    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
     "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListDomainsInputListDomainsPaginateTypeDef",
     "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
+    "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
-    "DecisionTypeDef",
+    "RespondDecisionTaskCompletedInputRequestTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
-    "RespondDecisionTaskCompletedInputRequestTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "activityId": str,
@@ -227,22 +221,20 @@
     {
         "details": str,
         "latestCancelRequestedEventId": int,
     },
     total=False,
 )
 
-
 class ActivityTaskCanceledEventAttributesTypeDef(
     _RequiredActivityTaskCanceledEventAttributesTypeDef,
     _OptionalActivityTaskCanceledEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredActivityTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -250,22 +242,20 @@
     "_OptionalActivityTaskCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class ActivityTaskCompletedEventAttributesTypeDef(
     _RequiredActivityTaskCompletedEventAttributesTypeDef,
     _OptionalActivityTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -274,32 +264,30 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class ActivityTaskFailedEventAttributesTypeDef(
     _RequiredActivityTaskFailedEventAttributesTypeDef,
     _OptionalActivityTaskFailedEventAttributesTypeDef,
 ):
     pass
 
-
-ActivityTypeOutputTypeDef = TypedDict(
-    "ActivityTypeOutputTypeDef",
+ActivityTypeTypeDef = TypedDict(
+    "ActivityTypeTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-TaskListOutputTypeDef = TypedDict(
-    "TaskListOutputTypeDef",
+TaskListTypeDef = TypedDict(
+    "TaskListTypeDef",
     {
         "name": str,
     },
 )
 
 _RequiredActivityTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskStartedEventAttributesTypeDef",
@@ -311,22 +299,20 @@
     "_OptionalActivityTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
-
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -346,38 +332,28 @@
     "_OptionalActivityTaskTimedOutEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class ActivityTaskTimedOutEventAttributesTypeDef(
     _RequiredActivityTaskTimedOutEventAttributesTypeDef,
     _OptionalActivityTaskTimedOutEventAttributesTypeDef,
 ):
     pass
 
-
-WorkflowExecutionOutputTypeDef = TypedDict(
-    "WorkflowExecutionOutputTypeDef",
+WorkflowExecutionTypeDef = TypedDict(
+    "WorkflowExecutionTypeDef",
     {
         "workflowId": str,
         "runId": str,
     },
 )
 
-ActivityTypeTypeDef = TypedDict(
-    "ActivityTypeTypeDef",
-    {
-        "name": str,
-        "version": str,
-    },
-)
-
 CancelTimerDecisionAttributesTypeDef = TypedDict(
     "CancelTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
     },
 )
 
@@ -402,16 +378,16 @@
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CancelWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-WorkflowTypeOutputTypeDef = TypedDict(
-    "WorkflowTypeOutputTypeDef",
+WorkflowTypeTypeDef = TypedDict(
+    "WorkflowTypeTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
 CloseStatusFilterTypeDef = TypedDict(
@@ -433,21 +409,14 @@
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CompleteWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-TaskListTypeDef = TypedDict(
-    "TaskListTypeDef",
-    {
-        "name": str,
-    },
-)
-
 ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -462,21 +431,19 @@
     "_OptionalExecutionTimeFilterTypeDef",
     {
         "latestDate": Union[datetime, str],
     },
     total=False,
 )
 
-
 class ExecutionTimeFilterTypeDef(
     _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
-
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -497,21 +464,19 @@
     "_OptionalWorkflowTypeFilterTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
-
 class WorkflowTypeFilterTypeDef(
     _RequiredWorkflowTypeFilterTypeDef, _OptionalWorkflowTypeFilterTypeDef
 ):
     pass
 
-
 _RequiredDecisionTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -519,44 +484,40 @@
     "_OptionalDecisionTaskCompletedEventAttributesTypeDef",
     {
         "executionContext": str,
     },
     total=False,
 )
 
-
 class DecisionTaskCompletedEventAttributesTypeDef(
     _RequiredDecisionTaskCompletedEventAttributesTypeDef,
     _OptionalDecisionTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 _OptionalDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
-
 class DecisionTaskStartedEventAttributesTypeDef(
     _RequiredDecisionTaskStartedEventAttributesTypeDef,
     _OptionalDecisionTaskStartedEventAttributesTypeDef,
 ):
     pass
 
-
 DecisionTaskTimedOutEventAttributesTypeDef = TypedDict(
     "DecisionTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "scheduledEventId": int,
         "startedEventId": int,
     },
@@ -581,21 +542,19 @@
     "_OptionalRecordMarkerDecisionAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class RecordMarkerDecisionAttributesTypeDef(
     _RequiredRecordMarkerDecisionAttributesTypeDef, _OptionalRecordMarkerDecisionAttributesTypeDef
 ):
     pass
 
-
 RequestCancelActivityTaskDecisionAttributesTypeDef = TypedDict(
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     {
         "activityId": str,
     },
 )
 
@@ -610,22 +569,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
-
 _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef = TypedDict(
     "_RequiredScheduleLambdaFunctionDecisionAttributesTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
@@ -635,22 +592,20 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
-
 class ScheduleLambdaFunctionDecisionAttributesTypeDef(
     _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef,
     _OptionalScheduleLambdaFunctionDecisionAttributesTypeDef,
 ):
     pass
 
-
 _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
     },
 )
@@ -660,22 +615,20 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
-
 class SignalExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
-
 _RequiredStartTimerDecisionAttributesTypeDef = TypedDict(
     "_RequiredStartTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
         "startToFireTimeout": str,
     },
 )
@@ -683,51 +636,33 @@
     "_OptionalStartTimerDecisionAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
-
 class StartTimerDecisionAttributesTypeDef(
     _RequiredStartTimerDecisionAttributesTypeDef, _OptionalStartTimerDecisionAttributesTypeDef
 ):
     pass
 
-
 DeprecateDomainInputRequestTypeDef = TypedDict(
     "DeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
-WorkflowTypeTypeDef = TypedDict(
-    "WorkflowTypeTypeDef",
-    {
-        "name": str,
-        "version": str,
-    },
-)
-
 DescribeDomainInputRequestTypeDef = TypedDict(
     "DescribeDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
-WorkflowExecutionTypeDef = TypedDict(
-    "WorkflowExecutionTypeDef",
-    {
-        "workflowId": str,
-        "runId": str,
-    },
-)
-
 DomainConfigurationTypeDef = TypedDict(
     "DomainConfigurationTypeDef",
     {
         "workflowExecutionRetentionPeriodInDays": str,
     },
 )
 
@@ -743,19 +678,17 @@
     {
         "description": str,
         "arn": str,
     },
     total=False,
 )
 
-
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
-
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -781,22 +714,20 @@
     "_OptionalLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class LambdaFunctionCompletedEventAttributesTypeDef(
     _RequiredLambdaFunctionCompletedEventAttributesTypeDef,
     _OptionalLambdaFunctionCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -805,22 +736,20 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class LambdaFunctionFailedEventAttributesTypeDef(
     _RequiredLambdaFunctionFailedEventAttributesTypeDef,
     _OptionalLambdaFunctionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredLambdaFunctionScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -831,22 +760,20 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
-
 class LambdaFunctionScheduledEventAttributesTypeDef(
     _RequiredLambdaFunctionScheduledEventAttributesTypeDef,
     _OptionalLambdaFunctionScheduledEventAttributesTypeDef,
 ):
     pass
 
-
 LambdaFunctionStartedEventAttributesTypeDef = TypedDict(
     "LambdaFunctionStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 
@@ -861,22 +788,20 @@
     "_OptionalLambdaFunctionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
     },
     total=False,
 )
 
-
 class LambdaFunctionTimedOutEventAttributesTypeDef(
     _RequiredLambdaFunctionTimedOutEventAttributesTypeDef,
     _OptionalLambdaFunctionTimedOutEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredMarkerRecordedEventAttributesTypeDef = TypedDict(
     "_RequiredMarkerRecordedEventAttributesTypeDef",
     {
         "markerName": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -884,21 +809,19 @@
     "_OptionalMarkerRecordedEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class MarkerRecordedEventAttributesTypeDef(
     _RequiredMarkerRecordedEventAttributesTypeDef, _OptionalMarkerRecordedEventAttributesTypeDef
 ):
     pass
 
-
 RecordMarkerFailedEventAttributesTypeDef = TypedDict(
     "RecordMarkerFailedEventAttributesTypeDef",
     {
         "markerName": str,
         "cause": Literal["OPERATION_NOT_PERMITTED"],
         "decisionTaskCompletedEventId": int,
     },
@@ -927,22 +850,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -951,22 +872,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
-
 ScheduleLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "ScheduleLambdaFunctionFailedEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "cause": ScheduleLambdaFunctionFailedCauseType,
         "decisionTaskCompletedEventId": int,
@@ -987,22 +906,20 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
-
 class SignalExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -1013,22 +930,20 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
-
 class SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
-
 StartLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "StartLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "cause": Literal["ASSUME_ROLE_FAILED"],
         "message": str,
     },
@@ -1073,65 +988,59 @@
     "_OptionalTimerStartedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
-
 class TimerStartedEventAttributesTypeDef(
     _RequiredTimerStartedEventAttributesTypeDef, _OptionalTimerStartedEventAttributesTypeDef
 ):
     pass
 
-
 _RequiredWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
@@ -1139,22 +1048,20 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
@@ -1163,22 +1070,20 @@
         "reason": str,
         "details": str,
         "cause": WorkflowExecutionTerminatedCauseType,
     },
     total=False,
 )
 
-
 class WorkflowExecutionTerminatedEventAttributesTypeDef(
     _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef,
     _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef,
 ):
     pass
 
-
 WorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
@@ -1197,21 +1102,19 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
-
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputRequestTypeDef = TypedDict(
@@ -1220,49 +1123,43 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
-
 class ListDomainsInputRequestTypeDef(
     _RequiredListDomainsInputRequestTypeDef, _OptionalListDomainsInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredResourceTagOutputTypeDef = TypedDict(
-    "_RequiredResourceTagOutputTypeDef",
+_RequiredResourceTagTypeDef = TypedDict(
+    "_RequiredResourceTagTypeDef",
     {
         "key": str,
     },
 )
-_OptionalResourceTagOutputTypeDef = TypedDict(
-    "_OptionalResourceTagOutputTypeDef",
+_OptionalResourceTagTypeDef = TypedDict(
+    "_OptionalResourceTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
-class ResourceTagOutputTypeDef(
-    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
-):
+class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
-
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1273,62 +1170,39 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
-
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
 ):
     pass
 
-
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_OptionalRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class RecordActivityTaskHeartbeatInputRequestTypeDef(
     _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef,
     _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredResourceTagTypeDef = TypedDict(
-    "_RequiredResourceTagTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalResourceTagTypeDef = TypedDict(
-    "_OptionalResourceTagTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
-    pass
-
-
 _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
 )
@@ -1336,66 +1210,60 @@
     "_OptionalRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "runId": str,
     },
     total=False,
 )
 
-
 class RequestCancelWorkflowExecutionInputRequestTypeDef(
     _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef,
     _OptionalRequestCancelWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class RespondActivityTaskCanceledInputRequestTypeDef(
     _RequiredRespondActivityTaskCanceledInputRequestTypeDef,
     _OptionalRespondActivityTaskCanceledInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class RespondActivityTaskCompletedInputRequestTypeDef(
     _RequiredRespondActivityTaskCompletedInputRequestTypeDef,
     _OptionalRespondActivityTaskCompletedInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskFailedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
@@ -1403,22 +1271,20 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
     },
@@ -1428,22 +1294,20 @@
     {
         "runId": str,
         "input": str,
     },
     total=False,
 )
 
-
 class SignalWorkflowExecutionInputRequestTypeDef(
     _RequiredSignalWorkflowExecutionInputRequestTypeDef,
     _OptionalSignalWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredTerminateWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredTerminateWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
 )
@@ -1454,22 +1318,20 @@
         "reason": str,
         "details": str,
         "childPolicy": ChildPolicyType,
     },
     total=False,
 )
 
-
 class TerminateWorkflowExecutionInputRequestTypeDef(
     _RequiredTerminateWorkflowExecutionInputRequestTypeDef,
     _OptionalTerminateWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
-
 UndeprecateDomainInputRequestTypeDef = TypedDict(
     "UndeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -1494,59 +1356,79 @@
     "_OptionalWorkflowExecutionOpenCountsTypeDef",
     {
         "openLambdaFunctions": int,
     },
     total=False,
 )
 
-
 class WorkflowExecutionOpenCountsTypeDef(
     _RequiredWorkflowExecutionOpenCountsTypeDef, _OptionalWorkflowExecutionOpenCountsTypeDef
 ):
     pass
 
-
 _RequiredActivityTypeInfoTypeDef = TypedDict(
     "_RequiredActivityTypeInfoTypeDef",
     {
-        "activityType": ActivityTypeOutputTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalActivityTypeInfoTypeDef = TypedDict(
     "_OptionalActivityTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
-
 class ActivityTypeInfoTypeDef(_RequiredActivityTypeInfoTypeDef, _OptionalActivityTypeInfoTypeDef):
     pass
 
+DeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "DeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
+DescribeActivityTypeInputRequestTypeDef = TypedDict(
+    "DescribeActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
 
 ScheduleActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeOutputTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "activityId": str,
         "cause": ScheduleActivityTaskFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
+UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
 _RequiredActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskScheduledEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeOutputTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "activityId": str,
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalActivityTaskScheduledEventAttributesTypeDef",
     {
         "input": str,
@@ -1556,89 +1438,243 @@
         "startToCloseTimeout": str,
         "taskPriority": str,
         "heartbeatTimeout": str,
     },
     total=False,
 )
 
-
 class ActivityTaskScheduledEventAttributesTypeDef(
     _RequiredActivityTaskScheduledEventAttributesTypeDef,
     _OptionalActivityTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
-
 ActivityTypeConfigurationTypeDef = TypedDict(
     "ActivityTypeConfigurationTypeDef",
     {
         "defaultTaskStartToCloseTimeout": str,
         "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListOutputTypeDef,
+        "defaultTaskList": TaskListTypeDef,
         "defaultTaskPriority": str,
         "defaultTaskScheduleToStartTimeout": str,
         "defaultTaskScheduleToCloseTimeout": str,
     },
     total=False,
 )
 
+ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "workflowTypeVersion": str,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+CountPendingActivityTasksInputRequestTypeDef = TypedDict(
+    "CountPendingActivityTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
+CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
+    "CountPendingDecisionTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
 _RequiredDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskScheduledEventAttributesTypeDef",
     {
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
     },
 )
 _OptionalDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskScheduledEventAttributesTypeDef",
     {
         "taskPriority": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
-
 class DecisionTaskScheduledEventAttributesTypeDef(
     _RequiredDecisionTaskScheduledEventAttributesTypeDef,
     _OptionalDecisionTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
+_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForActivityTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForActivityTaskInputRequestTypeDef",
+    {
+        "identity": str,
+    },
+    total=False,
+)
+
+class PollForActivityTaskInputRequestTypeDef(
+    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
+):
+    pass
+
+_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputRequestTypeDef",
+    {
+        "identity": str,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+    },
+    total=False,
+)
+
+class PollForDecisionTaskInputRequestTypeDef(
+    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
+):
+    pass
+
+_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterActivityTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultTaskHeartbeatTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultTaskScheduleToStartTimeout": str,
+        "defaultTaskScheduleToCloseTimeout": str,
+    },
+    total=False,
+)
+
+class RegisterActivityTypeInputRequestTypeDef(
+    _RequiredRegisterActivityTypeInputRequestTypeDef,
+    _OptionalRegisterActivityTypeInputRequestTypeDef,
+):
+    pass
+
+_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultExecutionStartToCloseTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultChildPolicy": ChildPolicyType,
+        "defaultLambdaRole": str,
+    },
+    total=False,
+)
+
+class RegisterWorkflowTypeInputRequestTypeDef(
+    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
+    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
+):
+    pass
+
+_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "activityType": ActivityTypeTypeDef,
+        "activityId": str,
+    },
+)
+_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "scheduleToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "scheduleToStartTimeout": str,
+        "startToCloseTimeout": str,
+        "heartbeatTimeout": str,
+    },
+    total=False,
+)
+
+class ScheduleActivityTaskDecisionAttributesTypeDef(
+    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
+    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
+):
+    pass
 
 _RequiredWorkflowExecutionConfigurationTypeDef = TypedDict(
     "_RequiredWorkflowExecutionConfigurationTypeDef",
     {
         "taskStartToCloseTimeout": str,
         "executionStartToCloseTimeout": str,
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalWorkflowExecutionConfigurationTypeDef = TypedDict(
     "_OptionalWorkflowExecutionConfigurationTypeDef",
     {
         "taskPriority": str,
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionConfigurationTypeDef(
     _RequiredWorkflowExecutionConfigurationTypeDef, _OptionalWorkflowExecutionConfigurationTypeDef
 ):
     pass
 
-
 WorkflowTypeConfigurationTypeDef = TypedDict(
     "WorkflowTypeConfigurationTypeDef",
     {
         "defaultTaskStartToCloseTimeout": str,
         "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListOutputTypeDef,
+        "defaultTaskList": TaskListTypeDef,
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
@@ -1685,41 +1721,72 @@
 
 ActivityTaskTypeDef = TypedDict(
     "ActivityTaskTypeDef",
     {
         "taskToken": str,
         "activityId": str,
         "startedEventId": int,
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "activityType": ActivityTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "input": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+
 ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
 ExternalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
+_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+class GetWorkflowExecutionHistoryInputRequestTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
+):
+    pass
+
 WorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionTypeDef,
         "externalInitiatedEventId": int,
         "cause": Literal["CHILD_POLICY_APPLIED"],
     },
     total=False,
 )
 
 _RequiredWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
@@ -1728,190 +1795,201 @@
         "signalName": str,
     },
 )
 _OptionalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "input": str,
-        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionTypeDef,
         "externalInitiatedEventId": int,
     },
     total=False,
 )
 
-
 class WorkflowExecutionSignaledEventAttributesTypeDef(
     _RequiredWorkflowExecutionSignaledEventAttributesTypeDef,
     _OptionalWorkflowExecutionSignaledEventAttributesTypeDef,
 ):
     pass
 
-
-DeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "DeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
-DescribeActivityTypeInputRequestTypeDef = TypedDict(
-    "DescribeActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
-UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
 _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
-
 class ChildWorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
-
 class ChildWorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
-
 class ChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 ChildWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "timeoutType": Literal["START_TO_CLOSE"],
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
+DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "workflowType": WorkflowTypeTypeDef,
+        "workflowId": str,
+    },
+)
+_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+class StartChildWorkflowExecutionDecisionAttributesTypeDef(
+    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
+    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
+):
+    pass
+
 _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "cause": StartChildWorkflowExecutionFailedCauseType,
         "workflowId": str,
         "initiatedEventId": int,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
-
 class StartChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
-        "workflowType": WorkflowTypeOutputTypeDef,
-        "taskList": TaskListOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
+        "taskList": TaskListTypeDef,
         "decisionTaskCompletedEventId": int,
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
@@ -1922,30 +2000,65 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class StartChildWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
+_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowId": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "tagList": Sequence[str],
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+class StartWorkflowExecutionInputRequestTypeDef(
+    _RequiredStartWorkflowExecutionInputRequestTypeDef,
+    _OptionalStartWorkflowExecutionInputRequestTypeDef,
+):
+    pass
+
+UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
 
 _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "newExecutionRunId": str,
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
         "childPolicy": ChildPolicyType,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
     },
 )
 _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
@@ -1953,274 +2066,96 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionContinuedAsNewEventAttributesTypeDef(
     _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowExecutionInfoTypeDef = TypedDict(
     "_RequiredWorkflowExecutionInfoTypeDef",
     {
-        "execution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "execution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "startTimestamp": datetime,
         "executionStatus": ExecutionStatusType,
     },
 )
 _OptionalWorkflowExecutionInfoTypeDef = TypedDict(
     "_OptionalWorkflowExecutionInfoTypeDef",
     {
         "closeTimestamp": datetime,
         "closeStatus": CloseStatusType,
-        "parent": WorkflowExecutionOutputTypeDef,
+        "parent": WorkflowExecutionTypeDef,
         "tagList": List[str],
         "cancelRequested": bool,
     },
     total=False,
 )
 
-
 class WorkflowExecutionInfoTypeDef(
     _RequiredWorkflowExecutionInfoTypeDef, _OptionalWorkflowExecutionInfoTypeDef
 ):
     pass
 
-
 _RequiredWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
-        "taskList": TaskListOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "taskList": TaskListTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
     },
 )
 _OptionalWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
         "taskStartToCloseTimeout": str,
         "taskPriority": str,
         "tagList": List[str],
         "continuedExecutionRunId": str,
-        "parentWorkflowExecution": WorkflowExecutionOutputTypeDef,
+        "parentWorkflowExecution": WorkflowExecutionTypeDef,
         "parentInitiatedEventId": int,
         "lambdaRole": str,
     },
     total=False,
 )
 
-
 class WorkflowExecutionStartedEventAttributesTypeDef(
     _RequiredWorkflowExecutionStartedEventAttributesTypeDef,
     _OptionalWorkflowExecutionStartedEventAttributesTypeDef,
 ):
     pass
 
-
 _RequiredWorkflowTypeInfoTypeDef = TypedDict(
     "_RequiredWorkflowTypeInfoTypeDef",
     {
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalWorkflowTypeInfoTypeDef = TypedDict(
     "_OptionalWorkflowTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
-
 class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
-
-ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "workflowTypeVersion": str,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-CountPendingActivityTasksInputRequestTypeDef = TypedDict(
-    "CountPendingActivityTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-
-CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
-    "CountPendingDecisionTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-
-_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForActivityTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForActivityTaskInputRequestTypeDef",
-    {
-        "identity": str,
-    },
-    total=False,
-)
-
-
-class PollForActivityTaskInputRequestTypeDef(
-    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
-):
-    pass
-
-
-_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputRequestTypeDef",
-    {
-        "identity": str,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-    },
-    total=False,
-)
-
-
-class PollForDecisionTaskInputRequestTypeDef(
-    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
-):
-    pass
-
-
-_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterActivityTypeInputRequestTypeDef",
-    {
-        "description": str,
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultTaskScheduleToStartTimeout": str,
-        "defaultTaskScheduleToCloseTimeout": str,
-    },
-    total=False,
-)
-
-
-class RegisterActivityTypeInputRequestTypeDef(
-    _RequiredRegisterActivityTypeInputRequestTypeDef,
-    _OptionalRegisterActivityTypeInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
-    {
-        "description": str,
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultChildPolicy": ChildPolicyType,
-        "defaultLambdaRole": str,
-    },
-    total=False,
-)
-
-
-class RegisterWorkflowTypeInputRequestTypeDef(
-    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
-    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
-    {
-        "activityType": ActivityTypeTypeDef,
-        "activityId": str,
-    },
-)
-_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
-    {
-        "control": str,
-        "input": str,
-        "scheduleToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "scheduleToStartTimeout": str,
-        "startToCloseTimeout": str,
-        "heartbeatTimeout": str,
-    },
-    total=False,
-)
-
-
-class ScheduleActivityTaskDecisionAttributesTypeDef(
-    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
-    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
-):
-    pass
-
-
 _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
@@ -2232,22 +2167,20 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
     },
     total=False,
 )
 
-
 class CountClosedWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2257,22 +2190,20 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
-
 class CountOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
@@ -2287,22 +2218,20 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
-
 class ListClosedWorkflowExecutionsInputRequestTypeDef(
     _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
     _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2315,141 +2244,20 @@
         "maximumPageSize": int,
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
-
 class ListOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-
-DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "workflowType": WorkflowTypeTypeDef,
-        "workflowId": str,
-    },
-)
-_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "control": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-
-class StartChildWorkflowExecutionDecisionAttributesTypeDef(
-    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
-    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
-):
-    pass
-
-
-_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowId": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "tagList": Sequence[str],
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-
-class StartWorkflowExecutionInputRequestTypeDef(
-    _RequiredStartWorkflowExecutionInputRequestTypeDef,
-    _OptionalStartWorkflowExecutionInputRequestTypeDef,
-):
-    pass
-
-
-UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowExecutionInputRequestTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-
-_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
-    {
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-    },
-    total=False,
-)
-
-
-class GetWorkflowExecutionHistoryInputRequestTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
-):
-    pass
-
-
 DomainDetailTypeDef = TypedDict(
     "DomainDetailTypeDef",
     {
         "domainInfo": DomainInfoTypeDef,
         "configuration": DomainConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2476,22 +2284,20 @@
     {
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
     _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
     "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -2501,22 +2307,20 @@
         "name": str,
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListActivityTypesInputListActivityTypesPaginateTypeDef(
     _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
     _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
@@ -2530,22 +2334,20 @@
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
     _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
     "_RequiredListDomainsInputListDomainsPaginateTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
@@ -2553,22 +2355,20 @@
     {
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDomainsInputListDomainsPaginateTypeDef(
     _RequiredListDomainsInputListDomainsPaginateTypeDef,
     _OptionalListDomainsInputListDomainsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2580,22 +2380,20 @@
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
     _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -2605,22 +2403,20 @@
         "name": str,
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
     _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
     "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
         "domain": str,
         "taskList": TaskListTypeDef,
     },
 )
@@ -2631,26 +2427,24 @@
         "reverseOrder": bool,
         "startAtPreviousStartedEvent": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
     _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
 ):
     pass
 
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "tags": List[ResourceTagOutputTypeDef],
+        "tags": List[ResourceTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
@@ -2663,21 +2457,19 @@
     {
         "description": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
-
 class RegisterDomainInputRequestTypeDef(
     _RequiredRegisterDomainInputRequestTypeDef, _OptionalRegisterDomainInputRequestTypeDef
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
 )
@@ -2696,14 +2488,57 @@
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDecisionTypeDef = TypedDict(
+    "_RequiredDecisionTypeDef",
+    {
+        "decisionType": DecisionTypeType,
+    },
+)
+_OptionalDecisionTypeDef = TypedDict(
+    "_OptionalDecisionTypeDef",
+    {
+        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
+        "requestCancelActivityTaskDecisionAttributes": (
+            RequestCancelActivityTaskDecisionAttributesTypeDef
+        ),
+        "completeWorkflowExecutionDecisionAttributes": (
+            CompleteWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
+        "cancelWorkflowExecutionDecisionAttributes": (
+            CancelWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionDecisionAttributes": (
+            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
+        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
+        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
+        "signalExternalWorkflowExecutionDecisionAttributes": (
+            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
+            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "startChildWorkflowExecutionDecisionAttributes": (
+            StartChildWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
+    },
+    total=False,
+)
+
+class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
+    pass
+
 WorkflowExecutionDetailTypeDef = TypedDict(
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
@@ -2838,19 +2673,17 @@
             ScheduleLambdaFunctionFailedEventAttributesTypeDef
         ),
         "startLambdaFunctionFailedEventAttributes": StartLambdaFunctionFailedEventAttributesTypeDef,
     },
     total=False,
 )
 
-
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
-
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2861,66 +2694,42 @@
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDecisionTypeDef = TypedDict(
-    "_RequiredDecisionTypeDef",
+_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
-        "decisionType": DecisionTypeType,
+        "taskToken": str,
     },
 )
-_OptionalDecisionTypeDef = TypedDict(
-    "_OptionalDecisionTypeDef",
+_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
     {
-        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
-        "requestCancelActivityTaskDecisionAttributes": (
-            RequestCancelActivityTaskDecisionAttributesTypeDef
-        ),
-        "completeWorkflowExecutionDecisionAttributes": (
-            CompleteWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
-        "cancelWorkflowExecutionDecisionAttributes": (
-            CancelWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "continueAsNewWorkflowExecutionDecisionAttributes": (
-            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
-        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
-        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
-        "signalExternalWorkflowExecutionDecisionAttributes": (
-            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
-            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "startChildWorkflowExecutionDecisionAttributes": (
-            StartChildWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
+        "decisions": Sequence[DecisionTypeDef],
+        "executionContext": str,
     },
     total=False,
 )
 
-
-class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
+class RespondDecisionTaskCompletedInputRequestTypeDef(
+    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
+    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
+):
     pass
 
-
 DecisionTaskTypeDef = TypedDict(
     "DecisionTaskTypeDef",
     {
         "taskToken": str,
         "startedEventId": int,
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2928,29 +2737,7 @@
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
-    {
-        "taskToken": str,
-    },
-)
-_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
-    {
-        "decisions": Sequence[DecisionTypeDef],
-        "executionContext": str,
-    },
-    total=False,
-)
-
-
-class RespondDecisionTaskCompletedInputRequestTypeDef(
-    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
-    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
-):
-    pass
```

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf/type_defs.pyi` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,35 +43,34 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
-    "ActivityTypeOutputTypeDef",
-    "TaskListOutputTypeDef",
+    "ActivityTypeTypeDef",
+    "TaskListTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
     "ResponseMetadataTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
-    "WorkflowExecutionOutputTypeDef",
-    "ActivityTypeTypeDef",
+    "WorkflowExecutionTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
-    "WorkflowTypeOutputTypeDef",
+    "WorkflowTypeTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
-    "TaskListTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
@@ -80,17 +79,15 @@
     "RecordMarkerDecisionAttributesTypeDef",
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     "RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef",
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
-    "WorkflowTypeTypeDef",
     "DescribeDomainInputRequestTypeDef",
-    "WorkflowExecutionTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
@@ -113,101 +110,100 @@
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     "ListActivityTypesInputRequestTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResourceTagOutputTypeDef",
+    "ResourceTagTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
-    "ResourceTagTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
+    "DeprecateActivityTypeInputRequestTypeDef",
+    "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
+    "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    "CountPendingActivityTasksInputRequestTypeDef",
+    "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
+    "PollForActivityTaskInputRequestTypeDef",
+    "PollForDecisionTaskInputRequestTypeDef",
+    "RegisterActivityTypeInputRequestTypeDef",
+    "RegisterWorkflowTypeInputRequestTypeDef",
+    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
     "ActivityTaskStatusTypeDef",
     "EmptyResponseMetadataTypeDef",
     "PendingTaskCountTypeDef",
     "RunTypeDef",
     "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
+    "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
+    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
-    "DeprecateActivityTypeInputRequestTypeDef",
-    "DescribeActivityTypeInputRequestTypeDef",
-    "UndeprecateActivityTypeInputRequestTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    "DescribeWorkflowTypeInputRequestTypeDef",
+    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
     "StartChildWorkflowExecutionFailedEventAttributesTypeDef",
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
+    "StartWorkflowExecutionInputRequestTypeDef",
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    "CountPendingActivityTasksInputRequestTypeDef",
-    "CountPendingDecisionTasksInputRequestTypeDef",
-    "PollForActivityTaskInputRequestTypeDef",
-    "PollForDecisionTaskInputRequestTypeDef",
-    "RegisterActivityTypeInputRequestTypeDef",
-    "RegisterWorkflowTypeInputRequestTypeDef",
-    "ScheduleActivityTaskDecisionAttributesTypeDef",
     "CountClosedWorkflowExecutionsInputRequestTypeDef",
     "CountOpenWorkflowExecutionsInputRequestTypeDef",
     "ListClosedWorkflowExecutionsInputRequestTypeDef",
     "ListOpenWorkflowExecutionsInputRequestTypeDef",
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    "StartChildWorkflowExecutionDecisionAttributesTypeDef",
-    "StartWorkflowExecutionInputRequestTypeDef",
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
-    "DescribeWorkflowExecutionInputRequestTypeDef",
-    "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
     "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListDomainsInputListDomainsPaginateTypeDef",
     "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
+    "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
-    "DecisionTypeDef",
+    "RespondDecisionTaskCompletedInputRequestTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
-    "RespondDecisionTaskCompletedInputRequestTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "activityId": str,
@@ -226,20 +222,22 @@
     {
         "details": str,
         "latestCancelRequestedEventId": int,
     },
     total=False,
 )
 
+
 class ActivityTaskCanceledEventAttributesTypeDef(
     _RequiredActivityTaskCanceledEventAttributesTypeDef,
     _OptionalActivityTaskCanceledEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredActivityTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -247,20 +245,22 @@
     "_OptionalActivityTaskCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class ActivityTaskCompletedEventAttributesTypeDef(
     _RequiredActivityTaskCompletedEventAttributesTypeDef,
     _OptionalActivityTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -269,30 +269,32 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class ActivityTaskFailedEventAttributesTypeDef(
     _RequiredActivityTaskFailedEventAttributesTypeDef,
     _OptionalActivityTaskFailedEventAttributesTypeDef,
 ):
     pass
 
-ActivityTypeOutputTypeDef = TypedDict(
-    "ActivityTypeOutputTypeDef",
+
+ActivityTypeTypeDef = TypedDict(
+    "ActivityTypeTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-TaskListOutputTypeDef = TypedDict(
-    "TaskListOutputTypeDef",
+TaskListTypeDef = TypedDict(
+    "TaskListTypeDef",
     {
         "name": str,
     },
 )
 
 _RequiredActivityTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskStartedEventAttributesTypeDef",
@@ -304,20 +306,22 @@
     "_OptionalActivityTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
+
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -337,36 +341,30 @@
     "_OptionalActivityTaskTimedOutEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class ActivityTaskTimedOutEventAttributesTypeDef(
     _RequiredActivityTaskTimedOutEventAttributesTypeDef,
     _OptionalActivityTaskTimedOutEventAttributesTypeDef,
 ):
     pass
 
-WorkflowExecutionOutputTypeDef = TypedDict(
-    "WorkflowExecutionOutputTypeDef",
+
+WorkflowExecutionTypeDef = TypedDict(
+    "WorkflowExecutionTypeDef",
     {
         "workflowId": str,
         "runId": str,
     },
 )
 
-ActivityTypeTypeDef = TypedDict(
-    "ActivityTypeTypeDef",
-    {
-        "name": str,
-        "version": str,
-    },
-)
-
 CancelTimerDecisionAttributesTypeDef = TypedDict(
     "CancelTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
     },
 )
 
@@ -391,16 +389,16 @@
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CancelWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-WorkflowTypeOutputTypeDef = TypedDict(
-    "WorkflowTypeOutputTypeDef",
+WorkflowTypeTypeDef = TypedDict(
+    "WorkflowTypeTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
 CloseStatusFilterTypeDef = TypedDict(
@@ -422,21 +420,14 @@
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": CompleteWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-TaskListTypeDef = TypedDict(
-    "TaskListTypeDef",
-    {
-        "name": str,
-    },
-)
-
 ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -451,19 +442,21 @@
     "_OptionalExecutionTimeFilterTypeDef",
     {
         "latestDate": Union[datetime, str],
     },
     total=False,
 )
 
+
 class ExecutionTimeFilterTypeDef(
     _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
+
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -484,19 +477,21 @@
     "_OptionalWorkflowTypeFilterTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
+
 class WorkflowTypeFilterTypeDef(
     _RequiredWorkflowTypeFilterTypeDef, _OptionalWorkflowTypeFilterTypeDef
 ):
     pass
 
+
 _RequiredDecisionTaskCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -504,40 +499,44 @@
     "_OptionalDecisionTaskCompletedEventAttributesTypeDef",
     {
         "executionContext": str,
     },
     total=False,
 )
 
+
 class DecisionTaskCompletedEventAttributesTypeDef(
     _RequiredDecisionTaskCompletedEventAttributesTypeDef,
     _OptionalDecisionTaskCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 _OptionalDecisionTaskStartedEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskStartedEventAttributesTypeDef",
     {
         "identity": str,
     },
     total=False,
 )
 
+
 class DecisionTaskStartedEventAttributesTypeDef(
     _RequiredDecisionTaskStartedEventAttributesTypeDef,
     _OptionalDecisionTaskStartedEventAttributesTypeDef,
 ):
     pass
 
+
 DecisionTaskTimedOutEventAttributesTypeDef = TypedDict(
     "DecisionTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "scheduledEventId": int,
         "startedEventId": int,
     },
@@ -562,19 +561,21 @@
     "_OptionalRecordMarkerDecisionAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class RecordMarkerDecisionAttributesTypeDef(
     _RequiredRecordMarkerDecisionAttributesTypeDef, _OptionalRecordMarkerDecisionAttributesTypeDef
 ):
     pass
 
+
 RequestCancelActivityTaskDecisionAttributesTypeDef = TypedDict(
     "RequestCancelActivityTaskDecisionAttributesTypeDef",
     {
         "activityId": str,
     },
 )
 
@@ -589,20 +590,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
+
 _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef = TypedDict(
     "_RequiredScheduleLambdaFunctionDecisionAttributesTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
@@ -612,20 +615,22 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
+
 class ScheduleLambdaFunctionDecisionAttributesTypeDef(
     _RequiredScheduleLambdaFunctionDecisionAttributesTypeDef,
     _OptionalScheduleLambdaFunctionDecisionAttributesTypeDef,
 ):
     pass
 
+
 _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
     },
 )
@@ -635,20 +640,22 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
+
 class SignalExternalWorkflowExecutionDecisionAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionDecisionAttributesTypeDef,
 ):
     pass
 
+
 _RequiredStartTimerDecisionAttributesTypeDef = TypedDict(
     "_RequiredStartTimerDecisionAttributesTypeDef",
     {
         "timerId": str,
         "startToFireTimeout": str,
     },
 )
@@ -656,49 +663,35 @@
     "_OptionalStartTimerDecisionAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
+
 class StartTimerDecisionAttributesTypeDef(
     _RequiredStartTimerDecisionAttributesTypeDef, _OptionalStartTimerDecisionAttributesTypeDef
 ):
     pass
 
+
 DeprecateDomainInputRequestTypeDef = TypedDict(
     "DeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
-WorkflowTypeTypeDef = TypedDict(
-    "WorkflowTypeTypeDef",
-    {
-        "name": str,
-        "version": str,
-    },
-)
-
 DescribeDomainInputRequestTypeDef = TypedDict(
     "DescribeDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
-WorkflowExecutionTypeDef = TypedDict(
-    "WorkflowExecutionTypeDef",
-    {
-        "workflowId": str,
-        "runId": str,
-    },
-)
-
 DomainConfigurationTypeDef = TypedDict(
     "DomainConfigurationTypeDef",
     {
         "workflowExecutionRetentionPeriodInDays": str,
     },
 )
 
@@ -714,17 +707,19 @@
     {
         "description": str,
         "arn": str,
     },
     total=False,
 )
 
+
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
+
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -750,20 +745,22 @@
     "_OptionalLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class LambdaFunctionCompletedEventAttributesTypeDef(
     _RequiredLambdaFunctionCompletedEventAttributesTypeDef,
     _OptionalLambdaFunctionCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -772,20 +769,22 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class LambdaFunctionFailedEventAttributesTypeDef(
     _RequiredLambdaFunctionFailedEventAttributesTypeDef,
     _OptionalLambdaFunctionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredLambdaFunctionScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -796,20 +795,22 @@
         "control": str,
         "input": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
+
 class LambdaFunctionScheduledEventAttributesTypeDef(
     _RequiredLambdaFunctionScheduledEventAttributesTypeDef,
     _OptionalLambdaFunctionScheduledEventAttributesTypeDef,
 ):
     pass
 
+
 LambdaFunctionStartedEventAttributesTypeDef = TypedDict(
     "LambdaFunctionStartedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
     },
 )
 
@@ -824,20 +825,22 @@
     "_OptionalLambdaFunctionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
     },
     total=False,
 )
 
+
 class LambdaFunctionTimedOutEventAttributesTypeDef(
     _RequiredLambdaFunctionTimedOutEventAttributesTypeDef,
     _OptionalLambdaFunctionTimedOutEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredMarkerRecordedEventAttributesTypeDef = TypedDict(
     "_RequiredMarkerRecordedEventAttributesTypeDef",
     {
         "markerName": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -845,19 +848,21 @@
     "_OptionalMarkerRecordedEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class MarkerRecordedEventAttributesTypeDef(
     _RequiredMarkerRecordedEventAttributesTypeDef, _OptionalMarkerRecordedEventAttributesTypeDef
 ):
     pass
 
+
 RecordMarkerFailedEventAttributesTypeDef = TypedDict(
     "RecordMarkerFailedEventAttributesTypeDef",
     {
         "markerName": str,
         "cause": Literal["OPERATION_NOT_PERMITTED"],
         "decisionTaskCompletedEventId": int,
     },
@@ -886,20 +891,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -908,20 +915,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalRequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
+
 ScheduleLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "ScheduleLambdaFunctionFailedEventAttributesTypeDef",
     {
         "id": str,
         "name": str,
         "cause": ScheduleLambdaFunctionFailedCauseType,
         "decisionTaskCompletedEventId": int,
@@ -942,20 +951,22 @@
     {
         "runId": str,
         "control": str,
     },
     total=False,
 )
 
+
 class SignalExternalWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
         "signalName": str,
         "decisionTaskCompletedEventId": int,
     },
@@ -966,20 +977,22 @@
         "runId": str,
         "input": str,
         "control": str,
     },
     total=False,
 )
 
+
 class SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalSignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
+
 StartLambdaFunctionFailedEventAttributesTypeDef = TypedDict(
     "StartLambdaFunctionFailedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "cause": Literal["ASSUME_ROLE_FAILED"],
         "message": str,
     },
@@ -1024,59 +1037,65 @@
     "_OptionalTimerStartedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
+
 class TimerStartedEventAttributesTypeDef(
     _RequiredTimerStartedEventAttributesTypeDef, _OptionalTimerStartedEventAttributesTypeDef
 ):
     pass
 
+
 _RequiredWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
@@ -1084,20 +1103,22 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
@@ -1106,20 +1127,22 @@
         "reason": str,
         "details": str,
         "cause": WorkflowExecutionTerminatedCauseType,
     },
     total=False,
 )
 
+
 class WorkflowExecutionTerminatedEventAttributesTypeDef(
     _RequiredWorkflowExecutionTerminatedEventAttributesTypeDef,
     _OptionalWorkflowExecutionTerminatedEventAttributesTypeDef,
 ):
     pass
 
+
 WorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
@@ -1138,19 +1161,21 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
+
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputRequestTypeDef = TypedDict(
@@ -1159,45 +1184,47 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
+
 class ListDomainsInputRequestTypeDef(
     _RequiredListDomainsInputRequestTypeDef, _OptionalListDomainsInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredResourceTagOutputTypeDef = TypedDict(
-    "_RequiredResourceTagOutputTypeDef",
+_RequiredResourceTagTypeDef = TypedDict(
+    "_RequiredResourceTagTypeDef",
     {
         "key": str,
     },
 )
-_OptionalResourceTagOutputTypeDef = TypedDict(
-    "_OptionalResourceTagOutputTypeDef",
+_OptionalResourceTagTypeDef = TypedDict(
+    "_OptionalResourceTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-class ResourceTagOutputTypeDef(
-    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
-):
+
+class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1208,55 +1235,42 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
+
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
 ):
     pass
 
+
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_OptionalRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class RecordActivityTaskHeartbeatInputRequestTypeDef(
     _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef,
     _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef,
 ):
     pass
 
-_RequiredResourceTagTypeDef = TypedDict(
-    "_RequiredResourceTagTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalResourceTagTypeDef = TypedDict(
-    "_OptionalResourceTagTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
-    pass
 
 _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
@@ -1265,60 +1279,66 @@
     "_OptionalRequestCancelWorkflowExecutionInputRequestTypeDef",
     {
         "runId": str,
     },
     total=False,
 )
 
+
 class RequestCancelWorkflowExecutionInputRequestTypeDef(
     _RequiredRequestCancelWorkflowExecutionInputRequestTypeDef,
     _OptionalRequestCancelWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCanceledInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCanceledInputRequestTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class RespondActivityTaskCanceledInputRequestTypeDef(
     _RequiredRespondActivityTaskCanceledInputRequestTypeDef,
     _OptionalRespondActivityTaskCanceledInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskCompletedInputRequestTypeDef = TypedDict(
     "_OptionalRespondActivityTaskCompletedInputRequestTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class RespondActivityTaskCompletedInputRequestTypeDef(
     _RequiredRespondActivityTaskCompletedInputRequestTypeDef,
     _OptionalRespondActivityTaskCompletedInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
     "_RequiredRespondActivityTaskFailedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondActivityTaskFailedInputRequestTypeDef = TypedDict(
@@ -1326,20 +1346,22 @@
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
     },
@@ -1349,20 +1371,22 @@
     {
         "runId": str,
         "input": str,
     },
     total=False,
 )
 
+
 class SignalWorkflowExecutionInputRequestTypeDef(
     _RequiredSignalWorkflowExecutionInputRequestTypeDef,
     _OptionalSignalWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredTerminateWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredTerminateWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
     },
 )
@@ -1373,20 +1397,22 @@
         "reason": str,
         "details": str,
         "childPolicy": ChildPolicyType,
     },
     total=False,
 )
 
+
 class TerminateWorkflowExecutionInputRequestTypeDef(
     _RequiredTerminateWorkflowExecutionInputRequestTypeDef,
     _OptionalTerminateWorkflowExecutionInputRequestTypeDef,
 ):
     pass
 
+
 UndeprecateDomainInputRequestTypeDef = TypedDict(
     "UndeprecateDomainInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -1411,55 +1437,83 @@
     "_OptionalWorkflowExecutionOpenCountsTypeDef",
     {
         "openLambdaFunctions": int,
     },
     total=False,
 )
 
+
 class WorkflowExecutionOpenCountsTypeDef(
     _RequiredWorkflowExecutionOpenCountsTypeDef, _OptionalWorkflowExecutionOpenCountsTypeDef
 ):
     pass
 
+
 _RequiredActivityTypeInfoTypeDef = TypedDict(
     "_RequiredActivityTypeInfoTypeDef",
     {
-        "activityType": ActivityTypeOutputTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalActivityTypeInfoTypeDef = TypedDict(
     "_OptionalActivityTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
+
 class ActivityTypeInfoTypeDef(_RequiredActivityTypeInfoTypeDef, _OptionalActivityTypeInfoTypeDef):
     pass
 
+
+DeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "DeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
+DescribeActivityTypeInputRequestTypeDef = TypedDict(
+    "DescribeActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
 ScheduleActivityTaskFailedEventAttributesTypeDef = TypedDict(
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeOutputTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "activityId": str,
         "cause": ScheduleActivityTaskFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
+UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "activityType": ActivityTypeTypeDef,
+    },
+)
+
 _RequiredActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskScheduledEventAttributesTypeDef",
     {
-        "activityType": ActivityTypeOutputTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "activityId": str,
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalActivityTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalActivityTaskScheduledEventAttributesTypeDef",
     {
         "input": str,
@@ -1469,83 +1523,259 @@
         "startToCloseTimeout": str,
         "taskPriority": str,
         "heartbeatTimeout": str,
     },
     total=False,
 )
 
+
 class ActivityTaskScheduledEventAttributesTypeDef(
     _RequiredActivityTaskScheduledEventAttributesTypeDef,
     _OptionalActivityTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
+
 ActivityTypeConfigurationTypeDef = TypedDict(
     "ActivityTypeConfigurationTypeDef",
     {
         "defaultTaskStartToCloseTimeout": str,
         "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListOutputTypeDef,
+        "defaultTaskList": TaskListTypeDef,
         "defaultTaskPriority": str,
         "defaultTaskScheduleToStartTimeout": str,
         "defaultTaskScheduleToCloseTimeout": str,
     },
     total=False,
 )
 
+ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "workflowTypeVersion": str,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+CountPendingActivityTasksInputRequestTypeDef = TypedDict(
+    "CountPendingActivityTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
+CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
+    "CountPendingDecisionTasksInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+
 _RequiredDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_RequiredDecisionTaskScheduledEventAttributesTypeDef",
     {
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
     },
 )
 _OptionalDecisionTaskScheduledEventAttributesTypeDef = TypedDict(
     "_OptionalDecisionTaskScheduledEventAttributesTypeDef",
     {
         "taskPriority": str,
         "startToCloseTimeout": str,
     },
     total=False,
 )
 
+
 class DecisionTaskScheduledEventAttributesTypeDef(
     _RequiredDecisionTaskScheduledEventAttributesTypeDef,
     _OptionalDecisionTaskScheduledEventAttributesTypeDef,
 ):
     pass
 
+
+_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForActivityTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForActivityTaskInputRequestTypeDef",
+    {
+        "identity": str,
+    },
+    total=False,
+)
+
+
+class PollForActivityTaskInputRequestTypeDef(
+    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
+):
+    pass
+
+
+_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputRequestTypeDef",
+    {
+        "domain": str,
+        "taskList": TaskListTypeDef,
+    },
+)
+_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputRequestTypeDef",
+    {
+        "identity": str,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+    },
+    total=False,
+)
+
+
+class PollForDecisionTaskInputRequestTypeDef(
+    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
+):
+    pass
+
+
+_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterActivityTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterActivityTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultTaskHeartbeatTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultTaskScheduleToStartTimeout": str,
+        "defaultTaskScheduleToCloseTimeout": str,
+    },
+    total=False,
+)
+
+
+class RegisterActivityTypeInputRequestTypeDef(
+    _RequiredRegisterActivityTypeInputRequestTypeDef,
+    _OptionalRegisterActivityTypeInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "name": str,
+        "version": str,
+    },
+)
+_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
+    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
+    {
+        "description": str,
+        "defaultTaskStartToCloseTimeout": str,
+        "defaultExecutionStartToCloseTimeout": str,
+        "defaultTaskList": TaskListTypeDef,
+        "defaultTaskPriority": str,
+        "defaultChildPolicy": ChildPolicyType,
+        "defaultLambdaRole": str,
+    },
+    total=False,
+)
+
+
+class RegisterWorkflowTypeInputRequestTypeDef(
+    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
+    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "activityType": ActivityTypeTypeDef,
+        "activityId": str,
+    },
+)
+_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
+    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "scheduleToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "scheduleToStartTimeout": str,
+        "startToCloseTimeout": str,
+        "heartbeatTimeout": str,
+    },
+    total=False,
+)
+
+
+class ScheduleActivityTaskDecisionAttributesTypeDef(
+    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
+    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
+):
+    pass
+
+
 _RequiredWorkflowExecutionConfigurationTypeDef = TypedDict(
     "_RequiredWorkflowExecutionConfigurationTypeDef",
     {
         "taskStartToCloseTimeout": str,
         "executionStartToCloseTimeout": str,
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalWorkflowExecutionConfigurationTypeDef = TypedDict(
     "_OptionalWorkflowExecutionConfigurationTypeDef",
     {
         "taskPriority": str,
         "lambdaRole": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionConfigurationTypeDef(
     _RequiredWorkflowExecutionConfigurationTypeDef, _OptionalWorkflowExecutionConfigurationTypeDef
 ):
     pass
 
+
 WorkflowTypeConfigurationTypeDef = TypedDict(
     "WorkflowTypeConfigurationTypeDef",
     {
         "defaultTaskStartToCloseTimeout": str,
         "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListOutputTypeDef,
+        "defaultTaskList": TaskListTypeDef,
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
@@ -1592,41 +1822,74 @@
 
 ActivityTaskTypeDef = TypedDict(
     "ActivityTaskTypeDef",
     {
         "taskToken": str,
         "activityId": str,
         "startedEventId": int,
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "activityType": ActivityTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "activityType": ActivityTypeTypeDef,
         "input": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+
 ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
 ExternalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
+_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "domain": str,
+        "execution": WorkflowExecutionTypeDef,
+    },
+)
+_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
+    {
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+
+class GetWorkflowExecutionHistoryInputRequestTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
+):
+    pass
+
+
 WorkflowExecutionCancelRequestedEventAttributesTypeDef = TypedDict(
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     {
-        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionTypeDef,
         "externalInitiatedEventId": int,
         "cause": Literal["CHILD_POLICY_APPLIED"],
     },
     total=False,
 )
 
 _RequiredWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
@@ -1635,180 +1898,213 @@
         "signalName": str,
     },
 )
 _OptionalWorkflowExecutionSignaledEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "input": str,
-        "externalWorkflowExecution": WorkflowExecutionOutputTypeDef,
+        "externalWorkflowExecution": WorkflowExecutionTypeDef,
         "externalInitiatedEventId": int,
     },
     total=False,
 )
 
+
 class WorkflowExecutionSignaledEventAttributesTypeDef(
     _RequiredWorkflowExecutionSignaledEventAttributesTypeDef,
     _OptionalWorkflowExecutionSignaledEventAttributesTypeDef,
 ):
     pass
 
-DeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "DeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
-DescribeActivityTypeInputRequestTypeDef = TypedDict(
-    "DescribeActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
-
-UndeprecateActivityTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "activityType": ActivityTypeTypeDef,
-    },
-)
 
 _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef",
     {
         "details": str,
     },
     total=False,
 )
 
+
 class ChildWorkflowExecutionCanceledEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCanceledEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCanceledEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef",
     {
         "result": str,
     },
     total=False,
 )
 
+
 class ChildWorkflowExecutionCompletedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionCompletedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionCompletedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "reason": str,
         "details": str,
     },
     total=False,
 )
 
+
 class ChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 ChildWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTerminatedEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTerminatedEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
 ChildWorkflowExecutionTimedOutEventAttributesTypeDef = TypedDict(
     "ChildWorkflowExecutionTimedOutEventAttributesTypeDef",
     {
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "timeoutType": Literal["START_TO_CLOSE"],
         "initiatedEventId": int,
         "startedEventId": int,
     },
 )
 
+DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
+    "DescribeWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
+_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "workflowType": WorkflowTypeTypeDef,
+        "workflowId": str,
+    },
+)
+_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
+    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
+    {
+        "control": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "tagList": Sequence[str],
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+
+class StartChildWorkflowExecutionDecisionAttributesTypeDef(
+    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
+    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
+):
+    pass
+
+
 _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "cause": StartChildWorkflowExecutionFailedCauseType,
         "workflowId": str,
         "initiatedEventId": int,
         "decisionTaskCompletedEventId": int,
     },
 )
 _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "control": str,
     },
     total=False,
 )
 
+
 class StartChildWorkflowExecutionFailedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionFailedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionFailedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
         "workflowId": str,
-        "workflowType": WorkflowTypeOutputTypeDef,
-        "taskList": TaskListOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
+        "taskList": TaskListTypeDef,
         "decisionTaskCompletedEventId": int,
         "childPolicy": ChildPolicyType,
     },
 )
 _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef = TypedDict(
     "_OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     {
@@ -1819,28 +2115,69 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
+
 class StartChildWorkflowExecutionInitiatedEventAttributesTypeDef(
     _RequiredStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     _OptionalStartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
 ):
     pass
 
+
+_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowId": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
+    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
+    {
+        "taskList": TaskListTypeDef,
+        "taskPriority": str,
+        "input": str,
+        "executionStartToCloseTimeout": str,
+        "tagList": Sequence[str],
+        "taskStartToCloseTimeout": str,
+        "childPolicy": ChildPolicyType,
+        "lambdaRole": str,
+    },
+    total=False,
+)
+
+
+class StartWorkflowExecutionInputRequestTypeDef(
+    _RequiredStartWorkflowExecutionInputRequestTypeDef,
+    _OptionalStartWorkflowExecutionInputRequestTypeDef,
+):
+    pass
+
+
+UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
+    "UndeprecateWorkflowTypeInputRequestTypeDef",
+    {
+        "domain": str,
+        "workflowType": WorkflowTypeTypeDef,
+    },
+)
+
 _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "decisionTaskCompletedEventId": int,
         "newExecutionRunId": str,
-        "taskList": TaskListOutputTypeDef,
+        "taskList": TaskListTypeDef,
         "childPolicy": ChildPolicyType,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
     },
 )
 _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
@@ -1848,255 +2185,103 @@
         "taskStartToCloseTimeout": str,
         "tagList": List[str],
         "lambdaRole": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionContinuedAsNewEventAttributesTypeDef(
     _RequiredWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     _OptionalWorkflowExecutionContinuedAsNewEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowExecutionInfoTypeDef = TypedDict(
     "_RequiredWorkflowExecutionInfoTypeDef",
     {
-        "execution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "execution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "startTimestamp": datetime,
         "executionStatus": ExecutionStatusType,
     },
 )
 _OptionalWorkflowExecutionInfoTypeDef = TypedDict(
     "_OptionalWorkflowExecutionInfoTypeDef",
     {
         "closeTimestamp": datetime,
         "closeStatus": CloseStatusType,
-        "parent": WorkflowExecutionOutputTypeDef,
+        "parent": WorkflowExecutionTypeDef,
         "tagList": List[str],
         "cancelRequested": bool,
     },
     total=False,
 )
 
+
 class WorkflowExecutionInfoTypeDef(
     _RequiredWorkflowExecutionInfoTypeDef, _OptionalWorkflowExecutionInfoTypeDef
 ):
     pass
 
+
 _RequiredWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_RequiredWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "childPolicy": ChildPolicyType,
-        "taskList": TaskListOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "taskList": TaskListTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
     },
 )
 _OptionalWorkflowExecutionStartedEventAttributesTypeDef = TypedDict(
     "_OptionalWorkflowExecutionStartedEventAttributesTypeDef",
     {
         "input": str,
         "executionStartToCloseTimeout": str,
         "taskStartToCloseTimeout": str,
         "taskPriority": str,
         "tagList": List[str],
         "continuedExecutionRunId": str,
-        "parentWorkflowExecution": WorkflowExecutionOutputTypeDef,
+        "parentWorkflowExecution": WorkflowExecutionTypeDef,
         "parentInitiatedEventId": int,
         "lambdaRole": str,
     },
     total=False,
 )
 
+
 class WorkflowExecutionStartedEventAttributesTypeDef(
     _RequiredWorkflowExecutionStartedEventAttributesTypeDef,
     _OptionalWorkflowExecutionStartedEventAttributesTypeDef,
 ):
     pass
 
+
 _RequiredWorkflowTypeInfoTypeDef = TypedDict(
     "_RequiredWorkflowTypeInfoTypeDef",
     {
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "status": RegistrationStatusType,
         "creationDate": datetime,
     },
 )
 _OptionalWorkflowTypeInfoTypeDef = TypedDict(
     "_OptionalWorkflowTypeInfoTypeDef",
     {
         "description": str,
         "deprecationDate": datetime,
     },
     total=False,
 )
 
-class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
-    pass
-
-ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "workflowTypeVersion": str,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-CountPendingActivityTasksInputRequestTypeDef = TypedDict(
-    "CountPendingActivityTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
 
-CountPendingDecisionTasksInputRequestTypeDef = TypedDict(
-    "CountPendingDecisionTasksInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-
-_RequiredPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForActivityTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForActivityTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForActivityTaskInputRequestTypeDef",
-    {
-        "identity": str,
-    },
-    total=False,
-)
-
-class PollForActivityTaskInputRequestTypeDef(
-    _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
-):
-    pass
-
-_RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputRequestTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForDecisionTaskInputRequestTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputRequestTypeDef",
-    {
-        "identity": str,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-    },
-    total=False,
-)
-
-class PollForDecisionTaskInputRequestTypeDef(
-    _RequiredPollForDecisionTaskInputRequestTypeDef, _OptionalPollForDecisionTaskInputRequestTypeDef
-):
-    pass
-
-_RequiredRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterActivityTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterActivityTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterActivityTypeInputRequestTypeDef",
-    {
-        "description": str,
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultTaskHeartbeatTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultTaskScheduleToStartTimeout": str,
-        "defaultTaskScheduleToCloseTimeout": str,
-    },
-    total=False,
-)
-
-class RegisterActivityTypeInputRequestTypeDef(
-    _RequiredRegisterActivityTypeInputRequestTypeDef,
-    _OptionalRegisterActivityTypeInputRequestTypeDef,
-):
+class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
-_RequiredRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_RequiredRegisterWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "name": str,
-        "version": str,
-    },
-)
-_OptionalRegisterWorkflowTypeInputRequestTypeDef = TypedDict(
-    "_OptionalRegisterWorkflowTypeInputRequestTypeDef",
-    {
-        "description": str,
-        "defaultTaskStartToCloseTimeout": str,
-        "defaultExecutionStartToCloseTimeout": str,
-        "defaultTaskList": TaskListTypeDef,
-        "defaultTaskPriority": str,
-        "defaultChildPolicy": ChildPolicyType,
-        "defaultLambdaRole": str,
-    },
-    total=False,
-)
-
-class RegisterWorkflowTypeInputRequestTypeDef(
-    _RequiredRegisterWorkflowTypeInputRequestTypeDef,
-    _OptionalRegisterWorkflowTypeInputRequestTypeDef,
-):
-    pass
-
-_RequiredScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_RequiredScheduleActivityTaskDecisionAttributesTypeDef",
-    {
-        "activityType": ActivityTypeTypeDef,
-        "activityId": str,
-    },
-)
-_OptionalScheduleActivityTaskDecisionAttributesTypeDef = TypedDict(
-    "_OptionalScheduleActivityTaskDecisionAttributesTypeDef",
-    {
-        "control": str,
-        "input": str,
-        "scheduleToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "scheduleToStartTimeout": str,
-        "startToCloseTimeout": str,
-        "heartbeatTimeout": str,
-    },
-    total=False,
-)
-
-class ScheduleActivityTaskDecisionAttributesTypeDef(
-    _RequiredScheduleActivityTaskDecisionAttributesTypeDef,
-    _OptionalScheduleActivityTaskDecisionAttributesTypeDef,
-):
-    pass
 
 _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
@@ -2109,20 +2294,22 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "closeStatusFilter": CloseStatusFilterTypeDef,
     },
     total=False,
 )
 
+
 class CountClosedWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2132,20 +2319,22 @@
         "typeFilter": WorkflowTypeFilterTypeDef,
         "tagFilter": TagFilterTypeDef,
         "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
+
 class CountOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
@@ -2160,20 +2349,22 @@
         "nextPageToken": str,
         "maximumPageSize": int,
         "reverseOrder": bool,
     },
     total=False,
 )
 
+
 class ListClosedWorkflowExecutionsInputRequestTypeDef(
     _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
     _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2186,132 +2377,21 @@
         "maximumPageSize": int,
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
     },
     total=False,
 )
 
+
 class ListOpenWorkflowExecutionsInputRequestTypeDef(
     _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
     _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
 ):
     pass
 
-DeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-DescribeWorkflowTypeInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "workflowType": WorkflowTypeTypeDef,
-        "workflowId": str,
-    },
-)
-_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef = TypedDict(
-    "_OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef",
-    {
-        "control": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "tagList": Sequence[str],
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-class StartChildWorkflowExecutionDecisionAttributesTypeDef(
-    _RequiredStartChildWorkflowExecutionDecisionAttributesTypeDef,
-    _OptionalStartChildWorkflowExecutionDecisionAttributesTypeDef,
-):
-    pass
-
-_RequiredStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_RequiredStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowId": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-_OptionalStartWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "_OptionalStartWorkflowExecutionInputRequestTypeDef",
-    {
-        "taskList": TaskListTypeDef,
-        "taskPriority": str,
-        "input": str,
-        "executionStartToCloseTimeout": str,
-        "tagList": Sequence[str],
-        "taskStartToCloseTimeout": str,
-        "childPolicy": ChildPolicyType,
-        "lambdaRole": str,
-    },
-    total=False,
-)
-
-class StartWorkflowExecutionInputRequestTypeDef(
-    _RequiredStartWorkflowExecutionInputRequestTypeDef,
-    _OptionalStartWorkflowExecutionInputRequestTypeDef,
-):
-    pass
-
-UndeprecateWorkflowTypeInputRequestTypeDef = TypedDict(
-    "UndeprecateWorkflowTypeInputRequestTypeDef",
-    {
-        "domain": str,
-        "workflowType": WorkflowTypeTypeDef,
-    },
-)
-
-DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
-    "DescribeWorkflowExecutionInputRequestTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-
-_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputRequestTypeDef",
-    {
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-    },
-    total=False,
-)
-
-class GetWorkflowExecutionHistoryInputRequestTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputRequestTypeDef,
-):
-    pass
 
 DomainDetailTypeDef = TypedDict(
     "DomainDetailTypeDef",
     {
         "domainInfo": DomainInfoTypeDef,
         "configuration": DomainConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2339,20 +2419,22 @@
     {
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
     _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
     "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -2362,20 +2444,22 @@
         "name": str,
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListActivityTypesInputListActivityTypesPaginateTypeDef(
     _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
     _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
@@ -2389,20 +2473,22 @@
         "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
     _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
     "_RequiredListDomainsInputListDomainsPaginateTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
@@ -2410,20 +2496,22 @@
     {
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDomainsInputListDomainsPaginateTypeDef(
     _RequiredListDomainsInputListDomainsPaginateTypeDef,
     _OptionalListDomainsInputListDomainsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     {
         "domain": str,
         "startTimeFilter": ExecutionTimeFilterTypeDef,
     },
 )
@@ -2435,20 +2523,22 @@
         "reverseOrder": bool,
         "executionFilter": WorkflowExecutionFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
     _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -2458,20 +2548,22 @@
         "name": str,
         "reverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
     _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
     "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
         "domain": str,
         "taskList": TaskListTypeDef,
     },
 )
@@ -2482,24 +2574,26 @@
         "reverseOrder": bool,
         "startAtPreviousStartedEvent": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
     _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
 ):
     pass
 
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "tags": List[ResourceTagOutputTypeDef],
+        "tags": List[ResourceTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
@@ -2512,19 +2606,21 @@
     {
         "description": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
+
 class RegisterDomainInputRequestTypeDef(
     _RequiredRegisterDomainInputRequestTypeDef, _OptionalRegisterDomainInputRequestTypeDef
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[ResourceTagTypeDef],
     },
 )
@@ -2543,14 +2639,59 @@
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDecisionTypeDef = TypedDict(
+    "_RequiredDecisionTypeDef",
+    {
+        "decisionType": DecisionTypeType,
+    },
+)
+_OptionalDecisionTypeDef = TypedDict(
+    "_OptionalDecisionTypeDef",
+    {
+        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
+        "requestCancelActivityTaskDecisionAttributes": (
+            RequestCancelActivityTaskDecisionAttributesTypeDef
+        ),
+        "completeWorkflowExecutionDecisionAttributes": (
+            CompleteWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
+        "cancelWorkflowExecutionDecisionAttributes": (
+            CancelWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "continueAsNewWorkflowExecutionDecisionAttributes": (
+            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
+        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
+        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
+        "signalExternalWorkflowExecutionDecisionAttributes": (
+            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
+            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "startChildWorkflowExecutionDecisionAttributes": (
+            StartChildWorkflowExecutionDecisionAttributesTypeDef
+        ),
+        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
+    },
+    total=False,
+)
+
+
+class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
+    pass
+
+
 WorkflowExecutionDetailTypeDef = TypedDict(
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
@@ -2685,17 +2826,19 @@
             ScheduleLambdaFunctionFailedEventAttributesTypeDef
         ),
         "startLambdaFunctionFailedEventAttributes": StartLambdaFunctionFailedEventAttributesTypeDef,
     },
     total=False,
 )
 
+
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
+
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2706,64 +2849,44 @@
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDecisionTypeDef = TypedDict(
-    "_RequiredDecisionTypeDef",
+_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
-        "decisionType": DecisionTypeType,
+        "taskToken": str,
     },
 )
-_OptionalDecisionTypeDef = TypedDict(
-    "_OptionalDecisionTypeDef",
+_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
+    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
     {
-        "scheduleActivityTaskDecisionAttributes": ScheduleActivityTaskDecisionAttributesTypeDef,
-        "requestCancelActivityTaskDecisionAttributes": (
-            RequestCancelActivityTaskDecisionAttributesTypeDef
-        ),
-        "completeWorkflowExecutionDecisionAttributes": (
-            CompleteWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "failWorkflowExecutionDecisionAttributes": FailWorkflowExecutionDecisionAttributesTypeDef,
-        "cancelWorkflowExecutionDecisionAttributes": (
-            CancelWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "continueAsNewWorkflowExecutionDecisionAttributes": (
-            ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "recordMarkerDecisionAttributes": RecordMarkerDecisionAttributesTypeDef,
-        "startTimerDecisionAttributes": StartTimerDecisionAttributesTypeDef,
-        "cancelTimerDecisionAttributes": CancelTimerDecisionAttributesTypeDef,
-        "signalExternalWorkflowExecutionDecisionAttributes": (
-            SignalExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "requestCancelExternalWorkflowExecutionDecisionAttributes": (
-            RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "startChildWorkflowExecutionDecisionAttributes": (
-            StartChildWorkflowExecutionDecisionAttributesTypeDef
-        ),
-        "scheduleLambdaFunctionDecisionAttributes": ScheduleLambdaFunctionDecisionAttributesTypeDef,
+        "decisions": Sequence[DecisionTypeDef],
+        "executionContext": str,
     },
     total=False,
 )
 
-class DecisionTypeDef(_RequiredDecisionTypeDef, _OptionalDecisionTypeDef):
+
+class RespondDecisionTaskCompletedInputRequestTypeDef(
+    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
+    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
+):
     pass
 
+
 DecisionTaskTypeDef = TypedDict(
     "DecisionTaskTypeDef",
     {
         "taskToken": str,
         "startedEventId": int,
-        "workflowExecution": WorkflowExecutionOutputTypeDef,
-        "workflowType": WorkflowTypeOutputTypeDef,
+        "workflowExecution": WorkflowExecutionTypeDef,
+        "workflowType": WorkflowTypeTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2771,28 +2894,7 @@
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
-    {
-        "taskToken": str,
-    },
-)
-_OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
-    "_OptionalRespondDecisionTaskCompletedInputRequestTypeDef",
-    {
-        "decisions": Sequence[DecisionTypeDef],
-        "executionContext": str,
-    },
-    total=False,
-)
-
-class RespondDecisionTaskCompletedInputRequestTypeDef(
-    _RequiredRespondDecisionTaskCompletedInputRequestTypeDef,
-    _OptionalRespondDecisionTaskCompletedInputRequestTypeDef,
-):
-    pass
```

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/PKG-INFO` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.28.12
-Summary: Type annotations for boto3.SWF 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SWF 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -379,30 +379,28 @@
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
-    ActivityTypeOutputTypeDef,
-    TaskListOutputTypeDef,
+    ActivityTypeTypeDef,
+    TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
     ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
-    WorkflowExecutionOutputTypeDef,
-    ActivityTypeTypeDef,
+    WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
-    WorkflowTypeOutputTypeDef,
+    WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
-    TaskListTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
     ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
@@ -411,17 +409,15 @@
     RecordMarkerDecisionAttributesTypeDef,
     RequestCancelActivityTaskDecisionAttributesTypeDef,
     RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef,
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
-    WorkflowTypeTypeDef,
     DescribeDomainInputRequestTypeDef,
-    WorkflowExecutionTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
     PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
@@ -444,101 +440,100 @@
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
     ListActivityTypesInputRequestTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResourceTagOutputTypeDef,
+    ResourceTagTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
-    ResourceTagTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
+    DeprecateActivityTypeInputRequestTypeDef,
+    DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
+    UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
+    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
+    CountPendingActivityTasksInputRequestTypeDef,
+    CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
+    PollForActivityTaskInputRequestTypeDef,
+    PollForDecisionTaskInputRequestTypeDef,
+    RegisterActivityTypeInputRequestTypeDef,
+    RegisterWorkflowTypeInputRequestTypeDef,
+    ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
     ActivityTaskStatusTypeDef,
     EmptyResponseMetadataTypeDef,
     PendingTaskCountTypeDef,
     RunTypeDef,
     WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
+    DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
+    GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
-    DeprecateActivityTypeInputRequestTypeDef,
-    DescribeActivityTypeInputRequestTypeDef,
-    UndeprecateActivityTypeInputRequestTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
     ChildWorkflowExecutionTerminatedEventAttributesTypeDef,
     ChildWorkflowExecutionTimedOutEventAttributesTypeDef,
+    DeprecateWorkflowTypeInputRequestTypeDef,
+    DescribeWorkflowTypeInputRequestTypeDef,
+    StartChildWorkflowExecutionDecisionAttributesTypeDef,
     StartChildWorkflowExecutionFailedEventAttributesTypeDef,
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
+    StartWorkflowExecutionInputRequestTypeDef,
+    UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
-    CountPendingActivityTasksInputRequestTypeDef,
-    CountPendingDecisionTasksInputRequestTypeDef,
-    PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputRequestTypeDef,
-    RegisterActivityTypeInputRequestTypeDef,
-    RegisterWorkflowTypeInputRequestTypeDef,
-    ScheduleActivityTaskDecisionAttributesTypeDef,
     CountClosedWorkflowExecutionsInputRequestTypeDef,
     CountOpenWorkflowExecutionsInputRequestTypeDef,
     ListClosedWorkflowExecutionsInputRequestTypeDef,
     ListOpenWorkflowExecutionsInputRequestTypeDef,
-    DeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowTypeInputRequestTypeDef,
-    StartChildWorkflowExecutionDecisionAttributesTypeDef,
-    StartWorkflowExecutionInputRequestTypeDef,
-    UndeprecateWorkflowTypeInputRequestTypeDef,
-    DescribeWorkflowExecutionInputRequestTypeDef,
-    GetWorkflowExecutionHistoryInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
     GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListDomainsInputListDomainsPaginateTypeDef,
     ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
+    DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
-    DecisionTypeDef,
+    RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
-    RespondDecisionTaskCompletedInputRequestTypeDef,
 )
 
 
 def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-swf-1.28.12/mypy_boto3_swf.egg-info/SOURCES.txt` & `mypy-boto3-swf-1.28.15/mypy_boto3_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.12/setup.py` & `mypy-boto3-swf-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-swf",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SWF 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SWF 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

