# Comparing `tmp/mypy-boto3-mgn-1.28.12.tar.gz` & `tmp/mypy-boto3-mgn-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgn-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
+gzip compressed data, was "mypy-boto3-mgn-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
```

## Comparing `mypy-boto3-mgn-1.28.12.tar` & `mypy-boto3-mgn-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.928434 mypy-boto3-mgn-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23791 2023-07-27 05:35:02.924434 mypy-boto3-mgn-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22320 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.920434 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51946 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51859 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-27 05:26:37.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    82975 2023-07-27 05:26:39.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    82856 2023-07-27 05:26:38.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.924434 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23791 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:35:02.000000 mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.928434 mypy-boto3-mgn-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:26:35.000000 mypy-boto3-mgn-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22021 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51698 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51611 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-28 20:31:56.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-07-28 20:31:56.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    80885 2023-07-28 20:32:00.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80768 2023-07-28 20:31:57.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:55.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:18.000000 mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.665521 mypy-boto3-mgn-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:31:54.000000 mypy-boto3-mgn-1.28.15/setup.py
```

### Comparing `mypy-boto3-mgn-1.28.12/LICENSE` & `mypy-boto3-mgn-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.12/PKG-INFO` & `mypy-boto3-mgn-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.28.12
-Summary: Type annotations for boto3.mgn 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -411,14 +411,15 @@
 
 `mypy_boto3_mgn.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mgn.type_defs import (
     ApplicationAggregatedStatusTypeDef,
+    ResponseMetadataTypeDef,
     ArchiveApplicationRequestRequestTypeDef,
     ArchiveWaveRequestRequestTypeDef,
     AssociateApplicationsRequestRequestTypeDef,
     AssociateSourceServersRequestRequestTypeDef,
     CPUTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     CreateApplicationRequestRequestTypeDef,
@@ -432,85 +433,68 @@
     DeleteApplicationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
     DeleteVcenterClientRequestRequestTypeDef,
     DeleteWaveRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
-    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
     DescribeVcenterClientsRequestRequestTypeDef,
     VcenterClientTypeDef,
     DisassociateApplicationsRequestRequestTypeDef,
     DisassociateSourceServersRequestRequestTypeDef,
     DisconnectFromServiceRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportErrorDataTypeDef,
     ExportTaskSummaryTypeDef,
     FinalizeCutoverRequestRequestTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
     ImportTaskSummaryApplicationsTypeDef,
     ImportTaskSummaryServersTypeDef,
     ImportTaskSummaryWavesTypeDef,
-    S3BucketSourceOutputTypeDef,
+    S3BucketSourceTypeDef,
     JobLogEventDataTypeDef,
-    LaunchTemplateDiskConfOutputTypeDef,
-    LicensingOutputTypeDef,
     LaunchedInstanceTypeDef,
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
     ListApplicationsRequestFiltersTypeDef,
-    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
-    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
-    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
     ListManagedAccountsRequestRequestTypeDef,
     ManagedAccountTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PaginatorConfigTypeDef,
     PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
-    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ResponseMetadataTypeDef,
     ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
-    S3BucketSourceTypeDef,
-    SsmExternalParameterOutputTypeDef,
-    SsmParameterStoreParameterOutputTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -518,28 +502,39 @@
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     UpdateSourceServerReplicationTypeRequestRequestTypeDef,
     UpdateWaveRequestRequestTypeDef,
     WaveAggregatedStatusTypeDef,
-    ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
+    ApplicationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ChangeServerLifeCycleStateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
+    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
+    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
+    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
     ExportTaskTypeDef,
     ImportTaskErrorTypeDef,
     ImportTaskSummaryTypeDef,
+    StartImportRequestRequestTypeDef,
     JobLogTypeDef,
     LifeCycleLastCutoverTypeDef,
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
@@ -551,51 +546,50 @@
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
     PutSourceServerActionRequestRequestTypeDef,
     PutTemplateActionRequestRequestTypeDef,
-    SsmDocumentTypeDef,
-    ReplicationConfigurationTypeDef,
-    UpdateReplicationConfigurationRequestRequestTypeDef,
-    StartImportRequestRequestTypeDef,
-    SourceServerActionDocumentResponseMetadataTypeDef,
+    SourceServerActionDocumentResponseTypeDef,
     SourceServerActionDocumentTypeDef,
     SsmDocumentOutputTypeDef,
-    TemplateActionDocumentResponseMetadataTypeDef,
+    SsmDocumentTypeDef,
+    TemplateActionDocumentResponseTypeDef,
     TemplateActionDocumentTypeDef,
-    WaveResponseMetadataTypeDef,
+    ReplicationConfigurationTypeDef,
+    UpdateReplicationConfigurationRequestRequestTypeDef,
+    WaveResponseTypeDef,
     WaveTypeDef,
     ListApplicationsResponseTypeDef,
     DataReplicationInfoTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsResponseTypeDef,
     StartExportResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ImportTaskTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     LifeCycleTypeDef,
-    PostLaunchActionsTypeDef,
     ListSourceServerActionsResponseTypeDef,
     JobPostLaunchActionsLaunchStatusTypeDef,
     PostLaunchActionsOutputTypeDef,
+    PostLaunchActionsTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesResponseTypeDef,
     ListImportsResponseTypeDef,
     StartImportResponseTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
-    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
-    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     PostLaunchActionsStatusTypeDef,
-    LaunchConfigurationTemplateResponseMetadataTypeDef,
+    LaunchConfigurationTemplateResponseTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
+    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     DescribeSourceServersResponseTypeDef,
     ParticipatingServerTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     DescribeJobsResponseTypeDef,
     StartCutoverResponseTypeDef,
     StartTestResponseTypeDef,
```

### Comparing `mypy-boto3-mgn-1.28.12/README.md` & `mypy-boto3-mgn-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -379,14 +379,15 @@
 
 `mypy_boto3_mgn.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mgn.type_defs import (
     ApplicationAggregatedStatusTypeDef,
+    ResponseMetadataTypeDef,
     ArchiveApplicationRequestRequestTypeDef,
     ArchiveWaveRequestRequestTypeDef,
     AssociateApplicationsRequestRequestTypeDef,
     AssociateSourceServersRequestRequestTypeDef,
     CPUTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     CreateApplicationRequestRequestTypeDef,
@@ -400,85 +401,68 @@
     DeleteApplicationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
     DeleteVcenterClientRequestRequestTypeDef,
     DeleteWaveRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
-    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
     DescribeVcenterClientsRequestRequestTypeDef,
     VcenterClientTypeDef,
     DisassociateApplicationsRequestRequestTypeDef,
     DisassociateSourceServersRequestRequestTypeDef,
     DisconnectFromServiceRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportErrorDataTypeDef,
     ExportTaskSummaryTypeDef,
     FinalizeCutoverRequestRequestTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
     ImportTaskSummaryApplicationsTypeDef,
     ImportTaskSummaryServersTypeDef,
     ImportTaskSummaryWavesTypeDef,
-    S3BucketSourceOutputTypeDef,
+    S3BucketSourceTypeDef,
     JobLogEventDataTypeDef,
-    LaunchTemplateDiskConfOutputTypeDef,
-    LicensingOutputTypeDef,
     LaunchedInstanceTypeDef,
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
     ListApplicationsRequestFiltersTypeDef,
-    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
-    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
-    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
     ListManagedAccountsRequestRequestTypeDef,
     ManagedAccountTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PaginatorConfigTypeDef,
     PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
-    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ResponseMetadataTypeDef,
     ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
-    S3BucketSourceTypeDef,
-    SsmExternalParameterOutputTypeDef,
-    SsmParameterStoreParameterOutputTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -486,28 +470,39 @@
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     UpdateSourceServerReplicationTypeRequestRequestTypeDef,
     UpdateWaveRequestRequestTypeDef,
     WaveAggregatedStatusTypeDef,
-    ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
+    ApplicationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ChangeServerLifeCycleStateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
+    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
+    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
+    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
     ExportTaskTypeDef,
     ImportTaskErrorTypeDef,
     ImportTaskSummaryTypeDef,
+    StartImportRequestRequestTypeDef,
     JobLogTypeDef,
     LifeCycleLastCutoverTypeDef,
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
@@ -519,51 +514,50 @@
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
     PutSourceServerActionRequestRequestTypeDef,
     PutTemplateActionRequestRequestTypeDef,
-    SsmDocumentTypeDef,
-    ReplicationConfigurationTypeDef,
-    UpdateReplicationConfigurationRequestRequestTypeDef,
-    StartImportRequestRequestTypeDef,
-    SourceServerActionDocumentResponseMetadataTypeDef,
+    SourceServerActionDocumentResponseTypeDef,
     SourceServerActionDocumentTypeDef,
     SsmDocumentOutputTypeDef,
-    TemplateActionDocumentResponseMetadataTypeDef,
+    SsmDocumentTypeDef,
+    TemplateActionDocumentResponseTypeDef,
     TemplateActionDocumentTypeDef,
-    WaveResponseMetadataTypeDef,
+    ReplicationConfigurationTypeDef,
+    UpdateReplicationConfigurationRequestRequestTypeDef,
+    WaveResponseTypeDef,
     WaveTypeDef,
     ListApplicationsResponseTypeDef,
     DataReplicationInfoTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsResponseTypeDef,
     StartExportResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ImportTaskTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     LifeCycleTypeDef,
-    PostLaunchActionsTypeDef,
     ListSourceServerActionsResponseTypeDef,
     JobPostLaunchActionsLaunchStatusTypeDef,
     PostLaunchActionsOutputTypeDef,
+    PostLaunchActionsTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesResponseTypeDef,
     ListImportsResponseTypeDef,
     StartImportResponseTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
-    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
-    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     PostLaunchActionsStatusTypeDef,
-    LaunchConfigurationTemplateResponseMetadataTypeDef,
+    LaunchConfigurationTemplateResponseTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
+    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     DescribeSourceServersResponseTypeDef,
     ParticipatingServerTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     DescribeJobsResponseTypeDef,
     StartCutoverResponseTypeDef,
     StartTestResponseTypeDef,
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.py` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__init__.pyi` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/__main__.py` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mgn 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.mgn 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
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

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.py` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,26 +42,26 @@
     ListImportsPaginator,
     ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 from .type_defs import (
-    ApplicationResponseMetadataTypeDef,
+    ApplicationResponseTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     DescribeJobsRequestFiltersTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DescribeSourceServersResponseTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    LaunchConfigurationTemplateResponseMetadataTypeDef,
+    LaunchConfigurationTemplateResponseTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateDiskConfTypeDef,
     LicensingTypeDef,
     ListApplicationsRequestFiltersTypeDef,
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
@@ -73,30 +73,30 @@
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     S3BucketSourceTypeDef,
-    SourceServerActionDocumentResponseMetadataTypeDef,
+    SourceServerActionDocumentResponseTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     StartCutoverResponseTypeDef,
     StartExportResponseTypeDef,
     StartImportResponseTypeDef,
     StartTestResponseTypeDef,
-    TemplateActionDocumentResponseMetadataTypeDef,
+    TemplateActionDocumentResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     TerminateTargetInstancesResponseTypeDef,
-    WaveResponseMetadataTypeDef,
+    WaveResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -139,23 +139,23 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#exceptions)
         """
 
     def archive_application(
         self, *, applicationID: str, accountID: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Archive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_application)
         """
 
-    def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
+    def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Archive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_wave)
         """
 
@@ -189,15 +189,15 @@
 
     def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         sourceServerID: str,
         accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#change_server_life_cycle_state)
         """
@@ -213,15 +213,15 @@
     def create_application(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_application)
         """
 
@@ -238,15 +238,15 @@
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
-    ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
+    ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_launch_configuration_template)
         """
 
@@ -263,30 +263,30 @@
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
         useFipsEndpoint: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_replication_configuration_template)
         """
 
     def create_wave(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> WaveResponseMetadataTypeDef:
+    ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_wave)
         """
 
@@ -449,25 +449,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disassociate_source_servers)
         """
 
     def disconnect_from_service(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Disconnects specific Source Servers from Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disconnect_from_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disconnect_from_service)
         """
 
     def finalize_cutover(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Finalizes the cutover immediately for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.finalize_cutover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#finalize_cutover)
         """
 
@@ -638,26 +638,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_waves)
         """
 
     def mark_as_archived(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Archives specific Source Servers by setting the SourceServer.isArchived property
         to true for specified SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.mark_as_archived)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#mark_as_archived)
         """
 
     def pause_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Pause Replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.pause_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#pause_replication)
         """
 
@@ -674,15 +674,15 @@
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
         timeoutSeconds: int = ...
-    ) -> SourceServerActionDocumentResponseMetadataTypeDef:
+    ) -> SourceServerActionDocumentResponseTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_source_server_action)
         """
 
@@ -699,15 +699,15 @@
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         operatingSystem: str = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
         timeoutSeconds: int = ...
-    ) -> TemplateActionDocumentResponseMetadataTypeDef:
+    ) -> TemplateActionDocumentResponseTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_template_action)
         """
 
@@ -729,25 +729,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#remove_template_action)
         """
 
     def resume_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Resume Replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.resume_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#resume_replication)
         """
 
     def retry_data_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Causes the data replication initiation sequence to begin immediately upon next
         Handshake for specified SourceServer IDs, regardless of when the previous
         initiation started.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#retry_data_replication)
@@ -781,15 +781,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_import)
         """
 
     def start_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Starts replication for SNAPSHOT_SHIPPING agents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_replication)
         """
 
@@ -801,15 +801,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_test)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_test)
         """
 
     def stop_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Stop Replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#stop_replication)
         """
 
@@ -832,23 +832,23 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.terminate_target_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#terminate_target_instances)
         """
 
     def unarchive_application(
         self, *, applicationID: str, accountID: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Unarchive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_application)
         """
 
-    def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
+    def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Unarchive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_wave)
         """
 
@@ -861,15 +861,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#untag_resource)
         """
 
     def update_application(
         self, *, applicationID: str, accountID: str = ..., description: str = ..., name: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Update application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_application)
         """
 
@@ -909,15 +909,15 @@
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
-    ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
+    ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration_template)
         """
 
@@ -963,36 +963,36 @@
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
         useFipsEndpoint: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration_template)
         """
 
     def update_source_server_replication_type(
         self, *, replicationType: ReplicationTypeType, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Allows you to change between the AGENT_BASED replication type and the
         SNAPSHOT_SHIPPING replication type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server_replication_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_source_server_replication_type)
         """
 
     def update_wave(
         self, *, waveID: str, accountID: str = ..., description: str = ..., name: str = ...
-    ) -> WaveResponseMetadataTypeDef:
+    ) -> WaveResponseTypeDef:
         """
         Update wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_wave)
         """
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/client.pyi` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,26 @@
     ListImportsPaginator,
     ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 from .type_defs import (
-    ApplicationResponseMetadataTypeDef,
+    ApplicationResponseTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     DescribeJobsRequestFiltersTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DescribeSourceServersResponseTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    LaunchConfigurationTemplateResponseMetadataTypeDef,
+    LaunchConfigurationTemplateResponseTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateDiskConfTypeDef,
     LicensingTypeDef,
     ListApplicationsRequestFiltersTypeDef,
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
@@ -73,30 +73,30 @@
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     S3BucketSourceTypeDef,
-    SourceServerActionDocumentResponseMetadataTypeDef,
+    SourceServerActionDocumentResponseTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     StartCutoverResponseTypeDef,
     StartExportResponseTypeDef,
     StartImportResponseTypeDef,
     StartTestResponseTypeDef,
-    TemplateActionDocumentResponseMetadataTypeDef,
+    TemplateActionDocumentResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     TerminateTargetInstancesResponseTypeDef,
-    WaveResponseMetadataTypeDef,
+    WaveResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -134,22 +134,22 @@
         mgnClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#exceptions)
         """
     def archive_application(
         self, *, applicationID: str, accountID: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Archive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_application)
         """
-    def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
+    def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Archive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#archive_wave)
         """
     def associate_applications(
@@ -179,15 +179,15 @@
         """
     def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         sourceServerID: str,
         accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#change_server_life_cycle_state)
         """
@@ -201,15 +201,15 @@
     def create_application(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_application)
         """
     def create_launch_configuration_template(
@@ -225,15 +225,15 @@
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
-    ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
+    ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_launch_configuration_template)
         """
     def create_replication_configuration_template(
@@ -249,29 +249,29 @@
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...,
         useFipsEndpoint: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_replication_configuration_template)
         """
     def create_wave(
         self,
         *,
         name: str,
         accountID: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> WaveResponseMetadataTypeDef:
+    ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#create_wave)
         """
     def delete_application(self, *, applicationID: str, accountID: str = ...) -> Dict[str, Any]:
@@ -418,24 +418,24 @@
         Disassociate source servers from application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_source_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disassociate_source_servers)
         """
     def disconnect_from_service(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Disconnects specific Source Servers from Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disconnect_from_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#disconnect_from_service)
         """
     def finalize_cutover(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Finalizes the cutover immediately for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.finalize_cutover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#finalize_cutover)
         """
     def generate_presigned_url(
@@ -591,25 +591,25 @@
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#list_waves)
         """
     def mark_as_archived(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Archives specific Source Servers by setting the SourceServer.isArchived property
         to true for specified SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.mark_as_archived)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#mark_as_archived)
         """
     def pause_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Pause Replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.pause_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#pause_replication)
         """
     def put_source_server_action(
@@ -625,15 +625,15 @@
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
         timeoutSeconds: int = ...
-    ) -> SourceServerActionDocumentResponseMetadataTypeDef:
+    ) -> SourceServerActionDocumentResponseTypeDef:
         """
         Put source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_source_server_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_source_server_action)
         """
     def put_template_action(
@@ -649,15 +649,15 @@
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         operatingSystem: str = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
         timeoutSeconds: int = ...
-    ) -> TemplateActionDocumentResponseMetadataTypeDef:
+    ) -> TemplateActionDocumentResponseTypeDef:
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#put_template_action)
         """
     def remove_source_server_action(
@@ -676,24 +676,24 @@
         Remove template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_template_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#remove_template_action)
         """
     def resume_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Resume Replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.resume_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#resume_replication)
         """
     def retry_data_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Causes the data replication initiation sequence to begin immediately upon next
         Handshake for specified SourceServer IDs, regardless of when the previous
         initiation started.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.retry_data_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#retry_data_replication)
@@ -723,15 +723,15 @@
         Start import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_import)
         """
     def start_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Starts replication for SNAPSHOT_SHIPPING agents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_replication)
         """
     def start_test(
@@ -741,15 +741,15 @@
         Launches a Test Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_test)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#start_test)
         """
     def stop_replication(
         self, *, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Stop Replication.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.stop_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#stop_replication)
         """
     def tag_resource(
@@ -769,22 +769,22 @@
         Starts a job that terminates specific launched EC2 Test and Cutover instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.terminate_target_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#terminate_target_instances)
         """
     def unarchive_application(
         self, *, applicationID: str, accountID: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Unarchive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_application)
         """
-    def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseMetadataTypeDef:
+    def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Unarchive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#unarchive_wave)
         """
     def untag_resource(
@@ -795,15 +795,15 @@
         Migration Service resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#untag_resource)
         """
     def update_application(
         self, *, applicationID: str, accountID: str = ..., description: str = ..., name: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Update application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_application)
         """
     def update_launch_configuration(
@@ -841,15 +841,15 @@
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
-    ) -> LaunchConfigurationTemplateResponseMetadataTypeDef:
+    ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_launch_configuration_template)
         """
     def update_replication_configuration(
@@ -893,34 +893,34 @@
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...,
         useFipsEndpoint: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_replication_configuration_template)
         """
     def update_source_server_replication_type(
         self, *, replicationType: ReplicationTypeType, sourceServerID: str, accountID: str = ...
-    ) -> SourceServerResponseMetadataTypeDef:
+    ) -> SourceServerResponseTypeDef:
         """
         Allows you to change between the AGENT_BASED replication type and the
         SNAPSHOT_SHIPPING replication type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server_replication_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_source_server_replication_type)
         """
     def update_wave(
         self, *, waveID: str, accountID: str = ..., description: str = ..., name: str = ...
-    ) -> WaveResponseMetadataTypeDef:
+    ) -> WaveResponseTypeDef:
         """
         Update wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_wave)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/client/#update_wave)
         """
     @overload
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.py` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/literals.pyi` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.py` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, accountID: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, accountID: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
         """
 
 
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
 
 
@@ -147,15 +147,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 
@@ -165,15 +165,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 
@@ -184,30 +184,30 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
 
 
 class DescribeVcenterClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeVcenterClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
         """
 
 
@@ -218,30 +218,30 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
 
 
 class ListExportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
     """
 
     def paginate(
-        self, *, exportID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
         """
 
 
@@ -251,30 +251,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
         """
 
 
 class ListImportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
     """
 
     def paginate(
-        self, *, importID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, importID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
         """
 
 
@@ -284,30 +284,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
 
 class ListManagedAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
         """
 
 
@@ -319,15 +319,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 
@@ -338,15 +338,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listtemplateactionspaginator)
         """
 
 
@@ -357,13 +357,13 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/paginator.pyi` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, accountID: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, accountID: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
         """
 
 class DescribeJobsPaginator(Paginator):
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
 
 class DescribeLaunchConfigurationTemplatesPaginator(Paginator):
@@ -142,15 +142,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 class DescribeReplicationConfigurationTemplatesPaginator(Paginator):
@@ -159,15 +159,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 class DescribeSourceServersPaginator(Paginator):
@@ -177,29 +177,29 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
 
 class DescribeVcenterClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeVcenterClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
@@ -209,29 +209,29 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
 
 class ListExportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
     """
 
     def paginate(
-        self, *, exportID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
         """
 
 class ListExportsPaginator(Paginator):
@@ -240,29 +240,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
         """
 
 class ListImportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
     """
 
     def paginate(
-        self, *, importID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, importID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
         """
 
 class ListImportsPaginator(Paginator):
@@ -271,29 +271,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
 class ListManagedAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listmanagedaccountspaginator)
         """
 
 class ListSourceServerActionsPaginator(Paginator):
@@ -304,15 +304,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 class ListTemplateActionsPaginator(Paginator):
@@ -322,15 +322,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listtemplateactionspaginator)
         """
 
 class ListWavesPaginator(Paginator):
@@ -340,13 +340,13 @@
     """
 
     def paginate(
         self,
         *,
         accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.py` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApplicationAggregatedStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "ArchiveApplicationRequestRequestTypeDef",
     "ArchiveWaveRequestRequestTypeDef",
     "AssociateApplicationsRequestRequestTypeDef",
     "AssociateSourceServersRequestRequestTypeDef",
     "CPUTypeDef",
     "ChangeServerLifeCycleStateSourceServerLifecycleTypeDef",
     "CreateApplicationRequestRequestTypeDef",
@@ -78,85 +79,68 @@
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
     "DeleteVcenterClientRequestRequestTypeDef",
     "DeleteWaveRequestRequestTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
     "DescribeVcenterClientsRequestRequestTypeDef",
     "VcenterClientTypeDef",
     "DisassociateApplicationsRequestRequestTypeDef",
     "DisassociateSourceServersRequestRequestTypeDef",
     "DisconnectFromServiceRequestRequestTypeDef",
     "DiskTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportErrorDataTypeDef",
     "ExportTaskSummaryTypeDef",
     "FinalizeCutoverRequestRequestTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ImportErrorDataTypeDef",
     "ImportTaskSummaryApplicationsTypeDef",
     "ImportTaskSummaryServersTypeDef",
     "ImportTaskSummaryWavesTypeDef",
-    "S3BucketSourceOutputTypeDef",
+    "S3BucketSourceTypeDef",
     "JobLogEventDataTypeDef",
-    "LaunchTemplateDiskConfOutputTypeDef",
-    "LicensingOutputTypeDef",
     "LaunchedInstanceTypeDef",
     "LifeCycleLastCutoverFinalizedTypeDef",
     "LifeCycleLastCutoverInitiatedTypeDef",
     "LifeCycleLastCutoverRevertedTypeDef",
     "LifeCycleLastTestFinalizedTypeDef",
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
     "ListApplicationsRequestFiltersTypeDef",
-    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
-    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
-    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
     "ListManagedAccountsRequestRequestTypeDef",
     "ManagedAccountTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
-    "PaginatorConfigTypeDef",
     "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
-    "S3BucketSourceTypeDef",
-    "SsmExternalParameterOutputTypeDef",
-    "SsmParameterStoreParameterOutputTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
@@ -164,28 +148,39 @@
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
     "UpdateWaveRequestRequestTypeDef",
     "WaveAggregatedStatusTypeDef",
-    "ApplicationResponseMetadataTypeDef",
     "ApplicationTypeDef",
+    "ApplicationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ReplicationConfigurationTemplateResponseTypeDef",
     "ChangeServerLifeCycleStateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
+    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
     "ExportTaskTypeDef",
     "ImportTaskErrorTypeDef",
     "ImportTaskSummaryTypeDef",
+    "StartImportRequestRequestTypeDef",
     "JobLogTypeDef",
     "LifeCycleLastCutoverTypeDef",
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
@@ -197,51 +192,50 @@
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
     "PutSourceServerActionRequestRequestTypeDef",
     "PutTemplateActionRequestRequestTypeDef",
-    "SsmDocumentTypeDef",
-    "ReplicationConfigurationTypeDef",
-    "UpdateReplicationConfigurationRequestRequestTypeDef",
-    "StartImportRequestRequestTypeDef",
-    "SourceServerActionDocumentResponseMetadataTypeDef",
+    "SourceServerActionDocumentResponseTypeDef",
     "SourceServerActionDocumentTypeDef",
     "SsmDocumentOutputTypeDef",
-    "TemplateActionDocumentResponseMetadataTypeDef",
+    "SsmDocumentTypeDef",
+    "TemplateActionDocumentResponseTypeDef",
     "TemplateActionDocumentTypeDef",
-    "WaveResponseMetadataTypeDef",
+    "ReplicationConfigurationTypeDef",
+    "UpdateReplicationConfigurationRequestRequestTypeDef",
+    "WaveResponseTypeDef",
     "WaveTypeDef",
     "ListApplicationsResponseTypeDef",
     "DataReplicationInfoTypeDef",
     "ListExportErrorsResponseTypeDef",
     "ListExportsResponseTypeDef",
     "StartExportResponseTypeDef",
     "ListImportErrorsResponseTypeDef",
     "ImportTaskTypeDef",
     "DescribeJobLogItemsResponseTypeDef",
     "LifeCycleTypeDef",
-    "PostLaunchActionsTypeDef",
     "ListSourceServerActionsResponseTypeDef",
     "JobPostLaunchActionsLaunchStatusTypeDef",
     "PostLaunchActionsOutputTypeDef",
+    "PostLaunchActionsTypeDef",
     "ListTemplateActionsResponseTypeDef",
     "ListWavesResponseTypeDef",
     "ListImportsResponseTypeDef",
     "StartImportResponseTypeDef",
-    "SourceServerResponseMetadataTypeDef",
+    "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    "UpdateLaunchConfigurationRequestRequestTypeDef",
-    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "PostLaunchActionsStatusTypeDef",
-    "LaunchConfigurationTemplateResponseMetadataTypeDef",
+    "LaunchConfigurationTemplateResponseTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "ParticipatingServerTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartCutoverResponseTypeDef",
     "StartTestResponseTypeDef",
@@ -255,14 +249,25 @@
         "lastUpdateDateTime": str,
         "progressStatus": ApplicationProgressStatusType,
         "totalSourceServers": int,
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
 _RequiredArchiveApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
 _OptionalArchiveApplicationRequestRequestTypeDef = TypedDict(
@@ -594,37 +599,24 @@
 
 class DeleteWaveRequestRequestTypeDef(
     _RequiredDeleteWaveRequestRequestTypeDef, _OptionalDeleteWaveRequestRequestTypeDef
 ):
     pass
 
 
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
-        "accountID": str,
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
@@ -651,42 +643,24 @@
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
     total=False,
 )
 
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
@@ -737,22 +711,14 @@
         "lifeCycleStates": Sequence[LifeCycleStateType],
         "replicationTypes": Sequence[ReplicationTypeType],
         "sourceServerIDs": Sequence[str],
     },
     total=False,
 )
 
-DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeVcenterClientsRequestRequestTypeDef = TypedDict(
     "DescribeVcenterClientsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -846,21 +812,14 @@
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
 ExportErrorDataTypeDef = TypedDict(
     "ExportErrorDataTypeDef",
     {
         "rawError": str,
     },
     total=False,
 )
@@ -989,65 +948,45 @@
     {
         "createdCount": int,
         "modifiedCount": int,
     },
     total=False,
 )
 
-_RequiredS3BucketSourceOutputTypeDef = TypedDict(
-    "_RequiredS3BucketSourceOutputTypeDef",
+_RequiredS3BucketSourceTypeDef = TypedDict(
+    "_RequiredS3BucketSourceTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
-_OptionalS3BucketSourceOutputTypeDef = TypedDict(
-    "_OptionalS3BucketSourceOutputTypeDef",
+_OptionalS3BucketSourceTypeDef = TypedDict(
+    "_OptionalS3BucketSourceTypeDef",
     {
         "s3BucketOwner": str,
     },
     total=False,
 )
 
 
-class S3BucketSourceOutputTypeDef(
-    _RequiredS3BucketSourceOutputTypeDef, _OptionalS3BucketSourceOutputTypeDef
-):
+class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
 
 JobLogEventDataTypeDef = TypedDict(
     "JobLogEventDataTypeDef",
     {
         "conversionServerID": str,
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
-LaunchTemplateDiskConfOutputTypeDef = TypedDict(
-    "LaunchTemplateDiskConfOutputTypeDef",
-    {
-        "iops": int,
-        "throughput": int,
-        "volumeType": VolumeTypeType,
-    },
-    total=False,
-)
-
-LicensingOutputTypeDef = TypedDict(
-    "LicensingOutputTypeDef",
-    {
-        "osByol": bool,
-    },
-    total=False,
-)
-
 LaunchedInstanceTypeDef = TypedDict(
     "LaunchedInstanceTypeDef",
     {
         "ec2InstanceID": str,
         "firstBoot": FirstBootType,
         "jobID": str,
     },
@@ -1110,36 +1049,14 @@
         "applicationIDs": Sequence[str],
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
-_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "exportID": str,
-    },
-)
-_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
-    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
-    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListExportErrorsRequestRequestTypeDef",
     {
         "exportID": str,
     },
 )
 _OptionalListExportErrorsRequestRequestTypeDef = TypedDict(
@@ -1162,36 +1079,14 @@
     "ListExportsRequestFiltersTypeDef",
     {
         "exportIDs": Sequence[str],
     },
     total=False,
 )
 
-_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "importID": str,
-    },
-)
-_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
-    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
-    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListImportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListImportErrorsRequestRequestTypeDef",
     {
         "importID": str,
     },
 )
 _OptionalListImportErrorsRequestRequestTypeDef = TypedDict(
@@ -1214,22 +1109,14 @@
     "ListImportsRequestFiltersTypeDef",
     {
         "importIDs": Sequence[str],
     },
     total=False,
 )
 
-ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
-    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedAccountsRequestRequestTypeDef = TypedDict(
     "ListManagedAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1254,22 +1141,14 @@
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
 TemplateActionsRequestFiltersTypeDef = TypedDict(
     "TemplateActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -1318,24 +1197,14 @@
     "OSTypeDef",
     {
         "fullString": str,
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
 _RequiredPauseReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPauseReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalPauseReplicationRequestRequestTypeDef = TypedDict(
@@ -1396,72 +1265,26 @@
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
 )
 
-ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
-    {
-        "deviceName": str,
-        "iops": int,
-        "isBootDisk": bool,
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
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
     },
     total=False,
 )
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
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
 _RequiredResumeReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredResumeReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalResumeReplicationRequestRequestTypeDef = TypedDict(
@@ -1497,50 +1320,14 @@
 class RetryDataReplicationRequestRequestTypeDef(
     _RequiredRetryDataReplicationRequestRequestTypeDef,
     _OptionalRetryDataReplicationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredS3BucketSourceTypeDef = TypedDict(
-    "_RequiredS3BucketSourceTypeDef",
-    {
-        "s3Bucket": str,
-        "s3Key": str,
-    },
-)
-_OptionalS3BucketSourceTypeDef = TypedDict(
-    "_OptionalS3BucketSourceTypeDef",
-    {
-        "s3BucketOwner": str,
-    },
-    total=False,
-)
-
-
-class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
-    pass
-
-
-SsmExternalParameterOutputTypeDef = TypedDict(
-    "SsmExternalParameterOutputTypeDef",
-    {
-        "dynamicPath": str,
-    },
-    total=False,
-)
-
-SsmParameterStoreParameterOutputTypeDef = TypedDict(
-    "SsmParameterStoreParameterOutputTypeDef",
-    {
-        "parameterName": str,
-        "parameterType": Literal["STRING"],
-    },
-)
-
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
@@ -1839,46 +1626,84 @@
         "progressStatus": WaveProgressStatusType,
         "replicationStartedDateTime": str,
         "totalApplications": int,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+ApplicationResponseTypeDef = TypedDict(
+    "ApplicationResponseTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
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
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicationConfigurationTemplateResponseTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
     "_RequiredChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
@@ -1906,20 +1731,121 @@
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
+        "accountID": str,
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
+DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "exportID": str,
+    },
+)
+_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
+    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
+    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "importID": str,
+    },
+)
+_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
+    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
+    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
+):
+    pass
+
+
+ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1932,24 +1858,24 @@
 )
 
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1962,15 +1888,15 @@
 )
 
 DescribeVcenterClientsResponseTypeDef = TypedDict(
     "DescribeVcenterClientsResponseTypeDef",
     {
         "items": List[VcenterClientTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportTaskErrorTypeDef = TypedDict(
     "ExportTaskErrorTypeDef",
     {
         "errorData": ExportErrorDataTypeDef,
@@ -2011,14 +1937,35 @@
         "applications": ImportTaskSummaryApplicationsTypeDef,
         "servers": ImportTaskSummaryServersTypeDef,
         "waves": ImportTaskSummaryWavesTypeDef,
     },
     total=False,
 )
 
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "s3BucketSource": S3BucketSourceTypeDef,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
+
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
@@ -2046,15 +1993,15 @@
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
@@ -2066,15 +2013,15 @@
     total=False,
 )
 
 ListExportsRequestListExportsPaginateTypeDef = TypedDict(
     "ListExportsRequestListExportsPaginateTypeDef",
     {
         "filters": ListExportsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListExportsRequestRequestTypeDef = TypedDict(
     "ListExportsRequestRequestTypeDef",
     {
@@ -2085,15 +2032,15 @@
     total=False,
 )
 
 ListImportsRequestListImportsPaginateTypeDef = TypedDict(
     "ListImportsRequestListImportsPaginateTypeDef",
     {
         "filters": ListImportsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
@@ -2105,30 +2052,30 @@
 )
 
 ListManagedAccountsResponseTypeDef = TypedDict(
     "ListManagedAccountsResponseTypeDef",
     {
         "items": List[ManagedAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef(
     _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
@@ -2168,15 +2115,15 @@
         "launchConfigurationTemplateID": str,
     },
 )
 _OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef = TypedDict(
     "_OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     {
         "filters": TemplateActionsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListTemplateActionsRequestListTemplateActionsPaginateTypeDef(
     _RequiredListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
@@ -2210,15 +2157,15 @@
 
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
         "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
@@ -2308,151 +2255,47 @@
 
 class PutTemplateActionRequestRequestTypeDef(
     _RequiredPutTemplateActionRequestRequestTypeDef, _OptionalPutTemplateActionRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredSsmDocumentTypeDef = TypedDict(
-    "_RequiredSsmDocumentTypeDef",
-    {
-        "actionName": str,
-        "ssmDocumentName": str,
-    },
-)
-_OptionalSsmDocumentTypeDef = TypedDict(
-    "_OptionalSsmDocumentTypeDef",
-    {
-        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
-        "mustSucceedForCutover": bool,
-        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
-        "timeoutSeconds": int,
-    },
-    total=False,
-)
-
-
-class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
-    pass
-
-
-ReplicationConfigurationTypeDef = TypedDict(
-    "ReplicationConfigurationTypeDef",
-    {
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "sourceServerID": str,
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "sourceServerID": str,
-    },
-)
-_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "accountID": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": Sequence[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Mapping[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-    },
-    total=False,
-)
-
-
-class UpdateReplicationConfigurationRequestRequestTypeDef(
-    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
-    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
-    {
-        "s3BucketSource": S3BucketSourceTypeDef,
-    },
-)
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
-    pass
-
-
-SourceServerActionDocumentResponseMetadataTypeDef = TypedDict(
-    "SourceServerActionDocumentResponseMetadataTypeDef",
+SourceServerActionDocumentResponseTypeDef = TypedDict(
+    "SourceServerActionDocumentResponseTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerActionDocumentTypeDef = TypedDict(
     "SourceServerActionDocumentTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
 _RequiredSsmDocumentOutputTypeDef = TypedDict(
     "_RequiredSsmDocumentOutputTypeDef",
@@ -2460,82 +2303,165 @@
         "actionName": str,
         "ssmDocumentName": str,
     },
 )
 _OptionalSsmDocumentOutputTypeDef = TypedDict(
     "_OptionalSsmDocumentOutputTypeDef",
     {
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
 
 class SsmDocumentOutputTypeDef(
     _RequiredSsmDocumentOutputTypeDef, _OptionalSsmDocumentOutputTypeDef
 ):
     pass
 
 
-TemplateActionDocumentResponseMetadataTypeDef = TypedDict(
-    "TemplateActionDocumentResponseMetadataTypeDef",
+_RequiredSsmDocumentTypeDef = TypedDict(
+    "_RequiredSsmDocumentTypeDef",
+    {
+        "actionName": str,
+        "ssmDocumentName": str,
+    },
+)
+_OptionalSsmDocumentTypeDef = TypedDict(
+    "_OptionalSsmDocumentTypeDef",
+    {
+        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
+        "mustSucceedForCutover": bool,
+        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
+        "timeoutSeconds": int,
+    },
+    total=False,
+)
+
+
+class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
+    pass
+
+
+TemplateActionDocumentResponseTypeDef = TypedDict(
+    "TemplateActionDocumentResponseTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TemplateActionDocumentTypeDef = TypedDict(
     "TemplateActionDocumentTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-WaveResponseMetadataTypeDef = TypedDict(
-    "WaveResponseMetadataTypeDef",
+ReplicationConfigurationTypeDef = TypedDict(
+    "ReplicationConfigurationTypeDef",
+    {
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "sourceServerID": str,
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": Sequence[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Mapping[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+    },
+    total=False,
+)
+
+
+class UpdateReplicationConfigurationRequestRequestTypeDef(
+    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
+    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+WaveResponseTypeDef = TypedDict(
+    "WaveResponseTypeDef",
     {
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveAggregatedStatus": WaveAggregatedStatusTypeDef,
         "waveID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WaveTypeDef = TypedDict(
     "WaveTypeDef",
     {
         "arn": str,
@@ -2552,15 +2478,15 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "items": List[ApplicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -2575,64 +2501,64 @@
 )
 
 ListExportErrorsResponseTypeDef = TypedDict(
     "ListExportErrorsResponseTypeDef",
     {
         "items": List[ExportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
         "items": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExportResponseTypeDef = TypedDict(
     "StartExportResponseTypeDef",
     {
         "exportTask": ExportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportErrorsResponseTypeDef = TypedDict(
     "ListImportErrorsResponseTypeDef",
     {
         "items": List[ImportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTaskTypeDef = TypedDict(
     "ImportTaskTypeDef",
     {
         "creationDateTime": str,
         "endDateTime": str,
         "importID": str,
         "progressPercentage": float,
-        "s3BucketSource": S3BucketSourceOutputTypeDef,
+        "s3BucketSource": S3BucketSourceTypeDef,
         "status": ImportStatusType,
         "summary": ImportTaskSummaryTypeDef,
     },
     total=False,
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
 
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
@@ -2642,32 +2568,20 @@
         "lastSeenByServiceDateTime": str,
         "lastTest": LifeCycleLastTestTypeDef,
         "state": LifeCycleStateType,
     },
     total=False,
 )
 
-PostLaunchActionsTypeDef = TypedDict(
-    "PostLaunchActionsTypeDef",
-    {
-        "cloudWatchLogGroupName": str,
-        "deployment": PostLaunchActionsDeploymentTypeType,
-        "s3LogBucket": str,
-        "s3OutputKeyPrefix": str,
-        "ssmDocuments": Sequence[SsmDocumentTypeDef],
-    },
-    total=False,
-)
-
 ListSourceServerActionsResponseTypeDef = TypedDict(
     "ListSourceServerActionsResponseTypeDef",
     {
         "items": List[SourceServerActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
@@ -2687,66 +2601,78 @@
         "s3LogBucket": str,
         "s3OutputKeyPrefix": str,
         "ssmDocuments": List[SsmDocumentOutputTypeDef],
     },
     total=False,
 )
 
+PostLaunchActionsTypeDef = TypedDict(
+    "PostLaunchActionsTypeDef",
+    {
+        "cloudWatchLogGroupName": str,
+        "deployment": PostLaunchActionsDeploymentTypeType,
+        "s3LogBucket": str,
+        "s3OutputKeyPrefix": str,
+        "ssmDocuments": Sequence[SsmDocumentTypeDef],
+    },
+    total=False,
+)
+
 ListTemplateActionsResponseTypeDef = TypedDict(
     "ListTemplateActionsResponseTypeDef",
     {
         "items": List[TemplateActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWavesResponseTypeDef = TypedDict(
     "ListWavesResponseTypeDef",
     {
         "items": List[WaveTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "items": List[ImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "importTask": ImportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceServerResponseMetadataTypeDef = TypedDict(
-    "SourceServerResponseMetadataTypeDef",
+SourceServerResponseTypeDef = TypedDict(
+    "SourceServerResponseTypeDef",
     {
         "applicationID": str,
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "fqdnForActionFramework": str,
         "isArchived": bool,
         "launchedInstance": LaunchedInstanceTypeDef,
         "lifeCycle": LifeCycleTypeDef,
         "replicationType": ReplicationTypeType,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "applicationID": str,
@@ -2762,195 +2688,195 @@
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
     },
     total=False,
 )
 
-CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+PostLaunchActionsStatusTypeDef = TypedDict(
+    "PostLaunchActionsStatusTypeDef",
+    {
+        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
+        "ssmAgentDiscoveryDatetime": str,
+    },
+    total=False,
+)
+
+LaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "LaunchConfigurationTemplateResponseTypeDef",
     {
+        "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
+_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTemplateTypeDef",
     {
-        "sourceServerID": str,
+        "launchConfigurationTemplateID": str,
     },
 )
-_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
+_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTemplateTypeDef",
     {
-        "accountID": str,
+        "arn": str,
+        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
 
-class UpdateLaunchConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+class LaunchConfigurationTemplateTypeDef(
+    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
 ):
     pass
 
 
-_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
     {
-        "launchConfigurationTemplateID": str,
+        "bootMode": BootModeType,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "enableMapAutoTagging": bool,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "mapAutoTaggingMpeID": str,
+        "name": str,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+
+CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
+        "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-
-class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-):
-    pass
-
-
-PostLaunchActionsStatusTypeDef = TypedDict(
-    "PostLaunchActionsStatusTypeDef",
+_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
-        "ssmAgentDiscoveryDatetime": str,
+        "sourceServerID": str,
     },
-    total=False,
 )
-
-LaunchConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "LaunchConfigurationTemplateResponseMetadataTypeDef",
+_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
-        "associatePublicIpAddress": bool,
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
-        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
+        "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
-        "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
+        "name": str,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTemplateTypeDef",
+
+class UpdateLaunchConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
-_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTemplateTypeDef",
+_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
-        "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
+        "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
 
-class LaunchConfigurationTemplateTypeDef(
-    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
+class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
-    {
-        "bootMode": BootModeType,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "enableMapAutoTagging": bool,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
-        "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredParticipatingServerTypeDef = TypedDict(
     "_RequiredParticipatingServerTypeDef",
     {
         "sourceServerID": str,
@@ -2974,15 +2900,15 @@
 
 
 DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     {
         "items": List[LaunchConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
@@ -3009,34 +2935,34 @@
 
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartCutoverResponseTypeDef = TypedDict(
     "StartCutoverResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTestResponseTypeDef = TypedDict(
     "StartTestResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateTargetInstancesResponseTypeDef = TypedDict(
     "TerminateTargetInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn/type_defs.pyi` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationAggregatedStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "ArchiveApplicationRequestRequestTypeDef",
     "ArchiveWaveRequestRequestTypeDef",
     "AssociateApplicationsRequestRequestTypeDef",
     "AssociateSourceServersRequestRequestTypeDef",
     "CPUTypeDef",
     "ChangeServerLifeCycleStateSourceServerLifecycleTypeDef",
     "CreateApplicationRequestRequestTypeDef",
@@ -77,85 +78,68 @@
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
     "DeleteVcenterClientRequestRequestTypeDef",
     "DeleteWaveRequestRequestTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
     "DescribeVcenterClientsRequestRequestTypeDef",
     "VcenterClientTypeDef",
     "DisassociateApplicationsRequestRequestTypeDef",
     "DisassociateSourceServersRequestRequestTypeDef",
     "DisconnectFromServiceRequestRequestTypeDef",
     "DiskTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportErrorDataTypeDef",
     "ExportTaskSummaryTypeDef",
     "FinalizeCutoverRequestRequestTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ImportErrorDataTypeDef",
     "ImportTaskSummaryApplicationsTypeDef",
     "ImportTaskSummaryServersTypeDef",
     "ImportTaskSummaryWavesTypeDef",
-    "S3BucketSourceOutputTypeDef",
+    "S3BucketSourceTypeDef",
     "JobLogEventDataTypeDef",
-    "LaunchTemplateDiskConfOutputTypeDef",
-    "LicensingOutputTypeDef",
     "LaunchedInstanceTypeDef",
     "LifeCycleLastCutoverFinalizedTypeDef",
     "LifeCycleLastCutoverInitiatedTypeDef",
     "LifeCycleLastCutoverRevertedTypeDef",
     "LifeCycleLastTestFinalizedTypeDef",
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
     "ListApplicationsRequestFiltersTypeDef",
-    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
-    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
-    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
     "ListManagedAccountsRequestRequestTypeDef",
     "ManagedAccountTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
-    "PaginatorConfigTypeDef",
     "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
-    "S3BucketSourceTypeDef",
-    "SsmExternalParameterOutputTypeDef",
-    "SsmParameterStoreParameterOutputTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
@@ -163,28 +147,39 @@
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
     "UpdateWaveRequestRequestTypeDef",
     "WaveAggregatedStatusTypeDef",
-    "ApplicationResponseMetadataTypeDef",
     "ApplicationTypeDef",
+    "ApplicationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ReplicationConfigurationTemplateResponseTypeDef",
     "ChangeServerLifeCycleStateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
+    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
     "ExportTaskTypeDef",
     "ImportTaskErrorTypeDef",
     "ImportTaskSummaryTypeDef",
+    "StartImportRequestRequestTypeDef",
     "JobLogTypeDef",
     "LifeCycleLastCutoverTypeDef",
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
@@ -196,51 +191,50 @@
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
     "PutSourceServerActionRequestRequestTypeDef",
     "PutTemplateActionRequestRequestTypeDef",
-    "SsmDocumentTypeDef",
-    "ReplicationConfigurationTypeDef",
-    "UpdateReplicationConfigurationRequestRequestTypeDef",
-    "StartImportRequestRequestTypeDef",
-    "SourceServerActionDocumentResponseMetadataTypeDef",
+    "SourceServerActionDocumentResponseTypeDef",
     "SourceServerActionDocumentTypeDef",
     "SsmDocumentOutputTypeDef",
-    "TemplateActionDocumentResponseMetadataTypeDef",
+    "SsmDocumentTypeDef",
+    "TemplateActionDocumentResponseTypeDef",
     "TemplateActionDocumentTypeDef",
-    "WaveResponseMetadataTypeDef",
+    "ReplicationConfigurationTypeDef",
+    "UpdateReplicationConfigurationRequestRequestTypeDef",
+    "WaveResponseTypeDef",
     "WaveTypeDef",
     "ListApplicationsResponseTypeDef",
     "DataReplicationInfoTypeDef",
     "ListExportErrorsResponseTypeDef",
     "ListExportsResponseTypeDef",
     "StartExportResponseTypeDef",
     "ListImportErrorsResponseTypeDef",
     "ImportTaskTypeDef",
     "DescribeJobLogItemsResponseTypeDef",
     "LifeCycleTypeDef",
-    "PostLaunchActionsTypeDef",
     "ListSourceServerActionsResponseTypeDef",
     "JobPostLaunchActionsLaunchStatusTypeDef",
     "PostLaunchActionsOutputTypeDef",
+    "PostLaunchActionsTypeDef",
     "ListTemplateActionsResponseTypeDef",
     "ListWavesResponseTypeDef",
     "ListImportsResponseTypeDef",
     "StartImportResponseTypeDef",
-    "SourceServerResponseMetadataTypeDef",
+    "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    "UpdateLaunchConfigurationRequestRequestTypeDef",
-    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "PostLaunchActionsStatusTypeDef",
-    "LaunchConfigurationTemplateResponseMetadataTypeDef",
+    "LaunchConfigurationTemplateResponseTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    "UpdateLaunchConfigurationRequestRequestTypeDef",
+    "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "ParticipatingServerTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartCutoverResponseTypeDef",
     "StartTestResponseTypeDef",
@@ -254,14 +248,25 @@
         "lastUpdateDateTime": str,
         "progressStatus": ApplicationProgressStatusType,
         "totalSourceServers": int,
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
 _RequiredArchiveApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
 _OptionalArchiveApplicationRequestRequestTypeDef = TypedDict(
@@ -571,35 +576,24 @@
 )
 
 class DeleteWaveRequestRequestTypeDef(
     _RequiredDeleteWaveRequestRequestTypeDef, _OptionalDeleteWaveRequestRequestTypeDef
 ):
     pass
 
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
-        "accountID": str,
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
@@ -624,42 +618,24 @@
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
     total=False,
 )
 
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
@@ -708,22 +684,14 @@
         "lifeCycleStates": Sequence[LifeCycleStateType],
         "replicationTypes": Sequence[ReplicationTypeType],
         "sourceServerIDs": Sequence[str],
     },
     total=False,
 )
 
-DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeVcenterClientsRequestRequestTypeDef = TypedDict(
     "DescribeVcenterClientsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -811,21 +779,14 @@
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
 ExportErrorDataTypeDef = TypedDict(
     "ExportErrorDataTypeDef",
     {
         "rawError": str,
     },
     total=False,
 )
@@ -948,63 +909,43 @@
     {
         "createdCount": int,
         "modifiedCount": int,
     },
     total=False,
 )
 
-_RequiredS3BucketSourceOutputTypeDef = TypedDict(
-    "_RequiredS3BucketSourceOutputTypeDef",
+_RequiredS3BucketSourceTypeDef = TypedDict(
+    "_RequiredS3BucketSourceTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
-_OptionalS3BucketSourceOutputTypeDef = TypedDict(
-    "_OptionalS3BucketSourceOutputTypeDef",
+_OptionalS3BucketSourceTypeDef = TypedDict(
+    "_OptionalS3BucketSourceTypeDef",
     {
         "s3BucketOwner": str,
     },
     total=False,
 )
 
-class S3BucketSourceOutputTypeDef(
-    _RequiredS3BucketSourceOutputTypeDef, _OptionalS3BucketSourceOutputTypeDef
-):
+class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
 JobLogEventDataTypeDef = TypedDict(
     "JobLogEventDataTypeDef",
     {
         "conversionServerID": str,
         "rawError": str,
         "sourceServerID": str,
         "targetInstanceID": str,
     },
     total=False,
 )
 
-LaunchTemplateDiskConfOutputTypeDef = TypedDict(
-    "LaunchTemplateDiskConfOutputTypeDef",
-    {
-        "iops": int,
-        "throughput": int,
-        "volumeType": VolumeTypeType,
-    },
-    total=False,
-)
-
-LicensingOutputTypeDef = TypedDict(
-    "LicensingOutputTypeDef",
-    {
-        "osByol": bool,
-    },
-    total=False,
-)
-
 LaunchedInstanceTypeDef = TypedDict(
     "LaunchedInstanceTypeDef",
     {
         "ec2InstanceID": str,
         "firstBoot": FirstBootType,
         "jobID": str,
     },
@@ -1067,34 +1008,14 @@
         "applicationIDs": Sequence[str],
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
-_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "exportID": str,
-    },
-)
-_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
-    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
-    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListExportErrorsRequestRequestTypeDef",
     {
         "exportID": str,
     },
 )
 _OptionalListExportErrorsRequestRequestTypeDef = TypedDict(
@@ -1115,34 +1036,14 @@
     "ListExportsRequestFiltersTypeDef",
     {
         "exportIDs": Sequence[str],
     },
     total=False,
 )
 
-_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "importID": str,
-    },
-)
-_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
-    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
-    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
-):
-    pass
-
 _RequiredListImportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListImportErrorsRequestRequestTypeDef",
     {
         "importID": str,
     },
 )
 _OptionalListImportErrorsRequestRequestTypeDef = TypedDict(
@@ -1163,22 +1064,14 @@
     "ListImportsRequestFiltersTypeDef",
     {
         "importIDs": Sequence[str],
     },
     total=False,
 )
 
-ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
-    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedAccountsRequestRequestTypeDef = TypedDict(
     "ListManagedAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1203,22 +1096,14 @@
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
 TemplateActionsRequestFiltersTypeDef = TypedDict(
     "TemplateActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -1265,24 +1150,14 @@
     "OSTypeDef",
     {
         "fullString": str,
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
 _RequiredPauseReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPauseReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalPauseReplicationRequestRequestTypeDef = TypedDict(
@@ -1339,72 +1214,26 @@
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
 )
 
-ReplicationConfigurationReplicatedDiskOutputTypeDef = TypedDict(
-    "ReplicationConfigurationReplicatedDiskOutputTypeDef",
-    {
-        "deviceName": str,
-        "iops": int,
-        "isBootDisk": bool,
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
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
     },
     total=False,
 )
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
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
 _RequiredResumeReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredResumeReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalResumeReplicationRequestRequestTypeDef = TypedDict(
@@ -1436,48 +1265,14 @@
 
 class RetryDataReplicationRequestRequestTypeDef(
     _RequiredRetryDataReplicationRequestRequestTypeDef,
     _OptionalRetryDataReplicationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredS3BucketSourceTypeDef = TypedDict(
-    "_RequiredS3BucketSourceTypeDef",
-    {
-        "s3Bucket": str,
-        "s3Key": str,
-    },
-)
-_OptionalS3BucketSourceTypeDef = TypedDict(
-    "_OptionalS3BucketSourceTypeDef",
-    {
-        "s3BucketOwner": str,
-    },
-    total=False,
-)
-
-class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
-    pass
-
-SsmExternalParameterOutputTypeDef = TypedDict(
-    "SsmExternalParameterOutputTypeDef",
-    {
-        "dynamicPath": str,
-    },
-    total=False,
-)
-
-SsmParameterStoreParameterOutputTypeDef = TypedDict(
-    "SsmParameterStoreParameterOutputTypeDef",
-    {
-        "parameterName": str,
-        "parameterType": Literal["STRING"],
-    },
-)
-
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
@@ -1752,46 +1547,84 @@
         "progressStatus": WaveProgressStatusType,
         "replicationStartedDateTime": str,
         "totalApplications": int,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+ApplicationResponseTypeDef = TypedDict(
+    "ApplicationResponseTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
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
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicationConfigurationTemplateResponseTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
     "_RequiredChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
@@ -1817,20 +1650,115 @@
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
+        "accountID": str,
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
+DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "exportID": str,
+    },
+)
+_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
+    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
+    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
+):
+    pass
+
+_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "importID": str,
+    },
+)
+_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
+    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
+    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
+):
+    pass
+
+ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1843,24 +1771,24 @@
 )
 
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1873,15 +1801,15 @@
 )
 
 DescribeVcenterClientsResponseTypeDef = TypedDict(
     "DescribeVcenterClientsResponseTypeDef",
     {
         "items": List[VcenterClientTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportTaskErrorTypeDef = TypedDict(
     "ExportTaskErrorTypeDef",
     {
         "errorData": ExportErrorDataTypeDef,
@@ -1922,14 +1850,33 @@
         "applications": ImportTaskSummaryApplicationsTypeDef,
         "servers": ImportTaskSummaryServersTypeDef,
         "waves": ImportTaskSummaryWavesTypeDef,
     },
     total=False,
 )
 
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "s3BucketSource": S3BucketSourceTypeDef,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
@@ -1957,15 +1904,15 @@
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
@@ -1977,15 +1924,15 @@
     total=False,
 )
 
 ListExportsRequestListExportsPaginateTypeDef = TypedDict(
     "ListExportsRequestListExportsPaginateTypeDef",
     {
         "filters": ListExportsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListExportsRequestRequestTypeDef = TypedDict(
     "ListExportsRequestRequestTypeDef",
     {
@@ -1996,15 +1943,15 @@
     total=False,
 )
 
 ListImportsRequestListImportsPaginateTypeDef = TypedDict(
     "ListImportsRequestListImportsPaginateTypeDef",
     {
         "filters": ListImportsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
@@ -2016,30 +1963,30 @@
 )
 
 ListManagedAccountsResponseTypeDef = TypedDict(
     "ListManagedAccountsResponseTypeDef",
     {
         "items": List[ManagedAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef(
     _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
     _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
@@ -2075,15 +2022,15 @@
         "launchConfigurationTemplateID": str,
     },
 )
 _OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef = TypedDict(
     "_OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     {
         "filters": TemplateActionsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListTemplateActionsRequestListTemplateActionsPaginateTypeDef(
     _RequiredListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     _OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
@@ -2113,15 +2060,15 @@
     pass
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
         "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
@@ -2207,145 +2154,47 @@
 )
 
 class PutTemplateActionRequestRequestTypeDef(
     _RequiredPutTemplateActionRequestRequestTypeDef, _OptionalPutTemplateActionRequestRequestTypeDef
 ):
     pass
 
-_RequiredSsmDocumentTypeDef = TypedDict(
-    "_RequiredSsmDocumentTypeDef",
-    {
-        "actionName": str,
-        "ssmDocumentName": str,
-    },
-)
-_OptionalSsmDocumentTypeDef = TypedDict(
-    "_OptionalSsmDocumentTypeDef",
-    {
-        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
-        "mustSucceedForCutover": bool,
-        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
-        "timeoutSeconds": int,
-    },
-    total=False,
-)
-
-class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
-    pass
-
-ReplicationConfigurationTypeDef = TypedDict(
-    "ReplicationConfigurationTypeDef",
-    {
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskOutputTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "sourceServerID": str,
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "sourceServerID": str,
-    },
-)
-_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
-    {
-        "accountID": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "name": str,
-        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": Sequence[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Mapping[str, str],
-        "useDedicatedReplicationServer": bool,
-        "useFipsEndpoint": bool,
-    },
-    total=False,
-)
-
-class UpdateReplicationConfigurationRequestRequestTypeDef(
-    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
-    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
-    {
-        "s3BucketSource": S3BucketSourceTypeDef,
-    },
-)
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
-    pass
-
-SourceServerActionDocumentResponseMetadataTypeDef = TypedDict(
-    "SourceServerActionDocumentResponseMetadataTypeDef",
+SourceServerActionDocumentResponseTypeDef = TypedDict(
+    "SourceServerActionDocumentResponseTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerActionDocumentTypeDef = TypedDict(
     "SourceServerActionDocumentTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
 _RequiredSsmDocumentOutputTypeDef = TypedDict(
     "_RequiredSsmDocumentOutputTypeDef",
@@ -2353,80 +2202,159 @@
         "actionName": str,
         "ssmDocumentName": str,
     },
 )
 _OptionalSsmDocumentOutputTypeDef = TypedDict(
     "_OptionalSsmDocumentOutputTypeDef",
     {
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
 class SsmDocumentOutputTypeDef(
     _RequiredSsmDocumentOutputTypeDef, _OptionalSsmDocumentOutputTypeDef
 ):
     pass
 
-TemplateActionDocumentResponseMetadataTypeDef = TypedDict(
-    "TemplateActionDocumentResponseMetadataTypeDef",
+_RequiredSsmDocumentTypeDef = TypedDict(
+    "_RequiredSsmDocumentTypeDef",
+    {
+        "actionName": str,
+        "ssmDocumentName": str,
+    },
+)
+_OptionalSsmDocumentTypeDef = TypedDict(
+    "_OptionalSsmDocumentTypeDef",
+    {
+        "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
+        "mustSucceedForCutover": bool,
+        "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
+        "timeoutSeconds": int,
+    },
+    total=False,
+)
+
+class SsmDocumentTypeDef(_RequiredSsmDocumentTypeDef, _OptionalSsmDocumentTypeDef):
+    pass
+
+TemplateActionDocumentResponseTypeDef = TypedDict(
+    "TemplateActionDocumentResponseTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TemplateActionDocumentTypeDef = TypedDict(
     "TemplateActionDocumentTypeDef",
     {
         "actionID": str,
         "actionName": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentIdentifier": str,
         "documentVersion": str,
-        "externalParameters": Dict[str, SsmExternalParameterOutputTypeDef],
+        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
-        "parameters": Dict[str, List[SsmParameterStoreParameterOutputTypeDef]],
+        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-WaveResponseMetadataTypeDef = TypedDict(
-    "WaveResponseMetadataTypeDef",
+ReplicationConfigurationTypeDef = TypedDict(
+    "ReplicationConfigurationTypeDef",
+    {
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "sourceServerID": str,
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "name": str,
+        "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": Sequence[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Mapping[str, str],
+        "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
+    },
+    total=False,
+)
+
+class UpdateReplicationConfigurationRequestRequestTypeDef(
+    _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
+    _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
+
+WaveResponseTypeDef = TypedDict(
+    "WaveResponseTypeDef",
     {
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveAggregatedStatus": WaveAggregatedStatusTypeDef,
         "waveID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WaveTypeDef = TypedDict(
     "WaveTypeDef",
     {
         "arn": str,
@@ -2443,15 +2371,15 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "items": List[ApplicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -2466,64 +2394,64 @@
 )
 
 ListExportErrorsResponseTypeDef = TypedDict(
     "ListExportErrorsResponseTypeDef",
     {
         "items": List[ExportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
         "items": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExportResponseTypeDef = TypedDict(
     "StartExportResponseTypeDef",
     {
         "exportTask": ExportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportErrorsResponseTypeDef = TypedDict(
     "ListImportErrorsResponseTypeDef",
     {
         "items": List[ImportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportTaskTypeDef = TypedDict(
     "ImportTaskTypeDef",
     {
         "creationDateTime": str,
         "endDateTime": str,
         "importID": str,
         "progressPercentage": float,
-        "s3BucketSource": S3BucketSourceOutputTypeDef,
+        "s3BucketSource": S3BucketSourceTypeDef,
         "status": ImportStatusType,
         "summary": ImportTaskSummaryTypeDef,
     },
     total=False,
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
 
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
@@ -2533,32 +2461,20 @@
         "lastSeenByServiceDateTime": str,
         "lastTest": LifeCycleLastTestTypeDef,
         "state": LifeCycleStateType,
     },
     total=False,
 )
 
-PostLaunchActionsTypeDef = TypedDict(
-    "PostLaunchActionsTypeDef",
-    {
-        "cloudWatchLogGroupName": str,
-        "deployment": PostLaunchActionsDeploymentTypeType,
-        "s3LogBucket": str,
-        "s3OutputKeyPrefix": str,
-        "ssmDocuments": Sequence[SsmDocumentTypeDef],
-    },
-    total=False,
-)
-
 ListSourceServerActionsResponseTypeDef = TypedDict(
     "ListSourceServerActionsResponseTypeDef",
     {
         "items": List[SourceServerActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
@@ -2578,66 +2494,78 @@
         "s3LogBucket": str,
         "s3OutputKeyPrefix": str,
         "ssmDocuments": List[SsmDocumentOutputTypeDef],
     },
     total=False,
 )
 
+PostLaunchActionsTypeDef = TypedDict(
+    "PostLaunchActionsTypeDef",
+    {
+        "cloudWatchLogGroupName": str,
+        "deployment": PostLaunchActionsDeploymentTypeType,
+        "s3LogBucket": str,
+        "s3OutputKeyPrefix": str,
+        "ssmDocuments": Sequence[SsmDocumentTypeDef],
+    },
+    total=False,
+)
+
 ListTemplateActionsResponseTypeDef = TypedDict(
     "ListTemplateActionsResponseTypeDef",
     {
         "items": List[TemplateActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWavesResponseTypeDef = TypedDict(
     "ListWavesResponseTypeDef",
     {
         "items": List[WaveTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "items": List[ImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "importTask": ImportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SourceServerResponseMetadataTypeDef = TypedDict(
-    "SourceServerResponseMetadataTypeDef",
+SourceServerResponseTypeDef = TypedDict(
+    "SourceServerResponseTypeDef",
     {
         "applicationID": str,
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "fqdnForActionFramework": str,
         "isArchived": bool,
         "launchedInstance": LaunchedInstanceTypeDef,
         "lifeCycle": LifeCycleTypeDef,
         "replicationType": ReplicationTypeType,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "applicationID": str,
@@ -2653,189 +2581,189 @@
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
     },
     total=False,
 )
 
-CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+PostLaunchActionsStatusTypeDef = TypedDict(
+    "PostLaunchActionsStatusTypeDef",
+    {
+        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
+        "ssmAgentDiscoveryDatetime": str,
+    },
+    total=False,
+)
+
+LaunchConfigurationTemplateResponseTypeDef = TypedDict(
+    "LaunchConfigurationTemplateResponseTypeDef",
     {
+        "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
+_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_RequiredLaunchConfigurationTemplateTypeDef",
     {
-        "sourceServerID": str,
+        "launchConfigurationTemplateID": str,
     },
 )
-_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
+_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
+    "_OptionalLaunchConfigurationTemplateTypeDef",
     {
-        "accountID": str,
+        "arn": str,
+        "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
+        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-class UpdateLaunchConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+class LaunchConfigurationTemplateTypeDef(
+    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
 ):
     pass
 
-_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+LaunchConfigurationTypeDef = TypedDict(
+    "LaunchConfigurationTypeDef",
     {
-        "launchConfigurationTemplateID": str,
+        "bootMode": BootModeType,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "ec2LaunchTemplateID": str,
+        "enableMapAutoTagging": bool,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "mapAutoTaggingMpeID": str,
+        "name": str,
+        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "sourceServerID": str,
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
+
+CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
+        "tags": Mapping[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
-    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
-):
-    pass
-
-PostLaunchActionsStatusTypeDef = TypedDict(
-    "PostLaunchActionsStatusTypeDef",
+_RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
-        "ssmAgentDiscoveryDatetime": str,
+        "sourceServerID": str,
     },
-    total=False,
 )
-
-LaunchConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "LaunchConfigurationTemplateResponseMetadataTypeDef",
+_OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
-        "associatePublicIpAddress": bool,
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
-        "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
+        "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
-        "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
+        "name": str,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-_RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_RequiredLaunchConfigurationTemplateTypeDef",
+class UpdateLaunchConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
-_OptionalLaunchConfigurationTemplateTypeDef = TypedDict(
-    "_OptionalLaunchConfigurationTemplateTypeDef",
+_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
-        "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
-        "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
+        "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
-        "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
 
-class LaunchConfigurationTemplateTypeDef(
-    _RequiredLaunchConfigurationTemplateTypeDef, _OptionalLaunchConfigurationTemplateTypeDef
+class UpdateLaunchConfigurationTemplateRequestRequestTypeDef(
+    _RequiredUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
+    _OptionalUpdateLaunchConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
-LaunchConfigurationTypeDef = TypedDict(
-    "LaunchConfigurationTypeDef",
-    {
-        "bootMode": BootModeType,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "ec2LaunchTemplateID": str,
-        "enableMapAutoTagging": bool,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingOutputTypeDef,
-        "mapAutoTaggingMpeID": str,
-        "name": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
-        "sourceServerID": str,
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredParticipatingServerTypeDef = TypedDict(
     "_RequiredParticipatingServerTypeDef",
     {
         "sourceServerID": str,
@@ -2857,15 +2785,15 @@
     pass
 
 DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     {
         "items": List[LaunchConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
@@ -2890,34 +2818,34 @@
     pass
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartCutoverResponseTypeDef = TypedDict(
     "StartCutoverResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTestResponseTypeDef = TypedDict(
     "StartTestResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateTargetInstancesResponseTypeDef = TypedDict(
     "TerminateTargetInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/PKG-INFO` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.28.12
-Summary: Type annotations for boto3.mgn 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgn)](https://pepy.tech/project/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -411,14 +411,15 @@
 
 `mypy_boto3_mgn.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mgn.type_defs import (
     ApplicationAggregatedStatusTypeDef,
+    ResponseMetadataTypeDef,
     ArchiveApplicationRequestRequestTypeDef,
     ArchiveWaveRequestRequestTypeDef,
     AssociateApplicationsRequestRequestTypeDef,
     AssociateSourceServersRequestRequestTypeDef,
     CPUTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     CreateApplicationRequestRequestTypeDef,
@@ -432,85 +433,68 @@
     DeleteApplicationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
     DeleteVcenterClientRequestRequestTypeDef,
     DeleteWaveRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
-    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
     DescribeVcenterClientsRequestRequestTypeDef,
     VcenterClientTypeDef,
     DisassociateApplicationsRequestRequestTypeDef,
     DisassociateSourceServersRequestRequestTypeDef,
     DisconnectFromServiceRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportErrorDataTypeDef,
     ExportTaskSummaryTypeDef,
     FinalizeCutoverRequestRequestTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
     ImportTaskSummaryApplicationsTypeDef,
     ImportTaskSummaryServersTypeDef,
     ImportTaskSummaryWavesTypeDef,
-    S3BucketSourceOutputTypeDef,
+    S3BucketSourceTypeDef,
     JobLogEventDataTypeDef,
-    LaunchTemplateDiskConfOutputTypeDef,
-    LicensingOutputTypeDef,
     LaunchedInstanceTypeDef,
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
     ListApplicationsRequestFiltersTypeDef,
-    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
-    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
-    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
     ListManagedAccountsRequestRequestTypeDef,
     ManagedAccountTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PaginatorConfigTypeDef,
     PauseReplicationRequestRequestTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
-    ReplicationConfigurationReplicatedDiskOutputTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
-    ResponseMetadataTypeDef,
     ResumeReplicationRequestRequestTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
-    S3BucketSourceTypeDef,
-    SsmExternalParameterOutputTypeDef,
-    SsmParameterStoreParameterOutputTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -518,28 +502,39 @@
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     UpdateSourceServerReplicationTypeRequestRequestTypeDef,
     UpdateWaveRequestRequestTypeDef,
     WaveAggregatedStatusTypeDef,
-    ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
+    ApplicationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ChangeServerLifeCycleStateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
+    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
+    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
+    ListManagedAccountsRequestListManagedAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
     ExportTaskTypeDef,
     ImportTaskErrorTypeDef,
     ImportTaskSummaryTypeDef,
+    StartImportRequestRequestTypeDef,
     JobLogTypeDef,
     LifeCycleLastCutoverTypeDef,
     LifeCycleLastTestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListExportsRequestListExportsPaginateTypeDef,
     ListExportsRequestRequestTypeDef,
@@ -551,51 +546,50 @@
     ListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     ListTemplateActionsRequestRequestTypeDef,
     ListWavesRequestListWavesPaginateTypeDef,
     ListWavesRequestRequestTypeDef,
     SourcePropertiesTypeDef,
     PutSourceServerActionRequestRequestTypeDef,
     PutTemplateActionRequestRequestTypeDef,
-    SsmDocumentTypeDef,
-    ReplicationConfigurationTypeDef,
-    UpdateReplicationConfigurationRequestRequestTypeDef,
-    StartImportRequestRequestTypeDef,
-    SourceServerActionDocumentResponseMetadataTypeDef,
+    SourceServerActionDocumentResponseTypeDef,
     SourceServerActionDocumentTypeDef,
     SsmDocumentOutputTypeDef,
-    TemplateActionDocumentResponseMetadataTypeDef,
+    SsmDocumentTypeDef,
+    TemplateActionDocumentResponseTypeDef,
     TemplateActionDocumentTypeDef,
-    WaveResponseMetadataTypeDef,
+    ReplicationConfigurationTypeDef,
+    UpdateReplicationConfigurationRequestRequestTypeDef,
+    WaveResponseTypeDef,
     WaveTypeDef,
     ListApplicationsResponseTypeDef,
     DataReplicationInfoTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsResponseTypeDef,
     StartExportResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ImportTaskTypeDef,
     DescribeJobLogItemsResponseTypeDef,
     LifeCycleTypeDef,
-    PostLaunchActionsTypeDef,
     ListSourceServerActionsResponseTypeDef,
     JobPostLaunchActionsLaunchStatusTypeDef,
     PostLaunchActionsOutputTypeDef,
+    PostLaunchActionsTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesResponseTypeDef,
     ListImportsResponseTypeDef,
     StartImportResponseTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
-    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
-    UpdateLaunchConfigurationRequestRequestTypeDef,
-    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     PostLaunchActionsStatusTypeDef,
-    LaunchConfigurationTemplateResponseMetadataTypeDef,
+    LaunchConfigurationTemplateResponseTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
+    CreateLaunchConfigurationTemplateRequestRequestTypeDef,
+    UpdateLaunchConfigurationRequestRequestTypeDef,
+    UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     DescribeSourceServersResponseTypeDef,
     ParticipatingServerTypeDef,
     DescribeLaunchConfigurationTemplatesResponseTypeDef,
     JobTypeDef,
     DescribeJobsResponseTypeDef,
     StartCutoverResponseTypeDef,
     StartTestResponseTypeDef,
```

### Comparing `mypy-boto3-mgn-1.28.12/mypy_boto3_mgn.egg-info/SOURCES.txt` & `mypy-boto3-mgn-1.28.15/mypy_boto3_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.28.12/setup.py` & `mypy-boto3-mgn-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgn",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mgn 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.mgn 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

