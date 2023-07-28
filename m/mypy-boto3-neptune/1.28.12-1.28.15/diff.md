# Comparing `tmp/mypy-boto3-neptune-1.28.12.tar.gz` & `tmp/mypy-boto3-neptune-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-neptune-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
+gzip compressed data, was "mypy-boto3-neptune-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
```

## Comparing `mypy-boto3-neptune-1.28.12.tar` & `mypy-boto3-neptune-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25580 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67621 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67527 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85182 2023-07-27 05:26:54.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85105 2023-07-27 05:26:54.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25580 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.409558 mypy-boto3-neptune-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-28 20:43:21.409558 mypy-boto3-neptune-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.409558 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67621 2023-07-28 20:32:20.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67527 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-28 20:32:20.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-28 20:32:20.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-07-28 20:32:20.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-07-28 20:32:20.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    84422 2023-07-28 20:32:23.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84345 2023-07-28 20:32:21.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-28 20:32:20.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-28 20:32:20.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.409558 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-28 20:43:21.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:43:21.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:21.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:21.000000 mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.409558 mypy-boto3-neptune-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:32:19.000000 mypy-boto3-neptune-1.28.15/setup.py
```

### Comparing `mypy-boto3-neptune-1.28.12/LICENSE` & `mypy-boto3-neptune-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/PKG-INFO` & `mypy-boto3-neptune-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.28.12
-Summary: Type annotations for boto3.Neptune 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Neptune 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -424,104 +424,102 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CharacterSetTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     DBParameterGroupTypeDef,
-    CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
-    ParameterOutputTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
+    ParameterTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     DomainMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
-    DBParameterGroupNameMessageTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
-    DeleteDBClusterEndpointOutputTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
-    ModifyDBClusterEndpointOutputTypeDef,
-    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
-    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
+    CreateDBClusterEndpointOutputTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
+    DBParameterGroupNameMessageTypeDef,
+    DeleteDBClusterEndpointOutputTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
+    ModifyDBClusterEndpointOutputTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CopyDBParameterGroupMessageRequestTypeDef,
     CreateDBClusterEndpointMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     PendingModifiedValuesTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -537,61 +535,61 @@
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
-    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParameterGroupsMessageRequestTypeDef,
-    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
+    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DBClusterTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
```

### Comparing `mypy-boto3-neptune-1.28.12/README.md` & `mypy-boto3-neptune-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,104 +392,102 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CharacterSetTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     DBParameterGroupTypeDef,
-    CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
-    ParameterOutputTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
+    ParameterTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     DomainMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
-    DBParameterGroupNameMessageTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
-    DeleteDBClusterEndpointOutputTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
-    ModifyDBClusterEndpointOutputTypeDef,
-    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
-    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
+    CreateDBClusterEndpointOutputTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
+    DBParameterGroupNameMessageTypeDef,
+    DeleteDBClusterEndpointOutputTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
+    ModifyDBClusterEndpointOutputTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CopyDBParameterGroupMessageRequestTypeDef,
     CreateDBClusterEndpointMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     PendingModifiedValuesTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -505,61 +503,61 @@
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
-    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParameterGroupsMessageRequestTypeDef,
-    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
+    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DBClusterTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
```

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.py` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.pyi` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__main__.py` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Neptune 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Neptune 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune\nOther"
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

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.py` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.pyi` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.py` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.pyi` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.py` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterendpointspaginator)
         """
 
 
@@ -133,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterparametergroupspaginator)
         """
 
 
@@ -153,15 +153,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterparameterspaginator)
         """
 
 
@@ -176,15 +176,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclustersnapshotspaginator)
         """
 
 
@@ -195,15 +195,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterspaginator)
         """
 
 
@@ -219,15 +219,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbengineversionspaginator)
         """
 
 
@@ -238,15 +238,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbinstancespaginator)
         """
 
 
@@ -257,15 +257,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbparametergroupspaginator)
         """
 
 
@@ -277,15 +277,15 @@
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbparameterspaginator)
         """
 
 
@@ -296,15 +296,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbsubnetgroupspaginator)
         """
 
 
@@ -315,15 +315,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeenginedefaultparameterspaginator)
         """
 
 
@@ -334,15 +334,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -358,33 +358,30 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeeventspaginator)
         """
 
 
 class DescribeGlobalClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeglobalclusterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        GlobalClusterIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GlobalClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeglobalclusterspaginator)
         """
 
 
@@ -399,15 +396,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 
@@ -418,13 +415,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.pyi` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterendpointspaginator)
         """
 
 class DescribeDBClusterParameterGroupsPaginator(Paginator):
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterparametergroupspaginator)
         """
 
 class DescribeDBClusterParametersPaginator(Paginator):
@@ -148,15 +148,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterparameterspaginator)
         """
 
 class DescribeDBClusterSnapshotsPaginator(Paginator):
@@ -170,15 +170,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclustersnapshotspaginator)
         """
 
 class DescribeDBClustersPaginator(Paginator):
@@ -188,15 +188,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbclusterspaginator)
         """
 
 class DescribeDBEngineVersionsPaginator(Paginator):
@@ -211,15 +211,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbengineversionspaginator)
         """
 
 class DescribeDBInstancesPaginator(Paginator):
@@ -229,15 +229,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbinstancespaginator)
         """
 
 class DescribeDBParameterGroupsPaginator(Paginator):
@@ -247,15 +247,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbparametergroupspaginator)
         """
 
 class DescribeDBParametersPaginator(Paginator):
@@ -266,15 +266,15 @@
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbparameterspaginator)
         """
 
 class DescribeDBSubnetGroupsPaginator(Paginator):
@@ -284,15 +284,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describedbsubnetgroupspaginator)
         """
 
 class DescribeEngineDefaultParametersPaginator(Paginator):
@@ -302,15 +302,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeenginedefaultparameterspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(Paginator):
@@ -320,15 +320,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -343,32 +343,29 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeglobalclusterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        GlobalClusterIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GlobalClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeglobalclusterspaginator)
         """
 
 class DescribeOrderableDBInstanceOptionsPaginator(Paginator):
@@ -382,15 +379,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 class DescribePendingMaintenanceActionsPaginator(Paginator):
@@ -400,13 +397,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.py` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,104 +23,102 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CharacterSetTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "DBParameterGroupTypeDef",
-    "CreateDBClusterEndpointOutputTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterOutputTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
+    "ParameterTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "DomainMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
-    "DBParameterGroupNameMessageTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
-    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeValidDBInstanceModificationsMessageRequestTypeDef",
     "DoubleRangeTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
-    "ModifyDBClusterEndpointOutputTypeDef",
-    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveRoleFromDBClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
-    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
+    "CreateDBClusterEndpointOutputTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
+    "DBParameterGroupNameMessageTypeDef",
+    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
+    "ModifyDBClusterEndpointOutputTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CopyDBParameterGroupMessageRequestTypeDef",
     "CreateDBClusterEndpointMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBParameterGroupMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ClusterPendingModifiedValuesTypeDef",
     "PendingModifiedValuesTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -136,61 +134,61 @@
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     "DescribeDBParameterGroupsMessageRequestTypeDef",
-    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     "DescribeDBParametersMessageRequestTypeDef",
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
+    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DBClusterTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
@@ -270,14 +268,25 @@
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -372,31 +381,14 @@
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBParameterGroupArn": str,
     },
     total=False,
 )
 
-CreateDBClusterEndpointOutputTypeDef = TypedDict(
-    "CreateDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServerlessV2ScalingConfigurationTypeDef = TypedDict(
     "ServerlessV2ScalingConfigurationTypeDef",
     {
         "MinCapacity": float,
         "MaxCapacity": float,
     },
     total=False,
@@ -461,16 +453,16 @@
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
@@ -478,22 +470,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
     total=False,
 )
 
-DBClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "DBClusterParameterGroupNameMessageTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
         "FeatureName": str,
     },
@@ -603,46 +587,21 @@
     {
         "OptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-DBParameterGroupNameMessageTypeDef = TypedDict(
-    "DBParameterGroupNameMessageTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
-DeleteDBClusterEndpointOutputTypeDef = TypedDict(
-    "DeleteDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
@@ -729,14 +688,24 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeDBClusterSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
     },
 )
 
@@ -745,23 +714,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
-    {
-        "GlobalClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -780,21 +740,14 @@
     {
         "From": float,
         "To": float,
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
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -860,48 +813,14 @@
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
 
-ModifyDBClusterEndpointOutputTypeDef = TypedDict(
-    "ModifyDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-        "Description": str,
-        "Source": str,
-        "ApplyType": str,
-        "DataType": str,
-        "AllowedValues": str,
-        "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-        "ApplyMethod": ApplyMethodType,
-    },
-    total=False,
-)
-
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -991,24 +910,14 @@
 class ModifyGlobalClusterMessageRequestTypeDef(
     _RequiredModifyGlobalClusterMessageRequestTypeDef,
     _OptionalModifyGlobalClusterMessageRequestTypeDef,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1099,94 +1008,148 @@
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
         "TagKeys": Sequence[str],
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
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
+    "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "EventSubscription": EventSubscriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
-    "AddSourceIdentifierToSubscriptionResultTypeDef",
+CreateDBClusterEndpointOutputTypeDef = TypedDict(
+    "CreateDBClusterEndpointOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "DBClusterParameterGroupNameMessageTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBParameterGroupNameMessageTypeDef = TypedDict(
+    "DBParameterGroupNameMessageTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBClusterEndpointOutputTypeDef = TypedDict(
+    "DeleteDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResultTypeDef = TypedDict(
     "DeleteEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyDBClusterEndpointOutputTypeDef = TypedDict(
+    "ModifyDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveSourceIdentifierFromSubscriptionResultTypeDef = TypedDict(
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
@@ -1475,14 +1438,22 @@
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
 
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
@@ -1608,90 +1579,90 @@
     total=False,
 )
 
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterParameterGroupResultTypeDef = TypedDict(
     "CreateDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupsMessageTypeDef = TypedDict(
     "DBClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBClusterParameterGroups": List[DBClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBClusterSnapshotResultTypeDef = TypedDict(
     "CopyDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterSnapshotResultTypeDef = TypedDict(
     "CreateDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterSnapshotMessageTypeDef = TypedDict(
     "DBClusterSnapshotMessageTypeDef",
     {
         "Marker": str,
         "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterSnapshotResultTypeDef = TypedDict(
     "DeleteDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBParameterGroupResultTypeDef = TypedDict(
     "CopyDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBParameterGroupResultTypeDef = TypedDict(
     "CreateDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupsMessageTypeDef = TypedDict(
     "DBParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBParameterGroups": List[DBParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1851,46 +1822,108 @@
 
 
 DBClusterEndpointMessageTypeDef = TypedDict(
     "DBClusterEndpointMessageTypeDef",
     {
         "Marker": str,
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
     },
     total=False,
 )
 
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -1912,82 +1945,37 @@
         "SupportsLogExportsToCloudwatchLogs": bool,
         "SupportsReadReplica": bool,
         "SupportsGlobalDatabases": bool,
     },
     total=False,
 )
 
-DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
-    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterParametersMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 _OptionalDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
@@ -2005,28 +1993,14 @@
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterSnapshotIdentifier": str,
-        "SnapshotType": str,
-        "Filters": Sequence[FilterTypeDef],
-        "IncludeShared": bool,
-        "IncludePublic": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
@@ -2034,50 +2008,25 @@
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
     },
     total=False,
 )
 
-DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "DBParameterGroupFamily": str,
-        "Filters": Sequence[FilterTypeDef],
-        "DefaultOnly": bool,
-        "ListSupportedCharacterSets": bool,
-        "ListSupportedTimezones": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
@@ -2086,80 +2035,36 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBInstancesMessageRequestTypeDef = TypedDict(
     "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
-    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
-    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDBParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBParametersMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
     },
 )
 _OptionalDescribeDBParametersMessageRequestTypeDef = TypedDict(
@@ -2177,24 +2082,14 @@
 class DescribeDBParametersMessageRequestTypeDef(
     _RequiredDescribeDBParametersMessageRequestTypeDef,
     _OptionalDescribeDBParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
-    {
-        "DBSubnetGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -2222,37 +2117,14 @@
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "DBParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -2278,50 +2150,25 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -2330,41 +2177,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "Engine": str,
-    },
-)
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
         "Engine": str,
     },
 )
 _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
@@ -2385,26 +2205,14 @@
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
 
-DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
-    TypedDict(
-        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
-        {
-            "ResourceIdentifier": str,
-            "Filters": Sequence[FilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -2430,133 +2238,305 @@
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
+DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
-        "DBInstanceIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     {
-        "DBInstanceIdentifier": str,
+        "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-EventCategoriesMessageTypeDef = TypedDict(
-    "EventCategoriesMessageTypeDef",
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     {
-        "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-EventsMessageTypeDef = TypedDict(
-    "EventsMessageTypeDef",
+
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
-        "Marker": str,
-        "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
+        "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GlobalClusterTypeDef = TypedDict(
-    "GlobalClusterTypeDef",
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     {
-        "GlobalClusterIdentifier": str,
-        "GlobalClusterResourceId": str,
-        "GlobalClusterArn": str,
-        "Status": str,
         "Engine": str,
         "EngineVersion": str,
-        "StorageEncrypted": bool,
-        "DeletionProtection": bool,
-        "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
+        "DBParameterGroupFamily": str,
+        "Filters": Sequence[FilterTypeDef],
+        "DefaultOnly": bool,
+        "ListSupportedCharacterSets": bool,
+        "ListSupportedTimezones": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
+DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
         "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "DBClusterParameterGroupName": str,
+        "DBParameterGroupName": str,
     },
 )
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
+    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
 
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBSubnetGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "DBParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "Engine": str,
+    },
+)
+_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+):
+    pass
+
+
+DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
+    TypedDict(
+        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
+        {
+            "ResourceIdentifier": str,
+            "Filters": Sequence[FilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+EventCategoriesMessageTypeDef = TypedDict(
+    "EventCategoriesMessageTypeDef",
+    {
+        "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EventsMessageTypeDef = TypedDict(
+    "EventsMessageTypeDef",
+    {
+        "Marker": str,
+        "Events": List[EventTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GlobalClusterTypeDef = TypedDict(
+    "GlobalClusterTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "GlobalClusterResourceId": str,
+        "GlobalClusterArn": str,
+        "Status": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "StorageEncrypted": bool,
+        "DeletionProtection": bool,
+        "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
+    },
+    total=False,
+)
+
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2569,28 +2549,20 @@
         "StorageSize": List[RangeTypeDef],
         "ProvisionedIops": List[RangeTypeDef],
         "IopsToStorageRatio": List[DoubleRangeTypeDef],
     },
     total=False,
 )
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
@@ -2653,114 +2625,114 @@
     total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterSnapshotAttributeResultTypeDef = TypedDict(
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionMessageTypeDef = TypedDict(
     "DBEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "DBEngineVersions": List[DBEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalClusterResultTypeDef = TypedDict(
     "CreateGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalClusterResultTypeDef = TypedDict(
     "DeleteGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalClusterResultTypeDef = TypedDict(
     "FailoverGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClustersMessageTypeDef = TypedDict(
     "GlobalClustersMessageTypeDef",
     {
         "Marker": str,
         "GlobalClusters": List[GlobalClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalClusterResultTypeDef = TypedDict(
     "ModifyGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PendingMaintenanceActionsMessageTypeDef = TypedDict(
     "PendingMaintenanceActionsMessageTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidDBInstanceModificationsMessageTypeDef = TypedDict(
     "ValidDBInstanceModificationsMessageTypeDef",
     {
         "Storage": List[ValidStorageOptionsTypeDef],
@@ -2768,15 +2740,15 @@
     total=False,
 )
 
 CreateDBSubnetGroupResultTypeDef = TypedDict(
     "CreateDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceTypeDef = TypedDict(
     "DBInstanceTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -2837,148 +2809,148 @@
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBSubnetGroupResultTypeDef = TypedDict(
     "ModifyDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterResultTypeDef = TypedDict(
     "CreateDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterMessageTypeDef = TypedDict(
     "DBClusterMessageTypeDef",
     {
         "Marker": str,
         "DBClusters": List[DBClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterResultTypeDef = TypedDict(
     "DeleteDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverDBClusterResultTypeDef = TypedDict(
     "FailoverDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterResultTypeDef = TypedDict(
     "ModifyDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromoteReadReplicaDBClusterResultTypeDef = TypedDict(
     "PromoteReadReplicaDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterFromSnapshotResultTypeDef = TypedDict(
     "RestoreDBClusterFromSnapshotResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterToPointInTimeResultTypeDef = TypedDict(
     "RestoreDBClusterToPointInTimeResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDBClusterResultTypeDef = TypedDict(
     "StartDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDBClusterResultTypeDef = TypedDict(
     "StopDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeValidDBInstanceModificationsResultTypeDef = TypedDict(
     "DescribeValidDBInstanceModificationsResultTypeDef",
     {
         "ValidDBInstanceModificationsMessage": ValidDBInstanceModificationsMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBInstanceResultTypeDef = TypedDict(
     "CreateDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceMessageTypeDef = TypedDict(
     "DBInstanceMessageTypeDef",
     {
         "Marker": str,
         "DBInstances": List[DBInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBInstanceResultTypeDef = TypedDict(
     "DeleteDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBInstanceResultTypeDef = TypedDict(
     "ModifyDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootDBInstanceResultTypeDef = TypedDict(
     "RebootDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.pyi` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,104 +22,102 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CharacterSetTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "DBParameterGroupTypeDef",
-    "CreateDBClusterEndpointOutputTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterOutputTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
+    "ParameterTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "DomainMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
-    "DBParameterGroupNameMessageTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
-    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeValidDBInstanceModificationsMessageRequestTypeDef",
     "DoubleRangeTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
-    "ModifyDBClusterEndpointOutputTypeDef",
-    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveRoleFromDBClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
-    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
+    "CreateDBClusterEndpointOutputTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
+    "DBParameterGroupNameMessageTypeDef",
+    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
+    "ModifyDBClusterEndpointOutputTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CopyDBParameterGroupMessageRequestTypeDef",
     "CreateDBClusterEndpointMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBParameterGroupMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ClusterPendingModifiedValuesTypeDef",
     "PendingModifiedValuesTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -135,61 +133,61 @@
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     "DescribeDBParameterGroupsMessageRequestTypeDef",
-    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     "DescribeDBParametersMessageRequestTypeDef",
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
+    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DBClusterTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
@@ -267,14 +265,25 @@
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -369,31 +378,14 @@
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBParameterGroupArn": str,
     },
     total=False,
 )
 
-CreateDBClusterEndpointOutputTypeDef = TypedDict(
-    "CreateDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServerlessV2ScalingConfigurationTypeDef = TypedDict(
     "ServerlessV2ScalingConfigurationTypeDef",
     {
         "MinCapacity": float,
         "MaxCapacity": float,
     },
     total=False,
@@ -456,16 +448,16 @@
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
@@ -473,22 +465,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
     total=False,
 )
 
-DBClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "DBClusterParameterGroupNameMessageTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
         "FeatureName": str,
     },
@@ -598,46 +582,21 @@
     {
         "OptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-DBParameterGroupNameMessageTypeDef = TypedDict(
-    "DBParameterGroupNameMessageTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
-DeleteDBClusterEndpointOutputTypeDef = TypedDict(
-    "DeleteDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
@@ -720,14 +679,24 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeDBClusterSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
     },
 )
 
@@ -736,23 +705,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
-    {
-        "GlobalClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -771,21 +731,14 @@
     {
         "From": float,
         "To": float,
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
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -849,48 +802,14 @@
 
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
-ModifyDBClusterEndpointOutputTypeDef = TypedDict(
-    "ModifyDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-        "Description": str,
-        "Source": str,
-        "ApplyType": str,
-        "DataType": str,
-        "AllowedValues": str,
-        "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-        "ApplyMethod": ApplyMethodType,
-    },
-    total=False,
-)
-
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -972,24 +891,14 @@
 
 class ModifyGlobalClusterMessageRequestTypeDef(
     _RequiredModifyGlobalClusterMessageRequestTypeDef,
     _OptionalModifyGlobalClusterMessageRequestTypeDef,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1076,94 +985,148 @@
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
         "TagKeys": Sequence[str],
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
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
+    "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "EventSubscription": EventSubscriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
-    "AddSourceIdentifierToSubscriptionResultTypeDef",
+CreateDBClusterEndpointOutputTypeDef = TypedDict(
+    "CreateDBClusterEndpointOutputTypeDef",
     {
-        "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "DBClusterParameterGroupNameMessageTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBParameterGroupNameMessageTypeDef = TypedDict(
+    "DBParameterGroupNameMessageTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBClusterEndpointOutputTypeDef = TypedDict(
+    "DeleteDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResultTypeDef = TypedDict(
     "DeleteEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyDBClusterEndpointOutputTypeDef = TypedDict(
+    "ModifyDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveSourceIdentifierFromSubscriptionResultTypeDef = TypedDict(
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
@@ -1432,14 +1395,22 @@
 
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
@@ -1563,90 +1534,90 @@
     total=False,
 )
 
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterParameterGroupResultTypeDef = TypedDict(
     "CreateDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupsMessageTypeDef = TypedDict(
     "DBClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBClusterParameterGroups": List[DBClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBClusterSnapshotResultTypeDef = TypedDict(
     "CopyDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterSnapshotResultTypeDef = TypedDict(
     "CreateDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterSnapshotMessageTypeDef = TypedDict(
     "DBClusterSnapshotMessageTypeDef",
     {
         "Marker": str,
         "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterSnapshotResultTypeDef = TypedDict(
     "DeleteDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBParameterGroupResultTypeDef = TypedDict(
     "CopyDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBParameterGroupResultTypeDef = TypedDict(
     "CreateDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupsMessageTypeDef = TypedDict(
     "DBParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBParameterGroups": List[DBParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1798,46 +1769,104 @@
     pass
 
 DBClusterEndpointMessageTypeDef = TypedDict(
     "DBClusterEndpointMessageTypeDef",
     {
         "Marker": str,
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
     },
     total=False,
 )
 
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -1859,80 +1888,37 @@
         "SupportsLogExportsToCloudwatchLogs": bool,
         "SupportsReadReplica": bool,
         "SupportsGlobalDatabases": bool,
     },
     total=False,
 )
 
-DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
-    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterParametersMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 _OptionalDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1948,28 +1934,14 @@
 
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterSnapshotIdentifier": str,
-        "SnapshotType": str,
-        "Filters": Sequence[FilterTypeDef],
-        "IncludeShared": bool,
-        "IncludePublic": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1977,50 +1949,25 @@
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
     },
     total=False,
 )
 
-DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "DBParameterGroupFamily": str,
-        "Filters": Sequence[FilterTypeDef],
-        "DefaultOnly": bool,
-        "ListSupportedCharacterSets": bool,
-        "ListSupportedTimezones": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
@@ -2029,78 +1976,36 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBInstancesMessageRequestTypeDef = TypedDict(
     "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
-    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
-    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDBParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBParametersMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
     },
 )
 _OptionalDescribeDBParametersMessageRequestTypeDef = TypedDict(
@@ -2116,24 +2021,14 @@
 
 class DescribeDBParametersMessageRequestTypeDef(
     _RequiredDescribeDBParametersMessageRequestTypeDef,
     _OptionalDescribeDBParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
-    {
-        "DBSubnetGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -2159,35 +2054,14 @@
 
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "DBParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -2211,50 +2085,25 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -2263,39 +2112,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "Engine": str,
-    },
-)
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
         "Engine": str,
     },
 )
 _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
@@ -2314,26 +2138,14 @@
 
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
-DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
-    TypedDict(
-        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
-        {
-            "ResourceIdentifier": str,
-            "Filters": Sequence[FilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -2357,129 +2169,297 @@
 
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
-DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
+DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
-        "DBInstanceIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     {
-        "DBInstanceIdentifier": str,
+        "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-EventCategoriesMessageTypeDef = TypedDict(
-    "EventCategoriesMessageTypeDef",
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     {
-        "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DBClusterParameterGroupName": str,
     },
 )
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-EventsMessageTypeDef = TypedDict(
-    "EventsMessageTypeDef",
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+):
+    pass
+
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
-        "Marker": str,
-        "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
+        "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GlobalClusterTypeDef = TypedDict(
-    "GlobalClusterTypeDef",
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     {
-        "GlobalClusterIdentifier": str,
-        "GlobalClusterResourceId": str,
-        "GlobalClusterArn": str,
-        "Status": str,
         "Engine": str,
         "EngineVersion": str,
-        "StorageEncrypted": bool,
-        "DeletionProtection": bool,
-        "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
+        "DBParameterGroupFamily": str,
+        "Filters": Sequence[FilterTypeDef],
+        "DefaultOnly": bool,
+        "ListSupportedCharacterSets": bool,
+        "ListSupportedTimezones": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
+DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
         "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "DBClusterParameterGroupName": str,
+        "DBParameterGroupName": str,
     },
 )
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
+    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBSubnetGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "DBParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "Engine": str,
+    },
+)
+_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+):
+    pass
+
+DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
+    TypedDict(
+        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
+        {
+            "ResourceIdentifier": str,
+            "Filters": Sequence[FilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
+EventCategoriesMessageTypeDef = TypedDict(
+    "EventCategoriesMessageTypeDef",
+    {
+        "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EventsMessageTypeDef = TypedDict(
+    "EventsMessageTypeDef",
+    {
+        "Marker": str,
+        "Events": List[EventTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GlobalClusterTypeDef = TypedDict(
+    "GlobalClusterTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "GlobalClusterResourceId": str,
+        "GlobalClusterArn": str,
+        "Status": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "StorageEncrypted": bool,
+        "DeletionProtection": bool,
+        "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
+    },
+    total=False,
+)
+
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2492,28 +2472,20 @@
         "StorageSize": List[RangeTypeDef],
         "ProvisionedIops": List[RangeTypeDef],
         "IopsToStorageRatio": List[DoubleRangeTypeDef],
     },
     total=False,
 )
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
@@ -2576,114 +2548,114 @@
     total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterSnapshotAttributeResultTypeDef = TypedDict(
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionMessageTypeDef = TypedDict(
     "DBEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "DBEngineVersions": List[DBEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalClusterResultTypeDef = TypedDict(
     "CreateGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalClusterResultTypeDef = TypedDict(
     "DeleteGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalClusterResultTypeDef = TypedDict(
     "FailoverGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClustersMessageTypeDef = TypedDict(
     "GlobalClustersMessageTypeDef",
     {
         "Marker": str,
         "GlobalClusters": List[GlobalClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalClusterResultTypeDef = TypedDict(
     "ModifyGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PendingMaintenanceActionsMessageTypeDef = TypedDict(
     "PendingMaintenanceActionsMessageTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidDBInstanceModificationsMessageTypeDef = TypedDict(
     "ValidDBInstanceModificationsMessageTypeDef",
     {
         "Storage": List[ValidStorageOptionsTypeDef],
@@ -2691,15 +2663,15 @@
     total=False,
 )
 
 CreateDBSubnetGroupResultTypeDef = TypedDict(
     "CreateDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceTypeDef = TypedDict(
     "DBInstanceTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -2760,148 +2732,148 @@
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBSubnetGroupResultTypeDef = TypedDict(
     "ModifyDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterResultTypeDef = TypedDict(
     "CreateDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterMessageTypeDef = TypedDict(
     "DBClusterMessageTypeDef",
     {
         "Marker": str,
         "DBClusters": List[DBClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterResultTypeDef = TypedDict(
     "DeleteDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverDBClusterResultTypeDef = TypedDict(
     "FailoverDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterResultTypeDef = TypedDict(
     "ModifyDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromoteReadReplicaDBClusterResultTypeDef = TypedDict(
     "PromoteReadReplicaDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterFromSnapshotResultTypeDef = TypedDict(
     "RestoreDBClusterFromSnapshotResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterToPointInTimeResultTypeDef = TypedDict(
     "RestoreDBClusterToPointInTimeResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDBClusterResultTypeDef = TypedDict(
     "StartDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDBClusterResultTypeDef = TypedDict(
     "StopDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeValidDBInstanceModificationsResultTypeDef = TypedDict(
     "DescribeValidDBInstanceModificationsResultTypeDef",
     {
         "ValidDBInstanceModificationsMessage": ValidDBInstanceModificationsMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBInstanceResultTypeDef = TypedDict(
     "CreateDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceMessageTypeDef = TypedDict(
     "DBInstanceMessageTypeDef",
     {
         "Marker": str,
         "DBInstances": List[DBInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBInstanceResultTypeDef = TypedDict(
     "DeleteDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBInstanceResultTypeDef = TypedDict(
     "ModifyDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootDBInstanceResultTypeDef = TypedDict(
     "RebootDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.py` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.pyi` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/PKG-INFO` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.28.12
-Summary: Type annotations for boto3.Neptune 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Neptune 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -424,104 +424,102 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CharacterSetTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     DBParameterGroupTypeDef,
-    CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
-    ParameterOutputTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
+    ParameterTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     DomainMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
-    DBParameterGroupNameMessageTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
-    DeleteDBClusterEndpointOutputTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
-    ModifyDBClusterEndpointOutputTypeDef,
-    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
-    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
+    CreateDBClusterEndpointOutputTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
+    DBParameterGroupNameMessageTypeDef,
+    DeleteDBClusterEndpointOutputTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
+    ModifyDBClusterEndpointOutputTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CopyDBParameterGroupMessageRequestTypeDef,
     CreateDBClusterEndpointMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     PendingModifiedValuesTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -537,61 +535,61 @@
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
-    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParameterGroupsMessageRequestTypeDef,
-    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
+    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DBClusterTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
```

### Comparing `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/SOURCES.txt` & `mypy-boto3-neptune-1.28.15/mypy_boto3_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.12/setup.py` & `mypy-boto3-neptune-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-neptune",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Neptune 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Neptune 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

