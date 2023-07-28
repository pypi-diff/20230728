# Comparing `tmp/mypy-boto3-kms-1.28.12.tar.gz` & `tmp/mypy-boto3-kms-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kms-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
+gzip compressed data, was "mypy-boto3-kms-1.28.15.tar", last modified: Fri Jul 28 20:43:07 2023, max compression
```

## Comparing `mypy-boto3-kms-1.28.12.tar` & `mypy-boto3-kms-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.140462 mypy-boto3-kms-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-07-27 05:34:55.128462 mypy-boto3-kms-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.128462 mypy-boto3-kms-1.28.12/mypy_boto3_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41185 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41426 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41365 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.128462 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:55.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.140462 mypy-boto3-kms-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:07.421366 mypy-boto3-kms-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17813 2023-07-28 20:43:07.421366 mypy-boto3-kms-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:07.409366 mypy-boto3-kms-1.28.15/mypy_boto3_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-07-28 20:29:26.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41185 2023-07-28 20:29:26.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-28 20:29:26.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-07-28 20:29:26.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-28 20:29:26.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-28 20:29:26.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41198 2023-07-28 20:29:29.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41137 2023-07-28 20:29:27.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:07.421366 mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17813 2023-07-28 20:43:07.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:07.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:07.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:07.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:07.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:07.000000 mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:07.421366 mypy-boto3-kms-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:29:25.000000 mypy-boto3-kms-1.28.15/setup.py
```

### Comparing `mypy-boto3-kms-1.28.12/LICENSE` & `mypy-boto3-kms-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/PKG-INFO` & `mypy-boto3-kms-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.28.12
-Summary: Type annotations for boto3.KMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,109 +365,108 @@
 `mypy_boto3_kms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kms.type_defs import (
     AliasListEntryTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
-    CancelKeyDeletionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
-    CreateCustomKeyStoreResponseTypeDef,
     GrantConstraintsTypeDef,
-    CreateGrantResponseTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
     RecipientInfoTypeDef,
-    DecryptResponseTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
-    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
     EncryptRequestRequestTypeDef,
-    EncryptResponseTypeDef,
-    GenerateDataKeyPairResponseTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
-    GenerateDataKeyResponseTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacRequestRequestTypeDef,
-    GenerateMacResponseTypeDef,
-    GenerateRandomResponseTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
-    GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
-    GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
-    GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
-    GetPublicKeyResponseTypeDef,
     GrantConstraintsOutputTypeDef,
     ImportKeyMaterialRequestRequestTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
-    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
-    ListKeyPoliciesResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
-    PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
     ReEncryptRequestRequestTypeDef,
-    ReEncryptResponseTypeDef,
-    ResponseMetadataTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    ScheduleKeyDeletionResponseTypeDef,
     SignRequestRequestTypeDef,
-    SignResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
-    VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
-    VerifyResponseTypeDef,
+    CancelKeyDeletionResponseTypeDef,
+    CreateCustomKeyStoreResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    DecryptResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptResponseTypeDef,
+    GenerateDataKeyPairResponseTypeDef,
+    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
+    GenerateDataKeyResponseTypeDef,
+    GenerateDataKeyWithoutPlaintextResponseTypeDef,
+    GenerateMacResponseTypeDef,
+    GenerateRandomResponseTypeDef,
+    GetKeyPolicyResponseTypeDef,
+    GetKeyRotationStatusResponseTypeDef,
+    GetParametersForImportResponseTypeDef,
+    GetPublicKeyResponseTypeDef,
     ListAliasesResponseTypeDef,
+    ListKeyPoliciesResponseTypeDef,
+    ReEncryptResponseTypeDef,
+    ScheduleKeyDeletionResponseTypeDef,
+    SignResponseTypeDef,
+    VerifyMacResponseTypeDef,
+    VerifyResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
+    ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
+    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListGrantsRequestListGrantsPaginateTypeDef,
+    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     GrantListEntryTypeDef,
     ListKeysResponseTypeDef,
-    ListResourceTagsResponseTypeDef,
     MultiRegionConfigurationTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
```

### Comparing `mypy-boto3-kms-1.28.12/README.md` & `mypy-boto3-kms-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,109 +333,108 @@
 `mypy_boto3_kms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kms.type_defs import (
     AliasListEntryTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
-    CancelKeyDeletionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
-    CreateCustomKeyStoreResponseTypeDef,
     GrantConstraintsTypeDef,
-    CreateGrantResponseTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
     RecipientInfoTypeDef,
-    DecryptResponseTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
-    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
     EncryptRequestRequestTypeDef,
-    EncryptResponseTypeDef,
-    GenerateDataKeyPairResponseTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
-    GenerateDataKeyResponseTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacRequestRequestTypeDef,
-    GenerateMacResponseTypeDef,
-    GenerateRandomResponseTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
-    GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
-    GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
-    GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
-    GetPublicKeyResponseTypeDef,
     GrantConstraintsOutputTypeDef,
     ImportKeyMaterialRequestRequestTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
-    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
-    ListKeyPoliciesResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
-    PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
     ReEncryptRequestRequestTypeDef,
-    ReEncryptResponseTypeDef,
-    ResponseMetadataTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    ScheduleKeyDeletionResponseTypeDef,
     SignRequestRequestTypeDef,
-    SignResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
-    VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
-    VerifyResponseTypeDef,
+    CancelKeyDeletionResponseTypeDef,
+    CreateCustomKeyStoreResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    DecryptResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptResponseTypeDef,
+    GenerateDataKeyPairResponseTypeDef,
+    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
+    GenerateDataKeyResponseTypeDef,
+    GenerateDataKeyWithoutPlaintextResponseTypeDef,
+    GenerateMacResponseTypeDef,
+    GenerateRandomResponseTypeDef,
+    GetKeyPolicyResponseTypeDef,
+    GetKeyRotationStatusResponseTypeDef,
+    GetParametersForImportResponseTypeDef,
+    GetPublicKeyResponseTypeDef,
     ListAliasesResponseTypeDef,
+    ListKeyPoliciesResponseTypeDef,
+    ReEncryptResponseTypeDef,
+    ScheduleKeyDeletionResponseTypeDef,
+    SignResponseTypeDef,
+    VerifyMacResponseTypeDef,
+    VerifyResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
+    ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
+    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListGrantsRequestListGrantsPaginateTypeDef,
+    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     GrantListEntryTypeDef,
     ListKeysResponseTypeDef,
-    ListResourceTagsResponseTypeDef,
     MultiRegionConfigurationTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
```

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.py` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.pyi` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/__main__.py` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KMS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.KMS 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
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

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.py` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.pyi` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.py` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.pyi` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.py` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,30 +73,30 @@
     """
 
     def paginate(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#describecustomkeystorespaginator)
         """
 
 
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
         """
 
 
@@ -108,73 +108,73 @@
 
     def paginate(
         self,
         *,
         KeyId: str,
         GrantId: str = ...,
         GranteePrincipal: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listgrantspaginator)
         """
 
 
 class ListKeyPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
         """
 
 
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
         """
 
 
 class ListResourceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
         """
 
 
 class ListRetirableGrantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listretirablegrantspaginator)
     """
 
     def paginate(
-        self, *, RetiringPrincipal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RetiringPrincipal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listretirablegrantspaginator)
         """
```

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.pyi` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,29 +70,29 @@
     """
 
     def paginate(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#describecustomkeystorespaginator)
         """
 
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
         """
 
 class ListGrantsPaginator(Paginator):
@@ -103,69 +103,69 @@
 
     def paginate(
         self,
         *,
         KeyId: str,
         GrantId: str = ...,
         GranteePrincipal: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listgrantspaginator)
         """
 
 class ListKeyPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
         """
 
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
         """
 
 class ListResourceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
         """
 
 class ListRetirableGrantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listretirablegrantspaginator)
     """
 
     def paginate(
-        self, *, RetiringPrincipal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RetiringPrincipal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listretirablegrantspaginator)
         """
```

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.py` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -46,113 +46,111 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasListEntryTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
-    "CancelKeyDeletionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
-    "CreateCustomKeyStoreResponseTypeDef",
     "GrantConstraintsTypeDef",
-    "CreateGrantResponseTypeDef",
     "TagTypeDef",
     "XksProxyConfigurationTypeTypeDef",
     "RecipientInfoTypeDef",
-    "DecryptResponseTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCustomKeyStoreRequestRequestTypeDef",
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DisableKeyRequestRequestTypeDef",
     "DisableKeyRotationRequestRequestTypeDef",
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableKeyRequestRequestTypeDef",
     "EnableKeyRotationRequestRequestTypeDef",
     "EncryptRequestRequestTypeDef",
-    "EncryptResponseTypeDef",
-    "GenerateDataKeyPairResponseTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    "GenerateDataKeyResponseTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
     "GenerateMacRequestRequestTypeDef",
-    "GenerateMacResponseTypeDef",
-    "GenerateRandomResponseTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
-    "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
-    "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
-    "GetParametersForImportResponseTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
-    "GetPublicKeyResponseTypeDef",
     "GrantConstraintsOutputTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListGrantsRequestRequestTypeDef",
-    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
-    "ListKeyPoliciesResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
-    "PaginatorConfigTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
     "ReEncryptRequestRequestTypeDef",
-    "ReEncryptResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
-    "ScheduleKeyDeletionResponseTypeDef",
     "SignRequestRequestTypeDef",
-    "SignResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
     "VerifyMacRequestRequestTypeDef",
-    "VerifyMacResponseTypeDef",
     "VerifyRequestRequestTypeDef",
-    "VerifyResponseTypeDef",
+    "CancelKeyDeletionResponseTypeDef",
+    "CreateCustomKeyStoreResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "DecryptResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EncryptResponseTypeDef",
+    "GenerateDataKeyPairResponseTypeDef",
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    "GenerateDataKeyResponseTypeDef",
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
+    "GenerateMacResponseTypeDef",
+    "GenerateRandomResponseTypeDef",
+    "GetKeyPolicyResponseTypeDef",
+    "GetKeyRotationStatusResponseTypeDef",
+    "GetParametersForImportResponseTypeDef",
+    "GetPublicKeyResponseTypeDef",
     "ListAliasesResponseTypeDef",
+    "ListKeyPoliciesResponseTypeDef",
+    "ReEncryptResponseTypeDef",
+    "ScheduleKeyDeletionResponseTypeDef",
+    "SignResponseTypeDef",
+    "VerifyMacResponseTypeDef",
+    "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
     "CreateKeyRequestRequestTypeDef",
+    "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListGrantsRequestListGrantsPaginateTypeDef",
+    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "GrantListEntryTypeDef",
     "ListKeysResponseTypeDef",
-    "ListResourceTagsResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
     "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
@@ -173,19 +171,22 @@
 CancelKeyDeletionRequestRequestTypeDef = TypedDict(
     "CancelKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-CancelKeyDeletionResponseTypeDef = TypedDict(
-    "CancelKeyDeletionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
@@ -204,40 +205,23 @@
     "XksProxyAuthenticationCredentialTypeTypeDef",
     {
         "AccessKeyId": str,
         "RawSecretAccessKey": str,
     },
 )
 
-CreateCustomKeyStoreResponseTypeDef = TypedDict(
-    "CreateCustomKeyStoreResponseTypeDef",
-    {
-        "CustomKeyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GrantConstraintsTypeDef = TypedDict(
     "GrantConstraintsTypeDef",
     {
         "EncryptionContextSubset": Mapping[str, str],
         "EncryptionContextEquals": Mapping[str, str],
     },
     total=False,
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantToken": str,
-        "GrantId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "TagKey": str,
         "TagValue": str,
     },
 )
@@ -259,25 +243,14 @@
     {
         "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
         "AttestationDocument": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-DecryptResponseTypeDef = TypedDict(
-    "DecryptResponseTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": bytes,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -291,20 +264,20 @@
 DeleteImportedKeyMaterialRequestRequestTypeDef = TypedDict(
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CustomKeyStoreId": str,
-        "CustomKeyStoreName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCustomKeyStoresRequestRequestTypeDef = TypedDict(
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     {
@@ -326,21 +299,19 @@
     "_OptionalDescribeKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeKeyRequestRequestTypeDef(
     _RequiredDescribeKeyRequestRequestTypeDef, _OptionalDescribeKeyRequestRequestTypeDef
 ):
     pass
 
-
 DisableKeyRequestRequestTypeDef = TypedDict(
     "DisableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -354,21 +325,14 @@
 DisconnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableKeyRequestRequestTypeDef = TypedDict(
     "EnableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -393,44 +357,19 @@
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
     pass
 
-
-EncryptResponseTypeDef = TypedDict(
-    "EncryptResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyPairResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PrivateKeyPlaintext": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -440,44 +379,20 @@
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-
-GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyResponseTypeDef = TypedDict(
-    "GenerateDataKeyResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "Plaintext": bytes,
-        "KeyId": str,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
@@ -488,31 +403,20 @@
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-
-GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateMacRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateMacRequestRequestTypeDef",
     {
         "Message": Union[str, bytes, IO[Any], StreamingBody],
         "KeyId": str,
         "MacAlgorithm": MacAlgorithmSpecType,
     },
@@ -522,126 +426,62 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
 ):
     pass
 
-
-GenerateMacResponseTypeDef = TypedDict(
-    "GenerateMacResponseTypeDef",
-    {
-        "Mac": bytes,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateRandomResponseTypeDef = TypedDict(
-    "GenerateRandomResponseTypeDef",
-    {
-        "Plaintext": bytes,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKeyPolicyRequestRequestTypeDef = TypedDict(
     "GetKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
     },
 )
 
-GetKeyPolicyResponseTypeDef = TypedDict(
-    "GetKeyPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKeyRotationStatusRequestRequestTypeDef = TypedDict(
     "GetKeyRotationStatusRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-GetKeyRotationStatusResponseTypeDef = TypedDict(
-    "GetKeyRotationStatusResponseTypeDef",
-    {
-        "KeyRotationEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParametersForImportRequestRequestTypeDef = TypedDict(
     "GetParametersForImportRequestRequestTypeDef",
     {
         "KeyId": str,
         "WrappingAlgorithm": AlgorithmSpecType,
         "WrappingKeySpec": WrappingKeySpecType,
     },
 )
 
-GetParametersForImportResponseTypeDef = TypedDict(
-    "GetParametersForImportResponseTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": bytes,
-        "PublicKey": bytes,
-        "ParametersValidTo": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGetPublicKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalGetPublicKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
-
-GetPublicKeyResponseTypeDef = TypedDict(
-    "GetPublicKeyResponseTypeDef",
-    {
-        "KeyId": str,
-        "PublicKey": bytes,
-        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
-        "KeySpec": KeySpecType,
-        "KeyUsage": KeyUsageTypeType,
-        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
-        "SigningAlgorithms": List[SigningAlgorithmSpecType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GrantConstraintsOutputTypeDef = TypedDict(
     "GrantConstraintsOutputTypeDef",
     {
         "EncryptionContextSubset": Dict[str, str],
         "EncryptionContextEquals": Dict[str, str],
     },
     total=False,
@@ -660,21 +500,19 @@
     {
         "ValidTo": Union[datetime, str],
         "ExpirationModel": ExpirationModelTypeType,
     },
     total=False,
 )
 
-
 class ImportKeyMaterialRequestRequestTypeDef(
     _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
 ):
     pass
 
-
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -684,57 +522,24 @@
     "XksKeyConfigurationTypeTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "KeyId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAliasesRequestRequestTypeDef = TypedDict(
     "ListAliasesRequestRequestTypeDef",
     {
         "KeyId": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "GrantId": str,
-        "GranteePrincipal": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGrantsRequestListGrantsPaginateTypeDef(
-    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
-    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListGrantsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListGrantsRequestRequestTypeDef = TypedDict(
@@ -744,43 +549,19 @@
         "Marker": str,
         "GrantId": str,
         "GranteePrincipal": str,
     },
     total=False,
 )
 
-
 class ListGrantsRequestRequestTypeDef(
     _RequiredListGrantsRequestRequestTypeDef, _OptionalListGrantsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
-    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListKeyPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListKeyPoliciesRequestRequestTypeDef = TypedDict(
@@ -788,70 +569,28 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListKeyPoliciesRequestRequestTypeDef(
     _RequiredListKeyPoliciesRequestRequestTypeDef, _OptionalListKeyPoliciesRequestRequestTypeDef
 ):
     pass
 
-
-ListKeyPoliciesResponseTypeDef = TypedDict(
-    "ListKeyPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
-    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
-    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceTagsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListResourceTagsRequestRequestTypeDef = TypedDict(
@@ -859,51 +598,19 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListResourceTagsRequestRequestTypeDef(
     _RequiredListResourceTagsRequestRequestTypeDef, _OptionalListResourceTagsRequestRequestTypeDef
 ):
     pass
 
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValue": str,
-    },
-)
-
-_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "RetiringPrincipal": str,
-    },
-)
-_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
-    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRetirableGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
 _OptionalListRetirableGrantsRequestRequestTypeDef = TypedDict(
@@ -911,41 +618,29 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListRetirableGrantsRequestRequestTypeDef(
     _RequiredListRetirableGrantsRequestRequestTypeDef,
     _OptionalListRetirableGrantsRequestRequestTypeDef,
 ):
     pass
 
-
 MultiRegionKeyTypeDef = TypedDict(
     "MultiRegionKeyTypeDef",
     {
         "Arn": str,
         "Region": str,
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
 _RequiredPutKeyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -954,21 +649,19 @@
     "_OptionalPutKeyPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
-
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredReEncryptRequestRequestTypeDef = TypedDict(
     "_RequiredReEncryptRequestRequestTypeDef",
     {
         "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
         "DestinationKeyId": str,
     },
 )
@@ -982,44 +675,19 @@
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
 ):
     pass
 
-
-ReEncryptResponseTypeDef = TypedDict(
-    "ReEncryptResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "SourceKeyId": str,
-        "KeyId": str,
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
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
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
         "DryRun": bool,
@@ -1038,54 +706,39 @@
     "_OptionalRevokeGrantRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class RevokeGrantRequestRequestTypeDef(
     _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_OptionalScheduleKeyDeletionRequestRequestTypeDef",
     {
         "PendingWindowInDays": int,
     },
     total=False,
 )
 
-
 class ScheduleKeyDeletionRequestRequestTypeDef(
     _RequiredScheduleKeyDeletionRequestRequestTypeDef,
     _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
-
-ScheduleKeyDeletionResponseTypeDef = TypedDict(
-    "ScheduleKeyDeletionResponseTypeDef",
-    {
-        "KeyId": str,
-        "DeletionDate": datetime,
-        "KeyState": KeyStateType,
-        "PendingWindowInDays": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSignRequestRequestTypeDef = TypedDict(
     "_RequiredSignRequestRequestTypeDef",
     {
         "KeyId": str,
         "Message": Union[str, bytes, IO[Any], StreamingBody],
         "SigningAlgorithm": SigningAlgorithmSpecType,
     },
@@ -1096,31 +749,19 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
 ):
     pass
 
-
-SignResponseTypeDef = TypedDict(
-    "SignResponseTypeDef",
-    {
-        "KeyId": str,
-        "Signature": bytes,
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1163,31 +804,19 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
 ):
     pass
 
-
-VerifyMacResponseTypeDef = TypedDict(
-    "VerifyMacResponseTypeDef",
-    {
-        "KeyId": str,
-        "MacValid": bool,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredVerifyRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyRequestRequestTypeDef",
     {
         "KeyId": str,
         "Message": Union[str, bytes, IO[Any], StreamingBody],
         "Signature": Union[str, bytes, IO[Any], StreamingBody],
         "SigningAlgorithm": SigningAlgorithmSpecType,
@@ -1199,38 +828,246 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
 ):
     pass
 
+CancelKeyDeletionResponseTypeDef = TypedDict(
+    "CancelKeyDeletionResponseTypeDef",
+    {
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-VerifyResponseTypeDef = TypedDict(
-    "VerifyResponseTypeDef",
+CreateCustomKeyStoreResponseTypeDef = TypedDict(
+    "CreateCustomKeyStoreResponseTypeDef",
+    {
+        "CustomKeyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
+    {
+        "GrantToken": str,
+        "GrantId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DecryptResponseTypeDef = TypedDict(
+    "DecryptResponseTypeDef",
     {
         "KeyId": str,
-        "SignatureValid": bool,
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Plaintext": bytes,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "CiphertextForRecipient": bytes,
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
+EncryptResponseTypeDef = TypedDict(
+    "EncryptResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "KeyId": str,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyPairResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PrivateKeyPlaintext": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyResponseTypeDef = TypedDict(
+    "GenerateDataKeyResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "Plaintext": bytes,
+        "KeyId": str,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMacResponseTypeDef = TypedDict(
+    "GenerateMacResponseTypeDef",
+    {
+        "Mac": bytes,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateRandomResponseTypeDef = TypedDict(
+    "GenerateRandomResponseTypeDef",
+    {
+        "Plaintext": bytes,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyPolicyResponseTypeDef = TypedDict(
+    "GetKeyPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyRotationStatusResponseTypeDef = TypedDict(
+    "GetKeyRotationStatusResponseTypeDef",
+    {
+        "KeyRotationEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetParametersForImportResponseTypeDef = TypedDict(
+    "GetParametersForImportResponseTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": bytes,
+        "PublicKey": bytes,
+        "ParametersValidTo": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicKeyResponseTypeDef = TypedDict(
+    "GetPublicKeyResponseTypeDef",
+    {
+        "KeyId": str,
+        "PublicKey": bytes,
+        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
+        "KeySpec": KeySpecType,
+        "KeyUsage": KeyUsageTypeType,
+        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
+        "SigningAlgorithms": List[SigningAlgorithmSpecType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "Aliases": List[AliasListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListKeyPoliciesResponseTypeDef = TypedDict(
+    "ListKeyPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReEncryptResponseTypeDef = TypedDict(
+    "ReEncryptResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "SourceKeyId": str,
+        "KeyId": str,
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduleKeyDeletionResponseTypeDef = TypedDict(
+    "ScheduleKeyDeletionResponseTypeDef",
+    {
+        "KeyId": str,
+        "DeletionDate": datetime,
+        "KeyState": KeyStateType,
+        "PendingWindowInDays": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignResponseTypeDef = TypedDict(
+    "SignResponseTypeDef",
+    {
+        "KeyId": str,
+        "Signature": bytes,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyMacResponseTypeDef = TypedDict(
+    "VerifyMacResponseTypeDef",
+    {
+        "KeyId": str,
+        "MacValid": bool,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyResponseTypeDef = TypedDict(
+    "VerifyResponseTypeDef",
+    {
+        "KeyId": str,
+        "SignatureValid": bool,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreName": str,
@@ -1248,22 +1085,20 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
-
 class CreateCustomKeyStoreRequestRequestTypeDef(
     _RequiredCreateCustomKeyStoreRequestRequestTypeDef,
     _OptionalCreateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 _OptionalUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
@@ -1277,22 +1112,20 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
-
 class UpdateCustomKeyStoreRequestRequestTypeDef(
     _RequiredUpdateCustomKeyStoreRequestRequestTypeDef,
     _OptionalUpdateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateGrantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GranteePrincipal": str,
         "Operations": Sequence[GrantOperationType],
     },
@@ -1305,21 +1138,19 @@
         "GrantTokens": Sequence[str],
         "Name": str,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
-
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
@@ -1330,14 +1161,24 @@
         "Tags": Sequence[TagTypeDef],
         "MultiRegion": bool,
         "XksKeyId": str,
     },
     total=False,
 )
 
+ListResourceTagsResponseTypeDef = TypedDict(
+    "ListResourceTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredReplicateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateKeyRequestRequestTypeDef",
     {
         "KeyId": str,
         "ReplicaRegion": str,
     },
 )
@@ -1348,21 +1189,19 @@
         "BypassPolicyLockoutSafetyCheck": bool,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ReplicateKeyRequestRequestTypeDef(
     _RequiredReplicateKeyRequestRequestTypeDef, _OptionalReplicateKeyRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1398,21 +1237,19 @@
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -1423,22 +1260,20 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
@@ -1450,31 +1285,138 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
     pass
 
-
 GenerateRandomRequestRequestTypeDef = TypedDict(
     "GenerateRandomRequestRequestTypeDef",
     {
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
+DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    {
+        "CustomKeyStoreId": str,
+        "CustomKeyStoreName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "KeyId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "GrantId": str,
+        "GranteePrincipal": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGrantsRequestListGrantsPaginateTypeDef(
+    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
+    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
+):
+    pass
+
+_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
+    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+):
+    pass
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
+    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "RetiringPrincipal": str,
+    },
+)
+_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
+    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+):
+    pass
+
 GrantListEntryTypeDef = TypedDict(
     "GrantListEntryTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
         "Name": str,
         "CreationDate": datetime,
@@ -1489,25 +1431,15 @@
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListResourceTagsResponseTypeDef = TypedDict(
-    "ListResourceTagsResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MultiRegionConfigurationTypeDef = TypedDict(
     "MultiRegionConfigurationTypeDef",
     {
         "MultiRegionKeyType": MultiRegionKeyTypeType,
@@ -1519,25 +1451,25 @@
 
 DescribeCustomKeyStoresResponseTypeDef = TypedDict(
     "DescribeCustomKeyStoresResponseTypeDef",
     {
         "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGrantsResponseTypeDef = TypedDict(
     "ListGrantsResponseTypeDef",
     {
         "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
     "_RequiredKeyMetadataTypeDef",
     {
         "KeyId": str,
@@ -1569,37 +1501,35 @@
         "PendingDeletionWindowInDays": int,
         "MacAlgorithms": List[MacAlgorithmSpecType],
         "XksKeyConfiguration": XksKeyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class KeyMetadataTypeDef(_RequiredKeyMetadataTypeDef, _OptionalKeyMetadataTypeDef):
     pass
 
-
 CreateKeyResponseTypeDef = TypedDict(
     "CreateKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyResponseTypeDef = TypedDict(
     "DescribeKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicateKeyResponseTypeDef = TypedDict(
     "ReplicateKeyResponseTypeDef",
     {
         "ReplicaKeyMetadata": KeyMetadataTypeDef,
         "ReplicaPolicy": str,
-        "ReplicaTags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReplicaTags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.pyi` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,112 +46,112 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasListEntryTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
-    "CancelKeyDeletionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
-    "CreateCustomKeyStoreResponseTypeDef",
     "GrantConstraintsTypeDef",
-    "CreateGrantResponseTypeDef",
     "TagTypeDef",
     "XksProxyConfigurationTypeTypeDef",
     "RecipientInfoTypeDef",
-    "DecryptResponseTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCustomKeyStoreRequestRequestTypeDef",
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DisableKeyRequestRequestTypeDef",
     "DisableKeyRotationRequestRequestTypeDef",
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableKeyRequestRequestTypeDef",
     "EnableKeyRotationRequestRequestTypeDef",
     "EncryptRequestRequestTypeDef",
-    "EncryptResponseTypeDef",
-    "GenerateDataKeyPairResponseTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    "GenerateDataKeyResponseTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
     "GenerateMacRequestRequestTypeDef",
-    "GenerateMacResponseTypeDef",
-    "GenerateRandomResponseTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
-    "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
-    "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
-    "GetParametersForImportResponseTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
-    "GetPublicKeyResponseTypeDef",
     "GrantConstraintsOutputTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListGrantsRequestRequestTypeDef",
-    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
-    "ListKeyPoliciesResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
-    "PaginatorConfigTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
     "ReEncryptRequestRequestTypeDef",
-    "ReEncryptResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
-    "ScheduleKeyDeletionResponseTypeDef",
     "SignRequestRequestTypeDef",
-    "SignResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
     "VerifyMacRequestRequestTypeDef",
-    "VerifyMacResponseTypeDef",
     "VerifyRequestRequestTypeDef",
-    "VerifyResponseTypeDef",
+    "CancelKeyDeletionResponseTypeDef",
+    "CreateCustomKeyStoreResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "DecryptResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EncryptResponseTypeDef",
+    "GenerateDataKeyPairResponseTypeDef",
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    "GenerateDataKeyResponseTypeDef",
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
+    "GenerateMacResponseTypeDef",
+    "GenerateRandomResponseTypeDef",
+    "GetKeyPolicyResponseTypeDef",
+    "GetKeyRotationStatusResponseTypeDef",
+    "GetParametersForImportResponseTypeDef",
+    "GetPublicKeyResponseTypeDef",
     "ListAliasesResponseTypeDef",
+    "ListKeyPoliciesResponseTypeDef",
+    "ReEncryptResponseTypeDef",
+    "ScheduleKeyDeletionResponseTypeDef",
+    "SignResponseTypeDef",
+    "VerifyMacResponseTypeDef",
+    "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
     "CreateKeyRequestRequestTypeDef",
+    "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListGrantsRequestListGrantsPaginateTypeDef",
+    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "GrantListEntryTypeDef",
     "ListKeysResponseTypeDef",
-    "ListResourceTagsResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
     "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
@@ -172,19 +172,22 @@
 CancelKeyDeletionRequestRequestTypeDef = TypedDict(
     "CancelKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-CancelKeyDeletionResponseTypeDef = TypedDict(
-    "CancelKeyDeletionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
@@ -203,40 +206,23 @@
     "XksProxyAuthenticationCredentialTypeTypeDef",
     {
         "AccessKeyId": str,
         "RawSecretAccessKey": str,
     },
 )
 
-CreateCustomKeyStoreResponseTypeDef = TypedDict(
-    "CreateCustomKeyStoreResponseTypeDef",
-    {
-        "CustomKeyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GrantConstraintsTypeDef = TypedDict(
     "GrantConstraintsTypeDef",
     {
         "EncryptionContextSubset": Mapping[str, str],
         "EncryptionContextEquals": Mapping[str, str],
     },
     total=False,
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantToken": str,
-        "GrantId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "TagKey": str,
         "TagValue": str,
     },
 )
@@ -258,25 +244,14 @@
     {
         "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
         "AttestationDocument": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-DecryptResponseTypeDef = TypedDict(
-    "DecryptResponseTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": bytes,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -290,20 +265,20 @@
 DeleteImportedKeyMaterialRequestRequestTypeDef = TypedDict(
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CustomKeyStoreId": str,
-        "CustomKeyStoreName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCustomKeyStoresRequestRequestTypeDef = TypedDict(
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     {
@@ -325,19 +300,21 @@
     "_OptionalDescribeKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeKeyRequestRequestTypeDef(
     _RequiredDescribeKeyRequestRequestTypeDef, _OptionalDescribeKeyRequestRequestTypeDef
 ):
     pass
 
+
 DisableKeyRequestRequestTypeDef = TypedDict(
     "DisableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -351,21 +328,14 @@
 DisconnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableKeyRequestRequestTypeDef = TypedDict(
     "EnableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -390,41 +360,20 @@
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
     pass
 
-EncryptResponseTypeDef = TypedDict(
-    "EncryptResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyPairResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PrivateKeyPlaintext": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
@@ -435,41 +384,21 @@
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyResponseTypeDef = TypedDict(
-    "GenerateDataKeyResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "Plaintext": bytes,
-        "KeyId": str,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -481,28 +410,21 @@
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGenerateMacRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateMacRequestRequestTypeDef",
     {
         "Message": Union[str, bytes, IO[Any], StreamingBody],
         "KeyId": str,
         "MacAlgorithm": MacAlgorithmSpecType,
@@ -513,121 +435,65 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
 ):
     pass
 
-GenerateMacResponseTypeDef = TypedDict(
-    "GenerateMacResponseTypeDef",
-    {
-        "Mac": bytes,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateRandomResponseTypeDef = TypedDict(
-    "GenerateRandomResponseTypeDef",
-    {
-        "Plaintext": bytes,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetKeyPolicyRequestRequestTypeDef = TypedDict(
     "GetKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
     },
 )
 
-GetKeyPolicyResponseTypeDef = TypedDict(
-    "GetKeyPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKeyRotationStatusRequestRequestTypeDef = TypedDict(
     "GetKeyRotationStatusRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-GetKeyRotationStatusResponseTypeDef = TypedDict(
-    "GetKeyRotationStatusResponseTypeDef",
-    {
-        "KeyRotationEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParametersForImportRequestRequestTypeDef = TypedDict(
     "GetParametersForImportRequestRequestTypeDef",
     {
         "KeyId": str,
         "WrappingAlgorithm": AlgorithmSpecType,
         "WrappingKeySpec": WrappingKeySpecType,
     },
 )
 
-GetParametersForImportResponseTypeDef = TypedDict(
-    "GetParametersForImportResponseTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": bytes,
-        "PublicKey": bytes,
-        "ParametersValidTo": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGetPublicKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalGetPublicKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
-GetPublicKeyResponseTypeDef = TypedDict(
-    "GetPublicKeyResponseTypeDef",
-    {
-        "KeyId": str,
-        "PublicKey": bytes,
-        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
-        "KeySpec": KeySpecType,
-        "KeyUsage": KeyUsageTypeType,
-        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
-        "SigningAlgorithms": List[SigningAlgorithmSpecType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GrantConstraintsOutputTypeDef = TypedDict(
     "GrantConstraintsOutputTypeDef",
     {
         "EncryptionContextSubset": Dict[str, str],
         "EncryptionContextEquals": Dict[str, str],
     },
@@ -647,19 +513,21 @@
     {
         "ValidTo": Union[datetime, str],
         "ExpirationModel": ExpirationModelTypeType,
     },
     total=False,
 )
 
+
 class ImportKeyMaterialRequestRequestTypeDef(
     _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
 ):
     pass
 
+
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -669,55 +537,24 @@
     "XksKeyConfigurationTypeTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "KeyId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAliasesRequestRequestTypeDef = TypedDict(
     "ListAliasesRequestRequestTypeDef",
     {
         "KeyId": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "GrantId": str,
-        "GranteePrincipal": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGrantsRequestListGrantsPaginateTypeDef(
-    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
-    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListGrantsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListGrantsRequestRequestTypeDef = TypedDict(
@@ -727,38 +564,20 @@
         "Marker": str,
         "GrantId": str,
         "GranteePrincipal": str,
     },
     total=False,
 )
 
+
 class ListGrantsRequestRequestTypeDef(
     _RequiredListGrantsRequestRequestTypeDef, _OptionalListGrantsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
-    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredListKeyPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -767,66 +586,30 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListKeyPoliciesRequestRequestTypeDef(
     _RequiredListKeyPoliciesRequestRequestTypeDef, _OptionalListKeyPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListKeyPoliciesResponseTypeDef = TypedDict(
-    "ListKeyPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
-    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
-    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceTagsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListResourceTagsRequestRequestTypeDef = TypedDict(
@@ -834,46 +617,20 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListResourceTagsRequestRequestTypeDef(
     _RequiredListResourceTagsRequestRequestTypeDef, _OptionalListResourceTagsRequestRequestTypeDef
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValue": str,
-    },
-)
-
-_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "RetiringPrincipal": str,
-    },
-)
-_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
-    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-):
-    pass
 
 _RequiredListRetirableGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
@@ -882,39 +639,31 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListRetirableGrantsRequestRequestTypeDef(
     _RequiredListRetirableGrantsRequestRequestTypeDef,
     _OptionalListRetirableGrantsRequestRequestTypeDef,
 ):
     pass
 
+
 MultiRegionKeyTypeDef = TypedDict(
     "MultiRegionKeyTypeDef",
     {
         "Arn": str,
         "Region": str,
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
 _RequiredPutKeyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -923,19 +672,21 @@
     "_OptionalPutKeyPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
+
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredReEncryptRequestRequestTypeDef = TypedDict(
     "_RequiredReEncryptRequestRequestTypeDef",
     {
         "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
         "DestinationKeyId": str,
     },
 )
@@ -949,41 +700,20 @@
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
 ):
     pass
 
-ReEncryptResponseTypeDef = TypedDict(
-    "ReEncryptResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "SourceKeyId": str,
-        "KeyId": str,
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
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
 
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
@@ -1003,49 +733,42 @@
     "_OptionalRevokeGrantRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class RevokeGrantRequestRequestTypeDef(
     _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_OptionalScheduleKeyDeletionRequestRequestTypeDef",
     {
         "PendingWindowInDays": int,
     },
     total=False,
 )
 
+
 class ScheduleKeyDeletionRequestRequestTypeDef(
     _RequiredScheduleKeyDeletionRequestRequestTypeDef,
     _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
-ScheduleKeyDeletionResponseTypeDef = TypedDict(
-    "ScheduleKeyDeletionResponseTypeDef",
-    {
-        "KeyId": str,
-        "DeletionDate": datetime,
-        "KeyState": KeyStateType,
-        "PendingWindowInDays": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredSignRequestRequestTypeDef = TypedDict(
     "_RequiredSignRequestRequestTypeDef",
     {
         "KeyId": str,
         "Message": Union[str, bytes, IO[Any], StreamingBody],
         "SigningAlgorithm": SigningAlgorithmSpecType,
@@ -1057,28 +780,20 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
 ):
     pass
 
-SignResponseTypeDef = TypedDict(
-    "SignResponseTypeDef",
-    {
-        "KeyId": str,
-        "Signature": bytes,
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "TagKeys": Sequence[str],
     },
@@ -1122,28 +837,20 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
 ):
     pass
 
-VerifyMacResponseTypeDef = TypedDict(
-    "VerifyMacResponseTypeDef",
-    {
-        "KeyId": str,
-        "MacValid": bool,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredVerifyRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyRequestRequestTypeDef",
     {
         "KeyId": str,
         "Message": Union[str, bytes, IO[Any], StreamingBody],
         "Signature": Union[str, bytes, IO[Any], StreamingBody],
@@ -1156,36 +863,248 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
 ):
     pass
 
-VerifyResponseTypeDef = TypedDict(
-    "VerifyResponseTypeDef",
+
+CancelKeyDeletionResponseTypeDef = TypedDict(
+    "CancelKeyDeletionResponseTypeDef",
     {
         "KeyId": str,
-        "SignatureValid": bool,
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomKeyStoreResponseTypeDef = TypedDict(
+    "CreateCustomKeyStoreResponseTypeDef",
+    {
+        "CustomKeyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
+    {
+        "GrantToken": str,
+        "GrantId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DecryptResponseTypeDef = TypedDict(
+    "DecryptResponseTypeDef",
+    {
+        "KeyId": str,
+        "Plaintext": bytes,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "CiphertextForRecipient": bytes,
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
+EncryptResponseTypeDef = TypedDict(
+    "EncryptResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "KeyId": str,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyPairResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PrivateKeyPlaintext": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyResponseTypeDef = TypedDict(
+    "GenerateDataKeyResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "Plaintext": bytes,
+        "KeyId": str,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMacResponseTypeDef = TypedDict(
+    "GenerateMacResponseTypeDef",
+    {
+        "Mac": bytes,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateRandomResponseTypeDef = TypedDict(
+    "GenerateRandomResponseTypeDef",
+    {
+        "Plaintext": bytes,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyPolicyResponseTypeDef = TypedDict(
+    "GetKeyPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyRotationStatusResponseTypeDef = TypedDict(
+    "GetKeyRotationStatusResponseTypeDef",
+    {
+        "KeyRotationEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetParametersForImportResponseTypeDef = TypedDict(
+    "GetParametersForImportResponseTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": bytes,
+        "PublicKey": bytes,
+        "ParametersValidTo": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicKeyResponseTypeDef = TypedDict(
+    "GetPublicKeyResponseTypeDef",
+    {
+        "KeyId": str,
+        "PublicKey": bytes,
+        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
+        "KeySpec": KeySpecType,
+        "KeyUsage": KeyUsageTypeType,
+        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
+        "SigningAlgorithms": List[SigningAlgorithmSpecType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "Aliases": List[AliasListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListKeyPoliciesResponseTypeDef = TypedDict(
+    "ListKeyPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReEncryptResponseTypeDef = TypedDict(
+    "ReEncryptResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "SourceKeyId": str,
+        "KeyId": str,
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduleKeyDeletionResponseTypeDef = TypedDict(
+    "ScheduleKeyDeletionResponseTypeDef",
+    {
+        "KeyId": str,
+        "DeletionDate": datetime,
+        "KeyState": KeyStateType,
+        "PendingWindowInDays": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignResponseTypeDef = TypedDict(
+    "SignResponseTypeDef",
+    {
+        "KeyId": str,
+        "Signature": bytes,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyMacResponseTypeDef = TypedDict(
+    "VerifyMacResponseTypeDef",
+    {
+        "KeyId": str,
+        "MacValid": bool,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyResponseTypeDef = TypedDict(
+    "VerifyResponseTypeDef",
+    {
+        "KeyId": str,
+        "SignatureValid": bool,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreName": str,
@@ -1203,20 +1122,22 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
+
 class CreateCustomKeyStoreRequestRequestTypeDef(
     _RequiredCreateCustomKeyStoreRequestRequestTypeDef,
     _OptionalCreateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 _OptionalUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
@@ -1230,20 +1151,22 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
+
 class UpdateCustomKeyStoreRequestRequestTypeDef(
     _RequiredUpdateCustomKeyStoreRequestRequestTypeDef,
     _OptionalUpdateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateGrantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GranteePrincipal": str,
         "Operations": Sequence[GrantOperationType],
     },
@@ -1256,19 +1179,21 @@
         "GrantTokens": Sequence[str],
         "Name": str,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
+
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
@@ -1279,14 +1204,24 @@
         "Tags": Sequence[TagTypeDef],
         "MultiRegion": bool,
         "XksKeyId": str,
     },
     total=False,
 )
 
+ListResourceTagsResponseTypeDef = TypedDict(
+    "ListResourceTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredReplicateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateKeyRequestRequestTypeDef",
     {
         "KeyId": str,
         "ReplicaRegion": str,
     },
 )
@@ -1297,19 +1232,21 @@
         "BypassPolicyLockoutSafetyCheck": bool,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ReplicateKeyRequestRequestTypeDef(
     _RequiredReplicateKeyRequestRequestTypeDef, _OptionalReplicateKeyRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1345,19 +1282,21 @@
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -1368,20 +1307,22 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
@@ -1393,29 +1334,148 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
     pass
 
+
 GenerateRandomRequestRequestTypeDef = TypedDict(
     "GenerateRandomRequestRequestTypeDef",
     {
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
+DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    {
+        "CustomKeyStoreId": str,
+        "CustomKeyStoreName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "KeyId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "GrantId": str,
+        "GranteePrincipal": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGrantsRequestListGrantsPaginateTypeDef(
+    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
+    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
+    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+):
+    pass
+
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
+    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "RetiringPrincipal": str,
+    },
+)
+_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
+    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+):
+    pass
+
+
 GrantListEntryTypeDef = TypedDict(
     "GrantListEntryTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
         "Name": str,
         "CreationDate": datetime,
@@ -1430,25 +1490,15 @@
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListResourceTagsResponseTypeDef = TypedDict(
-    "ListResourceTagsResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MultiRegionConfigurationTypeDef = TypedDict(
     "MultiRegionConfigurationTypeDef",
     {
         "MultiRegionKeyType": MultiRegionKeyTypeType,
@@ -1460,25 +1510,25 @@
 
 DescribeCustomKeyStoresResponseTypeDef = TypedDict(
     "DescribeCustomKeyStoresResponseTypeDef",
     {
         "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGrantsResponseTypeDef = TypedDict(
     "ListGrantsResponseTypeDef",
     {
         "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
     "_RequiredKeyMetadataTypeDef",
     {
         "KeyId": str,
@@ -1510,35 +1560,37 @@
         "PendingDeletionWindowInDays": int,
         "MacAlgorithms": List[MacAlgorithmSpecType],
         "XksKeyConfiguration": XksKeyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class KeyMetadataTypeDef(_RequiredKeyMetadataTypeDef, _OptionalKeyMetadataTypeDef):
     pass
 
+
 CreateKeyResponseTypeDef = TypedDict(
     "CreateKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyResponseTypeDef = TypedDict(
     "DescribeKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicateKeyResponseTypeDef = TypedDict(
     "ReplicateKeyResponseTypeDef",
     {
         "ReplicaKeyMetadata": KeyMetadataTypeDef,
         "ReplicaPolicy": str,
-        "ReplicaTags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReplicaTags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/PKG-INFO` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.28.12
-Summary: Type annotations for boto3.KMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,109 +365,108 @@
 `mypy_boto3_kms.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kms.type_defs import (
     AliasListEntryTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
-    CancelKeyDeletionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
-    CreateCustomKeyStoreResponseTypeDef,
     GrantConstraintsTypeDef,
-    CreateGrantResponseTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
     RecipientInfoTypeDef,
-    DecryptResponseTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
-    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
     EncryptRequestRequestTypeDef,
-    EncryptResponseTypeDef,
-    GenerateDataKeyPairResponseTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
-    GenerateDataKeyResponseTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacRequestRequestTypeDef,
-    GenerateMacResponseTypeDef,
-    GenerateRandomResponseTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
-    GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
-    GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
-    GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
-    GetPublicKeyResponseTypeDef,
     GrantConstraintsOutputTypeDef,
     ImportKeyMaterialRequestRequestTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
-    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
-    ListKeyPoliciesResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
-    PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
     ReEncryptRequestRequestTypeDef,
-    ReEncryptResponseTypeDef,
-    ResponseMetadataTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    ScheduleKeyDeletionResponseTypeDef,
     SignRequestRequestTypeDef,
-    SignResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
-    VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
-    VerifyResponseTypeDef,
+    CancelKeyDeletionResponseTypeDef,
+    CreateCustomKeyStoreResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    DecryptResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptResponseTypeDef,
+    GenerateDataKeyPairResponseTypeDef,
+    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
+    GenerateDataKeyResponseTypeDef,
+    GenerateDataKeyWithoutPlaintextResponseTypeDef,
+    GenerateMacResponseTypeDef,
+    GenerateRandomResponseTypeDef,
+    GetKeyPolicyResponseTypeDef,
+    GetKeyRotationStatusResponseTypeDef,
+    GetParametersForImportResponseTypeDef,
+    GetPublicKeyResponseTypeDef,
     ListAliasesResponseTypeDef,
+    ListKeyPoliciesResponseTypeDef,
+    ReEncryptResponseTypeDef,
+    ScheduleKeyDeletionResponseTypeDef,
+    SignResponseTypeDef,
+    VerifyMacResponseTypeDef,
+    VerifyResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
+    ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
+    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListGrantsRequestListGrantsPaginateTypeDef,
+    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     GrantListEntryTypeDef,
     ListKeysResponseTypeDef,
-    ListResourceTagsResponseTypeDef,
     MultiRegionConfigurationTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
```

### Comparing `mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/SOURCES.txt` & `mypy-boto3-kms-1.28.15/mypy_boto3_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.12/setup.py` & `mypy-boto3-kms-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kms",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KMS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.KMS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

