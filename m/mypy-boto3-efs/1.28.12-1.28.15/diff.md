# Comparing `tmp/mypy-boto3-efs-1.28.12.tar.gz` & `tmp/mypy-boto3-efs-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-efs-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
+gzip compressed data, was "mypy-boto3-efs-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
```

## Comparing `mypy-boto3-efs-1.28.12.tar` & `mypy-boto3-efs-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.064522 mypy-boto3-efs-1.28.12/mypy_boto3_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25747 2023-07-27 05:21:39.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-07-27 05:21:38.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.068522 mypy-boto3-efs-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:37.000000 mypy-boto3-efs-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.881042 mypy-boto3-efs-1.28.15/mypy_boto3_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23463 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-07-28 20:24:58.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-28 20:24:58.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:43.000000 mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.889042 mypy-boto3-efs-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:24:57.000000 mypy-boto3-efs-1.28.15/setup.py
```

### Comparing `mypy-boto3-efs-1.28.12/LICENSE` & `mypy-boto3-efs-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.12/PKG-INFO` & `mypy-boto3-efs-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.12
-Summary: Type annotations for boto3.EFS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,80 +339,75 @@
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserOutputTypeDef,
-    TagOutputTypeDef,
-    BackupPolicyOutputTypeDef,
+    ResponseMetadataTypeDef,
+    TagTypeDef,
     BackupPolicyTypeDef,
     PosixUserTypeDef,
-    TagTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
-    CreationInfoOutputTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
-    LifecyclePolicyOutputTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
+    MountTargetDescriptionResponseTypeDef,
+    CreateFileSystemRequestRequestTypeDef,
+    CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
-    CreateFileSystemRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
-    RootDirectoryOutputTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     AccessPointDescriptionTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-efs-1.28.12/README.md` & `mypy-boto3-efs-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,80 +307,75 @@
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserOutputTypeDef,
-    TagOutputTypeDef,
-    BackupPolicyOutputTypeDef,
+    ResponseMetadataTypeDef,
+    TagTypeDef,
     BackupPolicyTypeDef,
     PosixUserTypeDef,
-    TagTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
-    CreationInfoOutputTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
-    LifecyclePolicyOutputTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
+    MountTargetDescriptionResponseTypeDef,
+    CreateFileSystemRequestRequestTypeDef,
+    CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
-    CreateFileSystemRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
-    RootDirectoryOutputTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     AccessPointDescriptionTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.py` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/__init__.pyi` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/__main__.py` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EFS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.EFS 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.py` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
     DescribeTagsPaginator,
 )
 from .type_defs import (
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     BackupPolicyDescriptionTypeDef,
     BackupPolicyTypeDef,
     DescribeAccessPointsResponseTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeMountTargetSecurityGroupsResponseTypeDef,
     DescribeMountTargetsResponseTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DestinationToCreateTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
+    MountTargetDescriptionResponseTypeDef,
     PosixUserTypeDef,
     PutAccountPreferencesResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -138,15 +138,15 @@
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
         PosixUser: PosixUserTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
-    ) -> AccessPointDescriptionResponseMetadataTypeDef:
+    ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_access_point)
         """
 
@@ -158,40 +158,40 @@
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...,
         AvailabilityZoneName: str = ...,
         Backup: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Creates a new, empty file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_file_system)
         """
 
     def create_mount_target(
         self,
         *,
         FileSystemId: str,
         SubnetId: str,
         IpAddress: str = ...,
         SecurityGroups: Sequence[str] = ...
-    ) -> MountTargetDescriptionResponseMetadataTypeDef:
+    ) -> MountTargetDescriptionResponseTypeDef:
         """
         Creates a mount target for a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_mount_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_mount_target)
         """
 
     def create_replication_configuration(
         self, *, SourceFileSystemId: str, Destinations: Sequence[DestinationToCreateTypeDef]
-    ) -> ReplicationConfigurationDescriptionResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationDescriptionResponseTypeDef:
         """
         Creates a replication configuration that replicates an existing EFS file system
         to a new, read-only file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_replication_configuration)
         """
@@ -476,15 +476,15 @@
 
     def update_file_system(
         self,
         *,
         FileSystemId: str,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Updates the throughput mode or the amount of provisioned throughput of an
         existing file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#update_file_system)
         """
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/client.pyi` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
     DescribeTagsPaginator,
 )
 from .type_defs import (
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     BackupPolicyDescriptionTypeDef,
     BackupPolicyTypeDef,
     DescribeAccessPointsResponseTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeMountTargetSecurityGroupsResponseTypeDef,
     DescribeMountTargetsResponseTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DestinationToCreateTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
+    MountTargetDescriptionResponseTypeDef,
     PosixUserTypeDef,
     PutAccountPreferencesResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -131,15 +131,15 @@
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
         PosixUser: PosixUserTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
-    ) -> AccessPointDescriptionResponseMetadataTypeDef:
+    ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_access_point)
         """
     def create_file_system(
@@ -150,38 +150,38 @@
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...,
         AvailabilityZoneName: str = ...,
         Backup: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Creates a new, empty file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_file_system)
         """
     def create_mount_target(
         self,
         *,
         FileSystemId: str,
         SubnetId: str,
         IpAddress: str = ...,
         SecurityGroups: Sequence[str] = ...
-    ) -> MountTargetDescriptionResponseMetadataTypeDef:
+    ) -> MountTargetDescriptionResponseTypeDef:
         """
         Creates a mount target for a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_mount_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_mount_target)
         """
     def create_replication_configuration(
         self, *, SourceFileSystemId: str, Destinations: Sequence[DestinationToCreateTypeDef]
-    ) -> ReplicationConfigurationDescriptionResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationDescriptionResponseTypeDef:
         """
         Creates a replication configuration that replicates an existing EFS file system
         to a new, read-only file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_replication_configuration)
         """
@@ -439,15 +439,15 @@
         """
     def update_file_system(
         self,
         *,
         FileSystemId: str,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Updates the throughput mode or the amount of provisioned throughput of an
         existing file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#update_file_system)
         """
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.py` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/literals.pyi` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.py` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describefilesystemspaginator)
         """
 
 
@@ -74,28 +74,28 @@
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describemounttargetspaginator)
         """
 
 
 class DescribeTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
-        self, *, FileSystemId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FileSystemId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
         """
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/paginator.pyi` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describefilesystemspaginator)
         """
 
 class DescribeMountTargetsPaginator(Paginator):
@@ -70,27 +70,27 @@
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describemounttargetspaginator)
         """
 
 class DescribeTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
-        self, *, FileSystemId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FileSystemId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
         """
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.py` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,80 +34,75 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "PosixUserOutputTypeDef",
-    "TagOutputTypeDef",
-    "BackupPolicyOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "BackupPolicyTypeDef",
     "PosixUserTypeDef",
-    "TagTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
-    "CreationInfoOutputTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DescribeAccessPointsRequestRequestTypeDef",
     "DescribeAccountPreferencesRequestRequestTypeDef",
     "ResourceIdPreferenceTypeDef",
     "DescribeBackupPolicyRequestRequestTypeDef",
     "DescribeFileSystemPolicyRequestRequestTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
     "DescribeLifecycleConfigurationRequestRequestTypeDef",
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeMountTargetsRequestRequestTypeDef",
     "MountTargetDescriptionTypeDef",
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
-    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
-    "FileSystemPolicyDescriptionTypeDef",
-    "LifecyclePolicyOutputTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FileSystemPolicyDescriptionTypeDef",
+    "MountTargetDescriptionResponseTypeDef",
+    "CreateFileSystemRequestRequestTypeDef",
+    "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
-    "CreateFileSystemRequestRequestTypeDef",
-    "CreateTagsRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
-    "RootDirectoryOutputTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeMountTargetsResponseTypeDef",
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
-    "FileSystemDescriptionResponseMetadataTypeDef",
+    "FileSystemDescriptionResponseTypeDef",
     "FileSystemDescriptionTypeDef",
     "LifecycleConfigurationDescriptionTypeDef",
     "PutLifecycleConfigurationRequestRequestTypeDef",
-    "AccessPointDescriptionResponseMetadataTypeDef",
+    "AccessPointDescriptionResponseTypeDef",
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
@@ -127,26 +122,30 @@
 )
 
 
 class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-BackupPolicyOutputTypeDef = TypedDict(
-    "BackupPolicyOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "Status": StatusType,
+        "Key": str,
+        "Value": str,
     },
 )
 
 BackupPolicyTypeDef = TypedDict(
     "BackupPolicyTypeDef",
     {
         "Status": StatusType,
@@ -169,22 +168,14 @@
 )
 
 
 class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -210,23 +201,14 @@
         "Region": str,
         "AvailabilityZoneName": str,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-CreationInfoOutputTypeDef = TypedDict(
-    "CreationInfoOutputTypeDef",
-    {
-        "OwnerUid": int,
-        "OwnerGid": int,
-        "Permissions": str,
-    },
-)
-
 CreationInfoTypeDef = TypedDict(
     "CreationInfoTypeDef",
     {
         "OwnerUid": int,
         "OwnerGid": int,
         "Permissions": str,
     },
@@ -314,20 +296,20 @@
 DescribeFileSystemPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CreationToken": str,
-        "FileSystemId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
@@ -349,33 +331,14 @@
 DescribeMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 
-DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-        "MountTargetId": str,
-        "AccessPointId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMountTargetsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "Marker": str,
         "FileSystemId": str,
         "MountTargetId": str,
@@ -419,36 +382,14 @@
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-    },
-)
-_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeTagsRequestDescribeTagsPaginateTypeDef(
-    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
-    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -484,21 +425,14 @@
 )
 
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFileSystemSizeTypeDef = TypedDict(
     "_RequiredFileSystemSizeTypeDef",
     {
         "Value": int,
     },
 )
 _OptionalFileSystemSizeTypeDef = TypedDict(
@@ -512,32 +446,14 @@
 )
 
 
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
 
-FileSystemPolicyDescriptionTypeDef = TypedDict(
-    "FileSystemPolicyDescriptionTypeDef",
-    {
-        "FileSystemId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LifecyclePolicyOutputTypeDef = TypedDict(
-    "LifecyclePolicyOutputTypeDef",
-    {
-        "TransitionToIA": TransitionToIARulesType,
-        "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
-    },
-    total=False,
-)
-
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
     total=False,
@@ -584,41 +500,14 @@
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
 
-MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    {
-        "OwnerId": str,
-        "MountTargetId": str,
-        "FileSystemId": str,
-        "SubnetId": str,
-        "LifeCycleState": LifeCycleStateType,
-        "IpAddress": str,
-        "NetworkInterfaceId": str,
-        "AvailabilityZoneId": str,
-        "AvailabilityZoneName": str,
-        "VpcId": str,
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
 PutAccountPreferencesRequestRequestTypeDef = TypedDict(
     "PutAccountPreferencesRequestRequestTypeDef",
     {
         "ResourceIdType": ResourceIdTypeType,
     },
 )
 
@@ -641,25 +530,14 @@
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -682,46 +560,52 @@
 
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
 
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
+DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
     {
-        "Marker": str,
-        "Tags": List[TagOutputTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BackupPolicyDescriptionTypeDef = TypedDict(
-    "BackupPolicyDescriptionTypeDef",
+FileSystemPolicyDescriptionTypeDef = TypedDict(
+    "FileSystemPolicyDescriptionTypeDef",
     {
-        "BackupPolicy": BackupPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FileSystemId": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutBackupPolicyRequestRequestTypeDef = TypedDict(
-    "PutBackupPolicyRequestRequestTypeDef",
+MountTargetDescriptionResponseTypeDef = TypedDict(
+    "MountTargetDescriptionResponseTypeDef",
     {
+        "OwnerId": str,
+        "MountTargetId": str,
         "FileSystemId": str,
-        "BackupPolicy": BackupPolicyTypeDef,
+        "SubnetId": str,
+        "LifeCycleState": LifeCycleStateType,
+        "IpAddress": str,
+        "NetworkInterfaceId": str,
+        "AvailabilityZoneId": str,
+        "AvailabilityZoneName": str,
+        "VpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
@@ -753,37 +637,63 @@
     "CreateTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "Marker": str,
+        "Tags": List[TagTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateReplicationConfigurationRequestRequestTypeDef",
+BackupPolicyDescriptionTypeDef = TypedDict(
+    "BackupPolicyDescriptionTypeDef",
     {
-        "SourceFileSystemId": str,
-        "Destinations": Sequence[DestinationToCreateTypeDef],
+        "BackupPolicy": BackupPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RootDirectoryOutputTypeDef = TypedDict(
-    "RootDirectoryOutputTypeDef",
+PutBackupPolicyRequestRequestTypeDef = TypedDict(
+    "PutBackupPolicyRequestRequestTypeDef",
     {
-        "Path": str,
-        "CreationInfo": CreationInfoOutputTypeDef,
+        "FileSystemId": str,
+        "BackupPolicy": BackupPolicyTypeDef,
+    },
+)
+
+CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "SourceFileSystemId": str,
+        "Destinations": Sequence[DestinationToCreateTypeDef],
     },
-    total=False,
 )
 
 RootDirectoryTypeDef = TypedDict(
     "RootDirectoryTypeDef",
     {
         "Path": str,
         "CreationInfo": CreationInfoTypeDef,
@@ -792,46 +702,89 @@
 )
 
 DescribeAccountPreferencesResponseTypeDef = TypedDict(
     "DescribeAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountPreferencesResponseTypeDef = TypedDict(
     "PutAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    {
+        "CreationToken": str,
+        "FileSystemId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+        "MountTargetId": str,
+        "AccessPointId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+    },
+)
+_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTagsRequestDescribeTagsPaginateTypeDef(
+    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
+    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
+):
+    pass
+
+
 DescribeMountTargetsResponseTypeDef = TypedDict(
     "DescribeMountTargetsResponseTypeDef",
     {
         "Marker": str,
         "MountTargets": List[MountTargetDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationDescriptionResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+ReplicationConfigurationDescriptionResponseTypeDef = TypedDict(
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     {
         "SourceFileSystemId": str,
         "SourceFileSystemRegion": str,
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationConfigurationDescriptionTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionTypeDef",
     {
         "SourceFileSystemId": str,
@@ -839,16 +792,16 @@
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
     },
 )
 
-FileSystemDescriptionResponseMetadataTypeDef = TypedDict(
-    "FileSystemDescriptionResponseMetadataTypeDef",
+FileSystemDescriptionResponseTypeDef = TypedDict(
+    "FileSystemDescriptionResponseTypeDef",
     {
         "OwnerId": str,
         "CreationToken": str,
         "FileSystemId": str,
         "FileSystemArn": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
@@ -858,31 +811,31 @@
         "PerformanceMode": PerformanceModeType,
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
         "OwnerId": str,
         "CreationToken": str,
         "FileSystemId": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
         "NumberOfMountTargets": int,
         "SizeInBytes": FileSystemSizeTypeDef,
         "PerformanceMode": PerformanceModeType,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
 )
 _OptionalFileSystemDescriptionTypeDef = TypedDict(
     "_OptionalFileSystemDescriptionTypeDef",
     {
         "FileSystemArn": str,
         "Name": str,
@@ -902,55 +855,55 @@
 ):
     pass
 
 
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
-        "LifecyclePolicies": List[LifecyclePolicyOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LifecyclePolicies": List[LifecyclePolicyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "LifecyclePolicies": Sequence[LifecyclePolicyTypeDef],
     },
 )
 
-AccessPointDescriptionResponseMetadataTypeDef = TypedDict(
-    "AccessPointDescriptionResponseMetadataTypeDef",
+AccessPointDescriptionResponseTypeDef = TypedDict(
+    "AccessPointDescriptionResponseTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
         "PosixUser": PosixUserOutputTypeDef,
-        "RootDirectory": RootDirectoryOutputTypeDef,
+        "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
         "PosixUser": PosixUserOutputTypeDef,
-        "RootDirectory": RootDirectoryOutputTypeDef,
+        "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
 
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
@@ -978,29 +931,29 @@
 
 
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemsResponseTypeDef = TypedDict(
     "DescribeFileSystemsResponseTypeDef",
     {
         "Marker": str,
         "FileSystems": List[FileSystemDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsResponseTypeDef = TypedDict(
     "DescribeAccessPointsResponseTypeDef",
     {
         "AccessPoints": List[AccessPointDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs/type_defs.pyi` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -33,80 +33,75 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "PosixUserOutputTypeDef",
-    "TagOutputTypeDef",
-    "BackupPolicyOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "BackupPolicyTypeDef",
     "PosixUserTypeDef",
-    "TagTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
-    "CreationInfoOutputTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DescribeAccessPointsRequestRequestTypeDef",
     "DescribeAccountPreferencesRequestRequestTypeDef",
     "ResourceIdPreferenceTypeDef",
     "DescribeBackupPolicyRequestRequestTypeDef",
     "DescribeFileSystemPolicyRequestRequestTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
     "DescribeLifecycleConfigurationRequestRequestTypeDef",
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeMountTargetsRequestRequestTypeDef",
     "MountTargetDescriptionTypeDef",
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
-    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
-    "FileSystemPolicyDescriptionTypeDef",
-    "LifecyclePolicyOutputTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FileSystemPolicyDescriptionTypeDef",
+    "MountTargetDescriptionResponseTypeDef",
+    "CreateFileSystemRequestRequestTypeDef",
+    "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
-    "CreateFileSystemRequestRequestTypeDef",
-    "CreateTagsRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
-    "RootDirectoryOutputTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeMountTargetsResponseTypeDef",
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
-    "FileSystemDescriptionResponseMetadataTypeDef",
+    "FileSystemDescriptionResponseTypeDef",
     "FileSystemDescriptionTypeDef",
     "LifecycleConfigurationDescriptionTypeDef",
     "PutLifecycleConfigurationRequestRequestTypeDef",
-    "AccessPointDescriptionResponseMetadataTypeDef",
+    "AccessPointDescriptionResponseTypeDef",
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
@@ -124,26 +119,30 @@
     },
     total=False,
 )
 
 class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-BackupPolicyOutputTypeDef = TypedDict(
-    "BackupPolicyOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "Status": StatusType,
+        "Key": str,
+        "Value": str,
     },
 )
 
 BackupPolicyTypeDef = TypedDict(
     "BackupPolicyTypeDef",
     {
         "Status": StatusType,
@@ -164,22 +163,14 @@
     },
     total=False,
 )
 
 class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -203,23 +194,14 @@
         "Region": str,
         "AvailabilityZoneName": str,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-CreationInfoOutputTypeDef = TypedDict(
-    "CreationInfoOutputTypeDef",
-    {
-        "OwnerUid": int,
-        "OwnerGid": int,
-        "Permissions": str,
-    },
-)
-
 CreationInfoTypeDef = TypedDict(
     "CreationInfoTypeDef",
     {
         "OwnerUid": int,
         "OwnerGid": int,
         "Permissions": str,
     },
@@ -307,20 +289,20 @@
 DescribeFileSystemPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CreationToken": str,
-        "FileSystemId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
@@ -342,33 +324,14 @@
 DescribeMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 
-DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-        "MountTargetId": str,
-        "AccessPointId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMountTargetsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "Marker": str,
         "FileSystemId": str,
         "MountTargetId": str,
@@ -410,34 +373,14 @@
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-    },
-)
-_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeTagsRequestDescribeTagsPaginateTypeDef(
-    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
-    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -469,21 +412,14 @@
     },
     total=False,
 )
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFileSystemSizeTypeDef = TypedDict(
     "_RequiredFileSystemSizeTypeDef",
     {
         "Value": int,
     },
 )
 _OptionalFileSystemSizeTypeDef = TypedDict(
@@ -495,32 +431,14 @@
     },
     total=False,
 )
 
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
-FileSystemPolicyDescriptionTypeDef = TypedDict(
-    "FileSystemPolicyDescriptionTypeDef",
-    {
-        "FileSystemId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LifecyclePolicyOutputTypeDef = TypedDict(
-    "LifecyclePolicyOutputTypeDef",
-    {
-        "TransitionToIA": TransitionToIARulesType,
-        "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
-    },
-    total=False,
-)
-
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
     total=False,
@@ -563,41 +481,14 @@
 
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
-MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    {
-        "OwnerId": str,
-        "MountTargetId": str,
-        "FileSystemId": str,
-        "SubnetId": str,
-        "LifeCycleState": LifeCycleStateType,
-        "IpAddress": str,
-        "NetworkInterfaceId": str,
-        "AvailabilityZoneId": str,
-        "AvailabilityZoneName": str,
-        "VpcId": str,
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
 PutAccountPreferencesRequestRequestTypeDef = TypedDict(
     "PutAccountPreferencesRequestRequestTypeDef",
     {
         "ResourceIdType": ResourceIdTypeType,
     },
 )
 
@@ -618,25 +509,14 @@
 
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -657,46 +537,52 @@
 )
 
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
+DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
     {
-        "Marker": str,
-        "Tags": List[TagOutputTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BackupPolicyDescriptionTypeDef = TypedDict(
-    "BackupPolicyDescriptionTypeDef",
+FileSystemPolicyDescriptionTypeDef = TypedDict(
+    "FileSystemPolicyDescriptionTypeDef",
     {
-        "BackupPolicy": BackupPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FileSystemId": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutBackupPolicyRequestRequestTypeDef = TypedDict(
-    "PutBackupPolicyRequestRequestTypeDef",
+MountTargetDescriptionResponseTypeDef = TypedDict(
+    "MountTargetDescriptionResponseTypeDef",
     {
+        "OwnerId": str,
+        "MountTargetId": str,
         "FileSystemId": str,
-        "BackupPolicy": BackupPolicyTypeDef,
+        "SubnetId": str,
+        "LifeCycleState": LifeCycleStateType,
+        "IpAddress": str,
+        "NetworkInterfaceId": str,
+        "AvailabilityZoneId": str,
+        "AvailabilityZoneName": str,
+        "VpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
@@ -726,37 +612,63 @@
     "CreateTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "Marker": str,
+        "Tags": List[TagTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateReplicationConfigurationRequestRequestTypeDef",
+BackupPolicyDescriptionTypeDef = TypedDict(
+    "BackupPolicyDescriptionTypeDef",
     {
-        "SourceFileSystemId": str,
-        "Destinations": Sequence[DestinationToCreateTypeDef],
+        "BackupPolicy": BackupPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RootDirectoryOutputTypeDef = TypedDict(
-    "RootDirectoryOutputTypeDef",
+PutBackupPolicyRequestRequestTypeDef = TypedDict(
+    "PutBackupPolicyRequestRequestTypeDef",
     {
-        "Path": str,
-        "CreationInfo": CreationInfoOutputTypeDef,
+        "FileSystemId": str,
+        "BackupPolicy": BackupPolicyTypeDef,
+    },
+)
+
+CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateReplicationConfigurationRequestRequestTypeDef",
+    {
+        "SourceFileSystemId": str,
+        "Destinations": Sequence[DestinationToCreateTypeDef],
     },
-    total=False,
 )
 
 RootDirectoryTypeDef = TypedDict(
     "RootDirectoryTypeDef",
     {
         "Path": str,
         "CreationInfo": CreationInfoTypeDef,
@@ -765,46 +677,87 @@
 )
 
 DescribeAccountPreferencesResponseTypeDef = TypedDict(
     "DescribeAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountPreferencesResponseTypeDef = TypedDict(
     "PutAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    {
+        "CreationToken": str,
+        "FileSystemId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+        "MountTargetId": str,
+        "AccessPointId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+    },
+)
+_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTagsRequestDescribeTagsPaginateTypeDef(
+    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
+    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
+):
+    pass
+
 DescribeMountTargetsResponseTypeDef = TypedDict(
     "DescribeMountTargetsResponseTypeDef",
     {
         "Marker": str,
         "MountTargets": List[MountTargetDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationDescriptionResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+ReplicationConfigurationDescriptionResponseTypeDef = TypedDict(
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     {
         "SourceFileSystemId": str,
         "SourceFileSystemRegion": str,
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationConfigurationDescriptionTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionTypeDef",
     {
         "SourceFileSystemId": str,
@@ -812,16 +765,16 @@
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
     },
 )
 
-FileSystemDescriptionResponseMetadataTypeDef = TypedDict(
-    "FileSystemDescriptionResponseMetadataTypeDef",
+FileSystemDescriptionResponseTypeDef = TypedDict(
+    "FileSystemDescriptionResponseTypeDef",
     {
         "OwnerId": str,
         "CreationToken": str,
         "FileSystemId": str,
         "FileSystemArn": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
@@ -831,31 +784,31 @@
         "PerformanceMode": PerformanceModeType,
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
         "OwnerId": str,
         "CreationToken": str,
         "FileSystemId": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
         "NumberOfMountTargets": int,
         "SizeInBytes": FileSystemSizeTypeDef,
         "PerformanceMode": PerformanceModeType,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
 )
 _OptionalFileSystemDescriptionTypeDef = TypedDict(
     "_OptionalFileSystemDescriptionTypeDef",
     {
         "FileSystemArn": str,
         "Name": str,
@@ -873,55 +826,55 @@
     _RequiredFileSystemDescriptionTypeDef, _OptionalFileSystemDescriptionTypeDef
 ):
     pass
 
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
-        "LifecyclePolicies": List[LifecyclePolicyOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LifecyclePolicies": List[LifecyclePolicyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "LifecyclePolicies": Sequence[LifecyclePolicyTypeDef],
     },
 )
 
-AccessPointDescriptionResponseMetadataTypeDef = TypedDict(
-    "AccessPointDescriptionResponseMetadataTypeDef",
+AccessPointDescriptionResponseTypeDef = TypedDict(
+    "AccessPointDescriptionResponseTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
         "PosixUser": PosixUserOutputTypeDef,
-        "RootDirectory": RootDirectoryOutputTypeDef,
+        "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
         "Name": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
         "PosixUser": PosixUserOutputTypeDef,
-        "RootDirectory": RootDirectoryOutputTypeDef,
+        "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
 
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
@@ -947,29 +900,29 @@
     pass
 
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemsResponseTypeDef = TypedDict(
     "DescribeFileSystemsResponseTypeDef",
     {
         "Marker": str,
         "FileSystems": List[FileSystemDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsResponseTypeDef = TypedDict(
     "DescribeAccessPointsResponseTypeDef",
     {
         "AccessPoints": List[AccessPointDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/PKG-INFO` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.12
-Summary: Type annotations for boto3.EFS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,80 +339,75 @@
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserOutputTypeDef,
-    TagOutputTypeDef,
-    BackupPolicyOutputTypeDef,
+    ResponseMetadataTypeDef,
+    TagTypeDef,
     BackupPolicyTypeDef,
     PosixUserTypeDef,
-    TagTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
-    CreationInfoOutputTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
-    LifecyclePolicyOutputTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
+    MountTargetDescriptionResponseTypeDef,
+    CreateFileSystemRequestRequestTypeDef,
+    CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
-    CreateFileSystemRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
-    RootDirectoryOutputTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     AccessPointDescriptionTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-efs-1.28.12/mypy_boto3_efs.egg-info/SOURCES.txt` & `mypy-boto3-efs-1.28.15/mypy_boto3_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.12/setup.py` & `mypy-boto3-efs-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-efs",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EFS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

