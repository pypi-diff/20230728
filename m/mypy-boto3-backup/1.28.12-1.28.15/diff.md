# Comparing `tmp/mypy-boto3-backup-1.28.12.tar.gz` & `tmp/mypy-boto3-backup-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-backup-1.28.12.tar` & `mypy-boto3-backup-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20994 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/mypy_boto3_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54908 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    72958 2023-07-27 05:17:54.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72873 2023-07-27 05:17:53.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.440698 mypy-boto3-backup-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-07-28 20:42:19.436698 mypy-boto3-backup-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.432698 mypy-boto3-backup-1.28.15/mypy_boto3_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54908 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-28 20:20:03.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 20:20:03.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71441 2023-07-28 20:20:05.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71358 2023-07-28 20:20:04.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.436698 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:19.000000 mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.440698 mypy-boto3-backup-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:20:02.000000 mypy-boto3-backup-1.28.15/setup.py
```

### Comparing `mypy-boto3-backup-1.28.12/LICENSE` & `mypy-boto3-backup-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/PKG-INFO` & `mypy-boto3-backup-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.12
-Summary: Type annotations for boto3.Backup 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -383,162 +383,157 @@
 ```python
 from mypy_boto3_backup.type_defs import (
     AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
-    LifecycleOutputTypeDef,
-    ConditionOutputTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
-    ConditionParameterOutputTypeDef,
     ConditionParameterTypeDef,
-    ControlInputParameterOutputTypeDef,
     ControlInputParameterTypeDef,
     ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
-    CreateBackupSelectionOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
-    CreateReportPlanOutputTypeDef,
     DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
-    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
-    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
-    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupJobsInputRequestTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
     ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
     ListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
     ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
-    ListTagsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
     ReportSettingOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
-    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
-    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
-    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    CopyActionOutputTypeDef,
-    ListBackupSelectionsOutputTypeDef,
-    ListBackupVaultsOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
-    UpdateRecoveryPointLifecycleOutputTypeDef,
     ConditionsOutputTypeDef,
     ConditionsTypeDef,
     FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    CreateBackupSelectionOutputTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
+    CreateReportPlanOutputTypeDef,
+    DeleteBackupPlanOutputTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    DescribeBackupVaultOutputTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
+    DescribeRestoreJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
+    ListBackupSelectionsOutputTypeDef,
+    ListBackupVaultsOutputTypeDef,
+    ListTagsOutputTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
+    StartReportJobOutputTypeDef,
+    StartRestoreJobOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
+    UpdateFrameworkOutputTypeDef,
+    UpdateRecoveryPointLifecycleOutputTypeDef,
+    UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
     ReportPlanTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
```

### Comparing `mypy-boto3-backup-1.28.12/README.md` & `mypy-boto3-backup-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,162 +351,157 @@
 ```python
 from mypy_boto3_backup.type_defs import (
     AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
-    LifecycleOutputTypeDef,
-    ConditionOutputTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
-    ConditionParameterOutputTypeDef,
     ConditionParameterTypeDef,
-    ControlInputParameterOutputTypeDef,
     ControlInputParameterTypeDef,
     ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
-    CreateBackupSelectionOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
-    CreateReportPlanOutputTypeDef,
     DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
-    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
-    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
-    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupJobsInputRequestTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
     ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
     ListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
     ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
-    ListTagsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
     ReportSettingOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
-    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
-    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
-    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    CopyActionOutputTypeDef,
-    ListBackupSelectionsOutputTypeDef,
-    ListBackupVaultsOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
-    UpdateRecoveryPointLifecycleOutputTypeDef,
     ConditionsOutputTypeDef,
     ConditionsTypeDef,
     FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    CreateBackupSelectionOutputTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
+    CreateReportPlanOutputTypeDef,
+    DeleteBackupPlanOutputTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    DescribeBackupVaultOutputTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
+    DescribeRestoreJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
+    ListBackupSelectionsOutputTypeDef,
+    ListBackupVaultsOutputTypeDef,
+    ListTagsOutputTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
+    StartReportJobOutputTypeDef,
+    StartRestoreJobOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
+    UpdateFrameworkOutputTypeDef,
+    UpdateRecoveryPointLifecycleOutputTypeDef,
+    UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
     ReportPlanTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
```

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.py` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.pyi` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/__main__.py` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Backup 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Backup 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.py` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.pyi` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.py` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.pyi` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.py` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,90 +108,90 @@
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupjobspaginator)
         """
 
 
 class ListBackupPlanTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupPlanTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
         """
 
 
 class ListBackupPlanVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupPlanVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
         """
 
 
 class ListBackupPlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
     """
 
     def paginate(
-        self, *, IncludeDeleted: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IncludeDeleted: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
         """
 
 
 class ListBackupSelectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupSelectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
         """
 
 
 class ListBackupVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
         """
 
 
@@ -210,45 +210,45 @@
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listcopyjobspaginator)
         """
 
 
 class ListLegalHoldsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLegalHoldsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
         """
 
 
 class ListProtectedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtectedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
         """
 
 
@@ -264,45 +264,45 @@
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 
 class ListRecoveryPointsByLegalHoldPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
     """
 
     def paginate(
-        self, *, LegalHoldId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LegalHoldId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
         """
 
 
 class ListRecoveryPointsByResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
         """
 
 
@@ -317,13 +317,13 @@
         *,
         ByAccountId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.pyi` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -105,85 +105,85 @@
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupjobspaginator)
         """
 
 class ListBackupPlanTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupPlanTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
         """
 
 class ListBackupPlanVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupPlanVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
         """
 
 class ListBackupPlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
     """
 
     def paginate(
-        self, *, IncludeDeleted: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IncludeDeleted: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
         """
 
 class ListBackupSelectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupSelectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
         """
 
 class ListBackupVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
         """
 
 class ListCopyJobsPaginator(Paginator):
@@ -201,43 +201,43 @@
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listcopyjobspaginator)
         """
 
 class ListLegalHoldsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLegalHoldsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
         """
 
 class ListProtectedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtectedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
         """
 
 class ListRecoveryPointsByBackupVaultPaginator(Paginator):
@@ -252,43 +252,43 @@
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 class ListRecoveryPointsByLegalHoldPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
     """
 
     def paginate(
-        self, *, LegalHoldId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LegalHoldId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
         """
 
 class ListRecoveryPointsByResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
         """
 
 class ListRestoreJobsPaginator(Paginator):
@@ -302,13 +302,13 @@
         *,
         ByAccountId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.py` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,162 +37,157 @@
 
 __all__ = (
     "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
-    "LifecycleOutputTypeDef",
-    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
-    "ConditionParameterOutputTypeDef",
     "ConditionParameterTypeDef",
-    "ControlInputParameterOutputTypeDef",
     "ControlInputParameterTypeDef",
     "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
-    "CreateBackupSelectionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
-    "CreateBackupVaultOutputTypeDef",
-    "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
-    "CreateReportPlanOutputTypeDef",
     "DateRangeOutputTypeDef",
     "DateRangeTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
-    "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
     "DeleteRecoveryPointInputRequestTypeDef",
     "DeleteReportPlanInputRequestTypeDef",
     "DescribeBackupJobInputRequestTypeDef",
     "DescribeBackupVaultInputRequestTypeDef",
-    "DescribeBackupVaultOutputTypeDef",
     "DescribeCopyJobInputRequestTypeDef",
     "DescribeFrameworkInputRequestTypeDef",
-    "DescribeGlobalSettingsOutputTypeDef",
     "DescribeProtectedResourceInputRequestTypeDef",
-    "DescribeProtectedResourceOutputTypeDef",
     "DescribeRecoveryPointInputRequestTypeDef",
-    "DescribeRegionSettingsOutputTypeDef",
     "DescribeReportJobInputRequestTypeDef",
     "DescribeReportPlanInputRequestTypeDef",
     "DescribeRestoreJobInputRequestTypeDef",
-    "DescribeRestoreJobOutputTypeDef",
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     "DisassociateRecoveryPointInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportBackupPlanTemplateInputRequestTypeDef",
-    "ExportBackupPlanTemplateOutputTypeDef",
     "FrameworkTypeDef",
     "GetBackupPlanFromJSONInputRequestTypeDef",
     "GetBackupPlanFromTemplateInputRequestTypeDef",
     "GetBackupPlanInputRequestTypeDef",
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
-    "GetBackupVaultAccessPolicyOutputTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
-    "GetBackupVaultNotificationsOutputTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    "GetSupportedResourceTypesOutputTypeDef",
     "LegalHoldTypeDef",
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupJobsInputRequestTypeDef",
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
-    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupPlansInputRequestTypeDef",
-    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
     "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
-    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
     "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
-    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
     "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
-    "ListTagsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
     "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
     "ReportSettingOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartBackupJobOutputTypeDef",
-    "StartCopyJobOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
-    "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
-    "StartRestoreJobOutputTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateFrameworkOutputTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
-    "UpdateReportPlanOutputTypeDef",
     "BackupPlansListMemberTypeDef",
-    "CreateBackupPlanOutputTypeDef",
-    "UpdateBackupPlanOutputTypeDef",
     "BackupJobTypeDef",
     "CopyJobTypeDef",
-    "DescribeBackupJobOutputTypeDef",
-    "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
-    "CopyActionOutputTypeDef",
-    "ListBackupSelectionsOutputTypeDef",
-    "ListBackupVaultsOutputTypeDef",
-    "DescribeRecoveryPointOutputTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
     "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
     "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
+    "CreateBackupPlanOutputTypeDef",
+    "CreateBackupSelectionOutputTypeDef",
+    "CreateBackupVaultOutputTypeDef",
+    "CreateFrameworkOutputTypeDef",
+    "CreateReportPlanOutputTypeDef",
+    "DeleteBackupPlanOutputTypeDef",
+    "DescribeBackupJobOutputTypeDef",
+    "DescribeBackupVaultOutputTypeDef",
+    "DescribeGlobalSettingsOutputTypeDef",
+    "DescribeProtectedResourceOutputTypeDef",
+    "DescribeRecoveryPointOutputTypeDef",
+    "DescribeRegionSettingsOutputTypeDef",
+    "DescribeRestoreJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportBackupPlanTemplateOutputTypeDef",
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    "GetBackupVaultNotificationsOutputTypeDef",
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    "GetSupportedResourceTypesOutputTypeDef",
+    "ListBackupPlanTemplatesOutputTypeDef",
+    "ListBackupSelectionsOutputTypeDef",
+    "ListBackupVaultsOutputTypeDef",
+    "ListTagsOutputTypeDef",
+    "StartBackupJobOutputTypeDef",
+    "StartCopyJobOutputTypeDef",
+    "StartReportJobOutputTypeDef",
+    "StartRestoreJobOutputTypeDef",
+    "UpdateBackupPlanOutputTypeDef",
+    "UpdateFrameworkOutputTypeDef",
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
     "RecoveryPointSelectionOutputTypeDef",
     "RecoveryPointSelectionTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
     "ReportJobTypeDef",
     "ReportPlanTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
@@ -269,32 +264,14 @@
     {
         "MoveToColdStorageAfterDays": int,
         "DeleteAfterDays": int,
     },
     total=False,
 )
 
-LifecycleOutputTypeDef = TypedDict(
-    "LifecycleOutputTypeDef",
-    {
-        "MoveToColdStorageAfterDays": int,
-        "DeleteAfterDays": int,
-    },
-    total=False,
-)
-
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "ConditionType": Literal["STRINGEQUALS"],
-        "ConditionKey": str,
-        "ConditionValue": str,
-    },
-)
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ConditionType": Literal["STRINGEQUALS"],
         "ConditionKey": str,
         "ConditionValue": str,
     },
@@ -357,41 +334,23 @@
 
 class CancelLegalHoldInputRequestTypeDef(
     _RequiredCancelLegalHoldInputRequestTypeDef, _OptionalCancelLegalHoldInputRequestTypeDef
 ):
     pass
 
 
-ConditionParameterOutputTypeDef = TypedDict(
-    "ConditionParameterOutputTypeDef",
-    {
-        "ConditionKey": str,
-        "ConditionValue": str,
-    },
-    total=False,
-)
-
 ConditionParameterTypeDef = TypedDict(
     "ConditionParameterTypeDef",
     {
         "ConditionKey": str,
         "ConditionValue": str,
     },
     total=False,
 )
 
-ControlInputParameterOutputTypeDef = TypedDict(
-    "ControlInputParameterOutputTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-    },
-    total=False,
-)
-
 ControlInputParameterTypeDef = TypedDict(
     "ControlInputParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -413,21 +372,22 @@
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateBackupSelectionOutputTypeDef = TypedDict(
-    "CreateBackupSelectionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
@@ -446,33 +406,14 @@
 
 class CreateBackupVaultInputRequestTypeDef(
     _RequiredCreateBackupVaultInputRequestTypeDef, _OptionalCreateBackupVaultInputRequestTypeDef
 ):
     pass
 
 
-CreateBackupVaultOutputTypeDef = TypedDict(
-    "CreateBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFrameworkOutputTypeDef = TypedDict(
-    "CreateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReportDeliveryChannelTypeDef = TypedDict(
     "_RequiredReportDeliveryChannelTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalReportDeliveryChannelTypeDef = TypedDict(
@@ -510,24 +451,14 @@
 )
 
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
 
-CreateReportPlanOutputTypeDef = TypedDict(
-    "CreateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DateRangeOutputTypeDef = TypedDict(
     "DateRangeOutputTypeDef",
     {
         "FromDate": datetime,
         "ToDate": datetime,
     },
 )
@@ -543,25 +474,14 @@
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-DeleteBackupPlanOutputTypeDef = TypedDict(
-    "DeleteBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "DeletionDate": datetime,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBackupSelectionInputRequestTypeDef = TypedDict(
     "DeleteBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "SelectionId": str,
     },
 )
@@ -626,89 +546,43 @@
 DescribeBackupVaultInputRequestTypeDef = TypedDict(
     "DescribeBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-DescribeBackupVaultOutputTypeDef = TypedDict(
-    "DescribeBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "EncryptionKeyArn": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "NumberOfRecoveryPoints": int,
-        "Locked": bool,
-        "MinRetentionDays": int,
-        "MaxRetentionDays": int,
-        "LockDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCopyJobInputRequestTypeDef = TypedDict(
     "DescribeCopyJobInputRequestTypeDef",
     {
         "CopyJobId": str,
     },
 )
 
 DescribeFrameworkInputRequestTypeDef = TypedDict(
     "DescribeFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 
-DescribeGlobalSettingsOutputTypeDef = TypedDict(
-    "DescribeGlobalSettingsOutputTypeDef",
-    {
-        "GlobalSettings": Dict[str, str],
-        "LastUpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProtectedResourceInputRequestTypeDef = TypedDict(
     "DescribeProtectedResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeProtectedResourceOutputTypeDef = TypedDict(
-    "DescribeProtectedResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceType": str,
-        "LastBackupTime": datetime,
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRecoveryPointInputRequestTypeDef = TypedDict(
     "DescribeRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-DescribeRegionSettingsOutputTypeDef = TypedDict(
-    "DescribeRegionSettingsOutputTypeDef",
-    {
-        "ResourceTypeOptInPreference": Dict[str, bool],
-        "ResourceTypeManagementPreference": Dict[str, bool],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeReportJobInputRequestTypeDef = TypedDict(
     "DescribeReportJobInputRequestTypeDef",
     {
         "ReportJobId": str,
     },
 )
 
@@ -722,34 +596,14 @@
 DescribeRestoreJobInputRequestTypeDef = TypedDict(
     "DescribeRestoreJobInputRequestTypeDef",
     {
         "RestoreJobId": str,
     },
 )
 
-DescribeRestoreJobOutputTypeDef = TypedDict(
-    "DescribeRestoreJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "RestoreJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "Status": RestoreJobStatusType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "ExpectedCompletionTimeMinutes": int,
-        "CreatedResourceArn": str,
-        "ResourceType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateRecoveryPointFromParentInputRequestTypeDef = TypedDict(
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
@@ -758,36 +612,21 @@
     "DisassociateRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportBackupPlanTemplateInputRequestTypeDef = TypedDict(
     "ExportBackupPlanTemplateInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-ExportBackupPlanTemplateOutputTypeDef = TypedDict(
-    "ExportBackupPlanTemplateOutputTypeDef",
-    {
-        "BackupPlanTemplateJson": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FrameworkTypeDef = TypedDict(
     "FrameworkTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "NumberOfControls": int,
@@ -843,42 +682,21 @@
 GetBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBackupVaultNotificationsInputRequestTypeDef = TypedDict(
     "GetBackupVaultNotificationsInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultNotificationsOutputTypeDef = TypedDict(
-    "GetBackupVaultNotificationsOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "SNSTopicArn": str,
-        "BackupVaultEvents": List[BackupVaultEventType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLegalHoldInputRequestTypeDef = TypedDict(
     "GetLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 
@@ -886,60 +704,34 @@
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    {
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "RestoreMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSupportedResourceTypesOutputTypeDef = TypedDict(
-    "GetSupportedResourceTypesOutputTypeDef",
-    {
-        "ResourceTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LegalHoldTypeDef = TypedDict(
     "LegalHoldTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
     },
     total=False,
 )
 
-ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBackupJobsInputRequestTypeDef = TypedDict(
     "ListBackupJobsInputRequestTypeDef",
     {
@@ -955,53 +747,23 @@
         "ByCompleteAfter": Union[datetime, str],
         "ByCompleteBefore": Union[datetime, str],
         "ByParentJobId": str,
     },
     total=False,
 )
 
-ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
-    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBackupPlanVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupPlanVersionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupPlanVersionsInputRequestTypeDef = TypedDict(
@@ -1017,55 +779,24 @@
 class ListBackupPlanVersionsInputRequestTypeDef(
     _RequiredListBackupPlanVersionsInputRequestTypeDef,
     _OptionalListBackupPlanVersionsInputRequestTypeDef,
 ):
     pass
 
 
-ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    {
-        "IncludeDeleted": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupPlansInputRequestTypeDef = TypedDict(
     "ListBackupPlansInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IncludeDeleted": bool,
     },
     total=False,
 )
 
-_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
-    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBackupSelectionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupSelectionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupSelectionsInputRequestTypeDef = TypedDict(
@@ -1081,49 +812,23 @@
 class ListBackupSelectionsInputRequestTypeDef(
     _RequiredListBackupSelectionsInputRequestTypeDef,
     _OptionalListBackupSelectionsInputRequestTypeDef,
 ):
     pass
 
 
-ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupVaultsInputRequestTypeDef = TypedDict(
     "ListBackupVaultsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCopyJobsInputRequestTypeDef = TypedDict(
     "ListCopyJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByResourceArn": str,
         "ByState": CopyJobStateType,
@@ -1144,39 +849,23 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLegalHoldsInputRequestTypeDef = TypedDict(
     "ListLegalHoldsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProtectedResourcesInputRequestTypeDef = TypedDict(
     "ListProtectedResourcesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1189,42 +878,14 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
@@ -1246,36 +907,14 @@
 class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
     _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
     _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "LegalHoldId": str,
-    },
-)
-_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
-    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -1302,36 +941,14 @@
         "ResourceArn": str,
         "ResourceType": str,
         "BackupVaultName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
-    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
@@ -1386,28 +1003,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    {
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRestoreJobsInputRequestTypeDef = TypedDict(
     "ListRestoreJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByAccountId": str,
         "ByCreatedBefore": Union[datetime, str],
@@ -1457,33 +1060,14 @@
 
 class ListTagsInputRequestTypeDef(
     _RequiredListTagsInputRequestTypeDef, _OptionalListTagsInputRequestTypeDef
 ):
     pass
 
 
-ListTagsOutputTypeDef = TypedDict(
-    "ListTagsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -1587,46 +1171,14 @@
 
 class ReportSettingOutputTypeDef(
     _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
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
-StartBackupJobOutputTypeDef = TypedDict(
-    "StartBackupJobOutputTypeDef",
-    {
-        "BackupJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartCopyJobOutputTypeDef = TypedDict(
-    "StartCopyJobOutputTypeDef",
-    {
-        "CopyJobId": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1640,22 +1192,14 @@
 
 class StartReportJobInputRequestTypeDef(
     _RequiredStartReportJobInputRequestTypeDef, _OptionalStartReportJobInputRequestTypeDef
 ):
     pass
 
 
-StartReportJobOutputTypeDef = TypedDict(
-    "StartReportJobOutputTypeDef",
-    {
-        "ReportJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRestoreJobInputRequestTypeDef = TypedDict(
     "_RequiredStartRestoreJobInputRequestTypeDef",
     {
         "RecoveryPointArn": str,
         "Metadata": Mapping[str, str],
     },
 )
@@ -1673,22 +1217,14 @@
 
 class StartRestoreJobInputRequestTypeDef(
     _RequiredStartRestoreJobInputRequestTypeDef, _OptionalStartRestoreJobInputRequestTypeDef
 ):
     pass
 
 
-StartRestoreJobOutputTypeDef = TypedDict(
-    "StartRestoreJobOutputTypeDef",
-    {
-        "RestoreJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopBackupJobInputRequestTypeDef = TypedDict(
     "StopBackupJobInputRequestTypeDef",
     {
         "BackupJobId": str,
     },
 )
 
@@ -1704,24 +1240,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeyList": Sequence[str],
     },
 )
 
-UpdateFrameworkOutputTypeDef = TypedDict(
-    "UpdateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "GlobalSettings": Mapping[str, str],
     },
     total=False,
 )
@@ -1731,24 +1257,14 @@
     {
         "ResourceTypeOptInPreference": Mapping[str, bool],
         "ResourceTypeManagementPreference": Mapping[str, bool],
     },
     total=False,
 )
 
-UpdateReportPlanOutputTypeDef = TypedDict(
-    "UpdateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupPlansListMemberTypeDef = TypedDict(
     "BackupPlansListMemberTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
@@ -1757,38 +1273,14 @@
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
-CreateBackupPlanOutputTypeDef = TypedDict(
-    "CreateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBackupPlanOutputTypeDef = TypedDict(
-    "UpdateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
         "AccountId": str,
         "BackupJobId": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
@@ -1839,55 +1331,14 @@
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
         "ResourceName": str,
     },
     total=False,
 )
 
-DescribeBackupJobOutputTypeDef = TypedDict(
-    "DescribeBackupJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "BackupJobId": str,
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "State": BackupJobStateType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "ResourceType": str,
-        "BytesTransferred": int,
-        "ExpectedCompletionDate": datetime,
-        "StartBy": datetime,
-        "BackupOptions": Dict[str, str],
-        "BackupType": str,
-        "ParentJobId": str,
-        "IsParent": bool,
-        "NumberOfChildJobs": int,
-        "ChildJobsInState": Dict[BackupJobStateType, int],
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupPlanTemplatesOutputTypeDef = TypedDict(
-    "ListBackupPlanTemplatesOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
         "DestinationBackupVaultArn": str,
     },
 )
 _OptionalCopyActionTypeDef = TypedDict(
@@ -1975,83 +1426,240 @@
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredCopyActionOutputTypeDef = TypedDict(
-    "_RequiredCopyActionOutputTypeDef",
+RecoveryPointByBackupVaultTypeDef = TypedDict(
+    "RecoveryPointByBackupVaultTypeDef",
     {
-        "DestinationBackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SourceBackupVaultArn": str,
+        "ResourceArn": str,
+        "ResourceType": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "IamRoleArn": str,
+        "Status": RecoveryPointStatusType,
+        "StatusMessage": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "BackupSizeInBytes": int,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "Lifecycle": LifecycleTypeDef,
+        "EncryptionKeyArn": str,
+        "IsEncrypted": bool,
+        "LastRestoreTime": datetime,
+        "ParentRecoveryPointArn": str,
+        "CompositeMemberIdentifier": str,
+        "IsParent": bool,
+        "ResourceName": str,
     },
+    total=False,
 )
-_OptionalCopyActionOutputTypeDef = TypedDict(
-    "_OptionalCopyActionOutputTypeDef",
+
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
     {
-        "Lifecycle": LifecycleOutputTypeDef,
+        "StringEquals": List[ConditionParameterTypeDef],
+        "StringNotEquals": List[ConditionParameterTypeDef],
+        "StringLike": List[ConditionParameterTypeDef],
+        "StringNotLike": List[ConditionParameterTypeDef],
     },
     total=False,
 )
 
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
+    {
+        "StringEquals": Sequence[ConditionParameterTypeDef],
+        "StringNotEquals": Sequence[ConditionParameterTypeDef],
+        "StringLike": Sequence[ConditionParameterTypeDef],
+        "StringNotLike": Sequence[ConditionParameterTypeDef],
+    },
+    total=False,
+)
 
-class CopyActionOutputTypeDef(_RequiredCopyActionOutputTypeDef, _OptionalCopyActionOutputTypeDef):
+_RequiredFrameworkControlOutputTypeDef = TypedDict(
+    "_RequiredFrameworkControlOutputTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlOutputTypeDef = TypedDict(
+    "_OptionalFrameworkControlOutputTypeDef",
+    {
+        "ControlInputParameters": List[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FrameworkControlOutputTypeDef(
+    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
+):
     pass
 
 
-ListBackupSelectionsOutputTypeDef = TypedDict(
-    "ListBackupSelectionsOutputTypeDef",
+_RequiredFrameworkControlTypeDef = TypedDict(
+    "_RequiredFrameworkControlTypeDef",
     {
-        "NextToken": str,
-        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ControlName": str,
     },
 )
+_OptionalFrameworkControlTypeDef = TypedDict(
+    "_OptionalFrameworkControlTypeDef",
+    {
+        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeTypeDef,
+    },
+    total=False,
+)
 
-ListBackupVaultsOutputTypeDef = TypedDict(
-    "ListBackupVaultsOutputTypeDef",
+
+class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
+    pass
+
+
+CreateBackupPlanOutputTypeDef = TypedDict(
+    "CreateBackupPlanOutputTypeDef",
     {
-        "BackupVaultList": List[BackupVaultListMemberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRecoveryPointOutputTypeDef = TypedDict(
-    "DescribeRecoveryPointOutputTypeDef",
+CreateBackupSelectionOutputTypeDef = TypedDict(
+    "CreateBackupSelectionOutputTypeDef",
+    {
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBackupVaultOutputTypeDef = TypedDict(
+    "CreateBackupVaultOutputTypeDef",
     {
-        "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
-        "SourceBackupVaultArn": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFrameworkOutputTypeDef = TypedDict(
+    "CreateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateReportPlanOutputTypeDef = TypedDict(
+    "CreateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupPlanOutputTypeDef = TypedDict(
+    "DeleteBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "DeletionDate": datetime,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupJobOutputTypeDef = TypedDict(
+    "DescribeBackupJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "BackupJobId": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
         "ResourceArn": str,
-        "ResourceType": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "IamRoleArn": str,
-        "Status": RecoveryPointStatusType,
-        "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
+        "State": BackupJobStateType,
+        "StatusMessage": str,
+        "PercentDone": str,
         "BackupSizeInBytes": int,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleOutputTypeDef,
-        "EncryptionKeyArn": str,
-        "IsEncrypted": bool,
-        "StorageClass": StorageClassType,
-        "LastRestoreTime": datetime,
-        "ParentRecoveryPointArn": str,
-        "CompositeMemberIdentifier": str,
+        "IamRoleArn": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "ResourceType": str,
+        "BytesTransferred": int,
+        "ExpectedCompletionDate": datetime,
+        "StartBy": datetime,
+        "BackupOptions": Dict[str, str],
+        "BackupType": str,
+        "ParentJobId": str,
         "IsParent": bool,
+        "NumberOfChildJobs": int,
+        "ChildJobsInState": Dict[BackupJobStateType, int],
         "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecoveryPointByBackupVaultTypeDef = TypedDict(
-    "RecoveryPointByBackupVaultTypeDef",
+DescribeBackupVaultOutputTypeDef = TypedDict(
+    "DescribeBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "EncryptionKeyArn": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "NumberOfRecoveryPoints": int,
+        "Locked": bool,
+        "MinRetentionDays": int,
+        "MaxRetentionDays": int,
+        "LockDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGlobalSettingsOutputTypeDef = TypedDict(
+    "DescribeGlobalSettingsOutputTypeDef",
+    {
+        "GlobalSettings": Dict[str, str],
+        "LastUpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProtectedResourceOutputTypeDef = TypedDict(
+    "DescribeProtectedResourceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceType": str,
+        "LastBackupTime": datetime,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRecoveryPointOutputTypeDef = TypedDict(
+    "DescribeRecoveryPointOutputTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -2059,100 +1667,225 @@
         "IamRoleArn": str,
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleOutputTypeDef,
+        "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
+        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
+DescribeRegionSettingsOutputTypeDef = TypedDict(
+    "DescribeRegionSettingsOutputTypeDef",
+    {
+        "ResourceTypeOptInPreference": Dict[str, bool],
+        "ResourceTypeManagementPreference": Dict[str, bool],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRestoreJobOutputTypeDef = TypedDict(
+    "DescribeRestoreJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "RestoreJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "Status": RestoreJobStatusType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "ExpectedCompletionTimeMinutes": int,
+        "CreatedResourceArn": str,
+        "ResourceType": str,
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
+ExportBackupPlanTemplateOutputTypeDef = TypedDict(
+    "ExportBackupPlanTemplateOutputTypeDef",
+    {
+        "BackupPlanTemplateJson": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultNotificationsOutputTypeDef = TypedDict(
+    "GetBackupVaultNotificationsOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SNSTopicArn": str,
+        "BackupVaultEvents": List[BackupVaultEventType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "Lifecycle": LifecycleOutputTypeDef,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RestoreMetadata": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionsOutputTypeDef = TypedDict(
-    "ConditionsOutputTypeDef",
+GetSupportedResourceTypesOutputTypeDef = TypedDict(
+    "GetSupportedResourceTypesOutputTypeDef",
     {
-        "StringEquals": List[ConditionParameterOutputTypeDef],
-        "StringNotEquals": List[ConditionParameterOutputTypeDef],
-        "StringLike": List[ConditionParameterOutputTypeDef],
-        "StringNotLike": List[ConditionParameterOutputTypeDef],
+        "ResourceTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ConditionsTypeDef = TypedDict(
-    "ConditionsTypeDef",
+ListBackupPlanTemplatesOutputTypeDef = TypedDict(
+    "ListBackupPlanTemplatesOutputTypeDef",
     {
-        "StringEquals": Sequence[ConditionParameterTypeDef],
-        "StringNotEquals": Sequence[ConditionParameterTypeDef],
-        "StringLike": Sequence[ConditionParameterTypeDef],
-        "StringNotLike": Sequence[ConditionParameterTypeDef],
+        "NextToken": str,
+        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredFrameworkControlOutputTypeDef = TypedDict(
-    "_RequiredFrameworkControlOutputTypeDef",
+ListBackupSelectionsOutputTypeDef = TypedDict(
+    "ListBackupSelectionsOutputTypeDef",
     {
-        "ControlName": str,
+        "NextToken": str,
+        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFrameworkControlOutputTypeDef = TypedDict(
-    "_OptionalFrameworkControlOutputTypeDef",
+
+ListBackupVaultsOutputTypeDef = TypedDict(
+    "ListBackupVaultsOutputTypeDef",
     {
-        "ControlInputParameters": List[ControlInputParameterOutputTypeDef],
-        "ControlScope": ControlScopeOutputTypeDef,
+        "BackupVaultList": List[BackupVaultListMemberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTagsOutputTypeDef = TypedDict(
+    "ListTagsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class FrameworkControlOutputTypeDef(
-    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
-):
-    pass
+StartBackupJobOutputTypeDef = TypedDict(
+    "StartBackupJobOutputTypeDef",
+    {
+        "BackupJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartCopyJobOutputTypeDef = TypedDict(
+    "StartCopyJobOutputTypeDef",
+    {
+        "CopyJobId": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredFrameworkControlTypeDef = TypedDict(
-    "_RequiredFrameworkControlTypeDef",
+StartReportJobOutputTypeDef = TypedDict(
+    "StartReportJobOutputTypeDef",
     {
-        "ControlName": str,
+        "ReportJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFrameworkControlTypeDef = TypedDict(
-    "_OptionalFrameworkControlTypeDef",
+
+StartRestoreJobOutputTypeDef = TypedDict(
+    "StartRestoreJobOutputTypeDef",
     {
-        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeTypeDef,
+        "RestoreJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateBackupPlanOutputTypeDef = TypedDict(
+    "UpdateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
-    pass
+UpdateFrameworkOutputTypeDef = TypedDict(
+    "UpdateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "Lifecycle": LifecycleTypeDef,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateReportPlanOutputTypeDef = TypedDict(
+    "UpdateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
         "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
         "ReportSetting": ReportSettingTypeDef,
@@ -2220,60 +1953,267 @@
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
         "Frameworks": List[FrameworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLegalHoldsOutputTypeDef = TypedDict(
     "ListLegalHoldsOutputTypeDef",
     {
         "NextToken": str,
         "LegalHolds": List[LegalHoldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
+    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    {
+        "IncludeDeleted": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
+    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+):
+    pass
+
+
+ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByParentRecoveryPointArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "LegalHoldId": str,
+    },
+)
+_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
+    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
+    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+):
+    pass
+
+
+ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
+    {
+        "ByAccountId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
     {
         "Results": List[ProtectedResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByLegalHoldOutputTypeDef = TypedDict(
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     {
         "RecoveryPoints": List[RecoveryPointMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByResourceOutputTypeDef = TypedDict(
     "ListRecoveryPointsByResourceOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRestoreJobsOutputTypeDef = TypedDict(
     "ListRestoreJobsOutputTypeDef",
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
@@ -2305,50 +2245,50 @@
 )
 
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupPlansOutputTypeDef = TypedDict(
     "ListBackupPlansOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlansList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupJobsOutputTypeDef = TypedDict(
     "ListBackupJobsOutputTypeDef",
     {
         "BackupJobs": List[BackupJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCopyJobOutputTypeDef = TypedDict(
     "DescribeCopyJobOutputTypeDef",
     {
         "CopyJob": CopyJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCopyJobsOutputTypeDef = TypedDict(
     "ListCopyJobsOutputTypeDef",
     {
         "CopyJobs": List[CopyJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupRuleInputTypeDef = TypedDict(
     "_RequiredBackupRuleInputTypeDef",
     {
         "RuleName": str,
@@ -2383,18 +2323,18 @@
 )
 _OptionalBackupRuleTypeDef = TypedDict(
     "_OptionalBackupRuleTypeDef",
     {
         "ScheduleExpression": str,
         "StartWindowMinutes": int,
         "CompletionWindowMinutes": int,
-        "Lifecycle": LifecycleOutputTypeDef,
+        "Lifecycle": LifecycleTypeDef,
         "RecoveryPointTags": Dict[str, str],
         "RuleId": str,
-        "CopyActions": List[CopyActionOutputTypeDef],
+        "CopyActions": List[CopyActionTypeDef],
         "EnableContinuousBackup": bool,
     },
     total=False,
 )
 
 
 class BackupRuleTypeDef(_RequiredBackupRuleTypeDef, _OptionalBackupRuleTypeDef):
@@ -2402,30 +2342,30 @@
 
 
 ListRecoveryPointsByBackupVaultOutputTypeDef = TypedDict(
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupSelectionOutputTypeDef = TypedDict(
     "_RequiredBackupSelectionOutputTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
 _OptionalBackupSelectionOutputTypeDef = TypedDict(
     "_OptionalBackupSelectionOutputTypeDef",
     {
         "Resources": List[str],
-        "ListOfTags": List[ConditionOutputTypeDef],
+        "ListOfTags": List[ConditionTypeDef],
         "NotResources": List[str],
         "Conditions": ConditionsOutputTypeDef,
     },
     total=False,
 )
 
 
@@ -2465,15 +2405,15 @@
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "FrameworkControls": List[FrameworkControlOutputTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
@@ -2526,15 +2466,15 @@
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLegalHoldOutputTypeDef = TypedDict(
     "GetLegalHoldOutputTypeDef",
     {
         "Title": str,
@@ -2543,15 +2483,15 @@
         "CancelDescription": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
         "Title": str,
@@ -2575,41 +2515,41 @@
     pass
 
 
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReportJobsOutputTypeDef = TypedDict(
     "ListReportJobsOutputTypeDef",
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReportPlanOutputTypeDef = TypedDict(
     "DescribeReportPlanOutputTypeDef",
     {
         "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReportPlansOutputTypeDef = TypedDict(
     "ListReportPlansOutputTypeDef",
     {
         "ReportPlans": List[ReportPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
@@ -2653,15 +2593,15 @@
     "GetBackupSelectionOutputTypeDef",
     {
         "BackupSelection": BackupSelectionOutputTypeDef,
         "SelectionId": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "CreatorRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
@@ -2714,23 +2654,23 @@
     },
 )
 
 GetBackupPlanFromJSONOutputTypeDef = TypedDict(
     "GetBackupPlanFromJSONOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanFromTemplateOutputTypeDef = TypedDict(
     "GetBackupPlanFromTemplateOutputTypeDef",
     {
         "BackupPlanDocument": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanOutputTypeDef = TypedDict(
     "GetBackupPlanOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
@@ -2738,10 +2678,10 @@
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.pyi` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -36,162 +36,157 @@
 
 __all__ = (
     "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
-    "LifecycleOutputTypeDef",
-    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
-    "ConditionParameterOutputTypeDef",
     "ConditionParameterTypeDef",
-    "ControlInputParameterOutputTypeDef",
     "ControlInputParameterTypeDef",
     "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
-    "CreateBackupSelectionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
-    "CreateBackupVaultOutputTypeDef",
-    "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
-    "CreateReportPlanOutputTypeDef",
     "DateRangeOutputTypeDef",
     "DateRangeTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
-    "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
     "DeleteRecoveryPointInputRequestTypeDef",
     "DeleteReportPlanInputRequestTypeDef",
     "DescribeBackupJobInputRequestTypeDef",
     "DescribeBackupVaultInputRequestTypeDef",
-    "DescribeBackupVaultOutputTypeDef",
     "DescribeCopyJobInputRequestTypeDef",
     "DescribeFrameworkInputRequestTypeDef",
-    "DescribeGlobalSettingsOutputTypeDef",
     "DescribeProtectedResourceInputRequestTypeDef",
-    "DescribeProtectedResourceOutputTypeDef",
     "DescribeRecoveryPointInputRequestTypeDef",
-    "DescribeRegionSettingsOutputTypeDef",
     "DescribeReportJobInputRequestTypeDef",
     "DescribeReportPlanInputRequestTypeDef",
     "DescribeRestoreJobInputRequestTypeDef",
-    "DescribeRestoreJobOutputTypeDef",
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     "DisassociateRecoveryPointInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportBackupPlanTemplateInputRequestTypeDef",
-    "ExportBackupPlanTemplateOutputTypeDef",
     "FrameworkTypeDef",
     "GetBackupPlanFromJSONInputRequestTypeDef",
     "GetBackupPlanFromTemplateInputRequestTypeDef",
     "GetBackupPlanInputRequestTypeDef",
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
-    "GetBackupVaultAccessPolicyOutputTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
-    "GetBackupVaultNotificationsOutputTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    "GetSupportedResourceTypesOutputTypeDef",
     "LegalHoldTypeDef",
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupJobsInputRequestTypeDef",
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
-    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupPlansInputRequestTypeDef",
-    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
     "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
-    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
     "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
-    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
     "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
-    "ListTagsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
     "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
     "ReportSettingOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartBackupJobOutputTypeDef",
-    "StartCopyJobOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
-    "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
-    "StartRestoreJobOutputTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateFrameworkOutputTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
-    "UpdateReportPlanOutputTypeDef",
     "BackupPlansListMemberTypeDef",
-    "CreateBackupPlanOutputTypeDef",
-    "UpdateBackupPlanOutputTypeDef",
     "BackupJobTypeDef",
     "CopyJobTypeDef",
-    "DescribeBackupJobOutputTypeDef",
-    "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
-    "CopyActionOutputTypeDef",
-    "ListBackupSelectionsOutputTypeDef",
-    "ListBackupVaultsOutputTypeDef",
-    "DescribeRecoveryPointOutputTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
     "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
     "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
+    "CreateBackupPlanOutputTypeDef",
+    "CreateBackupSelectionOutputTypeDef",
+    "CreateBackupVaultOutputTypeDef",
+    "CreateFrameworkOutputTypeDef",
+    "CreateReportPlanOutputTypeDef",
+    "DeleteBackupPlanOutputTypeDef",
+    "DescribeBackupJobOutputTypeDef",
+    "DescribeBackupVaultOutputTypeDef",
+    "DescribeGlobalSettingsOutputTypeDef",
+    "DescribeProtectedResourceOutputTypeDef",
+    "DescribeRecoveryPointOutputTypeDef",
+    "DescribeRegionSettingsOutputTypeDef",
+    "DescribeRestoreJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportBackupPlanTemplateOutputTypeDef",
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    "GetBackupVaultNotificationsOutputTypeDef",
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    "GetSupportedResourceTypesOutputTypeDef",
+    "ListBackupPlanTemplatesOutputTypeDef",
+    "ListBackupSelectionsOutputTypeDef",
+    "ListBackupVaultsOutputTypeDef",
+    "ListTagsOutputTypeDef",
+    "StartBackupJobOutputTypeDef",
+    "StartCopyJobOutputTypeDef",
+    "StartReportJobOutputTypeDef",
+    "StartRestoreJobOutputTypeDef",
+    "UpdateBackupPlanOutputTypeDef",
+    "UpdateFrameworkOutputTypeDef",
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
     "RecoveryPointSelectionOutputTypeDef",
     "RecoveryPointSelectionTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
     "ReportJobTypeDef",
     "ReportPlanTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
@@ -268,32 +263,14 @@
     {
         "MoveToColdStorageAfterDays": int,
         "DeleteAfterDays": int,
     },
     total=False,
 )
 
-LifecycleOutputTypeDef = TypedDict(
-    "LifecycleOutputTypeDef",
-    {
-        "MoveToColdStorageAfterDays": int,
-        "DeleteAfterDays": int,
-    },
-    total=False,
-)
-
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "ConditionType": Literal["STRINGEQUALS"],
-        "ConditionKey": str,
-        "ConditionValue": str,
-    },
-)
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ConditionType": Literal["STRINGEQUALS"],
         "ConditionKey": str,
         "ConditionValue": str,
     },
@@ -354,41 +331,23 @@
 )
 
 class CancelLegalHoldInputRequestTypeDef(
     _RequiredCancelLegalHoldInputRequestTypeDef, _OptionalCancelLegalHoldInputRequestTypeDef
 ):
     pass
 
-ConditionParameterOutputTypeDef = TypedDict(
-    "ConditionParameterOutputTypeDef",
-    {
-        "ConditionKey": str,
-        "ConditionValue": str,
-    },
-    total=False,
-)
-
 ConditionParameterTypeDef = TypedDict(
     "ConditionParameterTypeDef",
     {
         "ConditionKey": str,
         "ConditionValue": str,
     },
     total=False,
 )
 
-ControlInputParameterOutputTypeDef = TypedDict(
-    "ControlInputParameterOutputTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-    },
-    total=False,
-)
-
 ControlInputParameterTypeDef = TypedDict(
     "ControlInputParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -410,21 +369,22 @@
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateBackupSelectionOutputTypeDef = TypedDict(
-    "CreateBackupSelectionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
@@ -441,33 +401,14 @@
 )
 
 class CreateBackupVaultInputRequestTypeDef(
     _RequiredCreateBackupVaultInputRequestTypeDef, _OptionalCreateBackupVaultInputRequestTypeDef
 ):
     pass
 
-CreateBackupVaultOutputTypeDef = TypedDict(
-    "CreateBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFrameworkOutputTypeDef = TypedDict(
-    "CreateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReportDeliveryChannelTypeDef = TypedDict(
     "_RequiredReportDeliveryChannelTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalReportDeliveryChannelTypeDef = TypedDict(
@@ -501,24 +442,14 @@
     },
     total=False,
 )
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
-CreateReportPlanOutputTypeDef = TypedDict(
-    "CreateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DateRangeOutputTypeDef = TypedDict(
     "DateRangeOutputTypeDef",
     {
         "FromDate": datetime,
         "ToDate": datetime,
     },
 )
@@ -534,25 +465,14 @@
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-DeleteBackupPlanOutputTypeDef = TypedDict(
-    "DeleteBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "DeletionDate": datetime,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBackupSelectionInputRequestTypeDef = TypedDict(
     "DeleteBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "SelectionId": str,
     },
 )
@@ -617,89 +537,43 @@
 DescribeBackupVaultInputRequestTypeDef = TypedDict(
     "DescribeBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-DescribeBackupVaultOutputTypeDef = TypedDict(
-    "DescribeBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "EncryptionKeyArn": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "NumberOfRecoveryPoints": int,
-        "Locked": bool,
-        "MinRetentionDays": int,
-        "MaxRetentionDays": int,
-        "LockDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCopyJobInputRequestTypeDef = TypedDict(
     "DescribeCopyJobInputRequestTypeDef",
     {
         "CopyJobId": str,
     },
 )
 
 DescribeFrameworkInputRequestTypeDef = TypedDict(
     "DescribeFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 
-DescribeGlobalSettingsOutputTypeDef = TypedDict(
-    "DescribeGlobalSettingsOutputTypeDef",
-    {
-        "GlobalSettings": Dict[str, str],
-        "LastUpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProtectedResourceInputRequestTypeDef = TypedDict(
     "DescribeProtectedResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeProtectedResourceOutputTypeDef = TypedDict(
-    "DescribeProtectedResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceType": str,
-        "LastBackupTime": datetime,
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRecoveryPointInputRequestTypeDef = TypedDict(
     "DescribeRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-DescribeRegionSettingsOutputTypeDef = TypedDict(
-    "DescribeRegionSettingsOutputTypeDef",
-    {
-        "ResourceTypeOptInPreference": Dict[str, bool],
-        "ResourceTypeManagementPreference": Dict[str, bool],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeReportJobInputRequestTypeDef = TypedDict(
     "DescribeReportJobInputRequestTypeDef",
     {
         "ReportJobId": str,
     },
 )
 
@@ -713,34 +587,14 @@
 DescribeRestoreJobInputRequestTypeDef = TypedDict(
     "DescribeRestoreJobInputRequestTypeDef",
     {
         "RestoreJobId": str,
     },
 )
 
-DescribeRestoreJobOutputTypeDef = TypedDict(
-    "DescribeRestoreJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "RestoreJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "Status": RestoreJobStatusType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "ExpectedCompletionTimeMinutes": int,
-        "CreatedResourceArn": str,
-        "ResourceType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateRecoveryPointFromParentInputRequestTypeDef = TypedDict(
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
@@ -749,36 +603,21 @@
     "DisassociateRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportBackupPlanTemplateInputRequestTypeDef = TypedDict(
     "ExportBackupPlanTemplateInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-ExportBackupPlanTemplateOutputTypeDef = TypedDict(
-    "ExportBackupPlanTemplateOutputTypeDef",
-    {
-        "BackupPlanTemplateJson": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FrameworkTypeDef = TypedDict(
     "FrameworkTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "NumberOfControls": int,
@@ -832,42 +671,21 @@
 GetBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBackupVaultNotificationsInputRequestTypeDef = TypedDict(
     "GetBackupVaultNotificationsInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultNotificationsOutputTypeDef = TypedDict(
-    "GetBackupVaultNotificationsOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "SNSTopicArn": str,
-        "BackupVaultEvents": List[BackupVaultEventType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLegalHoldInputRequestTypeDef = TypedDict(
     "GetLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 
@@ -875,60 +693,34 @@
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    {
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "RestoreMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSupportedResourceTypesOutputTypeDef = TypedDict(
-    "GetSupportedResourceTypesOutputTypeDef",
-    {
-        "ResourceTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LegalHoldTypeDef = TypedDict(
     "LegalHoldTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
     },
     total=False,
 )
 
-ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBackupJobsInputRequestTypeDef = TypedDict(
     "ListBackupJobsInputRequestTypeDef",
     {
@@ -944,51 +736,23 @@
         "ByCompleteAfter": Union[datetime, str],
         "ByCompleteBefore": Union[datetime, str],
         "ByParentJobId": str,
     },
     total=False,
 )
 
-ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
-    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListBackupPlanVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupPlanVersionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupPlanVersionsInputRequestTypeDef = TypedDict(
@@ -1002,53 +766,24 @@
 
 class ListBackupPlanVersionsInputRequestTypeDef(
     _RequiredListBackupPlanVersionsInputRequestTypeDef,
     _OptionalListBackupPlanVersionsInputRequestTypeDef,
 ):
     pass
 
-ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    {
-        "IncludeDeleted": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupPlansInputRequestTypeDef = TypedDict(
     "ListBackupPlansInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IncludeDeleted": bool,
     },
     total=False,
 )
 
-_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
-    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListBackupSelectionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupSelectionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupSelectionsInputRequestTypeDef = TypedDict(
@@ -1062,49 +797,23 @@
 
 class ListBackupSelectionsInputRequestTypeDef(
     _RequiredListBackupSelectionsInputRequestTypeDef,
     _OptionalListBackupSelectionsInputRequestTypeDef,
 ):
     pass
 
-ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupVaultsInputRequestTypeDef = TypedDict(
     "ListBackupVaultsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCopyJobsInputRequestTypeDef = TypedDict(
     "ListCopyJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByResourceArn": str,
         "ByState": CopyJobStateType,
@@ -1125,39 +834,23 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLegalHoldsInputRequestTypeDef = TypedDict(
     "ListLegalHoldsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProtectedResourcesInputRequestTypeDef = TypedDict(
     "ListProtectedResourcesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1170,40 +863,14 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-):
-    pass
-
 _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
@@ -1223,34 +890,14 @@
 
 class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
     _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
     _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
 ):
     pass
 
-_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "LegalHoldId": str,
-    },
-)
-_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
-    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-):
-    pass
-
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -1275,34 +922,14 @@
         "ResourceArn": str,
         "ResourceType": str,
         "BackupVaultName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
-    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
@@ -1355,28 +982,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    {
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRestoreJobsInputRequestTypeDef = TypedDict(
     "ListRestoreJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByAccountId": str,
         "ByCreatedBefore": Union[datetime, str],
@@ -1424,33 +1037,14 @@
 )
 
 class ListTagsInputRequestTypeDef(
     _RequiredListTagsInputRequestTypeDef, _OptionalListTagsInputRequestTypeDef
 ):
     pass
 
-ListTagsOutputTypeDef = TypedDict(
-    "ListTagsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -1546,46 +1140,14 @@
 )
 
 class ReportSettingOutputTypeDef(
     _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
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
-StartBackupJobOutputTypeDef = TypedDict(
-    "StartBackupJobOutputTypeDef",
-    {
-        "BackupJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartCopyJobOutputTypeDef = TypedDict(
-    "StartCopyJobOutputTypeDef",
-    {
-        "CopyJobId": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1597,22 +1159,14 @@
 )
 
 class StartReportJobInputRequestTypeDef(
     _RequiredStartReportJobInputRequestTypeDef, _OptionalStartReportJobInputRequestTypeDef
 ):
     pass
 
-StartReportJobOutputTypeDef = TypedDict(
-    "StartReportJobOutputTypeDef",
-    {
-        "ReportJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRestoreJobInputRequestTypeDef = TypedDict(
     "_RequiredStartRestoreJobInputRequestTypeDef",
     {
         "RecoveryPointArn": str,
         "Metadata": Mapping[str, str],
     },
 )
@@ -1628,22 +1182,14 @@
 )
 
 class StartRestoreJobInputRequestTypeDef(
     _RequiredStartRestoreJobInputRequestTypeDef, _OptionalStartRestoreJobInputRequestTypeDef
 ):
     pass
 
-StartRestoreJobOutputTypeDef = TypedDict(
-    "StartRestoreJobOutputTypeDef",
-    {
-        "RestoreJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopBackupJobInputRequestTypeDef = TypedDict(
     "StopBackupJobInputRequestTypeDef",
     {
         "BackupJobId": str,
     },
 )
 
@@ -1659,24 +1205,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeyList": Sequence[str],
     },
 )
 
-UpdateFrameworkOutputTypeDef = TypedDict(
-    "UpdateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "GlobalSettings": Mapping[str, str],
     },
     total=False,
 )
@@ -1686,24 +1222,14 @@
     {
         "ResourceTypeOptInPreference": Mapping[str, bool],
         "ResourceTypeManagementPreference": Mapping[str, bool],
     },
     total=False,
 )
 
-UpdateReportPlanOutputTypeDef = TypedDict(
-    "UpdateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupPlansListMemberTypeDef = TypedDict(
     "BackupPlansListMemberTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
@@ -1712,38 +1238,14 @@
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
-CreateBackupPlanOutputTypeDef = TypedDict(
-    "CreateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBackupPlanOutputTypeDef = TypedDict(
-    "UpdateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
         "AccountId": str,
         "BackupJobId": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
@@ -1794,55 +1296,14 @@
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
         "ResourceName": str,
     },
     total=False,
 )
 
-DescribeBackupJobOutputTypeDef = TypedDict(
-    "DescribeBackupJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "BackupJobId": str,
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "State": BackupJobStateType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "ResourceType": str,
-        "BytesTransferred": int,
-        "ExpectedCompletionDate": datetime,
-        "StartBy": datetime,
-        "BackupOptions": Dict[str, str],
-        "BackupType": str,
-        "ParentJobId": str,
-        "IsParent": bool,
-        "NumberOfChildJobs": int,
-        "ChildJobsInState": Dict[BackupJobStateType, int],
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupPlanTemplatesOutputTypeDef = TypedDict(
-    "ListBackupPlanTemplatesOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
         "DestinationBackupVaultArn": str,
     },
 )
 _OptionalCopyActionTypeDef = TypedDict(
@@ -1922,81 +1383,236 @@
 
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
-_RequiredCopyActionOutputTypeDef = TypedDict(
-    "_RequiredCopyActionOutputTypeDef",
+RecoveryPointByBackupVaultTypeDef = TypedDict(
+    "RecoveryPointByBackupVaultTypeDef",
     {
-        "DestinationBackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SourceBackupVaultArn": str,
+        "ResourceArn": str,
+        "ResourceType": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "IamRoleArn": str,
+        "Status": RecoveryPointStatusType,
+        "StatusMessage": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "BackupSizeInBytes": int,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "Lifecycle": LifecycleTypeDef,
+        "EncryptionKeyArn": str,
+        "IsEncrypted": bool,
+        "LastRestoreTime": datetime,
+        "ParentRecoveryPointArn": str,
+        "CompositeMemberIdentifier": str,
+        "IsParent": bool,
+        "ResourceName": str,
     },
+    total=False,
 )
-_OptionalCopyActionOutputTypeDef = TypedDict(
-    "_OptionalCopyActionOutputTypeDef",
+
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
     {
-        "Lifecycle": LifecycleOutputTypeDef,
+        "StringEquals": List[ConditionParameterTypeDef],
+        "StringNotEquals": List[ConditionParameterTypeDef],
+        "StringLike": List[ConditionParameterTypeDef],
+        "StringNotLike": List[ConditionParameterTypeDef],
     },
     total=False,
 )
 
-class CopyActionOutputTypeDef(_RequiredCopyActionOutputTypeDef, _OptionalCopyActionOutputTypeDef):
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
+    {
+        "StringEquals": Sequence[ConditionParameterTypeDef],
+        "StringNotEquals": Sequence[ConditionParameterTypeDef],
+        "StringLike": Sequence[ConditionParameterTypeDef],
+        "StringNotLike": Sequence[ConditionParameterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredFrameworkControlOutputTypeDef = TypedDict(
+    "_RequiredFrameworkControlOutputTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlOutputTypeDef = TypedDict(
+    "_OptionalFrameworkControlOutputTypeDef",
+    {
+        "ControlInputParameters": List[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeOutputTypeDef,
+    },
+    total=False,
+)
+
+class FrameworkControlOutputTypeDef(
+    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
+):
     pass
 
-ListBackupSelectionsOutputTypeDef = TypedDict(
-    "ListBackupSelectionsOutputTypeDef",
+_RequiredFrameworkControlTypeDef = TypedDict(
+    "_RequiredFrameworkControlTypeDef",
     {
-        "NextToken": str,
-        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ControlName": str,
     },
 )
+_OptionalFrameworkControlTypeDef = TypedDict(
+    "_OptionalFrameworkControlTypeDef",
+    {
+        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeTypeDef,
+    },
+    total=False,
+)
 
-ListBackupVaultsOutputTypeDef = TypedDict(
-    "ListBackupVaultsOutputTypeDef",
+class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
+    pass
+
+CreateBackupPlanOutputTypeDef = TypedDict(
+    "CreateBackupPlanOutputTypeDef",
     {
-        "BackupVaultList": List[BackupVaultListMemberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRecoveryPointOutputTypeDef = TypedDict(
-    "DescribeRecoveryPointOutputTypeDef",
+CreateBackupSelectionOutputTypeDef = TypedDict(
+    "CreateBackupSelectionOutputTypeDef",
+    {
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBackupVaultOutputTypeDef = TypedDict(
+    "CreateBackupVaultOutputTypeDef",
     {
-        "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
-        "SourceBackupVaultArn": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFrameworkOutputTypeDef = TypedDict(
+    "CreateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateReportPlanOutputTypeDef = TypedDict(
+    "CreateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupPlanOutputTypeDef = TypedDict(
+    "DeleteBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "DeletionDate": datetime,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupJobOutputTypeDef = TypedDict(
+    "DescribeBackupJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "BackupJobId": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
         "ResourceArn": str,
-        "ResourceType": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "IamRoleArn": str,
-        "Status": RecoveryPointStatusType,
-        "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
+        "State": BackupJobStateType,
+        "StatusMessage": str,
+        "PercentDone": str,
         "BackupSizeInBytes": int,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleOutputTypeDef,
-        "EncryptionKeyArn": str,
-        "IsEncrypted": bool,
-        "StorageClass": StorageClassType,
-        "LastRestoreTime": datetime,
-        "ParentRecoveryPointArn": str,
-        "CompositeMemberIdentifier": str,
+        "IamRoleArn": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "ResourceType": str,
+        "BytesTransferred": int,
+        "ExpectedCompletionDate": datetime,
+        "StartBy": datetime,
+        "BackupOptions": Dict[str, str],
+        "BackupType": str,
+        "ParentJobId": str,
         "IsParent": bool,
+        "NumberOfChildJobs": int,
+        "ChildJobsInState": Dict[BackupJobStateType, int],
         "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecoveryPointByBackupVaultTypeDef = TypedDict(
-    "RecoveryPointByBackupVaultTypeDef",
+DescribeBackupVaultOutputTypeDef = TypedDict(
+    "DescribeBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "EncryptionKeyArn": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "NumberOfRecoveryPoints": int,
+        "Locked": bool,
+        "MinRetentionDays": int,
+        "MaxRetentionDays": int,
+        "LockDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGlobalSettingsOutputTypeDef = TypedDict(
+    "DescribeGlobalSettingsOutputTypeDef",
+    {
+        "GlobalSettings": Dict[str, str],
+        "LastUpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProtectedResourceOutputTypeDef = TypedDict(
+    "DescribeProtectedResourceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceType": str,
+        "LastBackupTime": datetime,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRecoveryPointOutputTypeDef = TypedDict(
+    "DescribeRecoveryPointOutputTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -2004,96 +1620,225 @@
         "IamRoleArn": str,
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleOutputTypeDef,
+        "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
+        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
+DescribeRegionSettingsOutputTypeDef = TypedDict(
+    "DescribeRegionSettingsOutputTypeDef",
+    {
+        "ResourceTypeOptInPreference": Dict[str, bool],
+        "ResourceTypeManagementPreference": Dict[str, bool],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRestoreJobOutputTypeDef = TypedDict(
+    "DescribeRestoreJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "RestoreJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "Status": RestoreJobStatusType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "ExpectedCompletionTimeMinutes": int,
+        "CreatedResourceArn": str,
+        "ResourceType": str,
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
+ExportBackupPlanTemplateOutputTypeDef = TypedDict(
+    "ExportBackupPlanTemplateOutputTypeDef",
+    {
+        "BackupPlanTemplateJson": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultNotificationsOutputTypeDef = TypedDict(
+    "GetBackupVaultNotificationsOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SNSTopicArn": str,
+        "BackupVaultEvents": List[BackupVaultEventType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "Lifecycle": LifecycleOutputTypeDef,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RestoreMetadata": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionsOutputTypeDef = TypedDict(
-    "ConditionsOutputTypeDef",
+GetSupportedResourceTypesOutputTypeDef = TypedDict(
+    "GetSupportedResourceTypesOutputTypeDef",
     {
-        "StringEquals": List[ConditionParameterOutputTypeDef],
-        "StringNotEquals": List[ConditionParameterOutputTypeDef],
-        "StringLike": List[ConditionParameterOutputTypeDef],
-        "StringNotLike": List[ConditionParameterOutputTypeDef],
+        "ResourceTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ConditionsTypeDef = TypedDict(
-    "ConditionsTypeDef",
+ListBackupPlanTemplatesOutputTypeDef = TypedDict(
+    "ListBackupPlanTemplatesOutputTypeDef",
     {
-        "StringEquals": Sequence[ConditionParameterTypeDef],
-        "StringNotEquals": Sequence[ConditionParameterTypeDef],
-        "StringLike": Sequence[ConditionParameterTypeDef],
-        "StringNotLike": Sequence[ConditionParameterTypeDef],
+        "NextToken": str,
+        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredFrameworkControlOutputTypeDef = TypedDict(
-    "_RequiredFrameworkControlOutputTypeDef",
+ListBackupSelectionsOutputTypeDef = TypedDict(
+    "ListBackupSelectionsOutputTypeDef",
     {
-        "ControlName": str,
+        "NextToken": str,
+        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFrameworkControlOutputTypeDef = TypedDict(
-    "_OptionalFrameworkControlOutputTypeDef",
+
+ListBackupVaultsOutputTypeDef = TypedDict(
+    "ListBackupVaultsOutputTypeDef",
     {
-        "ControlInputParameters": List[ControlInputParameterOutputTypeDef],
-        "ControlScope": ControlScopeOutputTypeDef,
+        "BackupVaultList": List[BackupVaultListMemberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class FrameworkControlOutputTypeDef(
-    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
-):
-    pass
+ListTagsOutputTypeDef = TypedDict(
+    "ListTagsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredFrameworkControlTypeDef = TypedDict(
-    "_RequiredFrameworkControlTypeDef",
+StartBackupJobOutputTypeDef = TypedDict(
+    "StartBackupJobOutputTypeDef",
     {
-        "ControlName": str,
+        "BackupJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFrameworkControlTypeDef = TypedDict(
-    "_OptionalFrameworkControlTypeDef",
+
+StartCopyJobOutputTypeDef = TypedDict(
+    "StartCopyJobOutputTypeDef",
     {
-        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeTypeDef,
+        "CopyJobId": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
-    pass
+StartReportJobOutputTypeDef = TypedDict(
+    "StartReportJobOutputTypeDef",
+    {
+        "ReportJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRestoreJobOutputTypeDef = TypedDict(
+    "StartRestoreJobOutputTypeDef",
+    {
+        "RestoreJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBackupPlanOutputTypeDef = TypedDict(
+    "UpdateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFrameworkOutputTypeDef = TypedDict(
+    "UpdateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "Lifecycle": LifecycleTypeDef,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateReportPlanOutputTypeDef = TypedDict(
+    "UpdateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
         "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
         "ReportSetting": ReportSettingTypeDef,
@@ -2157,60 +1902,257 @@
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
         "Frameworks": List[FrameworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLegalHoldsOutputTypeDef = TypedDict(
     "ListLegalHoldsOutputTypeDef",
     {
         "NextToken": str,
         "LegalHolds": List[LegalHoldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
+    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+):
+    pass
+
+ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    {
+        "IncludeDeleted": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
+    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+):
+    pass
+
+ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByParentRecoveryPointArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+):
+    pass
+
+_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "LegalHoldId": str,
+    },
+)
+_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
+    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+):
+    pass
+
+_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
+    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+):
+    pass
+
+ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
+    {
+        "ByAccountId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
     {
         "Results": List[ProtectedResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByLegalHoldOutputTypeDef = TypedDict(
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     {
         "RecoveryPoints": List[RecoveryPointMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByResourceOutputTypeDef = TypedDict(
     "ListRecoveryPointsByResourceOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRestoreJobsOutputTypeDef = TypedDict(
     "ListRestoreJobsOutputTypeDef",
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
@@ -2242,50 +2184,50 @@
 )
 
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupPlansOutputTypeDef = TypedDict(
     "ListBackupPlansOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlansList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupJobsOutputTypeDef = TypedDict(
     "ListBackupJobsOutputTypeDef",
     {
         "BackupJobs": List[BackupJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCopyJobOutputTypeDef = TypedDict(
     "DescribeCopyJobOutputTypeDef",
     {
         "CopyJob": CopyJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCopyJobsOutputTypeDef = TypedDict(
     "ListCopyJobsOutputTypeDef",
     {
         "CopyJobs": List[CopyJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupRuleInputTypeDef = TypedDict(
     "_RequiredBackupRuleInputTypeDef",
     {
         "RuleName": str,
@@ -2318,47 +2260,47 @@
 )
 _OptionalBackupRuleTypeDef = TypedDict(
     "_OptionalBackupRuleTypeDef",
     {
         "ScheduleExpression": str,
         "StartWindowMinutes": int,
         "CompletionWindowMinutes": int,
-        "Lifecycle": LifecycleOutputTypeDef,
+        "Lifecycle": LifecycleTypeDef,
         "RecoveryPointTags": Dict[str, str],
         "RuleId": str,
-        "CopyActions": List[CopyActionOutputTypeDef],
+        "CopyActions": List[CopyActionTypeDef],
         "EnableContinuousBackup": bool,
     },
     total=False,
 )
 
 class BackupRuleTypeDef(_RequiredBackupRuleTypeDef, _OptionalBackupRuleTypeDef):
     pass
 
 ListRecoveryPointsByBackupVaultOutputTypeDef = TypedDict(
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupSelectionOutputTypeDef = TypedDict(
     "_RequiredBackupSelectionOutputTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
 _OptionalBackupSelectionOutputTypeDef = TypedDict(
     "_OptionalBackupSelectionOutputTypeDef",
     {
         "Resources": List[str],
-        "ListOfTags": List[ConditionOutputTypeDef],
+        "ListOfTags": List[ConditionTypeDef],
         "NotResources": List[str],
         "Conditions": ConditionsOutputTypeDef,
     },
     total=False,
 )
 
 class BackupSelectionOutputTypeDef(
@@ -2394,15 +2336,15 @@
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "FrameworkControls": List[FrameworkControlOutputTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
@@ -2451,15 +2393,15 @@
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLegalHoldOutputTypeDef = TypedDict(
     "GetLegalHoldOutputTypeDef",
     {
         "Title": str,
@@ -2468,15 +2410,15 @@
         "CancelDescription": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
         "Title": str,
@@ -2498,41 +2440,41 @@
 ):
     pass
 
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReportJobsOutputTypeDef = TypedDict(
     "ListReportJobsOutputTypeDef",
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReportPlanOutputTypeDef = TypedDict(
     "DescribeReportPlanOutputTypeDef",
     {
         "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReportPlansOutputTypeDef = TypedDict(
     "ListReportPlansOutputTypeDef",
     {
         "ReportPlans": List[ReportPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
@@ -2572,15 +2514,15 @@
     "GetBackupSelectionOutputTypeDef",
     {
         "BackupSelection": BackupSelectionOutputTypeDef,
         "SelectionId": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "CreatorRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
@@ -2629,23 +2571,23 @@
     },
 )
 
 GetBackupPlanFromJSONOutputTypeDef = TypedDict(
     "GetBackupPlanFromJSONOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanFromTemplateOutputTypeDef = TypedDict(
     "GetBackupPlanFromTemplateOutputTypeDef",
     {
         "BackupPlanDocument": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanOutputTypeDef = TypedDict(
     "GetBackupPlanOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
@@ -2653,10 +2595,10 @@
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/PKG-INFO` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.12
-Summary: Type annotations for boto3.Backup 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -383,162 +383,157 @@
 ```python
 from mypy_boto3_backup.type_defs import (
     AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
-    LifecycleOutputTypeDef,
-    ConditionOutputTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
-    ConditionParameterOutputTypeDef,
     ConditionParameterTypeDef,
-    ControlInputParameterOutputTypeDef,
     ControlInputParameterTypeDef,
     ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
-    CreateBackupSelectionOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
-    CreateReportPlanOutputTypeDef,
     DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
-    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
-    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
-    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupJobsInputRequestTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
     ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
     ListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
     ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
-    ListTagsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
     ReportSettingOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
-    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
-    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
-    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    CopyActionOutputTypeDef,
-    ListBackupSelectionsOutputTypeDef,
-    ListBackupVaultsOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
-    UpdateRecoveryPointLifecycleOutputTypeDef,
     ConditionsOutputTypeDef,
     ConditionsTypeDef,
     FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    CreateBackupSelectionOutputTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
+    CreateReportPlanOutputTypeDef,
+    DeleteBackupPlanOutputTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    DescribeBackupVaultOutputTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
+    DescribeRestoreJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
+    ListBackupSelectionsOutputTypeDef,
+    ListBackupVaultsOutputTypeDef,
+    ListTagsOutputTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
+    StartReportJobOutputTypeDef,
+    StartRestoreJobOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
+    UpdateFrameworkOutputTypeDef,
+    UpdateRecoveryPointLifecycleOutputTypeDef,
+    UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
     ReportPlanTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
```

### Comparing `mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/SOURCES.txt` & `mypy-boto3-backup-1.28.15/mypy_boto3_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.12/setup.py` & `mypy-boto3-backup-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Backup 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

