# Comparing `tmp/mypy-boto3-glacier-1.28.12.tar.gz` & `tmp/mypy-boto3-glacier-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glacier-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
+gzip compressed data, was "mypy-boto3-glacier-1.28.15.tar", last modified: Fri Jul 28 20:42:52 2023, max compression
```

## Comparing `mypy-boto3-glacier-1.28.12.tar` & `mypy-boto3-glacier-1.28.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.136501 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26565 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39259 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    39151 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42119 2023-07-27 05:22:45.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 05:34:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.365159 mypy-boto3-glacier-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-28 20:42:52.361159 mypy-boto3-glacier-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.361159 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26579 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-28 20:26:31.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-28 20:26:31.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39087 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39382 2023-07-28 20:26:32.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-28 20:26:32.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-28 20:26:30.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.361159 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:52.000000 mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:52.365159 mypy-boto3-glacier-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:26:29.000000 mypy-boto3-glacier-1.28.15/setup.py
```

### Comparing `mypy-boto3-glacier-1.28.12/LICENSE` & `mypy-boto3-glacier-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/PKG-INFO` & `mypy-boto3-glacier-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.28.12
-Summary: Type annotations for boto3.Glacier 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,118 +439,108 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
-    ArchiveCreationOutputTypeDef,
-    CSVInputOutputTypeDef,
+    ResponseMetadataTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
-    CreateVaultOutputTypeDef,
-    DataRetrievalRuleOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeVaultOutputTypeDef,
-    DescribeVaultResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
-    GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
-    VaultAccessPolicyOutputTypeDef,
+    VaultAccessPolicyTypeDef,
     GetVaultLockInputRequestTypeDef,
-    GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
     VaultNotificationConfigOutputTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
-    GranteeOutputTypeDef,
     GranteeTypeDef,
-    InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
-    InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
-    InitiateVaultLockOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
     InventoryRetrievalJobInputTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsInputRequestTypeDef,
-    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     ListMultipartUploadsInputRequestTypeDef,
     UploadListElementTypeDef,
-    ListPartsInputListPartsPaginateTypeDef,
     ListPartsInputMultipartUploadPartsTypeDef,
     ListPartsInputRequestTypeDef,
     PartListElementTypeDef,
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
-    ListTagsForVaultOutputTypeDef,
-    ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
-    PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    VaultAccessPolicyTypeDef,
     VaultNotificationConfigTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
+    ArchiveCreationOutputTypeDef,
+    CreateVaultOutputTypeDef,
+    DescribeVaultResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetJobOutputOutputTypeDef,
+    GetVaultLockOutputTypeDef,
+    InitiateJobOutputTypeDef,
+    InitiateMultipartUploadOutputTypeDef,
+    InitiateVaultLockOutputTypeDef,
+    InventoryRetrievalJobDescriptionResponseTypeDef,
+    ListTagsForVaultOutputTypeDef,
+    PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
-    InputSerializationOutputTypeDef,
     InputSerializationTypeDef,
-    OutputSerializationOutputTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
+    SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    GrantOutputTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
+    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+    ListPartsInputListPartsPaginateTypeDef,
+    ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
-    SetVaultAccessPolicyInputRequestTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
-    SelectParametersOutputTypeDef,
-    SelectParametersResponseMetadataTypeDef,
+    SelectParametersResponseTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
     S3LocationOutputTypeDef,
     S3LocationTypeDef,
     OutputLocationOutputTypeDef,
-    OutputLocationResponseMetadataTypeDef,
     OutputLocationTypeDef,
-    GlacierJobDescriptionResponseMetadataTypeDef,
+    GlacierJobDescriptionResponseTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-glacier-1.28.12/README.md` & `mypy-boto3-glacier-1.28.15/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,118 +407,108 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
-    ArchiveCreationOutputTypeDef,
-    CSVInputOutputTypeDef,
+    ResponseMetadataTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
-    CreateVaultOutputTypeDef,
-    DataRetrievalRuleOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeVaultOutputTypeDef,
-    DescribeVaultResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
-    GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
-    VaultAccessPolicyOutputTypeDef,
+    VaultAccessPolicyTypeDef,
     GetVaultLockInputRequestTypeDef,
-    GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
     VaultNotificationConfigOutputTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
-    GranteeOutputTypeDef,
     GranteeTypeDef,
-    InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
-    InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
-    InitiateVaultLockOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
     InventoryRetrievalJobInputTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsInputRequestTypeDef,
-    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     ListMultipartUploadsInputRequestTypeDef,
     UploadListElementTypeDef,
-    ListPartsInputListPartsPaginateTypeDef,
     ListPartsInputMultipartUploadPartsTypeDef,
     ListPartsInputRequestTypeDef,
     PartListElementTypeDef,
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
-    ListTagsForVaultOutputTypeDef,
-    ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
-    PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    VaultAccessPolicyTypeDef,
     VaultNotificationConfigTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
+    ArchiveCreationOutputTypeDef,
+    CreateVaultOutputTypeDef,
+    DescribeVaultResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetJobOutputOutputTypeDef,
+    GetVaultLockOutputTypeDef,
+    InitiateJobOutputTypeDef,
+    InitiateMultipartUploadOutputTypeDef,
+    InitiateVaultLockOutputTypeDef,
+    InventoryRetrievalJobDescriptionResponseTypeDef,
+    ListTagsForVaultOutputTypeDef,
+    PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
-    InputSerializationOutputTypeDef,
     InputSerializationTypeDef,
-    OutputSerializationOutputTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
+    SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    GrantOutputTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
+    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+    ListPartsInputListPartsPaginateTypeDef,
+    ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
-    SetVaultAccessPolicyInputRequestTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
-    SelectParametersOutputTypeDef,
-    SelectParametersResponseMetadataTypeDef,
+    SelectParametersResponseTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
     S3LocationOutputTypeDef,
     S3LocationTypeDef,
     OutputLocationOutputTypeDef,
-    OutputLocationResponseMetadataTypeDef,
     OutputLocationTypeDef,
-    GlacierJobDescriptionResponseMetadataTypeDef,
+    GlacierJobDescriptionResponseTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.pyi` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__main__.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glacier 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Glacier 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,22 @@
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     DataRetrievalPolicyTypeDef,
-    DescribeVaultResponseMetadataTypeDef,
+    DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    GlacierJobDescriptionResponseMetadataTypeDef,
+    GlacierJobDescriptionResponseTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     InitiateVaultLockOutputTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
@@ -222,28 +222,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.delete_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#delete_vault_notifications)
         """
 
     def describe_job(
         self, *, vaultName: str, jobId: str, accountId: str = "-"
-    ) -> GlacierJobDescriptionResponseMetadataTypeDef:
+    ) -> GlacierJobDescriptionResponseTypeDef:
         """
         This operation returns information about a job you previously initiated,
         including the job initiation date, the user who initiated the job, the job
         status code/message and the Amazon SNS topic to notify after Amazon S3 Glacier
         (Glacier) completes the job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_job)
         """
 
     def describe_vault(
         self, *, vaultName: str, accountId: str = "-"
-    ) -> DescribeVaultResponseMetadataTypeDef:
+    ) -> DescribeVaultResponseTypeDef:
         """
         This operation returns information about a vault, including the vault's Amazon
         Resource Name (ARN), the date the vault was created, the number of archives it
         contains, and the total size of all the archives in the vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_vault)
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.pyi` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,22 @@
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     DataRetrievalPolicyTypeDef,
-    DescribeVaultResponseMetadataTypeDef,
+    DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    GlacierJobDescriptionResponseMetadataTypeDef,
+    GlacierJobDescriptionResponseTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     InitiateVaultLockOutputTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
@@ -205,27 +205,27 @@
         This operation deletes the notification configuration set for a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.delete_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#delete_vault_notifications)
         """
     def describe_job(
         self, *, vaultName: str, jobId: str, accountId: str = "-"
-    ) -> GlacierJobDescriptionResponseMetadataTypeDef:
+    ) -> GlacierJobDescriptionResponseTypeDef:
         """
         This operation returns information about a job you previously initiated,
         including the job initiation date, the user who initiated the job, the job
         status code/message and the Amazon SNS topic to notify after Amazon S3 Glacier
         (Glacier) completes the job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_job)
         """
     def describe_vault(
         self, *, vaultName: str, accountId: str = "-"
-    ) -> DescribeVaultResponseMetadataTypeDef:
+    ) -> DescribeVaultResponseTypeDef:
         """
         This operation returns information about a vault, including the vault's Amazon
         Resource Name (ARN), the date the vault was created, the number of archives it
         contains, and the total size of all the archives in the vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_vault)
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.pyi` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,30 @@
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         statuscode: str = ...,
         completed: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listjobspaginator)
         """
 
 
 class ListMultipartUploadsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, vaultName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountId: str, vaultName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
         """
 
 
@@ -99,28 +99,28 @@
 
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         uploadId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listpartspaginator)
         """
 
 
 class ListVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
         """
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.pyi` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,29 @@
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         statuscode: str = ...,
         completed: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listjobspaginator)
         """
 
 class ListMultipartUploadsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, vaultName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountId: str, vaultName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
         """
 
 class ListPartsPaginator(Paginator):
@@ -94,27 +94,27 @@
 
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         uploadId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listpartspaginator)
         """
 
 class ListVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
         """
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
 from .client import GlacierClient
 from .literals import ActionCodeType, StatusCodeType
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     GetJobOutputOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
+    InventoryRetrievalJobDescriptionResponseTypeDef,
     ListPartsOutputTypeDef,
-    OutputLocationResponseMetadataTypeDef,
-    SelectParametersResponseMetadataTypeDef,
+    OutputLocationTypeDef,
+    SelectParametersResponseTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultNotificationConfigTypeDef,
 )
 
 __all__ = (
     "GlacierServiceResource",
     "Account",
@@ -410,18 +410,18 @@
     inventory_size_in_bytes: int
     sns_topic: str
     completion_date: str
     sha256_tree_hash: str
     archive_sha256_tree_hash: str
     retrieval_byte_range: str
     tier: str
-    inventory_retrieval_parameters: InventoryRetrievalJobDescriptionResponseMetadataTypeDef
+    inventory_retrieval_parameters: InventoryRetrievalJobDescriptionResponseTypeDef
     job_output_path: str
-    select_parameters: SelectParametersResponseMetadataTypeDef
-    output_location: OutputLocationResponseMetadataTypeDef
+    select_parameters: SelectParametersResponseTypeDef
+    output_location: OutputLocationTypeDef
     account_id: str
     vault_name: str
     id: str
 
     def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.pyi` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
 from .client import GlacierClient
 from .literals import ActionCodeType, StatusCodeType
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     GetJobOutputOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
+    InventoryRetrievalJobDescriptionResponseTypeDef,
     ListPartsOutputTypeDef,
-    OutputLocationResponseMetadataTypeDef,
-    SelectParametersResponseMetadataTypeDef,
+    OutputLocationTypeDef,
+    SelectParametersResponseTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultNotificationConfigTypeDef,
 )
 
 __all__ = (
     "GlacierServiceResource",
     "Account",
@@ -388,18 +388,18 @@
     inventory_size_in_bytes: int
     sns_topic: str
     completion_date: str
     sha256_tree_hash: str
     archive_sha256_tree_hash: str
     retrieval_byte_range: str
     tier: str
-    inventory_retrieval_parameters: InventoryRetrievalJobDescriptionResponseMetadataTypeDef
+    inventory_retrieval_parameters: InventoryRetrievalJobDescriptionResponseTypeDef
     job_output_path: str
-    select_parameters: SelectParametersResponseMetadataTypeDef
-    output_location: OutputLocationResponseMetadataTypeDef
+    select_parameters: SelectParametersResponseTypeDef
+    output_location: OutputLocationTypeDef
     account_id: str
     vault_name: str
     id: str
 
     def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,118 +38,108 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
-    "ArchiveCreationOutputTypeDef",
-    "CSVInputOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
     "CreateVaultInputServiceResourceCreateVaultTypeDef",
-    "CreateVaultOutputTypeDef",
-    "DataRetrievalRuleOutputTypeDef",
     "DataRetrievalRuleTypeDef",
     "DeleteArchiveInputRequestTypeDef",
     "DeleteVaultAccessPolicyInputRequestTypeDef",
     "DeleteVaultInputRequestTypeDef",
     "DeleteVaultNotificationsInputRequestTypeDef",
     "DescribeJobInputRequestTypeDef",
     "DescribeVaultInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeVaultOutputTypeDef",
-    "DescribeVaultResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
-    "GetJobOutputOutputTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
-    "VaultAccessPolicyOutputTypeDef",
+    "VaultAccessPolicyTypeDef",
     "GetVaultLockInputRequestTypeDef",
-    "GetVaultLockOutputTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
     "VaultNotificationConfigOutputTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
-    "GranteeOutputTypeDef",
     "GranteeTypeDef",
-    "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
-    "InitiateMultipartUploadOutputTypeDef",
     "VaultLockPolicyTypeDef",
-    "InitiateVaultLockOutputTypeDef",
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
     "InventoryRetrievalJobInputTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobsInputRequestTypeDef",
-    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     "ListMultipartUploadsInputRequestTypeDef",
     "UploadListElementTypeDef",
-    "ListPartsInputListPartsPaginateTypeDef",
     "ListPartsInputMultipartUploadPartsTypeDef",
     "ListPartsInputRequestTypeDef",
     "PartListElementTypeDef",
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
-    "ListTagsForVaultOutputTypeDef",
-    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListVaultsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
-    "PurchaseProvisionedCapacityOutputTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "VaultAccessPolicyTypeDef",
     "VaultNotificationConfigTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
+    "ArchiveCreationOutputTypeDef",
+    "CreateVaultOutputTypeDef",
+    "DescribeVaultResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetJobOutputOutputTypeDef",
+    "GetVaultLockOutputTypeDef",
+    "InitiateJobOutputTypeDef",
+    "InitiateMultipartUploadOutputTypeDef",
+    "InitiateVaultLockOutputTypeDef",
+    "InventoryRetrievalJobDescriptionResponseTypeDef",
+    "ListTagsForVaultOutputTypeDef",
+    "PurchaseProvisionedCapacityOutputTypeDef",
     "UploadMultipartPartOutputTypeDef",
-    "InputSerializationOutputTypeDef",
     "InputSerializationTypeDef",
-    "OutputSerializationOutputTypeDef",
     "OutputSerializationTypeDef",
     "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
+    "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
-    "GrantOutputTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
+    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    "ListPartsInputListPartsPaginateTypeDef",
+    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
-    "SetVaultAccessPolicyInputRequestTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
     "SetVaultNotificationsInputRequestTypeDef",
-    "SelectParametersOutputTypeDef",
-    "SelectParametersResponseMetadataTypeDef",
+    "SelectParametersResponseTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
     "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "OutputLocationOutputTypeDef",
-    "OutputLocationResponseMetadataTypeDef",
     "OutputLocationTypeDef",
-    "GlacierJobDescriptionResponseMetadataTypeDef",
+    "GlacierJobDescriptionResponseTypeDef",
     "GlacierJobDescriptionTypeDef",
     "JobParametersTypeDef",
     "ListJobsOutputTypeDef",
     "InitiateJobInputRequestTypeDef",
 )
 
 _RequiredAbortMultipartUploadInputRequestTypeDef = TypedDict(
@@ -214,35 +204,23 @@
 
 class AddTagsToVaultInputRequestTypeDef(
     _RequiredAddTagsToVaultInputRequestTypeDef, _OptionalAddTagsToVaultInputRequestTypeDef
 ):
     pass
 
 
-ArchiveCreationOutputTypeDef = TypedDict(
-    "ArchiveCreationOutputTypeDef",
-    {
-        "location": str,
-        "checksum": str,
-        "archiveId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CSVInputOutputTypeDef = TypedDict(
-    "CSVInputOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FileHeaderInfo": FileHeaderInfoType,
-        "Comments": str,
-        "QuoteEscapeCharacter": str,
-        "RecordDelimiter": str,
-        "FieldDelimiter": str,
-        "QuoteCharacter": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
@@ -368,31 +346,14 @@
 class CreateVaultInputServiceResourceCreateVaultTypeDef(
     _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef,
     _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef,
 ):
     pass
 
 
-CreateVaultOutputTypeDef = TypedDict(
-    "CreateVaultOutputTypeDef",
-    {
-        "location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataRetrievalRuleOutputTypeDef = TypedDict(
-    "DataRetrievalRuleOutputTypeDef",
-    {
-        "Strategy": str,
-        "BytesPerHour": int,
-    },
-    total=False,
-)
-
 DataRetrievalRuleTypeDef = TypedDict(
     "DataRetrievalRuleTypeDef",
     {
         "Strategy": str,
         "BytesPerHour": int,
     },
     total=False,
@@ -546,44 +507,14 @@
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
     },
     total=False,
 )
 
-DescribeVaultResponseMetadataTypeDef = TypedDict(
-    "DescribeVaultResponseMetadataTypeDef",
-    {
-        "VaultARN": str,
-        "VaultName": str,
-        "CreationDate": str,
-        "LastInventoryDate": str,
-        "NumberOfArchives": int,
-        "SizeInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EncryptionOutputTypeDef = TypedDict(
-    "EncryptionOutputTypeDef",
-    {
-        "EncryptionType": EncryptionTypeType,
-        "KMSKeyId": str,
-        "KMSContext": str,
-    },
-    total=False,
-)
-
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KMSKeyId": str,
         "KMSContext": str,
     },
@@ -625,28 +556,14 @@
 
 class GetJobOutputInputRequestTypeDef(
     _RequiredGetJobOutputInputRequestTypeDef, _OptionalGetJobOutputInputRequestTypeDef
 ):
     pass
 
 
-GetJobOutputOutputTypeDef = TypedDict(
-    "GetJobOutputOutputTypeDef",
-    {
-        "body": StreamingBody,
-        "checksum": str,
-        "status": int,
-        "contentRange": str,
-        "acceptRanges": str,
-        "contentType": str,
-        "archiveDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalGetVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -661,16 +578,16 @@
 class GetVaultAccessPolicyInputRequestTypeDef(
     _RequiredGetVaultAccessPolicyInputRequestTypeDef,
     _OptionalGetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
 
-VaultAccessPolicyOutputTypeDef = TypedDict(
-    "VaultAccessPolicyOutputTypeDef",
+VaultAccessPolicyTypeDef = TypedDict(
+    "VaultAccessPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
 _RequiredGetVaultLockInputRequestTypeDef = TypedDict(
@@ -690,25 +607,14 @@
 
 class GetVaultLockInputRequestTypeDef(
     _RequiredGetVaultLockInputRequestTypeDef, _OptionalGetVaultLockInputRequestTypeDef
 ):
     pass
 
 
-GetVaultLockOutputTypeDef = TypedDict(
-    "GetVaultLockOutputTypeDef",
-    {
-        "Policy": str,
-        "State": str,
-        "ExpirationDate": str,
-        "CreationDate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalGetVaultNotificationsInputRequestTypeDef = TypedDict(
@@ -744,36 +650,14 @@
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredGranteeOutputTypeDef = TypedDict(
-    "_RequiredGranteeOutputTypeDef",
-    {
-        "Type": TypeType,
-    },
-)
-_OptionalGranteeOutputTypeDef = TypedDict(
-    "_OptionalGranteeOutputTypeDef",
-    {
-        "DisplayName": str,
-        "URI": str,
-        "ID": str,
-        "EmailAddress": str,
-    },
-    total=False,
-)
-
-
-class GranteeOutputTypeDef(_RequiredGranteeOutputTypeDef, _OptionalGranteeOutputTypeDef):
-    pass
-
-
 _RequiredGranteeTypeDef = TypedDict(
     "_RequiredGranteeTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalGranteeTypeDef = TypedDict(
@@ -788,24 +672,14 @@
 )
 
 
 class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
     pass
 
 
-InitiateJobOutputTypeDef = TypedDict(
-    "InitiateJobOutputTypeDef",
-    {
-        "location": str,
-        "jobId": str,
-        "jobOutputPath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredInitiateMultipartUploadInputRequestTypeDef = TypedDict(
     "_RequiredInitiateMultipartUploadInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalInitiateMultipartUploadInputRequestTypeDef = TypedDict(
@@ -831,86 +705,43 @@
     {
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
-InitiateMultipartUploadOutputTypeDef = TypedDict(
-    "InitiateMultipartUploadOutputTypeDef",
-    {
-        "location": str,
-        "uploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VaultLockPolicyTypeDef = TypedDict(
     "VaultLockPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
-InitiateVaultLockOutputTypeDef = TypedDict(
-    "InitiateVaultLockOutputTypeDef",
-    {
-        "lockId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InventoryRetrievalJobDescriptionResponseMetadataTypeDef = TypedDict(
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
-    {
-        "Format": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Limit": str,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InventoryRetrievalJobInputTypeDef = TypedDict(
     "InventoryRetrievalJobInputTypeDef",
     {
         "StartDate": str,
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsInputListJobsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsInputListJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "statuscode": str,
-        "completed": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListJobsInputListJobsPaginateTypeDef(
-    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListJobsInputRequestTypeDef = TypedDict(
     "_RequiredListJobsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListJobsInputRequestTypeDef = TypedDict(
@@ -928,37 +759,14 @@
 
 class ListJobsInputRequestTypeDef(
     _RequiredListJobsInputRequestTypeDef, _OptionalListJobsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMultipartUploadsInputRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListMultipartUploadsInputRequestTypeDef = TypedDict(
@@ -987,37 +795,14 @@
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
     },
     total=False,
 )
 
-_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsInputListPartsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-        "uploadId": str,
-    },
-)
-_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsInputListPartsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPartsInputListPartsPaginateTypeDef(
-    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
-):
-    pass
-
-
 ListPartsInputMultipartUploadPartsTypeDef = TypedDict(
     "ListPartsInputMultipartUploadPartsTypeDef",
     {
         "marker": str,
         "limit": str,
     },
     total=False,
@@ -1091,80 +876,32 @@
 
 class ListTagsForVaultInputRequestTypeDef(
     _RequiredListTagsForVaultInputRequestTypeDef, _OptionalListTagsForVaultInputRequestTypeDef
 ):
     pass
 
 
-ListTagsForVaultOutputTypeDef = TypedDict(
-    "ListTagsForVaultOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "accountId": str,
-    },
-)
-_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVaultsInputListVaultsPaginateTypeDef(
-    _RequiredListVaultsInputListVaultsPaginateTypeDef,
-    _OptionalListVaultsInputListVaultsPaginateTypeDef,
-):
-    pass
-
-
 ListVaultsInputRequestTypeDef = TypedDict(
     "ListVaultsInputRequestTypeDef",
     {
         "accountId": str,
         "marker": str,
         "limit": str,
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
 PurchaseProvisionedCapacityInputRequestTypeDef = TypedDict(
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
-    "PurchaseProvisionedCapacityOutputTypeDef",
-    {
-        "capacityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
     "_RequiredRemoveTagsFromVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
@@ -1179,33 +916,14 @@
 
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
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
-VaultAccessPolicyTypeDef = TypedDict(
-    "VaultAccessPolicyTypeDef",
-    {
-        "Policy": str,
-    },
-    total=False,
-)
-
 VaultNotificationConfigTypeDef = TypedDict(
     "VaultNotificationConfigTypeDef",
     {
         "SNSTopic": str,
         "Events": Sequence[str],
     },
     total=False,
@@ -1276,42 +994,144 @@
 
 class UploadMultipartPartInputRequestTypeDef(
     _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
 ):
     pass
 
 
-UploadMultipartPartOutputTypeDef = TypedDict(
-    "UploadMultipartPartOutputTypeDef",
+ArchiveCreationOutputTypeDef = TypedDict(
+    "ArchiveCreationOutputTypeDef",
     {
+        "location": str,
         "checksum": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "archiveId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InputSerializationOutputTypeDef = TypedDict(
-    "InputSerializationOutputTypeDef",
+CreateVaultOutputTypeDef = TypedDict(
+    "CreateVaultOutputTypeDef",
     {
-        "csv": CSVInputOutputTypeDef,
+        "location": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-InputSerializationTypeDef = TypedDict(
-    "InputSerializationTypeDef",
+DescribeVaultResponseTypeDef = TypedDict(
+    "DescribeVaultResponseTypeDef",
     {
-        "csv": CSVInputTypeDef,
+        "VaultARN": str,
+        "VaultName": str,
+        "CreationDate": str,
+        "LastInventoryDate": str,
+        "NumberOfArchives": int,
+        "SizeInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-OutputSerializationOutputTypeDef = TypedDict(
-    "OutputSerializationOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "csv": CSVOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobOutputOutputTypeDef = TypedDict(
+    "GetJobOutputOutputTypeDef",
+    {
+        "body": StreamingBody,
+        "checksum": str,
+        "status": int,
+        "contentRange": str,
+        "acceptRanges": str,
+        "contentType": str,
+        "archiveDescription": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVaultLockOutputTypeDef = TypedDict(
+    "GetVaultLockOutputTypeDef",
+    {
+        "Policy": str,
+        "State": str,
+        "ExpirationDate": str,
+        "CreationDate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateJobOutputTypeDef = TypedDict(
+    "InitiateJobOutputTypeDef",
+    {
+        "location": str,
+        "jobId": str,
+        "jobOutputPath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateMultipartUploadOutputTypeDef = TypedDict(
+    "InitiateMultipartUploadOutputTypeDef",
+    {
+        "location": str,
+        "uploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateVaultLockOutputTypeDef = TypedDict(
+    "InitiateVaultLockOutputTypeDef",
+    {
+        "lockId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InventoryRetrievalJobDescriptionResponseTypeDef = TypedDict(
+    "InventoryRetrievalJobDescriptionResponseTypeDef",
+    {
+        "Format": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Limit": str,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForVaultOutputTypeDef = TypedDict(
+    "ListTagsForVaultOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
+    "PurchaseProvisionedCapacityOutputTypeDef",
+    {
+        "capacityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadMultipartPartOutputTypeDef = TypedDict(
+    "UploadMultipartPartOutputTypeDef",
+    {
+        "checksum": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InputSerializationTypeDef = TypedDict(
+    "InputSerializationTypeDef",
+    {
+        "csv": CSVInputTypeDef,
     },
     total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
@@ -1319,15 +1139,15 @@
     },
     total=False,
 )
 
 DataRetrievalPolicyOutputTypeDef = TypedDict(
     "DataRetrievalPolicyOutputTypeDef",
     {
-        "Rules": List[DataRetrievalRuleOutputTypeDef],
+        "Rules": List[DataRetrievalRuleTypeDef],
     },
     total=False,
 )
 
 DataRetrievalPolicyTypeDef = TypedDict(
     "DataRetrievalPolicyTypeDef",
     {
@@ -1383,43 +1203,57 @@
 
 
 ListVaultsOutputTypeDef = TypedDict(
     "ListVaultsOutputTypeDef",
     {
         "VaultList": List[DescribeVaultOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVaultAccessPolicyOutputTypeDef = TypedDict(
     "GetVaultAccessPolicyOutputTypeDef",
     {
-        "policy": VaultAccessPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policy": VaultAccessPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetVaultNotificationsOutputTypeDef = TypedDict(
-    "GetVaultNotificationsOutputTypeDef",
+_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "vaultName": str,
     },
 )
-
-GrantOutputTypeDef = TypedDict(
-    "GrantOutputTypeDef",
+_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
     {
-        "Grantee": GranteeOutputTypeDef,
-        "Permission": PermissionType,
+        "accountId": str,
+        "policy": VaultAccessPolicyTypeDef,
     },
     total=False,
 )
 
+
+class SetVaultAccessPolicyInputRequestTypeDef(
+    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
+    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
+):
+    pass
+
+
+GetVaultNotificationsOutputTypeDef = TypedDict(
+    "GetVaultNotificationsOutputTypeDef",
+    {
+        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1443,68 +1277,137 @@
 
 class InitiateVaultLockInputRequestTypeDef(
     _RequiredInitiateVaultLockInputRequestTypeDef, _OptionalInitiateVaultLockInputRequestTypeDef
 ):
     pass
 
 
+_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsInputListJobsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsInputListJobsPaginateTypeDef",
+    {
+        "statuscode": str,
+        "completed": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobsInputListJobsPaginateTypeDef(
+    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
+):
+    pass
+
+
+_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsInputListPartsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+        "uploadId": str,
+    },
+)
+_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsInputListPartsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPartsInputListPartsPaginateTypeDef(
+    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
+):
+    pass
+
+
+_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVaultsInputListVaultsPaginateTypeDef(
+    _RequiredListVaultsInputListVaultsPaginateTypeDef,
+    _OptionalListVaultsInputListVaultsPaginateTypeDef,
+):
+    pass
+
+
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "UploadsList": List[UploadListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
         "Parts": List[PartListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisionedCapacityOutputTypeDef = TypedDict(
     "ListProvisionedCapacityOutputTypeDef",
     {
         "ProvisionedCapacityList": List[ProvisionedCapacityDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "accountId": str,
-        "policy": VaultAccessPolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class SetVaultAccessPolicyInputRequestTypeDef(
-    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
-    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
-):
-    pass
-
-
 SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
     "SetVaultNotificationsInputNotificationSetTypeDef",
     {
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
     },
     total=False,
 )
@@ -1528,33 +1431,22 @@
 class SetVaultNotificationsInputRequestTypeDef(
     _RequiredSetVaultNotificationsInputRequestTypeDef,
     _OptionalSetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
 
-SelectParametersOutputTypeDef = TypedDict(
-    "SelectParametersOutputTypeDef",
+SelectParametersResponseTypeDef = TypedDict(
+    "SelectParametersResponseTypeDef",
     {
-        "InputSerialization": InputSerializationOutputTypeDef,
-        "ExpressionType": Literal["SQL"],
-        "Expression": str,
-        "OutputSerialization": OutputSerializationOutputTypeDef,
-    },
-    total=False,
-)
-
-SelectParametersResponseMetadataTypeDef = TypedDict(
-    "SelectParametersResponseMetadataTypeDef",
-    {
-        "InputSerialization": InputSerializationOutputTypeDef,
+        "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
-        "OutputSerialization": OutputSerializationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OutputSerialization": OutputSerializationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
@@ -1565,15 +1457,15 @@
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
         "Policy": DataRetrievalPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
@@ -1583,17 +1475,17 @@
 )
 
 S3LocationOutputTypeDef = TypedDict(
     "S3LocationOutputTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
-        "Encryption": EncryptionOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
         "CannedACL": CannedACLType,
-        "AccessControlList": List[GrantOutputTypeDef],
+        "AccessControlList": List[GrantTypeDef],
         "Tagging": Dict[str, str],
         "UserMetadata": Dict[str, str],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
@@ -1616,32 +1508,24 @@
     "OutputLocationOutputTypeDef",
     {
         "S3": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
-OutputLocationResponseMetadataTypeDef = TypedDict(
-    "OutputLocationResponseMetadataTypeDef",
-    {
-        "S3": S3LocationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
-        "S3": S3LocationTypeDef,
+        "S3": S3LocationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-GlacierJobDescriptionResponseMetadataTypeDef = TypedDict(
-    "GlacierJobDescriptionResponseMetadataTypeDef",
+GlacierJobDescriptionResponseTypeDef = TypedDict(
+    "GlacierJobDescriptionResponseTypeDef",
     {
         "JobId": str,
         "JobDescription": str,
         "Action": ActionCodeType,
         "ArchiveId": str,
         "VaultARN": str,
         "CreationDate": str,
@@ -1654,17 +1538,17 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersOutputTypeDef,
+        "SelectParameters": SelectParametersTypeDef,
         "OutputLocation": OutputLocationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
         "JobId": str,
@@ -1682,15 +1566,15 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersOutputTypeDef,
+        "SelectParameters": SelectParametersTypeDef,
         "OutputLocation": OutputLocationOutputTypeDef,
     },
     total=False,
 )
 
 JobParametersTypeDef = TypedDict(
     "JobParametersTypeDef",
@@ -1710,15 +1594,15 @@
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "JobList": List[GlacierJobDescriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInitiateJobInputRequestTypeDef = TypedDict(
     "_RequiredInitiateJobInputRequestTypeDef",
     {
         "vaultName": str,
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.pyi` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -37,118 +37,108 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
-    "ArchiveCreationOutputTypeDef",
-    "CSVInputOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
     "CreateVaultInputServiceResourceCreateVaultTypeDef",
-    "CreateVaultOutputTypeDef",
-    "DataRetrievalRuleOutputTypeDef",
     "DataRetrievalRuleTypeDef",
     "DeleteArchiveInputRequestTypeDef",
     "DeleteVaultAccessPolicyInputRequestTypeDef",
     "DeleteVaultInputRequestTypeDef",
     "DeleteVaultNotificationsInputRequestTypeDef",
     "DescribeJobInputRequestTypeDef",
     "DescribeVaultInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeVaultOutputTypeDef",
-    "DescribeVaultResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
-    "GetJobOutputOutputTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
-    "VaultAccessPolicyOutputTypeDef",
+    "VaultAccessPolicyTypeDef",
     "GetVaultLockInputRequestTypeDef",
-    "GetVaultLockOutputTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
     "VaultNotificationConfigOutputTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
-    "GranteeOutputTypeDef",
     "GranteeTypeDef",
-    "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
-    "InitiateMultipartUploadOutputTypeDef",
     "VaultLockPolicyTypeDef",
-    "InitiateVaultLockOutputTypeDef",
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
     "InventoryRetrievalJobInputTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobsInputRequestTypeDef",
-    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     "ListMultipartUploadsInputRequestTypeDef",
     "UploadListElementTypeDef",
-    "ListPartsInputListPartsPaginateTypeDef",
     "ListPartsInputMultipartUploadPartsTypeDef",
     "ListPartsInputRequestTypeDef",
     "PartListElementTypeDef",
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
-    "ListTagsForVaultOutputTypeDef",
-    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListVaultsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
-    "PurchaseProvisionedCapacityOutputTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "VaultAccessPolicyTypeDef",
     "VaultNotificationConfigTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
+    "ArchiveCreationOutputTypeDef",
+    "CreateVaultOutputTypeDef",
+    "DescribeVaultResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetJobOutputOutputTypeDef",
+    "GetVaultLockOutputTypeDef",
+    "InitiateJobOutputTypeDef",
+    "InitiateMultipartUploadOutputTypeDef",
+    "InitiateVaultLockOutputTypeDef",
+    "InventoryRetrievalJobDescriptionResponseTypeDef",
+    "ListTagsForVaultOutputTypeDef",
+    "PurchaseProvisionedCapacityOutputTypeDef",
     "UploadMultipartPartOutputTypeDef",
-    "InputSerializationOutputTypeDef",
     "InputSerializationTypeDef",
-    "OutputSerializationOutputTypeDef",
     "OutputSerializationTypeDef",
     "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
+    "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
-    "GrantOutputTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
+    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    "ListPartsInputListPartsPaginateTypeDef",
+    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
-    "SetVaultAccessPolicyInputRequestTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
     "SetVaultNotificationsInputRequestTypeDef",
-    "SelectParametersOutputTypeDef",
-    "SelectParametersResponseMetadataTypeDef",
+    "SelectParametersResponseTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
     "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "OutputLocationOutputTypeDef",
-    "OutputLocationResponseMetadataTypeDef",
     "OutputLocationTypeDef",
-    "GlacierJobDescriptionResponseMetadataTypeDef",
+    "GlacierJobDescriptionResponseTypeDef",
     "GlacierJobDescriptionTypeDef",
     "JobParametersTypeDef",
     "ListJobsOutputTypeDef",
     "InitiateJobInputRequestTypeDef",
 )
 
 _RequiredAbortMultipartUploadInputRequestTypeDef = TypedDict(
@@ -207,35 +197,23 @@
 )
 
 class AddTagsToVaultInputRequestTypeDef(
     _RequiredAddTagsToVaultInputRequestTypeDef, _OptionalAddTagsToVaultInputRequestTypeDef
 ):
     pass
 
-ArchiveCreationOutputTypeDef = TypedDict(
-    "ArchiveCreationOutputTypeDef",
-    {
-        "location": str,
-        "checksum": str,
-        "archiveId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CSVInputOutputTypeDef = TypedDict(
-    "CSVInputOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FileHeaderInfo": FileHeaderInfoType,
-        "Comments": str,
-        "QuoteEscapeCharacter": str,
-        "RecordDelimiter": str,
-        "FieldDelimiter": str,
-        "QuoteCharacter": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
@@ -353,31 +331,14 @@
 
 class CreateVaultInputServiceResourceCreateVaultTypeDef(
     _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef,
     _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef,
 ):
     pass
 
-CreateVaultOutputTypeDef = TypedDict(
-    "CreateVaultOutputTypeDef",
-    {
-        "location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataRetrievalRuleOutputTypeDef = TypedDict(
-    "DataRetrievalRuleOutputTypeDef",
-    {
-        "Strategy": str,
-        "BytesPerHour": int,
-    },
-    total=False,
-)
-
 DataRetrievalRuleTypeDef = TypedDict(
     "DataRetrievalRuleTypeDef",
     {
         "Strategy": str,
         "BytesPerHour": int,
     },
     total=False,
@@ -519,44 +480,14 @@
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
     },
     total=False,
 )
 
-DescribeVaultResponseMetadataTypeDef = TypedDict(
-    "DescribeVaultResponseMetadataTypeDef",
-    {
-        "VaultARN": str,
-        "VaultName": str,
-        "CreationDate": str,
-        "LastInventoryDate": str,
-        "NumberOfArchives": int,
-        "SizeInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EncryptionOutputTypeDef = TypedDict(
-    "EncryptionOutputTypeDef",
-    {
-        "EncryptionType": EncryptionTypeType,
-        "KMSKeyId": str,
-        "KMSContext": str,
-    },
-    total=False,
-)
-
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KMSKeyId": str,
         "KMSContext": str,
     },
@@ -596,28 +527,14 @@
 )
 
 class GetJobOutputInputRequestTypeDef(
     _RequiredGetJobOutputInputRequestTypeDef, _OptionalGetJobOutputInputRequestTypeDef
 ):
     pass
 
-GetJobOutputOutputTypeDef = TypedDict(
-    "GetJobOutputOutputTypeDef",
-    {
-        "body": StreamingBody,
-        "checksum": str,
-        "status": int,
-        "contentRange": str,
-        "acceptRanges": str,
-        "contentType": str,
-        "archiveDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalGetVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -630,16 +547,16 @@
 
 class GetVaultAccessPolicyInputRequestTypeDef(
     _RequiredGetVaultAccessPolicyInputRequestTypeDef,
     _OptionalGetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
-VaultAccessPolicyOutputTypeDef = TypedDict(
-    "VaultAccessPolicyOutputTypeDef",
+VaultAccessPolicyTypeDef = TypedDict(
+    "VaultAccessPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
 _RequiredGetVaultLockInputRequestTypeDef = TypedDict(
@@ -657,25 +574,14 @@
 )
 
 class GetVaultLockInputRequestTypeDef(
     _RequiredGetVaultLockInputRequestTypeDef, _OptionalGetVaultLockInputRequestTypeDef
 ):
     pass
 
-GetVaultLockOutputTypeDef = TypedDict(
-    "GetVaultLockOutputTypeDef",
-    {
-        "Policy": str,
-        "State": str,
-        "ExpirationDate": str,
-        "CreationDate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalGetVaultNotificationsInputRequestTypeDef = TypedDict(
@@ -709,34 +615,14 @@
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredGranteeOutputTypeDef = TypedDict(
-    "_RequiredGranteeOutputTypeDef",
-    {
-        "Type": TypeType,
-    },
-)
-_OptionalGranteeOutputTypeDef = TypedDict(
-    "_OptionalGranteeOutputTypeDef",
-    {
-        "DisplayName": str,
-        "URI": str,
-        "ID": str,
-        "EmailAddress": str,
-    },
-    total=False,
-)
-
-class GranteeOutputTypeDef(_RequiredGranteeOutputTypeDef, _OptionalGranteeOutputTypeDef):
-    pass
-
 _RequiredGranteeTypeDef = TypedDict(
     "_RequiredGranteeTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalGranteeTypeDef = TypedDict(
@@ -749,24 +635,14 @@
     },
     total=False,
 )
 
 class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
     pass
 
-InitiateJobOutputTypeDef = TypedDict(
-    "InitiateJobOutputTypeDef",
-    {
-        "location": str,
-        "jobId": str,
-        "jobOutputPath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredInitiateMultipartUploadInputRequestTypeDef = TypedDict(
     "_RequiredInitiateMultipartUploadInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalInitiateMultipartUploadInputRequestTypeDef = TypedDict(
@@ -790,84 +666,43 @@
     {
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
-InitiateMultipartUploadOutputTypeDef = TypedDict(
-    "InitiateMultipartUploadOutputTypeDef",
-    {
-        "location": str,
-        "uploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VaultLockPolicyTypeDef = TypedDict(
     "VaultLockPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
-InitiateVaultLockOutputTypeDef = TypedDict(
-    "InitiateVaultLockOutputTypeDef",
-    {
-        "lockId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InventoryRetrievalJobDescriptionResponseMetadataTypeDef = TypedDict(
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
-    {
-        "Format": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Limit": str,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InventoryRetrievalJobInputTypeDef = TypedDict(
     "InventoryRetrievalJobInputTypeDef",
     {
         "StartDate": str,
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsInputListJobsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsInputListJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "statuscode": str,
-        "completed": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListJobsInputListJobsPaginateTypeDef(
-    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
-):
-    pass
-
 _RequiredListJobsInputRequestTypeDef = TypedDict(
     "_RequiredListJobsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListJobsInputRequestTypeDef = TypedDict(
@@ -883,35 +718,14 @@
 )
 
 class ListJobsInputRequestTypeDef(
     _RequiredListJobsInputRequestTypeDef, _OptionalListJobsInputRequestTypeDef
 ):
     pass
 
-_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMultipartUploadsInputRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListMultipartUploadsInputRequestTypeDef = TypedDict(
@@ -938,35 +752,14 @@
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
     },
     total=False,
 )
 
-_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsInputListPartsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-        "uploadId": str,
-    },
-)
-_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsInputListPartsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPartsInputListPartsPaginateTypeDef(
-    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
-):
-    pass
-
 ListPartsInputMultipartUploadPartsTypeDef = TypedDict(
     "ListPartsInputMultipartUploadPartsTypeDef",
     {
         "marker": str,
         "limit": str,
     },
     total=False,
@@ -1036,78 +829,32 @@
 )
 
 class ListTagsForVaultInputRequestTypeDef(
     _RequiredListTagsForVaultInputRequestTypeDef, _OptionalListTagsForVaultInputRequestTypeDef
 ):
     pass
 
-ListTagsForVaultOutputTypeDef = TypedDict(
-    "ListTagsForVaultOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "accountId": str,
-    },
-)
-_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVaultsInputListVaultsPaginateTypeDef(
-    _RequiredListVaultsInputListVaultsPaginateTypeDef,
-    _OptionalListVaultsInputListVaultsPaginateTypeDef,
-):
-    pass
-
 ListVaultsInputRequestTypeDef = TypedDict(
     "ListVaultsInputRequestTypeDef",
     {
         "accountId": str,
         "marker": str,
         "limit": str,
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
 PurchaseProvisionedCapacityInputRequestTypeDef = TypedDict(
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
-    "PurchaseProvisionedCapacityOutputTypeDef",
-    {
-        "capacityId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
     "_RequiredRemoveTagsFromVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
@@ -1120,33 +867,14 @@
 )
 
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
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
-VaultAccessPolicyTypeDef = TypedDict(
-    "VaultAccessPolicyTypeDef",
-    {
-        "Policy": str,
-    },
-    total=False,
-)
-
 VaultNotificationConfigTypeDef = TypedDict(
     "VaultNotificationConfigTypeDef",
     {
         "SNSTopic": str,
         "Events": Sequence[str],
     },
     total=False,
@@ -1213,42 +941,144 @@
 )
 
 class UploadMultipartPartInputRequestTypeDef(
     _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
 ):
     pass
 
-UploadMultipartPartOutputTypeDef = TypedDict(
-    "UploadMultipartPartOutputTypeDef",
+ArchiveCreationOutputTypeDef = TypedDict(
+    "ArchiveCreationOutputTypeDef",
     {
+        "location": str,
         "checksum": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "archiveId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InputSerializationOutputTypeDef = TypedDict(
-    "InputSerializationOutputTypeDef",
+CreateVaultOutputTypeDef = TypedDict(
+    "CreateVaultOutputTypeDef",
     {
-        "csv": CSVInputOutputTypeDef,
+        "location": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-InputSerializationTypeDef = TypedDict(
-    "InputSerializationTypeDef",
+DescribeVaultResponseTypeDef = TypedDict(
+    "DescribeVaultResponseTypeDef",
     {
-        "csv": CSVInputTypeDef,
+        "VaultARN": str,
+        "VaultName": str,
+        "CreationDate": str,
+        "LastInventoryDate": str,
+        "NumberOfArchives": int,
+        "SizeInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-OutputSerializationOutputTypeDef = TypedDict(
-    "OutputSerializationOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "csv": CSVOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobOutputOutputTypeDef = TypedDict(
+    "GetJobOutputOutputTypeDef",
+    {
+        "body": StreamingBody,
+        "checksum": str,
+        "status": int,
+        "contentRange": str,
+        "acceptRanges": str,
+        "contentType": str,
+        "archiveDescription": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVaultLockOutputTypeDef = TypedDict(
+    "GetVaultLockOutputTypeDef",
+    {
+        "Policy": str,
+        "State": str,
+        "ExpirationDate": str,
+        "CreationDate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateJobOutputTypeDef = TypedDict(
+    "InitiateJobOutputTypeDef",
+    {
+        "location": str,
+        "jobId": str,
+        "jobOutputPath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateMultipartUploadOutputTypeDef = TypedDict(
+    "InitiateMultipartUploadOutputTypeDef",
+    {
+        "location": str,
+        "uploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateVaultLockOutputTypeDef = TypedDict(
+    "InitiateVaultLockOutputTypeDef",
+    {
+        "lockId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InventoryRetrievalJobDescriptionResponseTypeDef = TypedDict(
+    "InventoryRetrievalJobDescriptionResponseTypeDef",
+    {
+        "Format": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Limit": str,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForVaultOutputTypeDef = TypedDict(
+    "ListTagsForVaultOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
+    "PurchaseProvisionedCapacityOutputTypeDef",
+    {
+        "capacityId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadMultipartPartOutputTypeDef = TypedDict(
+    "UploadMultipartPartOutputTypeDef",
+    {
+        "checksum": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InputSerializationTypeDef = TypedDict(
+    "InputSerializationTypeDef",
+    {
+        "csv": CSVInputTypeDef,
     },
     total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
@@ -1256,15 +1086,15 @@
     },
     total=False,
 )
 
 DataRetrievalPolicyOutputTypeDef = TypedDict(
     "DataRetrievalPolicyOutputTypeDef",
     {
-        "Rules": List[DataRetrievalRuleOutputTypeDef],
+        "Rules": List[DataRetrievalRuleTypeDef],
     },
     total=False,
 )
 
 DataRetrievalPolicyTypeDef = TypedDict(
     "DataRetrievalPolicyTypeDef",
     {
@@ -1316,43 +1146,55 @@
     pass
 
 ListVaultsOutputTypeDef = TypedDict(
     "ListVaultsOutputTypeDef",
     {
         "VaultList": List[DescribeVaultOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVaultAccessPolicyOutputTypeDef = TypedDict(
     "GetVaultAccessPolicyOutputTypeDef",
     {
-        "policy": VaultAccessPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policy": VaultAccessPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetVaultNotificationsOutputTypeDef = TypedDict(
-    "GetVaultNotificationsOutputTypeDef",
+_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "vaultName": str,
     },
 )
-
-GrantOutputTypeDef = TypedDict(
-    "GrantOutputTypeDef",
+_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
     {
-        "Grantee": GranteeOutputTypeDef,
-        "Permission": PermissionType,
+        "accountId": str,
+        "policy": VaultAccessPolicyTypeDef,
     },
     total=False,
 )
 
+class SetVaultAccessPolicyInputRequestTypeDef(
+    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
+    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
+):
+    pass
+
+GetVaultNotificationsOutputTypeDef = TypedDict(
+    "GetVaultNotificationsOutputTypeDef",
+    {
+        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1374,65 +1216,128 @@
 )
 
 class InitiateVaultLockInputRequestTypeDef(
     _RequiredInitiateVaultLockInputRequestTypeDef, _OptionalInitiateVaultLockInputRequestTypeDef
 ):
     pass
 
+_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsInputListJobsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsInputListJobsPaginateTypeDef",
+    {
+        "statuscode": str,
+        "completed": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobsInputListJobsPaginateTypeDef(
+    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
+):
+    pass
+
+_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsInputListPartsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+        "uploadId": str,
+    },
+)
+_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsInputListPartsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPartsInputListPartsPaginateTypeDef(
+    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
+):
+    pass
+
+_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVaultsInputListVaultsPaginateTypeDef(
+    _RequiredListVaultsInputListVaultsPaginateTypeDef,
+    _OptionalListVaultsInputListVaultsPaginateTypeDef,
+):
+    pass
+
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "UploadsList": List[UploadListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
         "Parts": List[PartListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisionedCapacityOutputTypeDef = TypedDict(
     "ListProvisionedCapacityOutputTypeDef",
     {
         "ProvisionedCapacityList": List[ProvisionedCapacityDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "vaultName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "accountId": str,
-        "policy": VaultAccessPolicyTypeDef,
-    },
-    total=False,
-)
-
-class SetVaultAccessPolicyInputRequestTypeDef(
-    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
-    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
-):
-    pass
 
 SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
     "SetVaultNotificationsInputNotificationSetTypeDef",
     {
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
     },
     total=False,
@@ -1455,33 +1360,22 @@
 
 class SetVaultNotificationsInputRequestTypeDef(
     _RequiredSetVaultNotificationsInputRequestTypeDef,
     _OptionalSetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-SelectParametersOutputTypeDef = TypedDict(
-    "SelectParametersOutputTypeDef",
-    {
-        "InputSerialization": InputSerializationOutputTypeDef,
-        "ExpressionType": Literal["SQL"],
-        "Expression": str,
-        "OutputSerialization": OutputSerializationOutputTypeDef,
-    },
-    total=False,
-)
-
-SelectParametersResponseMetadataTypeDef = TypedDict(
-    "SelectParametersResponseMetadataTypeDef",
+SelectParametersResponseTypeDef = TypedDict(
+    "SelectParametersResponseTypeDef",
     {
-        "InputSerialization": InputSerializationOutputTypeDef,
+        "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
-        "OutputSerialization": OutputSerializationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OutputSerialization": OutputSerializationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
@@ -1492,15 +1386,15 @@
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
         "Policy": DataRetrievalPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
@@ -1510,17 +1404,17 @@
 )
 
 S3LocationOutputTypeDef = TypedDict(
     "S3LocationOutputTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
-        "Encryption": EncryptionOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
         "CannedACL": CannedACLType,
-        "AccessControlList": List[GrantOutputTypeDef],
+        "AccessControlList": List[GrantTypeDef],
         "Tagging": Dict[str, str],
         "UserMetadata": Dict[str, str],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
@@ -1543,32 +1437,24 @@
     "OutputLocationOutputTypeDef",
     {
         "S3": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
-OutputLocationResponseMetadataTypeDef = TypedDict(
-    "OutputLocationResponseMetadataTypeDef",
-    {
-        "S3": S3LocationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
-        "S3": S3LocationTypeDef,
+        "S3": S3LocationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-GlacierJobDescriptionResponseMetadataTypeDef = TypedDict(
-    "GlacierJobDescriptionResponseMetadataTypeDef",
+GlacierJobDescriptionResponseTypeDef = TypedDict(
+    "GlacierJobDescriptionResponseTypeDef",
     {
         "JobId": str,
         "JobDescription": str,
         "Action": ActionCodeType,
         "ArchiveId": str,
         "VaultARN": str,
         "CreationDate": str,
@@ -1581,17 +1467,17 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersOutputTypeDef,
+        "SelectParameters": SelectParametersTypeDef,
         "OutputLocation": OutputLocationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
         "JobId": str,
@@ -1609,15 +1495,15 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersOutputTypeDef,
+        "SelectParameters": SelectParametersTypeDef,
         "OutputLocation": OutputLocationOutputTypeDef,
     },
     total=False,
 )
 
 JobParametersTypeDef = TypedDict(
     "JobParametersTypeDef",
@@ -1637,15 +1523,15 @@
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "JobList": List[GlacierJobDescriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInitiateJobInputRequestTypeDef = TypedDict(
     "_RequiredInitiateJobInputRequestTypeDef",
     {
         "vaultName": str,
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.py` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.pyi` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/PKG-INFO` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.28.12
-Summary: Type annotations for boto3.Glacier 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,118 +439,108 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
-    ArchiveCreationOutputTypeDef,
-    CSVInputOutputTypeDef,
+    ResponseMetadataTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
-    CreateVaultOutputTypeDef,
-    DataRetrievalRuleOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeVaultOutputTypeDef,
-    DescribeVaultResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
-    GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
-    VaultAccessPolicyOutputTypeDef,
+    VaultAccessPolicyTypeDef,
     GetVaultLockInputRequestTypeDef,
-    GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
     VaultNotificationConfigOutputTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
-    GranteeOutputTypeDef,
     GranteeTypeDef,
-    InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
-    InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
-    InitiateVaultLockOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
     InventoryRetrievalJobInputTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsInputRequestTypeDef,
-    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     ListMultipartUploadsInputRequestTypeDef,
     UploadListElementTypeDef,
-    ListPartsInputListPartsPaginateTypeDef,
     ListPartsInputMultipartUploadPartsTypeDef,
     ListPartsInputRequestTypeDef,
     PartListElementTypeDef,
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
-    ListTagsForVaultOutputTypeDef,
-    ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
-    PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    VaultAccessPolicyTypeDef,
     VaultNotificationConfigTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
+    ArchiveCreationOutputTypeDef,
+    CreateVaultOutputTypeDef,
+    DescribeVaultResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetJobOutputOutputTypeDef,
+    GetVaultLockOutputTypeDef,
+    InitiateJobOutputTypeDef,
+    InitiateMultipartUploadOutputTypeDef,
+    InitiateVaultLockOutputTypeDef,
+    InventoryRetrievalJobDescriptionResponseTypeDef,
+    ListTagsForVaultOutputTypeDef,
+    PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
-    InputSerializationOutputTypeDef,
     InputSerializationTypeDef,
-    OutputSerializationOutputTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
+    SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    GrantOutputTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
+    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+    ListPartsInputListPartsPaginateTypeDef,
+    ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
-    SetVaultAccessPolicyInputRequestTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
-    SelectParametersOutputTypeDef,
-    SelectParametersResponseMetadataTypeDef,
+    SelectParametersResponseTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
     S3LocationOutputTypeDef,
     S3LocationTypeDef,
     OutputLocationOutputTypeDef,
-    OutputLocationResponseMetadataTypeDef,
     OutputLocationTypeDef,
-    GlacierJobDescriptionResponseMetadataTypeDef,
+    GlacierJobDescriptionResponseTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/SOURCES.txt` & `mypy-boto3-glacier-1.28.15/mypy_boto3_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.12/setup.py` & `mypy-boto3-glacier-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glacier",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glacier 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Glacier 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

