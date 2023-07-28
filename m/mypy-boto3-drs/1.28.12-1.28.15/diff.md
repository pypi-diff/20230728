# Comparing `tmp/mypy-boto3-drs-1.28.12.tar.gz` & `tmp/mypy-boto3-drs-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-drs-1.28.12.tar", last modified: Thu Jul 27 05:34:35 2023, max compression
+gzip compressed data, was "mypy-boto3-drs-1.28.15.tar", last modified: Fri Jul 28 20:42:40 2023, max compression
```

## Comparing `mypy-boto3-drs-1.28.12.tar` & `mypy-boto3-drs-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20420 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/mypy_boto3_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39630 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58187 2023-07-27 05:20:31.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58138 2023-07-27 05:20:31.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:35.000000 mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:35.896529 mypy-boto3-drs-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:20:29.000000 mypy-boto3-drs-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.813000 mypy-boto3-drs-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-07-28 20:42:40.809000 mypy-boto3-drs-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.809000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39632 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-07-28 20:23:19.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-28 20:23:19.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56826 2023-07-28 20:23:21.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56779 2023-07-28 20:23:19.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.809000 mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-07-28 20:42:40.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:40.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:40.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:40.000000 mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:40.813000 mypy-boto3-drs-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:23:18.000000 mypy-boto3-drs-1.28.15/setup.py
```

### Comparing `mypy-boto3-drs-1.28.12/LICENSE` & `mypy-boto3-drs-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.12/PKG-INFO` & `mypy-boto3-drs-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.12
-Summary: Type annotations for boto3.drs 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.drs 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,143 +397,140 @@
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
     LicensingTypeDef,
     PITPolicyRuleTypeDef,
     CreateSourceNetworkRequestRequestTypeDef,
-    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     SourceNetworkDataTypeDef,
     ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
-    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
-    LicensingOutputTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PITPolicyRuleOutputTypeDef,
-    PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
-    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
-    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReverseReplicationResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
+    ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
     DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     EventResourceDataTypeDef,
-    LaunchConfigurationTemplateTypeDef,
-    LaunchConfigurationTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ReplicationConfigurationTemplateTypeDef,
     ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
     SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestRequestTypeDef,
-    DataReplicationInfoTypeDef,
-    JobLogEventDataTypeDef,
     CreateLaunchConfigurationTemplateResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     UpdateLaunchConfigurationTemplateResponseTypeDef,
-    LifeCycleTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
+    DataReplicationInfoTypeDef,
+    JobLogEventDataTypeDef,
+    LifeCycleTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
     AssociateSourceNetworkStackResponseTypeDef,
     DescribeJobsResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryResponseTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
```

### Comparing `mypy-boto3-drs-1.28.12/README.md` & `mypy-boto3-drs-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,143 +365,140 @@
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
     LicensingTypeDef,
     PITPolicyRuleTypeDef,
     CreateSourceNetworkRequestRequestTypeDef,
-    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     SourceNetworkDataTypeDef,
     ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
-    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
-    LicensingOutputTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PITPolicyRuleOutputTypeDef,
-    PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
-    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
-    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReverseReplicationResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
+    ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
     DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     EventResourceDataTypeDef,
-    LaunchConfigurationTemplateTypeDef,
-    LaunchConfigurationTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ReplicationConfigurationTemplateTypeDef,
     ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
     SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestRequestTypeDef,
-    DataReplicationInfoTypeDef,
-    JobLogEventDataTypeDef,
     CreateLaunchConfigurationTemplateResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     UpdateLaunchConfigurationTemplateResponseTypeDef,
-    LifeCycleTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
+    DataReplicationInfoTypeDef,
+    JobLogEventDataTypeDef,
+    LifeCycleTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
     AssociateSourceNetworkStackResponseTypeDef,
     DescribeJobsResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryResponseTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.py` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/__init__.pyi` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/__main__.py` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.drs 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.drs 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.py` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     LaunchConfigurationTypeDef,
     LicensingTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PITPolicyRuleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     ReverseReplicationResponseTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartRecoveryResponseTypeDef,
     StartReplicationResponseTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
@@ -199,15 +199,15 @@
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_replication_configuration_template)
         """
 
@@ -392,17 +392,15 @@
         """
         Disconnect a Recovery Instance from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_recovery_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#disconnect_recovery_instance)
         """
 
-    def disconnect_source_server(
-        self, *, sourceServerID: str
-    ) -> SourceServerResponseMetadataTypeDef:
+    def disconnect_source_server(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         Disconnects a specific Source Server from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#disconnect_source_server)
         """
 
@@ -491,15 +489,15 @@
         """
         List all tags for your Elastic Disaster Recovery resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#list_tags_for_resource)
         """
 
-    def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+    def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         WARNING: RetryDataReplication is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#retry_data_replication)
         """
 
@@ -725,15 +723,15 @@
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates a ReplicationConfigurationTemplate by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#update_replication_configuration_template)
         """
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/client.pyi` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     LaunchConfigurationTypeDef,
     LicensingTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PITPolicyRuleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     ReverseReplicationResponseTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartRecoveryResponseTypeDef,
     StartReplicationResponseTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
@@ -189,15 +189,15 @@
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#create_replication_configuration_template)
         """
     def create_source_network(
@@ -365,17 +365,15 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disconnect a Recovery Instance from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_recovery_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#disconnect_recovery_instance)
         """
-    def disconnect_source_server(
-        self, *, sourceServerID: str
-    ) -> SourceServerResponseMetadataTypeDef:
+    def disconnect_source_server(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         Disconnects a specific Source Server from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_source_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#disconnect_source_server)
         """
     def export_source_network_cfn_template(
@@ -454,15 +452,15 @@
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         List all tags for your Elastic Disaster Recovery resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#list_tags_for_resource)
         """
-    def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseMetadataTypeDef:
+    def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         WARNING: RetryDataReplication is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#retry_data_replication)
         """
     def reverse_replication(self, *, recoveryInstanceID: str) -> ReverseReplicationResponseTypeDef:
@@ -671,15 +669,15 @@
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates a ReplicationConfigurationTemplate by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/client/#update_replication_configuration_template)
         """
     @overload
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.py` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -651,24 +651,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/literals.pyi` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -649,24 +649,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.py` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,189 +70,177 @@
     "DescribeReplicationConfigurationTemplatesPaginator",
     "DescribeSourceNetworksPaginator",
     "DescribeSourceServersPaginator",
     "ListExtensibleSourceServersPaginator",
     "ListStagingAccountsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
         """
 
-
 class DescribeJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
         """
 
-
 class DescribeLaunchConfigurationTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
-
 class DescribeRecoveryInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
         """
 
-
 class DescribeRecoverySnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoverysnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
-
 class DescribeReplicationConfigurationTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
-
 class DescribeSourceNetworksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSourceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
         """
 
-
 class DescribeSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
         """
 
-
 class ListExtensibleSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
     """
 
     def paginate(
-        self, *, stagingAccountID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, stagingAccountID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExtensibleSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
         """
 
-
 class ListStagingAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStagingAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
         """
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/paginator.pyi` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,177 +70,189 @@
     "DescribeReplicationConfigurationTemplatesPaginator",
     "DescribeSourceNetworksPaginator",
     "DescribeSourceServersPaginator",
     "ListExtensibleSourceServersPaginator",
     "ListStagingAccountsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejoblogitemspaginator)
         """
 
+
 class DescribeJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describejobspaginator)
         """
 
+
 class DescribeLaunchConfigurationTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
+
 class DescribeRecoveryInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoveryinstancespaginator)
         """
 
+
 class DescribeRecoverySnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoverysnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
+
 class DescribeReplicationConfigurationTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
+
 class DescribeSourceNetworksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSourceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourcenetworkspaginator)
         """
 
+
 class DescribeSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#describesourceserverspaginator)
         """
 
+
 class ListExtensibleSourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
     """
 
     def paginate(
-        self, *, stagingAccountID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, stagingAccountID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExtensibleSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#listextensiblesourceserverspaginator)
         """
 
+
 class ListStagingAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStagingAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/paginators/#liststagingaccountspaginator)
         """
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.py` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,143 +54,140 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountTypeDef",
     "AssociateSourceNetworkStackRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CPUTypeDef",
     "ConversionPropertiesTypeDef",
     "CreateExtendedSourceServerRequestRequestTypeDef",
     "LicensingTypeDef",
     "PITPolicyRuleTypeDef",
     "CreateSourceNetworkRequestRequestTypeDef",
-    "CreateSourceNetworkResponseTypeDef",
     "DataReplicationErrorTypeDef",
     "DataReplicationInfoReplicatedDiskTypeDef",
     "DataReplicationInitiationStepTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceNetworkRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     "DescribeRecoverySnapshotsRequestFiltersTypeDef",
     "RecoverySnapshotTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "DescribeSourceNetworksRequestFiltersTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
     "DisconnectRecoveryInstanceRequestRequestTypeDef",
     "DisconnectSourceServerRequestRequestTypeDef",
     "DiskTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "SourceNetworkDataTypeDef",
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
-    "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
-    "LicensingOutputTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
-    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
-    "PITPolicyRuleOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
     "RecoveryLifeCycleTypeDef",
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
-    "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
     "StartFailbackLaunchRequestRequestTypeDef",
     "StartRecoveryRequestSourceServerTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
     "StartSourceNetworkReplicationRequestRequestTypeDef",
     "StopFailbackRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
+    "CreateSourceNetworkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    "GetFailbackReplicationConfigurationResponseTypeDef",
     "ListStagingAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ReverseReplicationResponseTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "LaunchConfigurationTemplateTypeDef",
+    "LaunchConfigurationTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
+    "ReplicationConfigurationTemplateResponseTypeDef",
+    "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     "DescribeSourceNetworksRequestRequestTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "EventResourceDataTypeDef",
-    "LaunchConfigurationTemplateTypeDef",
-    "LaunchConfigurationTypeDef",
     "LifeCycleLastLaunchTypeDef",
     "ListExtensibleSourceServersResponseTypeDef",
     "SourcePropertiesTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    "ReplicationConfigurationTemplateTypeDef",
     "ParticipatingResourceTypeDef",
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     "RecoveryInstancePropertiesTypeDef",
     "SourceNetworkTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "StartRecoveryRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestRequestTypeDef",
-    "DataReplicationInfoTypeDef",
-    "JobLogEventDataTypeDef",
     "CreateLaunchConfigurationTemplateResponseTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    "LifeCycleTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
+    "DataReplicationInfoTypeDef",
+    "JobLogEventDataTypeDef",
+    "LifeCycleTypeDef",
     "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
     "DescribeSourceNetworksResponseTypeDef",
     "StartSourceNetworkReplicationResponseTypeDef",
     "StopSourceNetworkReplicationResponseTypeDef",
     "JobLogTypeDef",
-    "SourceServerResponseMetadataTypeDef",
+    "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
     "AssociateSourceNetworkStackResponseTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartFailbackLaunchResponseTypeDef",
     "StartRecoveryResponseTypeDef",
     "StartSourceNetworkRecoveryResponseTypeDef",
     "TerminateRecoveryInstancesResponseTypeDef",
@@ -215,14 +212,25 @@
     "AssociateSourceNetworkStackRequestRequestTypeDef",
     {
         "cfnStackName": str,
         "sourceNetworkID": str,
     },
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
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
     total=False,
@@ -312,22 +320,14 @@
 class CreateSourceNetworkRequestRequestTypeDef(
     _RequiredCreateSourceNetworkRequestRequestTypeDef,
     _OptionalCreateSourceNetworkRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSourceNetworkResponseTypeDef = TypedDict(
-    "CreateSourceNetworkResponseTypeDef",
-    {
-        "sourceNetworkID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataReplicationErrorTypeDef = TypedDict(
     "DataReplicationErrorTypeDef",
     {
         "error": DataReplicationErrorStringType,
         "rawError": str,
     },
     total=False,
@@ -392,36 +392,24 @@
 DeleteSourceServerRequestRequestTypeDef = TypedDict(
     "DeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -447,23 +435,14 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
-DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    {
-        "launchConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     {
         "launchConfigurationTemplateIDs": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -506,23 +485,14 @@
 )
 
 
 class RecoverySnapshotTypeDef(_RequiredRecoverySnapshotTypeDef, _OptionalRecoverySnapshotTypeDef):
     pass
 
 
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
@@ -568,21 +538,14 @@
     {
         "bytes": int,
         "deviceName": str,
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
 SourceNetworkDataTypeDef = TypedDict(
     "SourceNetworkDataTypeDef",
     {
         "sourceNetworkID": str,
         "sourceVpc": str,
         "stackName": str,
         "targetVpc": str,
@@ -593,40 +556,21 @@
 ExportSourceNetworkCfnTemplateRequestRequestTypeDef = TypedDict(
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
     {
         "sourceNetworkID": str,
     },
 )
 
-ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
-    {
-        "s3DestinationUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFailbackReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetFailbackReplicationConfigurationResponseTypeDef",
-    {
-        "bandwidthThrottling": int,
-        "name": str,
-        "recoveryInstanceID": str,
-        "usePrivateIP": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "GetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -654,54 +598,24 @@
         "launchStatus": LaunchStatusType,
         "recoveryInstanceID": str,
         "sourceServerID": str,
     },
     total=False,
 )
 
-LicensingOutputTypeDef = TypedDict(
-    "LicensingOutputTypeDef",
-    {
-        "osByol": bool,
-    },
-    total=False,
-)
-
 LifeCycleLastLaunchInitiatedTypeDef = TypedDict(
     "LifeCycleLastLaunchInitiatedTypeDef",
     {
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
     total=False,
 )
 
-_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "stagingAccountID": str,
-    },
-)
-_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
-    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensibleSourceServersRequestRequestTypeDef",
     {
         "stagingAccountID": str,
     },
 )
 _OptionalListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
@@ -727,22 +641,14 @@
         "arn": str,
         "hostname": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStagingAccountsRequestRequestTypeDef = TypedDict(
     "ListStagingAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -751,22 +657,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
     },
@@ -777,48 +675,14 @@
     "OSTypeDef",
     {
         "fullString": str,
     },
     total=False,
 )
 
-_RequiredPITPolicyRuleOutputTypeDef = TypedDict(
-    "_RequiredPITPolicyRuleOutputTypeDef",
-    {
-        "interval": int,
-        "retentionDuration": int,
-        "units": PITPolicyRuleUnitsType,
-    },
-)
-_OptionalPITPolicyRuleOutputTypeDef = TypedDict(
-    "_OptionalPITPolicyRuleOutputTypeDef",
-    {
-        "enabled": bool,
-        "ruleID": int,
-    },
-    total=False,
-)
-
-
-class PITPolicyRuleOutputTypeDef(
-    _RequiredPITPolicyRuleOutputTypeDef, _OptionalPITPolicyRuleOutputTypeDef
-):
-    pass
-
-
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
 ParticipatingResourceIDTypeDef = TypedDict(
     "ParticipatingResourceIDTypeDef",
     {
         "sourceNetworkID": str,
     },
     total=False,
 )
@@ -886,73 +750,41 @@
         "apiCallDateTime": datetime,
         "jobID": str,
         "lastRecoveryResult": RecoveryResultType,
     },
     total=False,
 )
 
-ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
-    {
-        "deviceName": str,
-        "iops": int,
-        "isBootDisk": bool,
-        "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
-        "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
-        "throughput": int,
-    },
-    total=False,
-)
-
 ReplicationConfigurationReplicatedDiskTypeDef = TypedDict(
     "ReplicationConfigurationReplicatedDiskTypeDef",
     {
         "deviceName": str,
         "iops": int,
         "isBootDisk": bool,
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
 ReverseReplicationRequestRequestTypeDef = TypedDict(
     "ReverseReplicationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-ReverseReplicationResponseTypeDef = TypedDict(
-    "ReverseReplicationResponseTypeDef",
-    {
-        "reversedDirectionSourceServerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": str,
         "originAvailabilityZone": str,
         "originRegion": str,
     },
@@ -1114,20 +946,70 @@
 class UpdateFailbackReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+CreateSourceNetworkResponseTypeDef = TypedDict(
+    "CreateSourceNetworkResponseTypeDef",
+    {
+        "sourceNetworkID": str,
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
+ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    {
+        "s3DestinationUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetFailbackReplicationConfigurationResponseTypeDef",
+    {
+        "bandwidthThrottling": int,
+        "name": str,
+        "recoveryInstanceID": str,
+        "usePrivateIP": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStagingAccountsResponseTypeDef = TypedDict(
     "ListStagingAccountsResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReverseReplicationResponseTypeDef = TypedDict(
+    "ReverseReplicationResponseTypeDef",
+    {
+        "reversedDirectionSourceServerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "copyPrivateIp": bool,
@@ -1137,14 +1019,45 @@
         "licensing": LicensingTypeDef,
         "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
+LaunchConfigurationTemplateTypeDef = TypedDict(
+    "LaunchConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchConfigurationTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "tags": Dict[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "name": str,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
@@ -1226,14 +1139,75 @@
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+ReplicationConfigurationTemplateResponseTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleTypeDef],
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredReplicationConfigurationTemplateTypeDef",
+    {
+        "replicationConfigurationTemplateID": str,
+    },
+)
+_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalReplicationConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+    },
+    total=False,
+)
+
+
+class ReplicationConfigurationTemplateTypeDef(
+    _RequiredReplicationConfigurationTemplateTypeDef,
+    _OptionalReplicationConfigurationTemplateTypeDef,
+):
+    pass
+
+
 _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
@@ -1272,19 +1246,89 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
+
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "stagingAccountID": str,
+    },
+)
+_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
+    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+):
+    pass
+
+
+ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1295,15 +1339,15 @@
     total=False,
 )
 
 DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     {
         "filters": DescribeRecoveryInstancesRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeRecoveryInstancesRequestRequestTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     {
@@ -1321,15 +1365,15 @@
     },
 )
 _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef = TypedDict(
     "_OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     {
         "filters": DescribeRecoverySnapshotsRequestFiltersTypeDef,
         "order": RecoverySnapshotsOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef(
     _RequiredDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
@@ -1364,23 +1408,23 @@
 
 
 DescribeRecoverySnapshotsResponseTypeDef = TypedDict(
     "DescribeRecoverySnapshotsResponseTypeDef",
     {
         "items": List[RecoverySnapshotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef = TypedDict(
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     {
         "filters": DescribeSourceNetworksRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceNetworksRequestRequestTypeDef = TypedDict(
     "DescribeSourceNetworksRequestRequestTypeDef",
     {
@@ -1391,15 +1435,15 @@
     total=False,
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1414,60 +1458,29 @@
     "EventResourceDataTypeDef",
     {
         "sourceNetworkData": SourceNetworkDataTypeDef,
     },
     total=False,
 )
 
-LaunchConfigurationTemplateTypeDef = TypedDict(
-    "LaunchConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "exportBucketArn": str,
-        "launchConfigurationTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
-        "tags": Dict[str, str],
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-    },
-    total=False,
-)
-
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
-    {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
-        "name": str,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
         "status": LaunchStatusType,
     },
     total=False,
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
         "items": List[StagingSourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourcePropertiesTypeDef = TypedDict(
     "SourcePropertiesTypeDef",
     {
         "cpus": List[CPUTypeDef],
@@ -1479,75 +1492,14 @@
         "ramBytes": int,
         "recommendedInstanceType": str,
         "supportsNitroInstances": bool,
     },
     total=False,
 )
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredReplicationConfigurationTemplateTypeDef",
-    {
-        "replicationConfigurationTemplateID": str,
-    },
-)
-_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalReplicationConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-    },
-    total=False,
-)
-
-
-class ReplicationConfigurationTemplateTypeDef(
-    _RequiredReplicationConfigurationTemplateTypeDef,
-    _OptionalReplicationConfigurationTemplateTypeDef,
-):
-    pass
-
-
 ParticipatingResourceTypeDef = TypedDict(
     "ParticipatingResourceTypeDef",
     {
         "launchStatus": LaunchStatusType,
         "participatingResourceID": ParticipatingResourceIDTypeDef,
     },
     total=False,
@@ -1602,23 +1554,23 @@
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
-        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
+        "pitPolicy": List[PITPolicyRuleTypeDef],
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1696,14 +1648,48 @@
 class StartSourceNetworkRecoveryRequestRequestTypeDef(
     _RequiredStartSourceNetworkRecoveryRequestRequestTypeDef,
     _OptionalStartSourceNetworkRecoveryRequestRequestTypeDef,
 ):
     pass
 
 
+CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[LaunchConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[ReplicationConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
         "dataReplicationInitiation": DataReplicationInitiationTypeDef,
         "dataReplicationState": DataReplicationStateType,
         "etaDateTime": str,
@@ -1723,60 +1709,26 @@
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
-CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[LaunchConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
         "elapsedReplicationDuration": str,
         "firstByteDateTime": str,
         "lastLaunch": LifeCycleLastLaunchTypeDef,
         "lastSeenByServiceDateTime": str,
     },
     total=False,
 )
 
-DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[ReplicationConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalJobTypeDef = TypedDict(
@@ -1815,61 +1767,61 @@
 )
 
 DescribeSourceNetworksResponseTypeDef = TypedDict(
     "DescribeSourceNetworksResponseTypeDef",
     {
         "items": List[SourceNetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StartSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StopSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
     total=False,
 )
 
-SourceServerResponseMetadataTypeDef = TypedDict(
-    "SourceServerResponseMetadataTypeDef",
+SourceServerResponseTypeDef = TypedDict(
+    "SourceServerResponseTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
         "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "arn": str,
@@ -1889,56 +1841,56 @@
     total=False,
 )
 
 AssociateSourceNetworkStackResponseTypeDef = TypedDict(
     "AssociateSourceNetworkStackResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFailbackLaunchResponseTypeDef = TypedDict(
     "StartFailbackLaunchResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRecoveryResponseTypeDef = TypedDict(
     "StartRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkRecoveryResponseTypeDef = TypedDict(
     "StartSourceNetworkRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateRecoveryInstancesResponseTypeDef = TypedDict(
     "TerminateRecoveryInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecoveryInstanceTypeDef = TypedDict(
     "RecoveryInstanceTypeDef",
     {
         "arn": str,
@@ -1960,52 +1912,52 @@
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
         "items": List[JobLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExtendedSourceServerResponseTypeDef = TypedDict(
     "CreateExtendedSourceServerResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecoveryInstancesResponseTypeDef = TypedDict(
     "DescribeRecoveryInstancesResponseTypeDef",
     {
         "items": List[RecoveryInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs/type_defs.pyi` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,143 +53,140 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountTypeDef",
     "AssociateSourceNetworkStackRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CPUTypeDef",
     "ConversionPropertiesTypeDef",
     "CreateExtendedSourceServerRequestRequestTypeDef",
     "LicensingTypeDef",
     "PITPolicyRuleTypeDef",
     "CreateSourceNetworkRequestRequestTypeDef",
-    "CreateSourceNetworkResponseTypeDef",
     "DataReplicationErrorTypeDef",
     "DataReplicationInfoReplicatedDiskTypeDef",
     "DataReplicationInitiationStepTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceNetworkRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     "DescribeRecoverySnapshotsRequestFiltersTypeDef",
     "RecoverySnapshotTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "DescribeSourceNetworksRequestFiltersTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
     "DisconnectRecoveryInstanceRequestRequestTypeDef",
     "DisconnectSourceServerRequestRequestTypeDef",
     "DiskTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "SourceNetworkDataTypeDef",
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
-    "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
-    "LicensingOutputTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
-    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
-    "PITPolicyRuleOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
     "RecoveryLifeCycleTypeDef",
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
-    "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
     "StartFailbackLaunchRequestRequestTypeDef",
     "StartRecoveryRequestSourceServerTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
     "StartSourceNetworkReplicationRequestRequestTypeDef",
     "StopFailbackRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
+    "CreateSourceNetworkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    "GetFailbackReplicationConfigurationResponseTypeDef",
     "ListStagingAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ReverseReplicationResponseTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "LaunchConfigurationTemplateTypeDef",
+    "LaunchConfigurationTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
+    "ReplicationConfigurationTemplateResponseTypeDef",
+    "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     "DescribeSourceNetworksRequestRequestTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "EventResourceDataTypeDef",
-    "LaunchConfigurationTemplateTypeDef",
-    "LaunchConfigurationTypeDef",
     "LifeCycleLastLaunchTypeDef",
     "ListExtensibleSourceServersResponseTypeDef",
     "SourcePropertiesTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    "ReplicationConfigurationTemplateTypeDef",
     "ParticipatingResourceTypeDef",
     "RecoveryInstanceDataReplicationInitiationTypeDef",
     "RecoveryInstancePropertiesTypeDef",
     "SourceNetworkTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "StartRecoveryRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestRequestTypeDef",
-    "DataReplicationInfoTypeDef",
-    "JobLogEventDataTypeDef",
     "CreateLaunchConfigurationTemplateResponseTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    "LifeCycleTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
+    "DataReplicationInfoTypeDef",
+    "JobLogEventDataTypeDef",
+    "LifeCycleTypeDef",
     "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
     "DescribeSourceNetworksResponseTypeDef",
     "StartSourceNetworkReplicationResponseTypeDef",
     "StopSourceNetworkReplicationResponseTypeDef",
     "JobLogTypeDef",
-    "SourceServerResponseMetadataTypeDef",
+    "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
     "AssociateSourceNetworkStackResponseTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartFailbackLaunchResponseTypeDef",
     "StartRecoveryResponseTypeDef",
     "StartSourceNetworkRecoveryResponseTypeDef",
     "TerminateRecoveryInstancesResponseTypeDef",
@@ -214,14 +211,25 @@
     "AssociateSourceNetworkStackRequestRequestTypeDef",
     {
         "cfnStackName": str,
         "sourceNetworkID": str,
     },
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
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
     total=False,
@@ -305,22 +313,14 @@
 
 class CreateSourceNetworkRequestRequestTypeDef(
     _RequiredCreateSourceNetworkRequestRequestTypeDef,
     _OptionalCreateSourceNetworkRequestRequestTypeDef,
 ):
     pass
 
-CreateSourceNetworkResponseTypeDef = TypedDict(
-    "CreateSourceNetworkResponseTypeDef",
-    {
-        "sourceNetworkID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataReplicationErrorTypeDef = TypedDict(
     "DataReplicationErrorTypeDef",
     {
         "error": DataReplicationErrorStringType,
         "rawError": str,
     },
     total=False,
@@ -385,34 +385,24 @@
 DeleteSourceServerRequestRequestTypeDef = TypedDict(
     "DeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -436,23 +426,14 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
-DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    {
-        "launchConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     {
         "launchConfigurationTemplateIDs": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -493,23 +474,14 @@
     },
     total=False,
 )
 
 class RecoverySnapshotTypeDef(_RequiredRecoverySnapshotTypeDef, _OptionalRecoverySnapshotTypeDef):
     pass
 
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
@@ -555,21 +527,14 @@
     {
         "bytes": int,
         "deviceName": str,
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
 SourceNetworkDataTypeDef = TypedDict(
     "SourceNetworkDataTypeDef",
     {
         "sourceNetworkID": str,
         "sourceVpc": str,
         "stackName": str,
         "targetVpc": str,
@@ -580,40 +545,21 @@
 ExportSourceNetworkCfnTemplateRequestRequestTypeDef = TypedDict(
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
     {
         "sourceNetworkID": str,
     },
 )
 
-ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
-    {
-        "s3DestinationUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFailbackReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetFailbackReplicationConfigurationResponseTypeDef",
-    {
-        "bandwidthThrottling": int,
-        "name": str,
-        "recoveryInstanceID": str,
-        "usePrivateIP": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "GetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -641,52 +587,24 @@
         "launchStatus": LaunchStatusType,
         "recoveryInstanceID": str,
         "sourceServerID": str,
     },
     total=False,
 )
 
-LicensingOutputTypeDef = TypedDict(
-    "LicensingOutputTypeDef",
-    {
-        "osByol": bool,
-    },
-    total=False,
-)
-
 LifeCycleLastLaunchInitiatedTypeDef = TypedDict(
     "LifeCycleLastLaunchInitiatedTypeDef",
     {
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
     total=False,
 )
 
-_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "stagingAccountID": str,
-    },
-)
-_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
-    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-):
-    pass
-
 _RequiredListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensibleSourceServersRequestRequestTypeDef",
     {
         "stagingAccountID": str,
     },
 )
 _OptionalListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
@@ -710,22 +628,14 @@
         "arn": str,
         "hostname": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStagingAccountsRequestRequestTypeDef = TypedDict(
     "ListStagingAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -734,22 +644,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
     },
@@ -760,46 +662,14 @@
     "OSTypeDef",
     {
         "fullString": str,
     },
     total=False,
 )
 
-_RequiredPITPolicyRuleOutputTypeDef = TypedDict(
-    "_RequiredPITPolicyRuleOutputTypeDef",
-    {
-        "interval": int,
-        "retentionDuration": int,
-        "units": PITPolicyRuleUnitsType,
-    },
-)
-_OptionalPITPolicyRuleOutputTypeDef = TypedDict(
-    "_OptionalPITPolicyRuleOutputTypeDef",
-    {
-        "enabled": bool,
-        "ruleID": int,
-    },
-    total=False,
-)
-
-class PITPolicyRuleOutputTypeDef(
-    _RequiredPITPolicyRuleOutputTypeDef, _OptionalPITPolicyRuleOutputTypeDef
-):
-    pass
-
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
 ParticipatingResourceIDTypeDef = TypedDict(
     "ParticipatingResourceIDTypeDef",
     {
         "sourceNetworkID": str,
     },
     total=False,
 )
@@ -867,73 +737,41 @@
         "apiCallDateTime": datetime,
         "jobID": str,
         "lastRecoveryResult": RecoveryResultType,
     },
     total=False,
 )
 
-ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
-    {
-        "deviceName": str,
-        "iops": int,
-        "isBootDisk": bool,
-        "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
-        "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
-        "throughput": int,
-    },
-    total=False,
-)
-
 ReplicationConfigurationReplicatedDiskTypeDef = TypedDict(
     "ReplicationConfigurationReplicatedDiskTypeDef",
     {
         "deviceName": str,
         "iops": int,
         "isBootDisk": bool,
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
 ReverseReplicationRequestRequestTypeDef = TypedDict(
     "ReverseReplicationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-ReverseReplicationResponseTypeDef = TypedDict(
-    "ReverseReplicationResponseTypeDef",
-    {
-        "reversedDirectionSourceServerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": str,
         "originAvailabilityZone": str,
         "originRegion": str,
     },
@@ -1087,20 +925,70 @@
 
 class UpdateFailbackReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+CreateSourceNetworkResponseTypeDef = TypedDict(
+    "CreateSourceNetworkResponseTypeDef",
+    {
+        "sourceNetworkID": str,
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
+ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    {
+        "s3DestinationUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetFailbackReplicationConfigurationResponseTypeDef",
+    {
+        "bandwidthThrottling": int,
+        "name": str,
+        "recoveryInstanceID": str,
+        "usePrivateIP": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStagingAccountsResponseTypeDef = TypedDict(
     "ListStagingAccountsResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReverseReplicationResponseTypeDef = TypedDict(
+    "ReverseReplicationResponseTypeDef",
+    {
+        "reversedDirectionSourceServerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "copyPrivateIp": bool,
@@ -1110,14 +998,45 @@
         "licensing": LicensingTypeDef,
         "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
+LaunchConfigurationTemplateTypeDef = TypedDict(
+    "LaunchConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "exportBucketArn": str,
+        "launchConfigurationTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "tags": Dict[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
+    {
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "name": str,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
@@ -1193,14 +1112,73 @@
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
+ReplicationConfigurationTemplateResponseTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleTypeDef],
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredReplicationConfigurationTemplateTypeDef",
+    {
+        "replicationConfigurationTemplateID": str,
+    },
+)
+_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalReplicationConfigurationTemplateTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "autoReplicateNewDisks": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "pitPolicy": List[PITPolicyRuleTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+    },
+    total=False,
+)
+
+class ReplicationConfigurationTemplateTypeDef(
+    _RequiredReplicationConfigurationTemplateTypeDef,
+    _OptionalReplicationConfigurationTemplateTypeDef,
+):
+    pass
+
 _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
@@ -1237,19 +1215,85 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "stagingAccountID": str,
+    },
+)
+_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
+    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+):
+    pass
+
+ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1260,15 +1304,15 @@
     total=False,
 )
 
 DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     {
         "filters": DescribeRecoveryInstancesRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeRecoveryInstancesRequestRequestTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     {
@@ -1286,15 +1330,15 @@
     },
 )
 _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef = TypedDict(
     "_OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     {
         "filters": DescribeRecoverySnapshotsRequestFiltersTypeDef,
         "order": RecoverySnapshotsOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef(
     _RequiredDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
@@ -1325,23 +1369,23 @@
     pass
 
 DescribeRecoverySnapshotsResponseTypeDef = TypedDict(
     "DescribeRecoverySnapshotsResponseTypeDef",
     {
         "items": List[RecoverySnapshotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef = TypedDict(
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     {
         "filters": DescribeSourceNetworksRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceNetworksRequestRequestTypeDef = TypedDict(
     "DescribeSourceNetworksRequestRequestTypeDef",
     {
@@ -1352,15 +1396,15 @@
     total=False,
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1375,60 +1419,29 @@
     "EventResourceDataTypeDef",
     {
         "sourceNetworkData": SourceNetworkDataTypeDef,
     },
     total=False,
 )
 
-LaunchConfigurationTemplateTypeDef = TypedDict(
-    "LaunchConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "exportBucketArn": str,
-        "launchConfigurationTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
-        "tags": Dict[str, str],
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-    },
-    total=False,
-)
-
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
-    {
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
-        "name": str,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
         "status": LaunchStatusType,
     },
     total=False,
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
         "items": List[StagingSourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourcePropertiesTypeDef = TypedDict(
     "SourcePropertiesTypeDef",
     {
         "cpus": List[CPUTypeDef],
@@ -1440,73 +1453,14 @@
         "ramBytes": int,
         "recommendedInstanceType": str,
         "supportsNitroInstances": bool,
     },
     total=False,
 )
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredReplicationConfigurationTemplateTypeDef",
-    {
-        "replicationConfigurationTemplateID": str,
-    },
-)
-_OptionalReplicationConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalReplicationConfigurationTemplateTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "autoReplicateNewDisks": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-    },
-    total=False,
-)
-
-class ReplicationConfigurationTemplateTypeDef(
-    _RequiredReplicationConfigurationTemplateTypeDef,
-    _OptionalReplicationConfigurationTemplateTypeDef,
-):
-    pass
-
 ParticipatingResourceTypeDef = TypedDict(
     "ParticipatingResourceTypeDef",
     {
         "launchStatus": LaunchStatusType,
         "participatingResourceID": ParticipatingResourceIDTypeDef,
     },
     total=False,
@@ -1561,23 +1515,23 @@
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
-        "pitPolicy": List[PITPolicyRuleOutputTypeDef],
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
+        "pitPolicy": List[PITPolicyRuleTypeDef],
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1649,14 +1603,48 @@
 
 class StartSourceNetworkRecoveryRequestRequestTypeDef(
     _RequiredStartSourceNetworkRecoveryRequestRequestTypeDef,
     _OptionalStartSourceNetworkRecoveryRequestRequestTypeDef,
 ):
     pass
 
+CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[LaunchConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "UpdateLaunchConfigurationTemplateResponseTypeDef",
+    {
+        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
+    {
+        "items": List[ReplicationConfigurationTemplateTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
         "dataReplicationInitiation": DataReplicationInitiationTypeDef,
         "dataReplicationState": DataReplicationStateType,
         "etaDateTime": str,
@@ -1676,60 +1664,26 @@
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
-CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[LaunchConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
-    "UpdateLaunchConfigurationTemplateResponseTypeDef",
-    {
-        "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
         "elapsedReplicationDuration": str,
         "firstByteDateTime": str,
         "lastLaunch": LifeCycleLastLaunchTypeDef,
         "lastSeenByServiceDateTime": str,
     },
     total=False,
 )
 
-DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesResponseTypeDef",
-    {
-        "items": List[ReplicationConfigurationTemplateTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalJobTypeDef = TypedDict(
@@ -1766,61 +1720,61 @@
 )
 
 DescribeSourceNetworksResponseTypeDef = TypedDict(
     "DescribeSourceNetworksResponseTypeDef",
     {
         "items": List[SourceNetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StartSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StopSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
     total=False,
 )
 
-SourceServerResponseMetadataTypeDef = TypedDict(
-    "SourceServerResponseMetadataTypeDef",
+SourceServerResponseTypeDef = TypedDict(
+    "SourceServerResponseTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
         "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "arn": str,
@@ -1840,56 +1794,56 @@
     total=False,
 )
 
 AssociateSourceNetworkStackResponseTypeDef = TypedDict(
     "AssociateSourceNetworkStackResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFailbackLaunchResponseTypeDef = TypedDict(
     "StartFailbackLaunchResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRecoveryResponseTypeDef = TypedDict(
     "StartRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkRecoveryResponseTypeDef = TypedDict(
     "StartSourceNetworkRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateRecoveryInstancesResponseTypeDef = TypedDict(
     "TerminateRecoveryInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecoveryInstanceTypeDef = TypedDict(
     "RecoveryInstanceTypeDef",
     {
         "arn": str,
@@ -1911,52 +1865,52 @@
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
         "items": List[JobLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExtendedSourceServerResponseTypeDef = TypedDict(
     "CreateExtendedSourceServerResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecoveryInstancesResponseTypeDef = TypedDict(
     "DescribeRecoveryInstancesResponseTypeDef",
     {
         "items": List[RecoveryInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/PKG-INFO` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.12
-Summary: Type annotations for boto3.drs 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.drs 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,143 +397,140 @@
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
     LicensingTypeDef,
     PITPolicyRuleTypeDef,
     CreateSourceNetworkRequestRequestTypeDef,
-    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     SourceNetworkDataTypeDef,
     ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
-    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
-    LicensingOutputTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PITPolicyRuleOutputTypeDef,
-    PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
-    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
-    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReverseReplicationResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    LaunchConfigurationTemplateTypeDef,
+    LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
+    ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
     DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef,
     DescribeSourceNetworksRequestRequestTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     EventResourceDataTypeDef,
-    LaunchConfigurationTemplateTypeDef,
-    LaunchConfigurationTypeDef,
     LifeCycleLastLaunchTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     SourcePropertiesTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ReplicationConfigurationTemplateTypeDef,
     ParticipatingResourceTypeDef,
     RecoveryInstanceDataReplicationInitiationTypeDef,
     RecoveryInstancePropertiesTypeDef,
     SourceNetworkTypeDef,
     ReplicationConfigurationTypeDef,
     UpdateReplicationConfigurationRequestRequestTypeDef,
     StartRecoveryRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestRequestTypeDef,
-    DataReplicationInfoTypeDef,
-    JobLogEventDataTypeDef,
     CreateLaunchConfigurationTemplateResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     UpdateLaunchConfigurationTemplateResponseTypeDef,
-    LifeCycleTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
+    DataReplicationInfoTypeDef,
+    JobLogEventDataTypeDef,
+    LifeCycleTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
     AssociateSourceNetworkStackResponseTypeDef,
     DescribeJobsResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryResponseTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
```

### Comparing `mypy-boto3-drs-1.28.12/mypy_boto3_drs.egg-info/SOURCES.txt` & `mypy-boto3-drs-1.28.15/mypy_boto3_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.12/setup.py` & `mypy-boto3-drs-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-drs",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.drs 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.drs 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

