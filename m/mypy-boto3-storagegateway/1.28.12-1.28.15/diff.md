# Comparing `tmp/mypy-boto3-storagegateway-1.28.12.tar.gz` & `tmp/mypy-boto3-storagegateway-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-storagegateway-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
+gzip compressed data, was "mypy-boto3-storagegateway-1.28.15.tar", last modified: Fri Jul 28 20:43:50 2023, max compression
```

## Comparing `mypy-boto3-storagegateway-1.28.12.tar` & `mypy-boto3-storagegateway-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24276 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22761 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68220 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68112 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-27 11:47:45.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-07-27 11:47:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-07-27 11:47:46.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79123 2023-07-27 11:47:45.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:42.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24276 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:44.000000 mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.277352 mypy-boto3-storagegateway-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:47:41.000000 mypy-boto3-storagegateway-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68220 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68112 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-07-28 20:40:19.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    77916 2023-07-28 20:40:22.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77837 2023-07-28 20:40:21.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:50.000000 mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:50.521957 mypy-boto3-storagegateway-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:40:18.000000 mypy-boto3-storagegateway-1.28.15/setup.py
```

### Comparing `mypy-boto3-storagegateway-1.28.12/LICENSE` & `mypy-boto3-storagegateway-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/PKG-INFO` & `mypy-boto3-storagegateway-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.12
-Summary: Type annotations for boto3.StorageGateway 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,19 +382,17 @@
     AddCacheInputRequestTypeDef,
     AddUploadBufferInputRequestTypeDef,
     AddWorkingStorageInputRequestTypeDef,
     AssignTapePoolInputRequestTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AutomaticTapeCreationRuleOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
     BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
-    CacheAttributesOutputTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
     CancelRetrievalInputRequestTypeDef,
     ChapInfoTypeDef,
     NFSFileShareDefaultsTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
@@ -411,15 +409,14 @@
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
-    TagOutputTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
     SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
@@ -455,15 +452,14 @@
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
-    NFSFileShareDefaultsOutputTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
     RefreshCacheInputRequestTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
     ResetCacheInputRequestTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
     SMBLocalGroupsTypeDef,
@@ -519,20 +515,22 @@
     DeleteTapeOutputTypeDef,
     DeleteTapePoolOutputTypeDef,
     DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitOutputTypeDef,
     DescribeCacheOutputTypeDef,
     DescribeMaintenanceStartTimeOutputTypeDef,
+    DescribeSnapshotScheduleOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
     JoinDomainOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListVolumeInitiatorsOutputTypeDef,
     NotifyWhenUploadedOutputTypeDef,
     RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
@@ -553,30 +551,29 @@
     UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityOutputTypeDef,
     UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyOutputTypeDef,
     UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
+    SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
     UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
+    NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
-    DescribeSnapshotScheduleOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    SMBFileShareInfoTypeDef,
     DescribeSMBSettingsOutputTypeDef,
     DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
     DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
@@ -594,23 +591,22 @@
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
-    NFSFileShareInfoTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
-    DescribeSMBFileSharesOutputTypeDef,
+    DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
-    DescribeNFSFileSharesOutputTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-storagegateway-1.28.12/README.md` & `mypy-boto3-storagegateway-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,19 +350,17 @@
     AddCacheInputRequestTypeDef,
     AddUploadBufferInputRequestTypeDef,
     AddWorkingStorageInputRequestTypeDef,
     AssignTapePoolInputRequestTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AutomaticTapeCreationRuleOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
     BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
-    CacheAttributesOutputTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
     CancelRetrievalInputRequestTypeDef,
     ChapInfoTypeDef,
     NFSFileShareDefaultsTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
@@ -379,15 +377,14 @@
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
-    TagOutputTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
     SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
@@ -423,15 +420,14 @@
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
-    NFSFileShareDefaultsOutputTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
     RefreshCacheInputRequestTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
     ResetCacheInputRequestTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
     SMBLocalGroupsTypeDef,
@@ -487,20 +483,22 @@
     DeleteTapeOutputTypeDef,
     DeleteTapePoolOutputTypeDef,
     DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitOutputTypeDef,
     DescribeCacheOutputTypeDef,
     DescribeMaintenanceStartTimeOutputTypeDef,
+    DescribeSnapshotScheduleOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
     JoinDomainOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListVolumeInitiatorsOutputTypeDef,
     NotifyWhenUploadedOutputTypeDef,
     RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
@@ -521,30 +519,29 @@
     UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityOutputTypeDef,
     UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyOutputTypeDef,
     UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
+    SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
     UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
+    NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
-    DescribeSnapshotScheduleOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    SMBFileShareInfoTypeDef,
     DescribeSMBSettingsOutputTypeDef,
     DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
     DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
@@ -562,23 +559,22 @@
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
-    NFSFileShareInfoTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
-    DescribeSMBFileSharesOutputTypeDef,
+    DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
-    DescribeNFSFileSharesOutputTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.py` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__init__.pyi` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/__main__.py` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.StorageGateway 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.StorageGateway 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.py` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/client.pyi` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.py` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/literals.pyi` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.py` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/paginator.pyi` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.py` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,19 +41,17 @@
     "AddCacheInputRequestTypeDef",
     "AddUploadBufferInputRequestTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
     "AssignTapePoolInputRequestTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
     "AttachVolumeInputRequestTypeDef",
-    "AutomaticTapeCreationRuleOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
     "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
-    "CacheAttributesOutputTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
     "CancelRetrievalInputRequestTypeDef",
     "ChapInfoTypeDef",
     "NFSFileShareDefaultsTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
@@ -70,15 +68,14 @@
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
-    "TagOutputTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
     "SMBLocalGroupsOutputTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
@@ -114,15 +111,14 @@
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
-    "NFSFileShareDefaultsOutputTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
     "RefreshCacheInputRequestTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
     "ResetCacheInputRequestTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     "SMBLocalGroupsTypeDef",
@@ -178,20 +174,22 @@
     "DeleteTapeOutputTypeDef",
     "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeCacheOutputTypeDef",
     "DescribeMaintenanceStartTimeOutputTypeDef",
+    "DescribeSnapshotScheduleOutputTypeDef",
     "DescribeUploadBufferOutputTypeDef",
     "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeOutputTypeDef",
     "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemOutputTypeDef",
     "JoinDomainOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListVolumeInitiatorsOutputTypeDef",
     "NotifyWhenUploadedOutputTypeDef",
     "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheOutputTypeDef",
     "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointOutputTypeDef",
@@ -212,30 +210,29 @@
     "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityOutputTypeDef",
     "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyOutputTypeDef",
     "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeOutputTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
+    "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
+    "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
-    "DescribeSnapshotScheduleOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "SMBFileShareInfoTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
@@ -253,23 +250,22 @@
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "NFSFileShareInfoTypeDef",
     "UpdateSMBLocalGroupsInputRequestTypeDef",
+    "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
-    "DescribeSMBFileSharesOutputTypeDef",
+    "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
-    "DescribeNFSFileSharesOutputTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -369,38 +365,14 @@
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
 
-_RequiredAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
-    "_RequiredAutomaticTapeCreationRuleOutputTypeDef",
-    {
-        "TapeBarcodePrefix": str,
-        "PoolId": str,
-        "TapeSizeInBytes": int,
-        "MinimumNumTapes": int,
-    },
-)
-_OptionalAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
-    "_OptionalAutomaticTapeCreationRuleOutputTypeDef",
-    {
-        "Worm": bool,
-    },
-    total=False,
-)
-
-
-class AutomaticTapeCreationRuleOutputTypeDef(
-    _RequiredAutomaticTapeCreationRuleOutputTypeDef, _OptionalAutomaticTapeCreationRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
@@ -470,22 +442,14 @@
 
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
 
-CacheAttributesOutputTypeDef = TypedDict(
-    "CacheAttributesOutputTypeDef",
-    {
-        "CacheStaleTimeoutInSeconds": int,
-    },
-    total=False,
-)
-
 VolumeiSCSIAttributesTypeDef = TypedDict(
     "VolumeiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "LunNumber": int,
@@ -709,22 +673,14 @@
         "Ipv4Address": str,
         "MacAddress": str,
         "Ipv6Address": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1241,25 +1197,14 @@
         "VolumeType": str,
         "VolumeSizeInBytes": int,
         "VolumeAttachmentStatus": str,
     },
     total=False,
 )
 
-NFSFileShareDefaultsOutputTypeDef = TypedDict(
-    "NFSFileShareDefaultsOutputTypeDef",
-    {
-        "FileMode": str,
-        "DirectoryMode": str,
-        "GroupId": int,
-        "OwnerId": int,
-    },
-    total=False,
-)
-
 NotifyWhenUploadedInputRequestTypeDef = TypedDict(
     "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 
@@ -2017,14 +1962,27 @@
         "DayOfWeek": int,
         "DayOfMonth": int,
         "Timezone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeSnapshotScheduleOutputTypeDef = TypedDict(
+    "DescribeSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "StartAt": int,
+        "RecurrenceInHours": int,
+        "Description": str,
+        "Timezone": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeUploadBufferOutputTypeDef = TypedDict(
     "DescribeUploadBufferOutputTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": List[str],
         "UploadBufferUsedInBytes": int,
         "UploadBufferAllocatedInBytes": int,
@@ -2072,14 +2030,24 @@
     {
         "GatewayARN": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Marker": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListVolumeInitiatorsOutputTypeDef = TypedDict(
     "ListVolumeInitiatorsOutputTypeDef",
     {
         "Initiators": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2337,14 +2305,50 @@
 
 class CreateSMBFileShareInputRequestTypeDef(
     _RequiredCreateSMBFileShareInputRequestTypeDef, _OptionalCreateSMBFileShareInputRequestTypeDef
 ):
     pass
 
 
+SMBFileShareInfoTypeDef = TypedDict(
+    "SMBFileShareInfoTypeDef",
+    {
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "SMBACLEnabled": bool,
+        "AccessBasedEnumeration": bool,
+        "AdminUserList": List[str],
+        "ValidUserList": List[str],
+        "InvalidUserList": List[str],
+        "AuditDestinationARN": str,
+        "Authentication": str,
+        "CaseSensitivity": CaseSensitivityType,
+        "Tags": List[TagTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "OplocksEnabled": bool,
+    },
+    total=False,
+)
+
 _RequiredUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemAssociationInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
@@ -2431,15 +2435,15 @@
 ):
     pass
 
 
 AutomaticTapeCreationPolicyInfoTypeDef = TypedDict(
     "AutomaticTapeCreationPolicyInfoTypeDef",
     {
-        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleOutputTypeDef],
+        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleTypeDef],
         "GatewayARN": str,
     },
     total=False,
 )
 
 UpdateAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -2552,14 +2556,45 @@
 
 class CreateNFSFileShareInputRequestTypeDef(
     _RequiredCreateNFSFileShareInputRequestTypeDef, _OptionalCreateNFSFileShareInputRequestTypeDef
 ):
     pass
 
 
+NFSFileShareInfoTypeDef = TypedDict(
+    "NFSFileShareInfoTypeDef",
+    {
+        "NFSFileShareDefaults": NFSFileShareDefaultsTypeDef,
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ClientList": List[str],
+        "Squash": str,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "Tags": List[TagTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "AuditDestinationARN": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNFSFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalUpdateNFSFileShareInputRequestTypeDef = TypedDict(
@@ -2600,87 +2635,28 @@
         "GatewayState": str,
         "GatewayNetworkInterfaces": List[NetworkInterfaceTypeDef],
         "GatewayType": str,
         "NextUpdateAvailabilityDate": str,
         "LastSoftwareUpdate": str,
         "Ec2InstanceId": str,
         "Ec2InstanceRegion": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "VPCEndpoint": str,
         "CloudWatchLogGroupARN": str,
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSnapshotScheduleOutputTypeDef = TypedDict(
-    "DescribeSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
-        "Description": str,
-        "Timezone": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "Marker": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SMBFileShareInfoTypeDef = TypedDict(
-    "SMBFileShareInfoTypeDef",
-    {
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
-        "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "SMBACLEnabled": bool,
-        "AccessBasedEnumeration": bool,
-        "AdminUserList": List[str],
-        "ValidUserList": List[str],
-        "InvalidUserList": List[str],
-        "AuditDestinationARN": str,
-        "Authentication": str,
-        "CaseSensitivity": CaseSensitivityType,
-        "Tags": List[TagOutputTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesOutputTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "OplocksEnabled": bool,
-    },
-    total=False,
-)
-
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
@@ -2906,16 +2882,16 @@
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
-        "Tags": List[TagOutputTypeDef],
-        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "Tags": List[TagTypeDef],
+        "CacheAttributes": CacheAttributesTypeDef,
         "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
@@ -2970,50 +2946,27 @@
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NFSFileShareInfoTypeDef = TypedDict(
-    "NFSFileShareInfoTypeDef",
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     {
-        "NFSFileShareDefaults": NFSFileShareDefaultsOutputTypeDef,
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
         "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ClientList": List[str],
-        "Squash": str,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "Tags": List[TagOutputTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesOutputTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "AuditDestinationARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
-    total=False,
 )
 
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+DescribeSMBFileSharesOutputTypeDef = TypedDict(
+    "DescribeSMBFileSharesOutputTypeDef",
     {
-        "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
+        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
@@ -3033,18 +2986,18 @@
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSMBFileSharesOutputTypeDef = TypedDict(
-    "DescribeSMBFileSharesOutputTypeDef",
+DescribeNFSFileSharesOutputTypeDef = TypedDict(
+    "DescribeNFSFileSharesOutputTypeDef",
     {
-        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
+        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
@@ -3058,15 +3011,7 @@
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-DescribeNFSFileSharesOutputTypeDef = TypedDict(
-    "DescribeNFSFileSharesOutputTypeDef",
-    {
-        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway/type_defs.pyi` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,17 @@
     "AddCacheInputRequestTypeDef",
     "AddUploadBufferInputRequestTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
     "AssignTapePoolInputRequestTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
     "AttachVolumeInputRequestTypeDef",
-    "AutomaticTapeCreationRuleOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
     "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
-    "CacheAttributesOutputTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
     "CancelRetrievalInputRequestTypeDef",
     "ChapInfoTypeDef",
     "NFSFileShareDefaultsTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
@@ -69,15 +67,14 @@
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
-    "TagOutputTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
     "SMBLocalGroupsOutputTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
@@ -113,15 +110,14 @@
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
-    "NFSFileShareDefaultsOutputTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
     "RefreshCacheInputRequestTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
     "ResetCacheInputRequestTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     "SMBLocalGroupsTypeDef",
@@ -177,20 +173,22 @@
     "DeleteTapeOutputTypeDef",
     "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeCacheOutputTypeDef",
     "DescribeMaintenanceStartTimeOutputTypeDef",
+    "DescribeSnapshotScheduleOutputTypeDef",
     "DescribeUploadBufferOutputTypeDef",
     "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeOutputTypeDef",
     "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemOutputTypeDef",
     "JoinDomainOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListVolumeInitiatorsOutputTypeDef",
     "NotifyWhenUploadedOutputTypeDef",
     "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheOutputTypeDef",
     "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointOutputTypeDef",
@@ -211,30 +209,29 @@
     "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityOutputTypeDef",
     "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyOutputTypeDef",
     "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeOutputTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
+    "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
+    "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
-    "DescribeSnapshotScheduleOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "SMBFileShareInfoTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
@@ -252,23 +249,22 @@
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "NFSFileShareInfoTypeDef",
     "UpdateSMBLocalGroupsInputRequestTypeDef",
+    "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
-    "DescribeSMBFileSharesOutputTypeDef",
+    "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
-    "DescribeNFSFileSharesOutputTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -364,36 +360,14 @@
 )
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
-_RequiredAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
-    "_RequiredAutomaticTapeCreationRuleOutputTypeDef",
-    {
-        "TapeBarcodePrefix": str,
-        "PoolId": str,
-        "TapeSizeInBytes": int,
-        "MinimumNumTapes": int,
-    },
-)
-_OptionalAutomaticTapeCreationRuleOutputTypeDef = TypedDict(
-    "_OptionalAutomaticTapeCreationRuleOutputTypeDef",
-    {
-        "Worm": bool,
-    },
-    total=False,
-)
-
-class AutomaticTapeCreationRuleOutputTypeDef(
-    _RequiredAutomaticTapeCreationRuleOutputTypeDef, _OptionalAutomaticTapeCreationRuleOutputTypeDef
-):
-    pass
-
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
@@ -457,22 +431,14 @@
 )
 
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
-CacheAttributesOutputTypeDef = TypedDict(
-    "CacheAttributesOutputTypeDef",
-    {
-        "CacheStaleTimeoutInSeconds": int,
-    },
-    total=False,
-)
-
 VolumeiSCSIAttributesTypeDef = TypedDict(
     "VolumeiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "LunNumber": int,
@@ -690,22 +656,14 @@
         "Ipv4Address": str,
         "MacAddress": str,
         "Ipv6Address": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1208,25 +1166,14 @@
         "VolumeType": str,
         "VolumeSizeInBytes": int,
         "VolumeAttachmentStatus": str,
     },
     total=False,
 )
 
-NFSFileShareDefaultsOutputTypeDef = TypedDict(
-    "NFSFileShareDefaultsOutputTypeDef",
-    {
-        "FileMode": str,
-        "DirectoryMode": str,
-        "GroupId": int,
-        "OwnerId": int,
-    },
-    total=False,
-)
-
 NotifyWhenUploadedInputRequestTypeDef = TypedDict(
     "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 
@@ -1956,14 +1903,27 @@
         "DayOfWeek": int,
         "DayOfMonth": int,
         "Timezone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeSnapshotScheduleOutputTypeDef = TypedDict(
+    "DescribeSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "StartAt": int,
+        "RecurrenceInHours": int,
+        "Description": str,
+        "Timezone": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeUploadBufferOutputTypeDef = TypedDict(
     "DescribeUploadBufferOutputTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": List[str],
         "UploadBufferUsedInBytes": int,
         "UploadBufferAllocatedInBytes": int,
@@ -2011,14 +1971,24 @@
     {
         "GatewayARN": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Marker": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListVolumeInitiatorsOutputTypeDef = TypedDict(
     "ListVolumeInitiatorsOutputTypeDef",
     {
         "Initiators": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2274,14 +2244,50 @@
 )
 
 class CreateSMBFileShareInputRequestTypeDef(
     _RequiredCreateSMBFileShareInputRequestTypeDef, _OptionalCreateSMBFileShareInputRequestTypeDef
 ):
     pass
 
+SMBFileShareInfoTypeDef = TypedDict(
+    "SMBFileShareInfoTypeDef",
+    {
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "SMBACLEnabled": bool,
+        "AccessBasedEnumeration": bool,
+        "AdminUserList": List[str],
+        "ValidUserList": List[str],
+        "InvalidUserList": List[str],
+        "AuditDestinationARN": str,
+        "Authentication": str,
+        "CaseSensitivity": CaseSensitivityType,
+        "Tags": List[TagTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "OplocksEnabled": bool,
+    },
+    total=False,
+)
+
 _RequiredUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemAssociationInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalUpdateFileSystemAssociationInputRequestTypeDef = TypedDict(
@@ -2362,15 +2368,15 @@
     _RequiredAssociateFileSystemInputRequestTypeDef, _OptionalAssociateFileSystemInputRequestTypeDef
 ):
     pass
 
 AutomaticTapeCreationPolicyInfoTypeDef = TypedDict(
     "AutomaticTapeCreationPolicyInfoTypeDef",
     {
-        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleOutputTypeDef],
+        "AutomaticTapeCreationRules": List[AutomaticTapeCreationRuleTypeDef],
         "GatewayARN": str,
     },
     total=False,
 )
 
 UpdateAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -2481,14 +2487,45 @@
 )
 
 class CreateNFSFileShareInputRequestTypeDef(
     _RequiredCreateNFSFileShareInputRequestTypeDef, _OptionalCreateNFSFileShareInputRequestTypeDef
 ):
     pass
 
+NFSFileShareInfoTypeDef = TypedDict(
+    "NFSFileShareInfoTypeDef",
+    {
+        "NFSFileShareDefaults": NFSFileShareDefaultsTypeDef,
+        "FileShareARN": str,
+        "FileShareId": str,
+        "FileShareStatus": str,
+        "GatewayARN": str,
+        "KMSEncrypted": bool,
+        "KMSKey": str,
+        "Path": str,
+        "Role": str,
+        "LocationARN": str,
+        "DefaultStorageClass": str,
+        "ObjectACL": ObjectACLType,
+        "ClientList": List[str],
+        "Squash": str,
+        "ReadOnly": bool,
+        "GuessMIMETypeEnabled": bool,
+        "RequesterPays": bool,
+        "Tags": List[TagTypeDef],
+        "FileShareName": str,
+        "CacheAttributes": CacheAttributesTypeDef,
+        "NotificationPolicy": str,
+        "VPCEndpointDNSName": str,
+        "BucketRegion": str,
+        "AuditDestinationARN": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdateNFSFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalUpdateNFSFileShareInputRequestTypeDef = TypedDict(
@@ -2527,87 +2564,28 @@
         "GatewayState": str,
         "GatewayNetworkInterfaces": List[NetworkInterfaceTypeDef],
         "GatewayType": str,
         "NextUpdateAvailabilityDate": str,
         "LastSoftwareUpdate": str,
         "Ec2InstanceId": str,
         "Ec2InstanceRegion": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "VPCEndpoint": str,
         "CloudWatchLogGroupARN": str,
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSnapshotScheduleOutputTypeDef = TypedDict(
-    "DescribeSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
-        "Description": str,
-        "Timezone": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "Marker": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SMBFileShareInfoTypeDef = TypedDict(
-    "SMBFileShareInfoTypeDef",
-    {
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
-        "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "SMBACLEnabled": bool,
-        "AccessBasedEnumeration": bool,
-        "AdminUserList": List[str],
-        "ValidUserList": List[str],
-        "InvalidUserList": List[str],
-        "AuditDestinationARN": str,
-        "Authentication": str,
-        "CaseSensitivity": CaseSensitivityType,
-        "Tags": List[TagOutputTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesOutputTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "OplocksEnabled": bool,
-    },
-    total=False,
-)
-
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
@@ -2825,16 +2803,16 @@
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
-        "Tags": List[TagOutputTypeDef],
-        "CacheAttributes": CacheAttributesOutputTypeDef,
+        "Tags": List[TagTypeDef],
+        "CacheAttributes": CacheAttributesTypeDef,
         "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
@@ -2889,50 +2867,27 @@
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NFSFileShareInfoTypeDef = TypedDict(
-    "NFSFileShareInfoTypeDef",
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     {
-        "NFSFileShareDefaults": NFSFileShareDefaultsOutputTypeDef,
-        "FileShareARN": str,
-        "FileShareId": str,
-        "FileShareStatus": str,
         "GatewayARN": str,
-        "KMSEncrypted": bool,
-        "KMSKey": str,
-        "Path": str,
-        "Role": str,
-        "LocationARN": str,
-        "DefaultStorageClass": str,
-        "ObjectACL": ObjectACLType,
-        "ClientList": List[str],
-        "Squash": str,
-        "ReadOnly": bool,
-        "GuessMIMETypeEnabled": bool,
-        "RequesterPays": bool,
-        "Tags": List[TagOutputTypeDef],
-        "FileShareName": str,
-        "CacheAttributes": CacheAttributesOutputTypeDef,
-        "NotificationPolicy": str,
-        "VPCEndpointDNSName": str,
-        "BucketRegion": str,
-        "AuditDestinationARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
-    total=False,
 )
 
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+DescribeSMBFileSharesOutputTypeDef = TypedDict(
+    "DescribeSMBFileSharesOutputTypeDef",
     {
-        "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
+        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
@@ -2952,18 +2907,18 @@
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSMBFileSharesOutputTypeDef = TypedDict(
-    "DescribeSMBFileSharesOutputTypeDef",
+DescribeNFSFileSharesOutputTypeDef = TypedDict(
+    "DescribeNFSFileSharesOutputTypeDef",
     {
-        "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
+        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
@@ -2977,15 +2932,7 @@
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-DescribeNFSFileSharesOutputTypeDef = TypedDict(
-    "DescribeNFSFileSharesOutputTypeDef",
-    {
-        "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/PKG-INFO` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.28.12
-Summary: Type annotations for boto3.StorageGateway 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.StorageGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-storagegateway)](https://pepy.tech/project/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,19 +382,17 @@
     AddCacheInputRequestTypeDef,
     AddUploadBufferInputRequestTypeDef,
     AddWorkingStorageInputRequestTypeDef,
     AssignTapePoolInputRequestTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AutomaticTapeCreationRuleOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
     BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
-    CacheAttributesOutputTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
     CancelRetrievalInputRequestTypeDef,
     ChapInfoTypeDef,
     NFSFileShareDefaultsTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
@@ -411,15 +409,14 @@
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
-    TagOutputTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
     SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
@@ -455,15 +452,14 @@
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
-    NFSFileShareDefaultsOutputTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
     RefreshCacheInputRequestTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
     ResetCacheInputRequestTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
     SMBLocalGroupsTypeDef,
@@ -519,20 +515,22 @@
     DeleteTapeOutputTypeDef,
     DeleteTapePoolOutputTypeDef,
     DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitOutputTypeDef,
     DescribeCacheOutputTypeDef,
     DescribeMaintenanceStartTimeOutputTypeDef,
+    DescribeSnapshotScheduleOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
     JoinDomainOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListVolumeInitiatorsOutputTypeDef,
     NotifyWhenUploadedOutputTypeDef,
     RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
@@ -553,30 +551,29 @@
     UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityOutputTypeDef,
     UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyOutputTypeDef,
     UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
+    SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
     UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
+    NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
-    DescribeSnapshotScheduleOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    SMBFileShareInfoTypeDef,
     DescribeSMBSettingsOutputTypeDef,
     DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
     DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
@@ -594,23 +591,22 @@
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
-    NFSFileShareInfoTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
-    DescribeSMBFileSharesOutputTypeDef,
+    DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
-    DescribeNFSFileSharesOutputTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-storagegateway-1.28.12/mypy_boto3_storagegateway.egg-info/SOURCES.txt` & `mypy-boto3-storagegateway-1.28.15/mypy_boto3_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.28.12/setup.py` & `mypy-boto3-storagegateway-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-storagegateway",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.StorageGateway 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.StorageGateway 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

