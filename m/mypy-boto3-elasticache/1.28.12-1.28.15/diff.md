# Comparing `tmp/mypy-boto3-elasticache-1.28.12.tar.gz` & `tmp/mypy-boto3-elasticache-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.28.15.tar", last modified: Fri Jul 28 20:42:44 2023, max compression
```

## Comparing `mypy-boto3-elasticache-1.28.12.tar` & `mypy-boto3-elasticache-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.536520 mypy-boto3-elasticache-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-27 05:34:38.532520 mypy-boto3-elasticache-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25958 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.532520 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68059 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67966 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    87751 2023-07-27 05:21:47.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    87684 2023-07-27 05:21:45.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.532520 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.536520 mypy-boto3-elasticache-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27283 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.989044 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67995 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67902 2023-07-28 20:25:06.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86615 2023-07-28 20:25:11.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86548 2023-07-28 20:25:08.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-28 20:25:07.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27283 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:43.000000 mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.997044 mypy-boto3-elasticache-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:25:05.000000 mypy-boto3-elasticache-1.28.15/setup.py
```

### Comparing `mypy-boto3-elasticache-1.28.12/LICENSE` & `mypy-boto3-elasticache-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/PKG-INFO` & `mypy-boto3-elasticache-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.12
-Summary: Type annotations for boto3.ElastiCache 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -466,15 +466,15 @@
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
@@ -482,18 +482,16 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
-    CloudWatchLogsDestinationDetailsOutputTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
@@ -503,91 +501,76 @@
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
-    KinesisFirehoseDestinationDetailsOutputTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
     NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
-    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
-    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
-    TagOutputTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
+    TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
@@ -595,48 +578,61 @@
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
-    DestinationDetailsOutputTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
     NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
-    TagListMessageTypeDef,
     UpdateActionResultsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
+    LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
-    LogDeliveryConfigurationRequestTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
@@ -647,20 +643,20 @@
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    PendingModifiedValuesTypeDef,
-    ReplicationGroupPendingModifiedValuesTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
+    PendingModifiedValuesTypeDef,
+    ReplicationGroupPendingModifiedValuesTypeDef,
     CopySnapshotResultTypeDef,
     CreateSnapshotResultTypeDef,
     DeleteSnapshotResultTypeDef,
     DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.12/README.md` & `mypy-boto3-elasticache-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -434,15 +434,15 @@
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
@@ -450,18 +450,16 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
-    CloudWatchLogsDestinationDetailsOutputTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
@@ -471,91 +469,76 @@
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
-    KinesisFirehoseDestinationDetailsOutputTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
     NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
-    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
-    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
-    TagOutputTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
+    TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
@@ -563,48 +546,61 @@
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
-    DestinationDetailsOutputTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
     NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
-    TagListMessageTypeDef,
     UpdateActionResultsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
+    LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
-    LogDeliveryConfigurationRequestTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
@@ -615,20 +611,20 @@
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    PendingModifiedValuesTypeDef,
-    ReplicationGroupPendingModifiedValuesTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
+    PendingModifiedValuesTypeDef,
+    ReplicationGroupPendingModifiedValuesTypeDef,
     CopySnapshotResultTypeDef,
     CreateSnapshotResultTypeDef,
     DeleteSnapshotResultTypeDef,
     DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ElastiCache 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
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

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,16 +111,16 @@
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
     TimeRangeFilterTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
-    UserResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
+    UserResponseTypeDef,
 )
 from .waiter import (
     CacheClusterAvailableWaiter,
     CacheClusterDeletedWaiter,
     ReplicationGroupAvailableWaiter,
     ReplicationGroupDeletedWaiter,
 )
@@ -494,30 +494,30 @@
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user)
         """
 
     def create_user_group(
         self,
         *,
         UserGroupId: str,
         Engine: str,
         UserIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user_group)
         """
 
@@ -626,23 +626,23 @@
         """
         Deletes an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_snapshot)
         """
 
-    def delete_user(self, *, UserId: str) -> UserResponseMetadataTypeDef:
+    def delete_user(self, *, UserId: str) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_user)
         """
 
-    def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseMetadataTypeDef:
+    def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_user_group)
         """
 
@@ -1128,29 +1128,29 @@
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user)
         """
 
     def modify_user_group(
         self,
         *,
         UserGroupId: str,
         UserIdsToAdd: Sequence[str] = ...,
         UserIdsToRemove: Sequence[str] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         Changes the list of users that belong to the user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user_group)
         """
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -111,16 +111,16 @@
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
     TimeRangeFilterTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
-    UserResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
+    UserResponseTypeDef,
 )
 from .waiter import (
     CacheClusterAvailableWaiter,
     CacheClusterDeletedWaiter,
     ReplicationGroupAvailableWaiter,
     ReplicationGroupDeletedWaiter,
 )
@@ -474,29 +474,29 @@
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user)
         """
     def create_user_group(
         self,
         *,
         UserGroupId: str,
         Engine: str,
         UserIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#create_user_group)
         """
     def decrease_node_groups_in_global_replication_group(
@@ -595,22 +595,22 @@
     def delete_snapshot(self, *, SnapshotName: str) -> DeleteSnapshotResultTypeDef:
         """
         Deletes an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_snapshot)
         """
-    def delete_user(self, *, UserId: str) -> UserResponseMetadataTypeDef:
+    def delete_user(self, *, UserId: str) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_user)
         """
-    def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseMetadataTypeDef:
+    def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#delete_user_group)
         """
     def describe_cache_clusters(
@@ -1065,28 +1065,28 @@
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user)
         """
     def modify_user_group(
         self,
         *,
         UserGroupId: str,
         UserIdsToAdd: Sequence[str] = ...,
         UserIdsToRemove: Sequence[str] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         Changes the list of users that belong to the user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#modify_user_group)
         """
     def purchase_reserved_cache_nodes_offering(
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 
@@ -140,33 +140,30 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 
 class DescribeCacheParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        CacheParameterGroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
         """
 
 
@@ -177,60 +174,60 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 
 class DescribeCacheSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
         """
 
 
 class DescribeCacheSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
         """
 
 
 class DescribeEngineDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
         """
 
 
@@ -244,15 +241,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeeventspaginator)
         """
 
 
@@ -263,30 +260,30 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 
 class DescribeReplicationGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
     """
 
     def paginate(
-        self, *, ReplicationGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReplicationGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReplicationGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
         """
 
 
@@ -301,15 +298,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 
@@ -323,15 +320,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 
@@ -342,15 +339,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 
@@ -364,15 +361,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describesnapshotspaginator)
         """
 
 
@@ -389,30 +386,30 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 
 class DescribeUserGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
     """
 
     def paginate(
-        self, *, UserGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUserGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
         """
 
 
@@ -424,13 +421,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 class DescribeCacheEngineVersionsPaginator(Paginator):
@@ -136,32 +136,29 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 class DescribeCacheParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        CacheParameterGroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparametergroupspaginator)
         """
 
 class DescribeCacheParametersPaginator(Paginator):
@@ -171,57 +168,57 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 class DescribeCacheSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesecuritygroupspaginator)
         """
 
 class DescribeCacheSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CacheSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describecachesubnetgroupspaginator)
         """
 
 class DescribeEngineDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeenginedefaultparameterspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -234,15 +231,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalReplicationGroupsPaginator(Paginator):
@@ -252,29 +249,29 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 class DescribeReplicationGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
     """
 
     def paginate(
-        self, *, ReplicationGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReplicationGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReplicationGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereplicationgroupspaginator)
         """
 
 class DescribeReservedCacheNodesPaginator(Paginator):
@@ -288,15 +285,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 class DescribeReservedCacheNodesOfferingsPaginator(Paginator):
@@ -309,15 +306,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 class DescribeServiceUpdatesPaginator(Paginator):
@@ -327,15 +324,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 class DescribeSnapshotsPaginator(Paginator):
@@ -348,15 +345,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describesnapshotspaginator)
         """
 
 class DescribeUpdateActionsPaginator(Paginator):
@@ -372,29 +369,29 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 class DescribeUserGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
     """
 
     def paginate(
-        self, *, UserGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUserGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeusergroupspaginator)
         """
 
 class DescribeUsersPaginator(Paginator):
@@ -405,13 +402,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "AllowedNodeTypeModificationsMessageTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
@@ -68,18 +68,16 @@
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "SecurityGroupMembershipTypeDef",
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
-    "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
-    "CloudWatchLogsDestinationDetailsOutputTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
     "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
@@ -89,91 +87,76 @@
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteReplicationGroupMessageRequestTypeDef",
     "DeleteSnapshotMessageRequestTypeDef",
     "DeleteUserGroupMessageRequestTypeDef",
     "DeleteUserMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCacheClustersMessageRequestTypeDef",
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
-    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
     "TimeRangeFilterTypeDef",
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
-    "KinesisFirehoseDestinationDetailsOutputTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
     "GlobalReplicationGroupMemberTypeDef",
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
     "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
-    "TagOutputTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    "CacheParameterGroupNameMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "TagListMessageTypeDef",
     "CreateUserMessageRequestTypeDef",
     "ModifyUserMessageRequestTypeDef",
-    "UserResponseMetadataTypeDef",
+    "UserResponseTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
@@ -181,48 +164,61 @@
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
-    "DestinationDetailsOutputTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
     "NodeSnapshotTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
-    "TagListMessageTypeDef",
     "UpdateActionResultsMessageTypeDef",
-    "UserGroupResponseMetadataTypeDef",
+    "UserGroupResponseTypeDef",
     "UserGroupTypeDef",
     "DescribeUsersResultTypeDef",
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
-    "LogDeliveryConfigurationRequestTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
@@ -233,20 +229,20 @@
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "PendingModifiedValuesTypeDef",
-    "ReplicationGroupPendingModifiedValuesTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
+    "PendingModifiedValuesTypeDef",
+    "ReplicationGroupPendingModifiedValuesTypeDef",
     "CopySnapshotResultTypeDef",
     "CreateSnapshotResultTypeDef",
     "DeleteSnapshotResultTypeDef",
     "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
@@ -275,20 +271,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
-    "AllowedNodeTypeModificationsMessageTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScaleUpModifications": List[str],
-        "ScaleDownModifications": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AuthenticationModeTypeDef = TypedDict(
     "AuthenticationModeTypeDef",
     {
         "Type": InputAuthenticationTypeType,
@@ -463,22 +461,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ChangeType": ChangeTypeType,
     },
     total=False,
 )
 
-CacheParameterGroupNameMessageTypeDef = TypedDict(
-    "CacheParameterGroupNameMessageTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheParameterGroupTypeDef = TypedDict(
     "CacheParameterGroupTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
         "IsGlobal": bool,
@@ -493,22 +483,14 @@
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-CloudWatchLogsDestinationDetailsOutputTypeDef = TypedDict(
-    "CloudWatchLogsDestinationDetailsOutputTypeDef",
-    {
-        "LogGroup": str,
-    },
-    total=False,
-)
-
 CloudWatchLogsDestinationDetailsTypeDef = TypedDict(
     "CloudWatchLogsDestinationDetailsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
@@ -726,21 +708,20 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CacheClusterId": str,
-        "ShowCacheNodeInfo": bool,
-        "ShowCacheClustersNotInReplicationGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCacheClustersMessageRequestTypeDef = TypedDict(
     "DescribeCacheClustersMessageRequestTypeDef",
     {
@@ -749,81 +730,37 @@
         "Marker": str,
         "ShowCacheNodeInfo": bool,
         "ShowCacheClustersNotInReplicationGroups": bool,
     },
     total=False,
 )
 
-DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "CacheParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
         "DefaultOnly": bool,
     },
     total=False,
 )
 
-DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-    },
-)
-_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
-    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCacheParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeCacheParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 _OptionalDescribeCacheParametersMessageRequestTypeDef = TypedDict(
@@ -840,74 +777,34 @@
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    {
-        "CacheSecurityGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    {
-        "CacheSubnetGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
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
         "CacheParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -923,95 +820,49 @@
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
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
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    {
-        "GlobalReplicationGroupId": str,
-        "ShowMemberInfo": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
     },
     total=False,
 )
 
-DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationGroupsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    {
-        "ReservedCacheNodeId": str,
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     {
         "ReservedCacheNodeId": str,
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
@@ -1019,75 +870,39 @@
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeServiceUpdatesMessageRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "CacheClusterId": str,
-        "SnapshotName": str,
-        "SnapshotSource": str,
-        "ShowNodeGroupConfig": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "SnapshotName": str,
         "SnapshotSource": str,
@@ -1103,23 +918,14 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
-DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    {
-        "UserGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1130,22 +936,14 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
-KinesisFirehoseDestinationDetailsOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationDetailsOutputTypeDef",
-    {
-        "DeliveryStream": str,
-    },
-    total=False,
-)
-
 KinesisFirehoseDestinationDetailsTypeDef = TypedDict(
     "KinesisFirehoseDestinationDetailsTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
@@ -1155,21 +953,14 @@
     {
         "GlobalReplicationGroupId": str,
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1348,24 +1139,14 @@
         "NodeUpdateInitiatedBy": NodeUpdateInitiatedByType,
         "NodeUpdateInitiatedDate": datetime,
         "NodeUpdateStatusModifiedDate": datetime,
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
 ProcessedUpdateActionTypeDef = TypedDict(
     "ProcessedUpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "UpdateActionStatus": UpdateActionStatusType,
@@ -1419,25 +1200,14 @@
     "SlotMigrationTypeDef",
     {
         "ProgressPercentage": float,
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
 RevokeCacheSecurityGroupIngressMessageRequestTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
@@ -1466,23 +1236,14 @@
     "SubnetOutpostTypeDef",
     {
         "SubnetOutpostArn": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 TestFailoverMessageRequestTypeDef = TypedDict(
     "TestFailoverMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupId": str,
     },
 )
@@ -1678,14 +1439,46 @@
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
 
+AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    {
+        "ScaleUpModifications": List[str],
+        "ScaleDownModifications": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CacheParameterGroupNameMessageTypeDef = TypedDict(
+    "CacheParameterGroupNameMessageTypeDef",
+    {
+        "CacheParameterGroupName": str,
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
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateUserMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserMessageRequestTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Engine": str,
         "AccessString": str,
@@ -1730,27 +1523,27 @@
 
 class ModifyUserMessageRequestTypeDef(
     _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
 ):
     pass
 
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
         "MinimumEngineVersion": str,
         "AccessString": str,
         "UserGroupIds": List[str],
         "Authentication": AuthenticationTypeDef,
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
@@ -1795,15 +1588,15 @@
 )
 
 CacheEngineVersionMessageTypeDef = TypedDict(
     "CacheEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "CacheEngineVersions": List[CacheEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheNodeTypeSpecificParameterTypeDef = TypedDict(
     "CacheNodeTypeSpecificParameterTypeDef",
     {
         "ParameterName": str,
@@ -1820,23 +1613,23 @@
 )
 
 CacheParameterGroupsMessageTypeDef = TypedDict(
     "CacheParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "CacheParameterGroups": List[CacheParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheParameterGroupResultTypeDef = TypedDict(
     "CreateCacheParameterGroupResultTypeDef",
     {
         "CacheParameterGroup": CacheParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupTypeDef = TypedDict(
     "CacheSecurityGroupTypeDef",
     {
         "OwnerId": str,
@@ -1949,26 +1742,212 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    {
+        "CacheClusterId": str,
+        "ShowCacheNodeInfo": bool,
+        "ShowCacheClustersNotInReplicationGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    {
+        "Engine": str,
+        "EngineVersion": str,
+        "CacheParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+    },
+)
+_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
+    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    {
+        "CacheSecurityGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    {
+        "CacheSubnetGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    {
+        "GlobalReplicationGroupId": str,
+        "ShowMemberInfo": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    {
+        "ReservedCacheNodeId": str,
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CacheClusterId": str,
+        "SnapshotName": str,
+        "SnapshotSource": str,
+        "ShowNodeGroupConfig": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    {
+        "UserGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
         "UpdateActionStatus": Sequence[UpdateActionStatusType],
         "ShowNodeLevelUpdateStatus": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
     "DescribeUpdateActionsMessageRequestTypeDef",
     {
@@ -1988,15 +1967,15 @@
 
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeUsersMessageRequestTypeDef = TypedDict(
     "DescribeUsersMessageRequestTypeDef",
     {
@@ -2005,38 +1984,29 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DestinationDetailsOutputTypeDef = TypedDict(
-    "DestinationDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsOutputTypeDef,
-        "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationDetailsTypeDef = TypedDict(
     "DestinationDetailsTypeDef",
     {
         "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsTypeDef,
         "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsTypeDef,
     },
     total=False,
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalReplicationGroupTypeDef = TypedDict(
     "GlobalReplicationGroupTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2189,58 +2159,50 @@
 )
 
 ServiceUpdatesMessageTypeDef = TypedDict(
     "ServiceUpdatesMessageTypeDef",
     {
         "Marker": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": SubnetOutpostTypeDef,
         "SupportedNetworkTypes": List[NetworkTypeType],
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
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserGroupResponseMetadataTypeDef = TypedDict(
-    "UserGroupResponseMetadataTypeDef",
+UserGroupResponseTypeDef = TypedDict(
+    "UserGroupResponseTypeDef",
     {
         "UserGroupId": str,
         "Status": str,
         "Engine": str,
         "UserIds": List[str],
         "MinimumEngineVersion": str,
         "PendingChanges": UserGroupPendingChangesTypeDef,
         "ReplicationGroups": List[str],
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserGroupTypeDef = TypedDict(
     "UserGroupTypeDef",
     {
         "UserGroupId": str,
@@ -2256,15 +2218,15 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeGroupTypeDef = TypedDict(
     "NodeGroupTypeDef",
     {
         "NodeGroupId": str,
@@ -2279,15 +2241,15 @@
 
 CacheParameterGroupDetailsTypeDef = TypedDict(
     "CacheParameterGroupDetailsTypeDef",
     {
         "Marker": str,
         "Parameters": List[ParameterTypeDef],
         "CacheNodeTypeSpecificParameters": List[CacheNodeTypeSpecificParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "CacheParameterGroupFamily": str,
@@ -2298,149 +2260,149 @@
     total=False,
 )
 
 AuthorizeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupMessageTypeDef = TypedDict(
     "CacheSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSecurityGroups": List[CacheSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSecurityGroupResultTypeDef = TypedDict(
     "CreateCacheSecurityGroupResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogDeliveryConfigurationTypeDef = TypedDict(
-    "LogDeliveryConfigurationTypeDef",
+LogDeliveryConfigurationRequestTypeDef = TypedDict(
+    "LogDeliveryConfigurationRequestTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsOutputTypeDef,
+        "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
-        "Status": LogDeliveryConfigurationStatusType,
-        "Message": str,
+        "Enabled": bool,
     },
     total=False,
 )
 
-PendingLogDeliveryConfigurationTypeDef = TypedDict(
-    "PendingLogDeliveryConfigurationTypeDef",
+LogDeliveryConfigurationTypeDef = TypedDict(
+    "LogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsOutputTypeDef,
+        "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
+        "Status": LogDeliveryConfigurationStatusType,
+        "Message": str,
     },
     total=False,
 )
 
-LogDeliveryConfigurationRequestTypeDef = TypedDict(
-    "LogDeliveryConfigurationRequestTypeDef",
+PendingLogDeliveryConfigurationTypeDef = TypedDict(
+    "PendingLogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
         "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
-        "Enabled": bool,
     },
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalReplicationGroupResultTypeDef = TypedDict(
     "DeleteGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalReplicationGroupsResultTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsResultTypeDef",
     {
         "Marker": str,
         "GlobalReplicationGroups": List[GlobalReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateGlobalReplicationGroupResultTypeDef = TypedDict(
     "DisassociateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalReplicationGroupResultTypeDef = TypedDict(
     "FailoverGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalReplicationGroupResultTypeDef = TypedDict(
     "ModifyGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebalanceSlotsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2523,33 +2485,33 @@
     total=False,
 )
 
 PurchaseReservedCacheNodesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     {
         "ReservedCacheNode": ReservedCacheNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodeMessageTypeDef = TypedDict(
     "ReservedCacheNodeMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodes": List[ReservedCacheNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodesOfferingMessageTypeDef = TypedDict(
     "ReservedCacheNodesOfferingMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodesOfferings": List[ReservedCacheNodesOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupTypeDef = TypedDict(
     "CacheSubnetGroupTypeDef",
     {
         "CacheSubnetGroupName": str,
@@ -2563,55 +2525,24 @@
 )
 
 DescribeUserGroupsResultTypeDef = TypedDict(
     "DescribeUserGroupsResultTypeDef",
     {
         "UserGroups": List[UserGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PendingModifiedValuesTypeDef = TypedDict(
-    "PendingModifiedValuesTypeDef",
-    {
-        "NumCacheNodes": int,
-        "CacheNodeIdsToRemove": List[str],
-        "EngineVersion": str,
-        "CacheNodeType": str,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
-)
-
-ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
-    "ReplicationGroupPendingModifiedValuesTypeDef",
-    {
-        "PrimaryClusterId": str,
-        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
-        "Resharding": ReshardingStatusTypeDef,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "UserGroups": UserGroupsUpdateStatusTypeDef,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
-        "ClusterMode": ClusterModeType,
-    },
-    total=False,
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
@@ -2804,78 +2735,109 @@
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
+PendingModifiedValuesTypeDef = TypedDict(
+    "PendingModifiedValuesTypeDef",
+    {
+        "NumCacheNodes": int,
+        "CacheNodeIdsToRemove": List[str],
+        "EngineVersion": str,
+        "CacheNodeType": str,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+    },
+    total=False,
+)
+
+ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
+    "ReplicationGroupPendingModifiedValuesTypeDef",
+    {
+        "PrimaryClusterId": str,
+        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
+        "Resharding": ReshardingStatusTypeDef,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "UserGroups": UserGroupsUpdateStatusTypeDef,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
+    },
+    total=False,
+)
+
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSnapshotResultTypeDef = TypedDict(
     "DeleteSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotsListMessageTypeDef = TypedDict(
     "DescribeSnapshotsListMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupMessageTypeDef = TypedDict(
     "CacheSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSubnetGroups": List[CacheSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSubnetGroupResultTypeDef = TypedDict(
     "CreateCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheSubnetGroupResultTypeDef = TypedDict(
     "ModifyCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheClusterTypeDef = TypedDict(
     "CacheClusterTypeDef",
     {
         "CacheClusterId": str,
@@ -2954,123 +2916,123 @@
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
         "Marker": str,
         "CacheClusters": List[CacheClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheClusterResultTypeDef = TypedDict(
     "CreateCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCacheClusterResultTypeDef = TypedDict(
     "DeleteCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheClusterResultTypeDef = TypedDict(
     "ModifyCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootCacheClusterResultTypeDef = TypedDict(
     "RebootCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompleteMigrationResponseTypeDef = TypedDict(
     "CompleteMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationGroupResultTypeDef = TypedDict(
     "CreateReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseReplicaCountResultTypeDef = TypedDict(
     "DecreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationGroupResultTypeDef = TypedDict(
     "DeleteReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseReplicaCountResultTypeDef = TypedDict(
     "IncreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupResultTypeDef = TypedDict(
     "ModifyReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupShardConfigurationResultTypeDef = TypedDict(
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationGroupMessageTypeDef = TypedDict(
     "ReplicationGroupMessageTypeDef",
     {
         "Marker": str,
         "ReplicationGroups": List[ReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "AllowedNodeTypeModificationsMessageTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
@@ -67,18 +67,16 @@
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "SecurityGroupMembershipTypeDef",
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
-    "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
-    "CloudWatchLogsDestinationDetailsOutputTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
     "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
@@ -88,91 +86,76 @@
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteReplicationGroupMessageRequestTypeDef",
     "DeleteSnapshotMessageRequestTypeDef",
     "DeleteUserGroupMessageRequestTypeDef",
     "DeleteUserMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCacheClustersMessageRequestTypeDef",
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
-    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
     "TimeRangeFilterTypeDef",
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
-    "KinesisFirehoseDestinationDetailsOutputTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
     "GlobalReplicationGroupMemberTypeDef",
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
     "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
-    "TagOutputTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    "CacheParameterGroupNameMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "TagListMessageTypeDef",
     "CreateUserMessageRequestTypeDef",
     "ModifyUserMessageRequestTypeDef",
-    "UserResponseMetadataTypeDef",
+    "UserResponseTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
@@ -180,48 +163,61 @@
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
-    "DestinationDetailsOutputTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
     "NodeSnapshotTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
-    "TagListMessageTypeDef",
     "UpdateActionResultsMessageTypeDef",
-    "UserGroupResponseMetadataTypeDef",
+    "UserGroupResponseTypeDef",
     "UserGroupTypeDef",
     "DescribeUsersResultTypeDef",
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
-    "LogDeliveryConfigurationRequestTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
@@ -232,20 +228,20 @@
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "PendingModifiedValuesTypeDef",
-    "ReplicationGroupPendingModifiedValuesTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
+    "PendingModifiedValuesTypeDef",
+    "ReplicationGroupPendingModifiedValuesTypeDef",
     "CopySnapshotResultTypeDef",
     "CreateSnapshotResultTypeDef",
     "DeleteSnapshotResultTypeDef",
     "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
@@ -274,20 +270,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
-    "AllowedNodeTypeModificationsMessageTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScaleUpModifications": List[str],
-        "ScaleDownModifications": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AuthenticationModeTypeDef = TypedDict(
     "AuthenticationModeTypeDef",
     {
         "Type": InputAuthenticationTypeType,
@@ -458,22 +456,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ChangeType": ChangeTypeType,
     },
     total=False,
 )
 
-CacheParameterGroupNameMessageTypeDef = TypedDict(
-    "CacheParameterGroupNameMessageTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheParameterGroupTypeDef = TypedDict(
     "CacheParameterGroupTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
         "IsGlobal": bool,
@@ -488,22 +478,14 @@
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-CloudWatchLogsDestinationDetailsOutputTypeDef = TypedDict(
-    "CloudWatchLogsDestinationDetailsOutputTypeDef",
-    {
-        "LogGroup": str,
-    },
-    total=False,
-)
-
 CloudWatchLogsDestinationDetailsTypeDef = TypedDict(
     "CloudWatchLogsDestinationDetailsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
@@ -709,21 +691,20 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CacheClusterId": str,
-        "ShowCacheNodeInfo": bool,
-        "ShowCacheClustersNotInReplicationGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCacheClustersMessageRequestTypeDef = TypedDict(
     "DescribeCacheClustersMessageRequestTypeDef",
     {
@@ -732,79 +713,37 @@
         "Marker": str,
         "ShowCacheNodeInfo": bool,
         "ShowCacheClustersNotInReplicationGroups": bool,
     },
     total=False,
 )
 
-DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "CacheParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
         "DefaultOnly": bool,
     },
     total=False,
 )
 
-DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-    },
-)
-_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
-    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCacheParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeCacheParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 _OptionalDescribeCacheParametersMessageRequestTypeDef = TypedDict(
@@ -819,72 +758,34 @@
 
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    {
-        "CacheSecurityGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    {
-        "CacheSubnetGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
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
         "CacheParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -898,95 +799,49 @@
 
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
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
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    {
-        "GlobalReplicationGroupId": str,
-        "ShowMemberInfo": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
     },
     total=False,
 )
 
-DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationGroupsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    {
-        "ReservedCacheNodeId": str,
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     {
         "ReservedCacheNodeId": str,
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
@@ -994,75 +849,39 @@
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeServiceUpdatesMessageRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "CacheClusterId": str,
-        "SnapshotName": str,
-        "SnapshotSource": str,
-        "ShowNodeGroupConfig": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "SnapshotName": str,
         "SnapshotSource": str,
@@ -1078,23 +897,14 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
-DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    {
-        "UserGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1105,22 +915,14 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
-KinesisFirehoseDestinationDetailsOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationDetailsOutputTypeDef",
-    {
-        "DeliveryStream": str,
-    },
-    total=False,
-)
-
 KinesisFirehoseDestinationDetailsTypeDef = TypedDict(
     "KinesisFirehoseDestinationDetailsTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
@@ -1130,21 +932,14 @@
     {
         "GlobalReplicationGroupId": str,
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1317,24 +1112,14 @@
         "NodeUpdateInitiatedBy": NodeUpdateInitiatedByType,
         "NodeUpdateInitiatedDate": datetime,
         "NodeUpdateStatusModifiedDate": datetime,
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
 ProcessedUpdateActionTypeDef = TypedDict(
     "ProcessedUpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "UpdateActionStatus": UpdateActionStatusType,
@@ -1388,25 +1173,14 @@
     "SlotMigrationTypeDef",
     {
         "ProgressPercentage": float,
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
 RevokeCacheSecurityGroupIngressMessageRequestTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
@@ -1435,23 +1209,14 @@
     "SubnetOutpostTypeDef",
     {
         "SubnetOutpostArn": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 TestFailoverMessageRequestTypeDef = TypedDict(
     "TestFailoverMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupId": str,
     },
 )
@@ -1633,14 +1398,46 @@
 
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
+AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    {
+        "ScaleUpModifications": List[str],
+        "ScaleDownModifications": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CacheParameterGroupNameMessageTypeDef = TypedDict(
+    "CacheParameterGroupNameMessageTypeDef",
+    {
+        "CacheParameterGroupName": str,
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
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateUserMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserMessageRequestTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Engine": str,
         "AccessString": str,
@@ -1681,27 +1478,27 @@
 )
 
 class ModifyUserMessageRequestTypeDef(
     _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
 ):
     pass
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
         "MinimumEngineVersion": str,
         "AccessString": str,
         "UserGroupIds": List[str],
         "Authentication": AuthenticationTypeDef,
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
@@ -1746,15 +1543,15 @@
 )
 
 CacheEngineVersionMessageTypeDef = TypedDict(
     "CacheEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "CacheEngineVersions": List[CacheEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheNodeTypeSpecificParameterTypeDef = TypedDict(
     "CacheNodeTypeSpecificParameterTypeDef",
     {
         "ParameterName": str,
@@ -1771,23 +1568,23 @@
 )
 
 CacheParameterGroupsMessageTypeDef = TypedDict(
     "CacheParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "CacheParameterGroups": List[CacheParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheParameterGroupResultTypeDef = TypedDict(
     "CreateCacheParameterGroupResultTypeDef",
     {
         "CacheParameterGroup": CacheParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupTypeDef = TypedDict(
     "CacheSecurityGroupTypeDef",
     {
         "OwnerId": str,
@@ -1896,26 +1693,208 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    {
+        "CacheClusterId": str,
+        "ShowCacheNodeInfo": bool,
+        "ShowCacheClustersNotInReplicationGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    {
+        "Engine": str,
+        "EngineVersion": str,
+        "CacheParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+    },
+)
+_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
+    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+):
+    pass
+
+DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    {
+        "CacheSecurityGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    {
+        "CacheSubnetGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+):
+    pass
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    {
+        "GlobalReplicationGroupId": str,
+        "ShowMemberInfo": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    {
+        "ReservedCacheNodeId": str,
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CacheClusterId": str,
+        "SnapshotName": str,
+        "SnapshotSource": str,
+        "ShowNodeGroupConfig": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    {
+        "UserGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
         "UpdateActionStatus": Sequence[UpdateActionStatusType],
         "ShowNodeLevelUpdateStatus": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
     "DescribeUpdateActionsMessageRequestTypeDef",
     {
@@ -1935,15 +1914,15 @@
 
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeUsersMessageRequestTypeDef = TypedDict(
     "DescribeUsersMessageRequestTypeDef",
     {
@@ -1952,38 +1931,29 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DestinationDetailsOutputTypeDef = TypedDict(
-    "DestinationDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsOutputTypeDef,
-        "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationDetailsTypeDef = TypedDict(
     "DestinationDetailsTypeDef",
     {
         "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsTypeDef,
         "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsTypeDef,
     },
     total=False,
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalReplicationGroupTypeDef = TypedDict(
     "GlobalReplicationGroupTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2132,58 +2102,50 @@
 )
 
 ServiceUpdatesMessageTypeDef = TypedDict(
     "ServiceUpdatesMessageTypeDef",
     {
         "Marker": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": SubnetOutpostTypeDef,
         "SupportedNetworkTypes": List[NetworkTypeType],
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
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserGroupResponseMetadataTypeDef = TypedDict(
-    "UserGroupResponseMetadataTypeDef",
+UserGroupResponseTypeDef = TypedDict(
+    "UserGroupResponseTypeDef",
     {
         "UserGroupId": str,
         "Status": str,
         "Engine": str,
         "UserIds": List[str],
         "MinimumEngineVersion": str,
         "PendingChanges": UserGroupPendingChangesTypeDef,
         "ReplicationGroups": List[str],
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserGroupTypeDef = TypedDict(
     "UserGroupTypeDef",
     {
         "UserGroupId": str,
@@ -2199,15 +2161,15 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeGroupTypeDef = TypedDict(
     "NodeGroupTypeDef",
     {
         "NodeGroupId": str,
@@ -2222,15 +2184,15 @@
 
 CacheParameterGroupDetailsTypeDef = TypedDict(
     "CacheParameterGroupDetailsTypeDef",
     {
         "Marker": str,
         "Parameters": List[ParameterTypeDef],
         "CacheNodeTypeSpecificParameters": List[CacheNodeTypeSpecificParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "CacheParameterGroupFamily": str,
@@ -2241,149 +2203,149 @@
     total=False,
 )
 
 AuthorizeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupMessageTypeDef = TypedDict(
     "CacheSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSecurityGroups": List[CacheSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSecurityGroupResultTypeDef = TypedDict(
     "CreateCacheSecurityGroupResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogDeliveryConfigurationTypeDef = TypedDict(
-    "LogDeliveryConfigurationTypeDef",
+LogDeliveryConfigurationRequestTypeDef = TypedDict(
+    "LogDeliveryConfigurationRequestTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsOutputTypeDef,
+        "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
-        "Status": LogDeliveryConfigurationStatusType,
-        "Message": str,
+        "Enabled": bool,
     },
     total=False,
 )
 
-PendingLogDeliveryConfigurationTypeDef = TypedDict(
-    "PendingLogDeliveryConfigurationTypeDef",
+LogDeliveryConfigurationTypeDef = TypedDict(
+    "LogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsOutputTypeDef,
+        "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
+        "Status": LogDeliveryConfigurationStatusType,
+        "Message": str,
     },
     total=False,
 )
 
-LogDeliveryConfigurationRequestTypeDef = TypedDict(
-    "LogDeliveryConfigurationRequestTypeDef",
+PendingLogDeliveryConfigurationTypeDef = TypedDict(
+    "PendingLogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
         "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
-        "Enabled": bool,
     },
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalReplicationGroupResultTypeDef = TypedDict(
     "DeleteGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalReplicationGroupsResultTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsResultTypeDef",
     {
         "Marker": str,
         "GlobalReplicationGroups": List[GlobalReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateGlobalReplicationGroupResultTypeDef = TypedDict(
     "DisassociateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalReplicationGroupResultTypeDef = TypedDict(
     "FailoverGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalReplicationGroupResultTypeDef = TypedDict(
     "ModifyGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebalanceSlotsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2464,33 +2426,33 @@
     total=False,
 )
 
 PurchaseReservedCacheNodesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     {
         "ReservedCacheNode": ReservedCacheNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodeMessageTypeDef = TypedDict(
     "ReservedCacheNodeMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodes": List[ReservedCacheNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodesOfferingMessageTypeDef = TypedDict(
     "ReservedCacheNodesOfferingMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodesOfferings": List[ReservedCacheNodesOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupTypeDef = TypedDict(
     "CacheSubnetGroupTypeDef",
     {
         "CacheSubnetGroupName": str,
@@ -2504,55 +2466,24 @@
 )
 
 DescribeUserGroupsResultTypeDef = TypedDict(
     "DescribeUserGroupsResultTypeDef",
     {
         "UserGroups": List[UserGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PendingModifiedValuesTypeDef = TypedDict(
-    "PendingModifiedValuesTypeDef",
-    {
-        "NumCacheNodes": int,
-        "CacheNodeIdsToRemove": List[str],
-        "EngineVersion": str,
-        "CacheNodeType": str,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
-    },
-    total=False,
-)
-
-ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
-    "ReplicationGroupPendingModifiedValuesTypeDef",
-    {
-        "PrimaryClusterId": str,
-        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
-        "Resharding": ReshardingStatusTypeDef,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "UserGroups": UserGroupsUpdateStatusTypeDef,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
-        "ClusterMode": ClusterModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
@@ -2737,78 +2668,109 @@
 
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+PendingModifiedValuesTypeDef = TypedDict(
+    "PendingModifiedValuesTypeDef",
+    {
+        "NumCacheNodes": int,
+        "CacheNodeIdsToRemove": List[str],
+        "EngineVersion": str,
+        "CacheNodeType": str,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+    },
+    total=False,
+)
+
+ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
+    "ReplicationGroupPendingModifiedValuesTypeDef",
+    {
+        "PrimaryClusterId": str,
+        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
+        "Resharding": ReshardingStatusTypeDef,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "UserGroups": UserGroupsUpdateStatusTypeDef,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
+    },
+    total=False,
+)
+
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSnapshotResultTypeDef = TypedDict(
     "DeleteSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotsListMessageTypeDef = TypedDict(
     "DescribeSnapshotsListMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupMessageTypeDef = TypedDict(
     "CacheSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSubnetGroups": List[CacheSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSubnetGroupResultTypeDef = TypedDict(
     "CreateCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheSubnetGroupResultTypeDef = TypedDict(
     "ModifyCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheClusterTypeDef = TypedDict(
     "CacheClusterTypeDef",
     {
         "CacheClusterId": str,
@@ -2887,123 +2849,123 @@
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
         "Marker": str,
         "CacheClusters": List[CacheClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheClusterResultTypeDef = TypedDict(
     "CreateCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCacheClusterResultTypeDef = TypedDict(
     "DeleteCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheClusterResultTypeDef = TypedDict(
     "ModifyCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootCacheClusterResultTypeDef = TypedDict(
     "RebootCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompleteMigrationResponseTypeDef = TypedDict(
     "CompleteMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationGroupResultTypeDef = TypedDict(
     "CreateReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseReplicaCountResultTypeDef = TypedDict(
     "DecreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationGroupResultTypeDef = TypedDict(
     "DeleteReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseReplicaCountResultTypeDef = TypedDict(
     "IncreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupResultTypeDef = TypedDict(
     "ModifyReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupShardConfigurationResultTypeDef = TypedDict(
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationGroupMessageTypeDef = TypedDict(
     "ReplicationGroupMessageTypeDef",
     {
         "Marker": str,
         "ReplicationGroups": List[ReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/PKG-INFO` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.12
-Summary: Type annotations for boto3.ElastiCache 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -466,15 +466,15 @@
 
 `mypy_boto3_elasticache.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticache.type_defs import (
     TagTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
@@ -482,18 +482,16 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
-    CloudWatchLogsDestinationDetailsOutputTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
@@ -503,91 +501,76 @@
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
-    KinesisFirehoseDestinationDetailsOutputTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
     NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
-    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
-    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
-    TagOutputTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
+    TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
@@ -595,48 +578,61 @@
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
-    DestinationDetailsOutputTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
     NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
-    TagListMessageTypeDef,
     UpdateActionResultsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
+    LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
-    LogDeliveryConfigurationRequestTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
@@ -647,20 +643,20 @@
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    PendingModifiedValuesTypeDef,
-    ReplicationGroupPendingModifiedValuesTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
+    PendingModifiedValuesTypeDef,
+    ReplicationGroupPendingModifiedValuesTypeDef,
     CopySnapshotResultTypeDef,
     CreateSnapshotResultTypeDef,
     DeleteSnapshotResultTypeDef,
     DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.28.15/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.12/setup.py` & `mypy-boto3-elasticache-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElastiCache 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ElastiCache 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

