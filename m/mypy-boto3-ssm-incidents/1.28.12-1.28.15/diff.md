# Comparing `tmp/mypy-boto3-ssm-incidents-1.28.12.tar.gz` & `tmp/mypy-boto3-ssm-incidents-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.12.tar", last modified: Thu Jul 27 11:49:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.15.tar", last modified: Fri Jul 28 20:43:48 2023, max compression
```

## Comparing `mypy-boto3-ssm-incidents-1.28.12.tar` & `mypy-boto3-ssm-incidents-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.165325 mypy-boto3-ssm-incidents-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-27 11:49:42.161325 mypy-boto3-ssm-incidents-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17261 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.153325 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38387 2023-07-27 11:47:32.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38315 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.161325 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:42.165325 mypy-boto3-ssm-incidents-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35552 2023-07-28 20:40:06.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35484 2023-07-28 20:40:06.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-28 20:40:05.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:48.000000 mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:48.757933 mypy-boto3-ssm-incidents-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:40:04.000000 mypy-boto3-ssm-incidents-1.28.15/setup.py
```

### Comparing `mypy-boto3-ssm-incidents-1.28.12/LICENSE` & `mypy-boto3-ssm-incidents-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.28.12
-Summary: Type annotations for boto3.SSMIncidents 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -400,36 +400,31 @@
     EventReferenceTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
-    DynamicSsmParameterValueOutputTypeDef,
     DynamicSsmParameterValueTypeDef,
-    EventReferenceOutputTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
     PaginatorConfigTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
-    NotificationTargetItemOutputTypeDef,
     NotificationTargetItemTypeDef,
-    PagerDutyIncidentDetailOutputTypeDef,
     PagerDutyIncidentDetailTypeDef,
     ListRelatedItemsInputRequestTypeDef,
     ListReplicationSetsInputRequestTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PagerDutyIncidentConfigurationOutputTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     RegionInfoTypeDef,
     TriggerDetailsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
@@ -439,59 +434,54 @@
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePolicyOutputTypeDef,
     StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
+    EventSummaryTypeDef,
+    TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
     SsmAutomationOutputTypeDef,
     SsmAutomationTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
     IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
-    ItemValueOutputTypeDef,
     ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
-    PagerDutyConfigurationOutputTypeDef,
     PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
+    ListTimelineEventsOutputTypeDef,
+    GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
-    ItemIdentifierOutputTypeDef,
     ItemIdentifierTypeDef,
-    IntegrationOutputTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
-    RelatedItemOutputTypeDef,
     RelatedItemTypeDef,
-    GetResponsePlanOutputTypeDef,
     CreateResponsePlanInputRequestTypeDef,
+    GetResponsePlanOutputTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-incidents-1.28.12/README.md` & `mypy-boto3-ssm-incidents-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,36 +368,31 @@
     EventReferenceTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
-    DynamicSsmParameterValueOutputTypeDef,
     DynamicSsmParameterValueTypeDef,
-    EventReferenceOutputTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
     PaginatorConfigTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
-    NotificationTargetItemOutputTypeDef,
     NotificationTargetItemTypeDef,
-    PagerDutyIncidentDetailOutputTypeDef,
     PagerDutyIncidentDetailTypeDef,
     ListRelatedItemsInputRequestTypeDef,
     ListReplicationSetsInputRequestTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PagerDutyIncidentConfigurationOutputTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     RegionInfoTypeDef,
     TriggerDetailsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
@@ -407,59 +402,54 @@
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePolicyOutputTypeDef,
     StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
+    EventSummaryTypeDef,
+    TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
     SsmAutomationOutputTypeDef,
     SsmAutomationTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
     IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
-    ItemValueOutputTypeDef,
     ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
-    PagerDutyConfigurationOutputTypeDef,
     PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
+    ListTimelineEventsOutputTypeDef,
+    GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
-    ItemIdentifierOutputTypeDef,
     ItemIdentifierTypeDef,
-    IntegrationOutputTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
-    RelatedItemOutputTypeDef,
     RelatedItemTypeDef,
-    GetResponsePlanOutputTypeDef,
     CreateResponsePlanInputRequestTypeDef,
+    GetResponsePlanOutputTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.py` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.pyi` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__main__.py` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMIncidents 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.SSMIncidents 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.py` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.pyi` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.py` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.pyi` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.py` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.pyi` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.py` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
     "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
     "RegionMapInputValueTypeDef",
@@ -46,36 +45,31 @@
     "EventReferenceTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteResponsePlanInputRequestTypeDef",
     "DeleteTimelineEventInputRequestTypeDef",
-    "DynamicSsmParameterValueOutputTypeDef",
     "DynamicSsmParameterValueTypeDef",
-    "EventReferenceOutputTypeDef",
     "GetIncidentRecordInputRequestTypeDef",
     "GetReplicationSetInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "PaginatorConfigTypeDef",
     "GetResourcePoliciesInputRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetResponsePlanInputRequestTypeDef",
     "GetTimelineEventInputRequestTypeDef",
     "IncidentRecordSourceTypeDef",
-    "NotificationTargetItemOutputTypeDef",
     "NotificationTargetItemTypeDef",
-    "PagerDutyIncidentDetailOutputTypeDef",
     "PagerDutyIncidentDetailTypeDef",
     "ListRelatedItemsInputRequestTypeDef",
     "ListReplicationSetsInputRequestTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PagerDutyIncidentConfigurationOutputTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "RegionInfoTypeDef",
     "TriggerDetailsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
@@ -85,59 +79,54 @@
     "CreateResponsePlanOutputTypeDef",
     "CreateTimelineEventOutputTypeDef",
     "ListReplicationSetsOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePolicyOutputTypeDef",
     "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
+    "EventSummaryTypeDef",
+    "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
     "SsmAutomationOutputTypeDef",
     "SsmAutomationTypeDef",
-    "EventSummaryTypeDef",
-    "TimelineEventTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
     "IncidentTemplateOutputTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
-    "ItemValueOutputTypeDef",
     "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
-    "PagerDutyConfigurationOutputTypeDef",
     "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
+    "ListTimelineEventsOutputTypeDef",
+    "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
-    "ListTimelineEventsOutputTypeDef",
-    "GetTimelineEventOutputTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
-    "ItemIdentifierOutputTypeDef",
     "ItemIdentifierTypeDef",
-    "IntegrationOutputTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
-    "RelatedItemOutputTypeDef",
     "RelatedItemTypeDef",
-    "GetResponsePlanOutputTypeDef",
     "CreateResponsePlanInputRequestTypeDef",
+    "GetResponsePlanOutputTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -151,19 +140,17 @@
     "_OptionalAddRegionActionTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
-
 class AddRegionActionTypeDef(_RequiredAddRegionActionTypeDef, _OptionalAddRegionActionTypeDef):
     pass
 
-
 AttributeValueListTypeDef = TypedDict(
     "AttributeValueListTypeDef",
     {
         "integerValues": Sequence[int],
         "stringValues": Sequence[str],
     },
     total=False,
@@ -263,39 +250,22 @@
     "DeleteTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
 
-DynamicSsmParameterValueOutputTypeDef = TypedDict(
-    "DynamicSsmParameterValueOutputTypeDef",
-    {
-        "variable": VariableTypeType,
-    },
-    total=False,
-)
-
 DynamicSsmParameterValueTypeDef = TypedDict(
     "DynamicSsmParameterValueTypeDef",
     {
         "variable": VariableTypeType,
     },
     total=False,
 )
 
-EventReferenceOutputTypeDef = TypedDict(
-    "EventReferenceOutputTypeDef",
-    {
-        "relatedItemId": str,
-        "resource": str,
-    },
-    total=False,
-)
-
 GetIncidentRecordInputRequestTypeDef = TypedDict(
     "GetIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -336,21 +306,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesInputRequestTypeDef(
     _RequiredGetResourcePoliciesInputRequestTypeDef, _OptionalGetResourcePoliciesInputRequestTypeDef
 ):
     pass
 
-
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "policyDocument": str,
         "policyId": str,
         "ramResourceShareRegion": str,
     },
@@ -383,59 +351,27 @@
     {
         "invokedBy": str,
         "resourceArn": str,
     },
     total=False,
 )
 
-
 class IncidentRecordSourceTypeDef(
     _RequiredIncidentRecordSourceTypeDef, _OptionalIncidentRecordSourceTypeDef
 ):
     pass
 
-
-NotificationTargetItemOutputTypeDef = TypedDict(
-    "NotificationTargetItemOutputTypeDef",
-    {
-        "snsTopicArn": str,
-    },
-    total=False,
-)
-
 NotificationTargetItemTypeDef = TypedDict(
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
 
-_RequiredPagerDutyIncidentDetailOutputTypeDef = TypedDict(
-    "_RequiredPagerDutyIncidentDetailOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalPagerDutyIncidentDetailOutputTypeDef = TypedDict(
-    "_OptionalPagerDutyIncidentDetailOutputTypeDef",
-    {
-        "autoResolve": bool,
-        "secretId": str,
-    },
-    total=False,
-)
-
-
-class PagerDutyIncidentDetailOutputTypeDef(
-    _RequiredPagerDutyIncidentDetailOutputTypeDef, _OptionalPagerDutyIncidentDetailOutputTypeDef
-):
-    pass
-
-
 _RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
     "_RequiredPagerDutyIncidentDetailTypeDef",
     {
         "id": str,
     },
 )
 _OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
@@ -443,21 +379,19 @@
     {
         "autoResolve": bool,
         "secretId": str,
     },
     total=False,
 )
 
-
 class PagerDutyIncidentDetailTypeDef(
     _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
 ):
     pass
 
-
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -465,21 +399,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
-
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -505,35 +437,26 @@
     "_OptionalResponsePlanSummaryTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
 
-
 class ResponsePlanSummaryTypeDef(
     _RequiredResponsePlanSummaryTypeDef, _OptionalResponsePlanSummaryTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-PagerDutyIncidentConfigurationOutputTypeDef = TypedDict(
-    "PagerDutyIncidentConfigurationOutputTypeDef",
-    {
-        "serviceId": str,
-    },
-)
-
 PagerDutyIncidentConfigurationTypeDef = TypedDict(
     "PagerDutyIncidentConfigurationTypeDef",
     {
         "serviceId": str,
     },
 )
 
@@ -557,19 +480,17 @@
     {
         "sseKmsKeyId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
     pass
 
-
 _RequiredTriggerDetailsTypeDef = TypedDict(
     "_RequiredTriggerDetailsTypeDef",
     {
         "source": str,
         "timestamp": Union[datetime, str],
     },
 )
@@ -578,19 +499,17 @@
     {
         "rawData": str,
         "triggerArn": str,
     },
     total=False,
 )
 
-
 class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -614,22 +533,20 @@
     "_OptionalUpdateDeletionProtectionInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "after": Union[datetime, str],
         "before": Union[datetime, str],
         "equals": AttributeValueListTypeDef,
     },
@@ -647,22 +564,20 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-
 CreateReplicationSetOutputTypeDef = TypedDict(
     "CreateReplicationSetOutputTypeDef",
     {
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -731,20 +646,61 @@
     {
         "clientToken": str,
         "eventReferences": Sequence[EventReferenceTypeDef],
     },
     total=False,
 )
 
-
 class CreateTimelineEventInputRequestTypeDef(
     _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
 ):
     pass
 
+_RequiredEventSummaryTypeDef = TypedDict(
+    "_RequiredEventSummaryTypeDef",
+    {
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalEventSummaryTypeDef = TypedDict(
+    "_OptionalEventSummaryTypeDef",
+    {
+        "eventReferences": List[EventReferenceTypeDef],
+    },
+    total=False,
+)
+
+class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
+    pass
+
+_RequiredTimelineEventTypeDef = TypedDict(
+    "_RequiredTimelineEventTypeDef",
+    {
+        "eventData": str,
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalTimelineEventTypeDef = TypedDict(
+    "_OptionalTimelineEventTypeDef",
+    {
+        "eventReferences": List[EventReferenceTypeDef],
+    },
+    total=False,
+)
+
+class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
+    pass
 
 _RequiredUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
@@ -757,21 +713,19 @@
         "eventReferences": Sequence[EventReferenceTypeDef],
         "eventTime": Union[datetime, str],
         "eventType": str,
     },
     total=False,
 )
 
-
 class UpdateTimelineEventInputRequestTypeDef(
     _RequiredUpdateTimelineEventInputRequestTypeDef, _OptionalUpdateTimelineEventInputRequestTypeDef
 ):
     pass
 
-
 UpdateReplicationSetActionTypeDef = TypedDict(
     "UpdateReplicationSetActionTypeDef",
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
@@ -784,28 +738,26 @@
         "roleArn": str,
     },
 )
 _OptionalSsmAutomationOutputTypeDef = TypedDict(
     "_OptionalSsmAutomationOutputTypeDef",
     {
         "documentVersion": str,
-        "dynamicParameters": Dict[str, DynamicSsmParameterValueOutputTypeDef],
+        "dynamicParameters": Dict[str, DynamicSsmParameterValueTypeDef],
         "parameters": Dict[str, List[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
-
 class SsmAutomationOutputTypeDef(
     _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
 ):
     pass
 
-
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -816,154 +768,97 @@
         "dynamicParameters": Mapping[str, DynamicSsmParameterValueTypeDef],
         "parameters": Mapping[str, Sequence[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
-
 class SsmAutomationTypeDef(_RequiredSsmAutomationTypeDef, _OptionalSsmAutomationTypeDef):
     pass
 
-
-_RequiredEventSummaryTypeDef = TypedDict(
-    "_RequiredEventSummaryTypeDef",
-    {
-        "eventId": str,
-        "eventTime": datetime,
-        "eventType": str,
-        "eventUpdatedTime": datetime,
-        "incidentRecordArn": str,
-    },
-)
-_OptionalEventSummaryTypeDef = TypedDict(
-    "_OptionalEventSummaryTypeDef",
-    {
-        "eventReferences": List[EventReferenceOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
-    pass
-
-
-_RequiredTimelineEventTypeDef = TypedDict(
-    "_RequiredTimelineEventTypeDef",
-    {
-        "eventData": str,
-        "eventId": str,
-        "eventTime": datetime,
-        "eventType": str,
-        "eventUpdatedTime": datetime,
-        "incidentRecordArn": str,
-    },
-)
-_OptionalTimelineEventTypeDef = TypedDict(
-    "_OptionalTimelineEventTypeDef",
-    {
-        "eventReferences": List[EventReferenceOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
-    pass
-
-
 _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
     _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
 ):
     pass
 
-
 ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1000,21 +895,19 @@
     "_OptionalIncidentRecordSummaryTypeDef",
     {
         "resolvedTime": datetime,
     },
     total=False,
 )
 
-
 class IncidentRecordSummaryTypeDef(
     _RequiredIncidentRecordSummaryTypeDef, _OptionalIncidentRecordSummaryTypeDef
 ):
     pass
 
-
 _RequiredIncidentRecordTypeDef = TypedDict(
     "_RequiredIncidentRecordTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "dedupeString": str,
         "impact": int,
@@ -1026,51 +919,47 @@
     },
 )
 _OptionalIncidentRecordTypeDef = TypedDict(
     "_OptionalIncidentRecordTypeDef",
     {
         "automationExecutions": List[AutomationExecutionTypeDef],
         "chatChannel": ChatChannelOutputTypeDef,
-        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
+        "notificationTargets": List[NotificationTargetItemTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
-
 _RequiredIncidentTemplateOutputTypeDef = TypedDict(
     "_RequiredIncidentTemplateOutputTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
 _OptionalIncidentTemplateOutputTypeDef = TypedDict(
     "_OptionalIncidentTemplateOutputTypeDef",
     {
         "dedupeString": str,
         "incidentTags": Dict[str, str],
-        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
+        "notificationTargets": List[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentTemplateOutputTypeDef(
     _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
 ):
     pass
 
-
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -1081,19 +970,17 @@
         "incidentTags": Mapping[str, str],
         "notificationTargets": Sequence[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentTemplateTypeDef(_RequiredIncidentTemplateTypeDef, _OptionalIncidentTemplateTypeDef):
     pass
 
-
 _RequiredUpdateIncidentRecordInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateIncidentRecordInputRequestTypeDef = TypedDict(
@@ -1106,33 +993,20 @@
         "status": IncidentRecordStatusType,
         "summary": str,
         "title": str,
     },
     total=False,
 )
 
-
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
-
-ItemValueOutputTypeDef = TypedDict(
-    "ItemValueOutputTypeDef",
-    {
-        "arn": str,
-        "metricDefinition": str,
-        "pagerDutyIncidentDetail": PagerDutyIncidentDetailOutputTypeDef,
-        "url": str,
-    },
-    total=False,
-)
-
 ItemValueTypeDef = TypedDict(
     "ItemValueTypeDef",
     {
         "arn": str,
         "metricDefinition": str,
         "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
         "url": str,
@@ -1145,23 +1019,14 @@
     {
         "nextToken": str,
         "responsePlanSummaries": List[ResponsePlanSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PagerDutyConfigurationOutputTypeDef = TypedDict(
-    "PagerDutyConfigurationOutputTypeDef",
-    {
-        "name": str,
-        "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationOutputTypeDef,
-        "secretId": str,
-    },
-)
-
 PagerDutyConfigurationTypeDef = TypedDict(
     "PagerDutyConfigurationTypeDef",
     {
         "name": str,
         "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationTypeDef,
         "secretId": str,
     },
@@ -1183,27 +1048,42 @@
     "_OptionalReplicationSetTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
-
 class ReplicationSetTypeDef(_RequiredReplicationSetTypeDef, _OptionalReplicationSetTypeDef):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "condition": ConditionTypeDef,
         "key": str,
     },
 )
 
+ListTimelineEventsOutputTypeDef = TypedDict(
+    "ListTimelineEventsOutputTypeDef",
+    {
+        "eventSummaries": List[EventSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTimelineEventOutputTypeDef = TypedDict(
+    "GetTimelineEventOutputTypeDef",
+    {
+        "event": TimelineEventTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationSetInputRequestTypeDef",
     {
         "actions": Sequence[UpdateReplicationSetActionTypeDef],
         "arn": str,
     },
 )
@@ -1211,22 +1091,20 @@
     "_OptionalUpdateReplicationSetInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "ssmAutomation": SsmAutomationOutputTypeDef,
     },
     total=False,
 )
@@ -1235,31 +1113,14 @@
     "ActionTypeDef",
     {
         "ssmAutomation": SsmAutomationTypeDef,
     },
     total=False,
 )
 
-ListTimelineEventsOutputTypeDef = TypedDict(
-    "ListTimelineEventsOutputTypeDef",
-    {
-        "eventSummaries": List[EventSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTimelineEventOutputTypeDef = TypedDict(
-    "GetTimelineEventOutputTypeDef",
-    {
-        "event": TimelineEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListIncidentRecordsOutputTypeDef = TypedDict(
     "ListIncidentRecordsOutputTypeDef",
     {
         "incidentRecordSummaries": List[IncidentRecordSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1269,38 +1130,22 @@
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ItemIdentifierOutputTypeDef = TypedDict(
-    "ItemIdentifierOutputTypeDef",
-    {
-        "type": ItemTypeType,
-        "value": ItemValueOutputTypeDef,
-    },
-)
-
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
 
-IntegrationOutputTypeDef = TypedDict(
-    "IntegrationOutputTypeDef",
-    {
-        "pagerDutyConfiguration": PagerDutyConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "pagerDutyConfiguration": PagerDutyConfigurationTypeDef,
     },
     total=False,
 )
@@ -1345,22 +1190,20 @@
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTimelineEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTimelineEventsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListTimelineEventsInputRequestTypeDef = TypedDict(
@@ -1371,43 +1214,19 @@
         "nextToken": str,
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
-
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
-
-_RequiredRelatedItemOutputTypeDef = TypedDict(
-    "_RequiredRelatedItemOutputTypeDef",
-    {
-        "identifier": ItemIdentifierOutputTypeDef,
-    },
-)
-_OptionalRelatedItemOutputTypeDef = TypedDict(
-    "_OptionalRelatedItemOutputTypeDef",
-    {
-        "generatedId": str,
-        "title": str,
-    },
-    total=False,
-)
-
-
-class RelatedItemOutputTypeDef(
-    _RequiredRelatedItemOutputTypeDef, _OptionalRelatedItemOutputTypeDef
-):
-    pass
-
-
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
 _OptionalRelatedItemTypeDef = TypedDict(
@@ -1415,34 +1234,17 @@
     {
         "generatedId": str,
         "title": str,
     },
     total=False,
 )
 
-
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
-
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionOutputTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelOutputTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateOutputTypeDef,
-        "integrations": List[IntegrationOutputTypeDef],
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
@@ -1456,20 +1258,33 @@
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionOutputTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelOutputTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateOutputTypeDef,
+        "integrations": List[IntegrationTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
@@ -1488,26 +1303,24 @@
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
         "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
 ):
     pass
 
-
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
-        "relatedItems": List[RelatedItemOutputTypeDef],
+        "relatedItems": List[RelatedItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemsUpdateTypeDef = TypedDict(
     "RelatedItemsUpdateTypeDef",
     {
@@ -1531,21 +1344,19 @@
         "relatedItems": Sequence[RelatedItemTypeDef],
         "title": str,
         "triggerDetails": TriggerDetailsTypeDef,
     },
     total=False,
 )
 
-
 class StartIncidentInputRequestTypeDef(
     _RequiredStartIncidentInputRequestTypeDef, _OptionalStartIncidentInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
         "relatedItemsUpdate": RelatedItemsUpdateTypeDef,
     },
 )
@@ -1553,12 +1364,11 @@
     "_OptionalUpdateRelatedItemsInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateRelatedItemsInputRequestTypeDef(
     _RequiredUpdateRelatedItemsInputRequestTypeDef, _OptionalUpdateRelatedItemsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.pyi` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
     "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
     "RegionMapInputValueTypeDef",
@@ -45,36 +46,31 @@
     "EventReferenceTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteResponsePlanInputRequestTypeDef",
     "DeleteTimelineEventInputRequestTypeDef",
-    "DynamicSsmParameterValueOutputTypeDef",
     "DynamicSsmParameterValueTypeDef",
-    "EventReferenceOutputTypeDef",
     "GetIncidentRecordInputRequestTypeDef",
     "GetReplicationSetInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "PaginatorConfigTypeDef",
     "GetResourcePoliciesInputRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetResponsePlanInputRequestTypeDef",
     "GetTimelineEventInputRequestTypeDef",
     "IncidentRecordSourceTypeDef",
-    "NotificationTargetItemOutputTypeDef",
     "NotificationTargetItemTypeDef",
-    "PagerDutyIncidentDetailOutputTypeDef",
     "PagerDutyIncidentDetailTypeDef",
     "ListRelatedItemsInputRequestTypeDef",
     "ListReplicationSetsInputRequestTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PagerDutyIncidentConfigurationOutputTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "RegionInfoTypeDef",
     "TriggerDetailsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
@@ -84,59 +80,54 @@
     "CreateResponsePlanOutputTypeDef",
     "CreateTimelineEventOutputTypeDef",
     "ListReplicationSetsOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePolicyOutputTypeDef",
     "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
+    "EventSummaryTypeDef",
+    "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
     "SsmAutomationOutputTypeDef",
     "SsmAutomationTypeDef",
-    "EventSummaryTypeDef",
-    "TimelineEventTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
     "IncidentTemplateOutputTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
-    "ItemValueOutputTypeDef",
     "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
-    "PagerDutyConfigurationOutputTypeDef",
     "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
+    "ListTimelineEventsOutputTypeDef",
+    "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
-    "ListTimelineEventsOutputTypeDef",
-    "GetTimelineEventOutputTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
-    "ItemIdentifierOutputTypeDef",
     "ItemIdentifierTypeDef",
-    "IntegrationOutputTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
-    "RelatedItemOutputTypeDef",
     "RelatedItemTypeDef",
-    "GetResponsePlanOutputTypeDef",
     "CreateResponsePlanInputRequestTypeDef",
+    "GetResponsePlanOutputTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -150,17 +141,19 @@
     "_OptionalAddRegionActionTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
+
 class AddRegionActionTypeDef(_RequiredAddRegionActionTypeDef, _OptionalAddRegionActionTypeDef):
     pass
 
+
 AttributeValueListTypeDef = TypedDict(
     "AttributeValueListTypeDef",
     {
         "integerValues": Sequence[int],
         "stringValues": Sequence[str],
     },
     total=False,
@@ -260,39 +253,22 @@
     "DeleteTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
 
-DynamicSsmParameterValueOutputTypeDef = TypedDict(
-    "DynamicSsmParameterValueOutputTypeDef",
-    {
-        "variable": VariableTypeType,
-    },
-    total=False,
-)
-
 DynamicSsmParameterValueTypeDef = TypedDict(
     "DynamicSsmParameterValueTypeDef",
     {
         "variable": VariableTypeType,
     },
     total=False,
 )
 
-EventReferenceOutputTypeDef = TypedDict(
-    "EventReferenceOutputTypeDef",
-    {
-        "relatedItemId": str,
-        "resource": str,
-    },
-    total=False,
-)
-
 GetIncidentRecordInputRequestTypeDef = TypedDict(
     "GetIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -333,19 +309,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesInputRequestTypeDef(
     _RequiredGetResourcePoliciesInputRequestTypeDef, _OptionalGetResourcePoliciesInputRequestTypeDef
 ):
     pass
 
+
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "policyDocument": str,
         "policyId": str,
         "ramResourceShareRegion": str,
     },
@@ -378,55 +356,29 @@
     {
         "invokedBy": str,
         "resourceArn": str,
     },
     total=False,
 )
 
+
 class IncidentRecordSourceTypeDef(
     _RequiredIncidentRecordSourceTypeDef, _OptionalIncidentRecordSourceTypeDef
 ):
     pass
 
-NotificationTargetItemOutputTypeDef = TypedDict(
-    "NotificationTargetItemOutputTypeDef",
-    {
-        "snsTopicArn": str,
-    },
-    total=False,
-)
 
 NotificationTargetItemTypeDef = TypedDict(
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
 
-_RequiredPagerDutyIncidentDetailOutputTypeDef = TypedDict(
-    "_RequiredPagerDutyIncidentDetailOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalPagerDutyIncidentDetailOutputTypeDef = TypedDict(
-    "_OptionalPagerDutyIncidentDetailOutputTypeDef",
-    {
-        "autoResolve": bool,
-        "secretId": str,
-    },
-    total=False,
-)
-
-class PagerDutyIncidentDetailOutputTypeDef(
-    _RequiredPagerDutyIncidentDetailOutputTypeDef, _OptionalPagerDutyIncidentDetailOutputTypeDef
-):
-    pass
-
 _RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
     "_RequiredPagerDutyIncidentDetailTypeDef",
     {
         "id": str,
     },
 )
 _OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
@@ -434,19 +386,21 @@
     {
         "autoResolve": bool,
         "secretId": str,
     },
     total=False,
 )
 
+
 class PagerDutyIncidentDetailTypeDef(
     _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
 ):
     pass
 
+
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -454,19 +408,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
+
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -492,33 +448,28 @@
     "_OptionalResponsePlanSummaryTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
 
+
 class ResponsePlanSummaryTypeDef(
     _RequiredResponsePlanSummaryTypeDef, _OptionalResponsePlanSummaryTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-PagerDutyIncidentConfigurationOutputTypeDef = TypedDict(
-    "PagerDutyIncidentConfigurationOutputTypeDef",
-    {
-        "serviceId": str,
-    },
-)
-
 PagerDutyIncidentConfigurationTypeDef = TypedDict(
     "PagerDutyIncidentConfigurationTypeDef",
     {
         "serviceId": str,
     },
 )
 
@@ -542,17 +493,19 @@
     {
         "sseKmsKeyId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
     pass
 
+
 _RequiredTriggerDetailsTypeDef = TypedDict(
     "_RequiredTriggerDetailsTypeDef",
     {
         "source": str,
         "timestamp": Union[datetime, str],
     },
 )
@@ -561,17 +514,19 @@
     {
         "rawData": str,
         "triggerArn": str,
     },
     total=False,
 )
 
+
 class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -595,20 +550,22 @@
     "_OptionalUpdateDeletionProtectionInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "after": Union[datetime, str],
         "before": Union[datetime, str],
         "equals": AttributeValueListTypeDef,
     },
@@ -626,20 +583,22 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
+
 CreateReplicationSetOutputTypeDef = TypedDict(
     "CreateReplicationSetOutputTypeDef",
     {
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -708,19 +667,68 @@
     {
         "clientToken": str,
         "eventReferences": Sequence[EventReferenceTypeDef],
     },
     total=False,
 )
 
+
 class CreateTimelineEventInputRequestTypeDef(
     _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
 ):
     pass
 
+
+_RequiredEventSummaryTypeDef = TypedDict(
+    "_RequiredEventSummaryTypeDef",
+    {
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalEventSummaryTypeDef = TypedDict(
+    "_OptionalEventSummaryTypeDef",
+    {
+        "eventReferences": List[EventReferenceTypeDef],
+    },
+    total=False,
+)
+
+
+class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
+    pass
+
+
+_RequiredTimelineEventTypeDef = TypedDict(
+    "_RequiredTimelineEventTypeDef",
+    {
+        "eventData": str,
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalTimelineEventTypeDef = TypedDict(
+    "_OptionalTimelineEventTypeDef",
+    {
+        "eventReferences": List[EventReferenceTypeDef],
+    },
+    total=False,
+)
+
+
+class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
+    pass
+
+
 _RequiredUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
@@ -732,19 +740,21 @@
         "eventReferences": Sequence[EventReferenceTypeDef],
         "eventTime": Union[datetime, str],
         "eventType": str,
     },
     total=False,
 )
 
+
 class UpdateTimelineEventInputRequestTypeDef(
     _RequiredUpdateTimelineEventInputRequestTypeDef, _OptionalUpdateTimelineEventInputRequestTypeDef
 ):
     pass
 
+
 UpdateReplicationSetActionTypeDef = TypedDict(
     "UpdateReplicationSetActionTypeDef",
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
@@ -757,26 +767,28 @@
         "roleArn": str,
     },
 )
 _OptionalSsmAutomationOutputTypeDef = TypedDict(
     "_OptionalSsmAutomationOutputTypeDef",
     {
         "documentVersion": str,
-        "dynamicParameters": Dict[str, DynamicSsmParameterValueOutputTypeDef],
+        "dynamicParameters": Dict[str, DynamicSsmParameterValueTypeDef],
         "parameters": Dict[str, List[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
+
 class SsmAutomationOutputTypeDef(
     _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
 ):
     pass
 
+
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -787,59 +799,18 @@
         "dynamicParameters": Mapping[str, DynamicSsmParameterValueTypeDef],
         "parameters": Mapping[str, Sequence[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
+
 class SsmAutomationTypeDef(_RequiredSsmAutomationTypeDef, _OptionalSsmAutomationTypeDef):
     pass
 
-_RequiredEventSummaryTypeDef = TypedDict(
-    "_RequiredEventSummaryTypeDef",
-    {
-        "eventId": str,
-        "eventTime": datetime,
-        "eventType": str,
-        "eventUpdatedTime": datetime,
-        "incidentRecordArn": str,
-    },
-)
-_OptionalEventSummaryTypeDef = TypedDict(
-    "_OptionalEventSummaryTypeDef",
-    {
-        "eventReferences": List[EventReferenceOutputTypeDef],
-    },
-    total=False,
-)
-
-class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
-    pass
-
-_RequiredTimelineEventTypeDef = TypedDict(
-    "_RequiredTimelineEventTypeDef",
-    {
-        "eventData": str,
-        "eventId": str,
-        "eventTime": datetime,
-        "eventType": str,
-        "eventUpdatedTime": datetime,
-        "incidentRecordArn": str,
-    },
-)
-_OptionalTimelineEventTypeDef = TypedDict(
-    "_OptionalTimelineEventTypeDef",
-    {
-        "eventReferences": List[EventReferenceOutputTypeDef],
-    },
-    total=False,
-)
-
-class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
-    pass
 
 _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "arn": str,
     },
 )
@@ -847,80 +818,88 @@
     "_OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
     _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
 ):
     pass
 
+
 ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -957,19 +936,21 @@
     "_OptionalIncidentRecordSummaryTypeDef",
     {
         "resolvedTime": datetime,
     },
     total=False,
 )
 
+
 class IncidentRecordSummaryTypeDef(
     _RequiredIncidentRecordSummaryTypeDef, _OptionalIncidentRecordSummaryTypeDef
 ):
     pass
 
+
 _RequiredIncidentRecordTypeDef = TypedDict(
     "_RequiredIncidentRecordTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "dedupeString": str,
         "impact": int,
@@ -981,47 +962,51 @@
     },
 )
 _OptionalIncidentRecordTypeDef = TypedDict(
     "_OptionalIncidentRecordTypeDef",
     {
         "automationExecutions": List[AutomationExecutionTypeDef],
         "chatChannel": ChatChannelOutputTypeDef,
-        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
+        "notificationTargets": List[NotificationTargetItemTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
+
 _RequiredIncidentTemplateOutputTypeDef = TypedDict(
     "_RequiredIncidentTemplateOutputTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
 _OptionalIncidentTemplateOutputTypeDef = TypedDict(
     "_OptionalIncidentTemplateOutputTypeDef",
     {
         "dedupeString": str,
         "incidentTags": Dict[str, str],
-        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
+        "notificationTargets": List[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentTemplateOutputTypeDef(
     _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
 ):
     pass
 
+
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -1032,17 +1017,19 @@
         "incidentTags": Mapping[str, str],
         "notificationTargets": Sequence[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentTemplateTypeDef(_RequiredIncidentTemplateTypeDef, _OptionalIncidentTemplateTypeDef):
     pass
 
+
 _RequiredUpdateIncidentRecordInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateIncidentRecordInputRequestTypeDef = TypedDict(
@@ -1055,30 +1042,21 @@
         "status": IncidentRecordStatusType,
         "summary": str,
         "title": str,
     },
     total=False,
 )
 
+
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
-ItemValueOutputTypeDef = TypedDict(
-    "ItemValueOutputTypeDef",
-    {
-        "arn": str,
-        "metricDefinition": str,
-        "pagerDutyIncidentDetail": PagerDutyIncidentDetailOutputTypeDef,
-        "url": str,
-    },
-    total=False,
-)
 
 ItemValueTypeDef = TypedDict(
     "ItemValueTypeDef",
     {
         "arn": str,
         "metricDefinition": str,
         "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
@@ -1092,23 +1070,14 @@
     {
         "nextToken": str,
         "responsePlanSummaries": List[ResponsePlanSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PagerDutyConfigurationOutputTypeDef = TypedDict(
-    "PagerDutyConfigurationOutputTypeDef",
-    {
-        "name": str,
-        "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationOutputTypeDef,
-        "secretId": str,
-    },
-)
-
 PagerDutyConfigurationTypeDef = TypedDict(
     "PagerDutyConfigurationTypeDef",
     {
         "name": str,
         "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationTypeDef,
         "secretId": str,
     },
@@ -1130,25 +1099,44 @@
     "_OptionalReplicationSetTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
+
 class ReplicationSetTypeDef(_RequiredReplicationSetTypeDef, _OptionalReplicationSetTypeDef):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "condition": ConditionTypeDef,
         "key": str,
     },
 )
 
+ListTimelineEventsOutputTypeDef = TypedDict(
+    "ListTimelineEventsOutputTypeDef",
+    {
+        "eventSummaries": List[EventSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTimelineEventOutputTypeDef = TypedDict(
+    "GetTimelineEventOutputTypeDef",
+    {
+        "event": TimelineEventTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationSetInputRequestTypeDef",
     {
         "actions": Sequence[UpdateReplicationSetActionTypeDef],
         "arn": str,
     },
 )
@@ -1156,20 +1144,22 @@
     "_OptionalUpdateReplicationSetInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
+
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "ssmAutomation": SsmAutomationOutputTypeDef,
     },
     total=False,
 )
@@ -1178,31 +1168,14 @@
     "ActionTypeDef",
     {
         "ssmAutomation": SsmAutomationTypeDef,
     },
     total=False,
 )
 
-ListTimelineEventsOutputTypeDef = TypedDict(
-    "ListTimelineEventsOutputTypeDef",
-    {
-        "eventSummaries": List[EventSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTimelineEventOutputTypeDef = TypedDict(
-    "GetTimelineEventOutputTypeDef",
-    {
-        "event": TimelineEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListIncidentRecordsOutputTypeDef = TypedDict(
     "ListIncidentRecordsOutputTypeDef",
     {
         "incidentRecordSummaries": List[IncidentRecordSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1212,38 +1185,22 @@
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ItemIdentifierOutputTypeDef = TypedDict(
-    "ItemIdentifierOutputTypeDef",
-    {
-        "type": ItemTypeType,
-        "value": ItemValueOutputTypeDef,
-    },
-)
-
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
 
-IntegrationOutputTypeDef = TypedDict(
-    "IntegrationOutputTypeDef",
-    {
-        "pagerDutyConfiguration": PagerDutyConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "pagerDutyConfiguration": PagerDutyConfigurationTypeDef,
     },
     total=False,
 )
@@ -1288,20 +1245,22 @@
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTimelineEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTimelineEventsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListTimelineEventsInputRequestTypeDef = TypedDict(
@@ -1312,38 +1271,20 @@
         "nextToken": str,
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
+
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
-_RequiredRelatedItemOutputTypeDef = TypedDict(
-    "_RequiredRelatedItemOutputTypeDef",
-    {
-        "identifier": ItemIdentifierOutputTypeDef,
-    },
-)
-_OptionalRelatedItemOutputTypeDef = TypedDict(
-    "_OptionalRelatedItemOutputTypeDef",
-    {
-        "generatedId": str,
-        "title": str,
-    },
-    total=False,
-)
-
-class RelatedItemOutputTypeDef(
-    _RequiredRelatedItemOutputTypeDef, _OptionalRelatedItemOutputTypeDef
-):
-    pass
 
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
@@ -1352,31 +1293,18 @@
     {
         "generatedId": str,
         "title": str,
     },
     total=False,
 )
 
+
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionOutputTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelOutputTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateOutputTypeDef,
-        "integrations": List[IntegrationOutputTypeDef],
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
@@ -1391,19 +1319,36 @@
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
+
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionOutputTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelOutputTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateOutputTypeDef,
+        "integrations": List[IntegrationTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
@@ -1421,24 +1366,26 @@
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
         "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
 ):
     pass
 
+
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
-        "relatedItems": List[RelatedItemOutputTypeDef],
+        "relatedItems": List[RelatedItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemsUpdateTypeDef = TypedDict(
     "RelatedItemsUpdateTypeDef",
     {
@@ -1462,19 +1409,21 @@
         "relatedItems": Sequence[RelatedItemTypeDef],
         "title": str,
         "triggerDetails": TriggerDetailsTypeDef,
     },
     total=False,
 )
 
+
 class StartIncidentInputRequestTypeDef(
     _RequiredStartIncidentInputRequestTypeDef, _OptionalStartIncidentInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
         "relatedItemsUpdate": RelatedItemsUpdateTypeDef,
     },
 )
@@ -1482,11 +1431,12 @@
     "_OptionalUpdateRelatedItemsInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateRelatedItemsInputRequestTypeDef(
     _RequiredUpdateRelatedItemsInputRequestTypeDef, _OptionalUpdateRelatedItemsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.py` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.pyi` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.28.12
-Summary: Type annotations for boto3.SSMIncidents 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -400,36 +400,31 @@
     EventReferenceTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
-    DynamicSsmParameterValueOutputTypeDef,
     DynamicSsmParameterValueTypeDef,
-    EventReferenceOutputTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
     PaginatorConfigTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
-    NotificationTargetItemOutputTypeDef,
     NotificationTargetItemTypeDef,
-    PagerDutyIncidentDetailOutputTypeDef,
     PagerDutyIncidentDetailTypeDef,
     ListRelatedItemsInputRequestTypeDef,
     ListReplicationSetsInputRequestTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PagerDutyIncidentConfigurationOutputTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     RegionInfoTypeDef,
     TriggerDetailsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
@@ -439,59 +434,54 @@
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePolicyOutputTypeDef,
     StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
+    EventSummaryTypeDef,
+    TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
     SsmAutomationOutputTypeDef,
     SsmAutomationTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
     IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
-    ItemValueOutputTypeDef,
     ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
-    PagerDutyConfigurationOutputTypeDef,
     PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
+    ListTimelineEventsOutputTypeDef,
+    GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
-    ItemIdentifierOutputTypeDef,
     ItemIdentifierTypeDef,
-    IntegrationOutputTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
-    RelatedItemOutputTypeDef,
     RelatedItemTypeDef,
-    GetResponsePlanOutputTypeDef,
     CreateResponsePlanInputRequestTypeDef,
+    GetResponsePlanOutputTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt` & `mypy-boto3-ssm-incidents-1.28.15/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.12/setup.py` & `mypy-boto3-ssm-incidents-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-incidents",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMIncidents 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

