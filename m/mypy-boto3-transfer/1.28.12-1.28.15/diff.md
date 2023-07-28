# Comparing `tmp/mypy-boto3-transfer-1.28.12.tar.gz` & `tmp/mypy-boto3-transfer-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.28.12.tar", last modified: Thu Jul 27 11:49:47 2023, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.28.15.tar", last modified: Fri Jul 28 20:43:53 2023, max compression
```

## Comparing `mypy-boto3-transfer-1.28.12.tar` & `mypy-boto3-transfer-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.153460 mypy-boto3-transfer-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-07-27 11:49:47.145460 mypy-boto3-transfer-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.145460 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-27 11:48:10.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-27 11:48:10.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66431 2023-07-27 11:48:12.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66336 2023-07-27 11:48:11.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.145460 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:46.000000 mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:47.153460 mypy-boto3-transfer-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:09.000000 mypy-boto3-transfer-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.890003 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47000 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62680 2023-07-28 20:40:51.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62587 2023-07-28 20:40:50.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-28 20:40:49.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:53.000000 mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:53.898003 mypy-boto3-transfer-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:40:48.000000 mypy-boto3-transfer-1.28.15/setup.py
```

### Comparing `mypy-boto3-transfer-1.28.12/LICENSE` & `mypy-boto3-transfer-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/PKG-INFO` & `mypy-boto3-transfer-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-transfer
-Version: 1.28.12
-Summary: Type annotations for boto3.Transfer 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 transfer type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-transfer"></a>
 
 # mypy-boto3-transfer
 
 [![PyPI - mypy-boto3-transfer](https://img.shields.io/pypi/v/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -404,35 +372,32 @@
 ### Typed dictionaries
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
-    As2ConnectorConfigOutputTypeDef,
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     SftpConnectorConfigTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CustomStepDetailsOutputTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
     DeleteSshPublicKeyRequestRequestTypeDef,
-    DeleteStepDetailsOutputTypeDef,
     DeleteStepDetailsTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DescribeAccessRequestRequestTypeDef,
     DescribeAgreementRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -441,29 +406,24 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
-    HomeDirectoryMapEntryOutputTypeDef,
     PosixProfileOutputTypeDef,
-    TagOutputTypeDef,
     SftpConnectorConfigOutputTypeDef,
     LoggingConfigurationTypeDef,
     EndpointDetailsOutputTypeDef,
-    IdentityProviderDetailsOutputTypeDef,
     ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
-    EfsFileLocationOutputTypeDef,
     EfsFileLocationTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    S3InputFileLocationOutputTypeDef,
     S3InputFileLocationTypeDef,
     PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
     ListCertificatesRequestRequestTypeDef,
@@ -479,29 +439,27 @@
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    S3TagOutputTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgreementRequestRequestTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    WorkflowDetailOutputTypeDef,
     WorkflowDetailTypeDef,
     CreateAccessRequestRequestTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateAccessResponseTypeDef,
     CreateAgreementResponseTypeDef,
     CreateConnectorResponseTypeDef,
@@ -524,33 +482,32 @@
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DescribedAgreementTypeDef,
+    DescribedCertificateTypeDef,
+    DescribedHostKeyTypeDef,
+    DescribedProfileTypeDef,
     ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
     DescribedAccessTypeDef,
-    DescribedAgreementTypeDef,
-    DescribedCertificateTypeDef,
-    DescribedHostKeyTypeDef,
-    DescribedProfileTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribedConnectorTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
-    InputFileLocationOutputTypeDef,
     InputFileLocationTypeDef,
     ListAccessesRequestListAccessesPaginateTypeDef,
     ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListProfilesRequestListProfilesPaginateTypeDef,
@@ -569,24 +526,22 @@
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
     WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
-    DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeAccessResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
-    CopyStepDetailsOutputTypeDef,
-    DecryptStepDetailsOutputTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
     DescribedServerTypeDef,
     CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     DescribedExecutionTypeDef,
@@ -597,15 +552,15 @@
     DescribeExecutionResponseTypeDef,
     DescribedWorkflowTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     DescribeWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigOutputTypeDef:
+def get_structure() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.12/README.md` & `mypy-boto3-transfer-1.28.15/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-transfer
+Version: 1.28.15
+Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 transfer type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-transfer"></a>
 
 # mypy-boto3-transfer
 
 [![PyPI - mypy-boto3-transfer](https://img.shields.io/pypi/v/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,35 +404,32 @@
 ### Typed dictionaries
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
-    As2ConnectorConfigOutputTypeDef,
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     SftpConnectorConfigTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CustomStepDetailsOutputTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
     DeleteSshPublicKeyRequestRequestTypeDef,
-    DeleteStepDetailsOutputTypeDef,
     DeleteStepDetailsTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DescribeAccessRequestRequestTypeDef,
     DescribeAgreementRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -409,29 +438,24 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
-    HomeDirectoryMapEntryOutputTypeDef,
     PosixProfileOutputTypeDef,
-    TagOutputTypeDef,
     SftpConnectorConfigOutputTypeDef,
     LoggingConfigurationTypeDef,
     EndpointDetailsOutputTypeDef,
-    IdentityProviderDetailsOutputTypeDef,
     ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
-    EfsFileLocationOutputTypeDef,
     EfsFileLocationTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    S3InputFileLocationOutputTypeDef,
     S3InputFileLocationTypeDef,
     PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
     ListCertificatesRequestRequestTypeDef,
@@ -447,29 +471,27 @@
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    S3TagOutputTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgreementRequestRequestTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    WorkflowDetailOutputTypeDef,
     WorkflowDetailTypeDef,
     CreateAccessRequestRequestTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateAccessResponseTypeDef,
     CreateAgreementResponseTypeDef,
     CreateConnectorResponseTypeDef,
@@ -492,33 +514,32 @@
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DescribedAgreementTypeDef,
+    DescribedCertificateTypeDef,
+    DescribedHostKeyTypeDef,
+    DescribedProfileTypeDef,
     ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
     DescribedAccessTypeDef,
-    DescribedAgreementTypeDef,
-    DescribedCertificateTypeDef,
-    DescribedHostKeyTypeDef,
-    DescribedProfileTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribedConnectorTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
-    InputFileLocationOutputTypeDef,
     InputFileLocationTypeDef,
     ListAccessesRequestListAccessesPaginateTypeDef,
     ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListProfilesRequestListProfilesPaginateTypeDef,
@@ -537,24 +558,22 @@
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
     WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
-    DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeAccessResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
-    CopyStepDetailsOutputTypeDef,
-    DecryptStepDetailsOutputTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
     DescribedServerTypeDef,
     CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     DescribedExecutionTypeDef,
@@ -565,15 +584,15 @@
     DescribeExecutionResponseTypeDef,
     DescribedWorkflowTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     DescribeWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigOutputTypeDef:
+def get_structure() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Transfer 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transfer service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transfer.type_defs import As2ConnectorConfigOutputTypeDef
+    from mypy_boto3_transfer.type_defs import As2ConnectorConfigTypeDef
 
-    data: As2ConnectorConfigOutputTypeDef = {...}
+    data: As2ConnectorConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -49,35 +49,32 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "As2ConnectorConfigOutputTypeDef",
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "SftpConnectorConfigTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
-    "CustomStepDetailsOutputTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
     "DeleteHostKeyRequestRequestTypeDef",
     "DeleteProfileRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
     "DeleteSshPublicKeyRequestRequestTypeDef",
-    "DeleteStepDetailsOutputTypeDef",
     "DeleteStepDetailsTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DescribeAccessRequestRequestTypeDef",
     "DescribeAgreementRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
@@ -86,29 +83,24 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
-    "HomeDirectoryMapEntryOutputTypeDef",
     "PosixProfileOutputTypeDef",
-    "TagOutputTypeDef",
     "SftpConnectorConfigOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "EndpointDetailsOutputTypeDef",
-    "IdentityProviderDetailsOutputTypeDef",
     "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
-    "EfsFileLocationOutputTypeDef",
     "EfsFileLocationTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
-    "S3InputFileLocationOutputTypeDef",
     "S3InputFileLocationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
     "ListCertificatesRequestRequestTypeDef",
@@ -124,29 +116,27 @@
     "ListServersRequestRequestTypeDef",
     "ListedServerTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
-    "S3TagOutputTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
-    "WorkflowDetailOutputTypeDef",
     "WorkflowDetailTypeDef",
     "CreateAccessRequestRequestTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateAccessResponseTypeDef",
     "CreateAgreementResponseTypeDef",
     "CreateConnectorResponseTypeDef",
@@ -169,33 +159,32 @@
     "UpdateHostKeyResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "UpdateServerResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DescribedAgreementTypeDef",
+    "DescribedCertificateTypeDef",
+    "DescribedHostKeyTypeDef",
+    "DescribedProfileTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConnectorRequestRequestTypeDef",
     "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
     "DescribedAccessTypeDef",
-    "DescribedAgreementTypeDef",
-    "DescribedCertificateTypeDef",
-    "DescribedHostKeyTypeDef",
-    "DescribedProfileTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribedConnectorTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
-    "InputFileLocationOutputTypeDef",
     "InputFileLocationTypeDef",
     "ListAccessesRequestListAccessesPaginateTypeDef",
     "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListProfilesRequestListProfilesPaginateTypeDef",
@@ -214,24 +203,22 @@
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
     "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
-    "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
+    "DescribeAccessResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
-    "CopyStepDetailsOutputTypeDef",
-    "DecryptStepDetailsOutputTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
     "DescribedServerTypeDef",
     "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
     "DescribedExecutionTypeDef",
@@ -241,30 +228,14 @@
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
     "DescribedWorkflowTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "DescribeWorkflowResponseTypeDef",
 )
 
-As2ConnectorConfigOutputTypeDef = TypedDict(
-    "As2ConnectorConfigOutputTypeDef",
-    {
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "MessageSubject": str,
-        "Compression": CompressionEnumType,
-        "EncryptionAlgorithm": EncryptionAlgType,
-        "SigningAlgorithm": SigningAlgType,
-        "MdnSigningAlgorithm": MdnSigningAlgType,
-        "MdnResponse": MdnResponseType,
-        "BasicAuthSecretId": str,
-    },
-    total=False,
-)
-
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "MessageSubject": str,
         "Compression": CompressionEnumType,
@@ -364,25 +335,14 @@
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": Sequence[Literal["HTTP"]],
     },
     total=False,
 )
 
-CustomStepDetailsOutputTypeDef = TypedDict(
-    "CustomStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Target": str,
-        "TimeoutSeconds": int,
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
         "Target": str,
         "TimeoutSeconds": int,
         "SourceFileLocation": str,
@@ -447,23 +407,14 @@
     {
         "ServerId": str,
         "SshPublicKeyId": str,
         "UserName": str,
     },
 )
 
-DeleteStepDetailsOutputTypeDef = TypedDict(
-    "DeleteStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
 DeleteStepDetailsTypeDef = TypedDict(
     "DeleteStepDetailsTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
     },
     total=False,
@@ -596,22 +547,14 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
-HomeDirectoryMapEntryOutputTypeDef = TypedDict(
-    "HomeDirectoryMapEntryOutputTypeDef",
-    {
-        "Entry": str,
-        "Target": str,
-    },
-)
-
 _RequiredPosixProfileOutputTypeDef = TypedDict(
     "_RequiredPosixProfileOutputTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
@@ -626,22 +569,14 @@
 
 class PosixProfileOutputTypeDef(
     _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 SftpConnectorConfigOutputTypeDef = TypedDict(
     "SftpConnectorConfigOutputTypeDef",
     {
         "UserSecretId": str,
         "TrustedHostKeys": List[str],
     },
     total=False,
@@ -664,26 +599,14 @@
         "VpcEndpointId": str,
         "VpcId": str,
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-IdentityProviderDetailsOutputTypeDef = TypedDict(
-    "IdentityProviderDetailsOutputTypeDef",
-    {
-        "Url": str,
-        "InvocationRole": str,
-        "DirectoryId": str,
-        "Function": str,
-        "SftpAuthenticationMethods": SftpAuthenticationMethodsType,
-    },
-    total=False,
-)
-
 ProtocolDetailsOutputTypeDef = TypedDict(
     "ProtocolDetailsOutputTypeDef",
     {
         "PassiveIp": str,
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": List[Literal["HTTP"]],
@@ -696,23 +619,14 @@
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
 )
 
-EfsFileLocationOutputTypeDef = TypedDict(
-    "EfsFileLocationOutputTypeDef",
-    {
-        "FileSystemId": str,
-        "Path": str,
-    },
-    total=False,
-)
-
 EfsFileLocationTypeDef = TypedDict(
     "EfsFileLocationTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
     },
     total=False,
@@ -742,23 +656,14 @@
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
 )
 
-S3InputFileLocationOutputTypeDef = TypedDict(
-    "S3InputFileLocationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-    total=False,
-)
-
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
@@ -1100,22 +1005,14 @@
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
     },
     total=False,
 )
 
-S3TagOutputTypeDef = TypedDict(
-    "S3TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -1304,22 +1201,14 @@
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
 
-WorkflowDetailOutputTypeDef = TypedDict(
-    "WorkflowDetailOutputTypeDef",
-    {
-        "WorkflowId": str,
-        "ExecutionRole": str,
-    },
-)
-
 WorkflowDetailTypeDef = TypedDict(
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
@@ -1677,14 +1566,123 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredDescribedAgreementTypeDef = TypedDict(
+    "_RequiredDescribedAgreementTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedAgreementTypeDef = TypedDict(
+    "_OptionalDescribedAgreementTypeDef",
+    {
+        "AgreementId": str,
+        "Description": str,
+        "Status": AgreementStatusTypeType,
+        "ServerId": str,
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "BaseDirectory": str,
+        "AccessRole": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class DescribedAgreementTypeDef(
+    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
+):
+    pass
+
+
+_RequiredDescribedCertificateTypeDef = TypedDict(
+    "_RequiredDescribedCertificateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedCertificateTypeDef = TypedDict(
+    "_OptionalDescribedCertificateTypeDef",
+    {
+        "CertificateId": str,
+        "Usage": CertificateUsageTypeType,
+        "Status": CertificateStatusTypeType,
+        "Certificate": str,
+        "CertificateChain": str,
+        "ActiveDate": datetime,
+        "InactiveDate": datetime,
+        "Serial": str,
+        "NotBeforeDate": datetime,
+        "NotAfterDate": datetime,
+        "Type": CertificateTypeType,
+        "Description": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class DescribedCertificateTypeDef(
+    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
+):
+    pass
+
+
+_RequiredDescribedHostKeyTypeDef = TypedDict(
+    "_RequiredDescribedHostKeyTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedHostKeyTypeDef = TypedDict(
+    "_OptionalDescribedHostKeyTypeDef",
+    {
+        "HostKeyId": str,
+        "HostKeyFingerprint": str,
+        "Description": str,
+        "Type": str,
+        "DateImported": datetime,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
+    pass
+
+
+_RequiredDescribedProfileTypeDef = TypedDict(
+    "_RequiredDescribedProfileTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedProfileTypeDef = TypedDict(
+    "_OptionalDescribedProfileTypeDef",
+    {
+        "ProfileId": str,
+        "ProfileType": ProfileTypeType,
+        "As2Id": str,
+        "CertificateIds": List[str],
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
+    pass
+
+
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
         "Usage": CertificateUsageTypeType,
         "Certificate": str,
     },
 )
@@ -1727,14 +1725,24 @@
 
 class ImportHostKeyRequestRequestTypeDef(
     _RequiredImportHostKeyRequestRequestTypeDef, _OptionalImportHostKeyRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Arn": str,
+        "NextToken": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1841,158 +1849,39 @@
     pass
 
 
 DescribedAccessTypeDef = TypedDict(
     "DescribedAccessTypeDef",
     {
         "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "ExternalId": str,
     },
     total=False,
 )
 
-_RequiredDescribedAgreementTypeDef = TypedDict(
-    "_RequiredDescribedAgreementTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedAgreementTypeDef = TypedDict(
-    "_OptionalDescribedAgreementTypeDef",
-    {
-        "AgreementId": str,
-        "Description": str,
-        "Status": AgreementStatusTypeType,
-        "ServerId": str,
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "BaseDirectory": str,
-        "AccessRole": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class DescribedAgreementTypeDef(
-    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
-):
-    pass
-
-
-_RequiredDescribedCertificateTypeDef = TypedDict(
-    "_RequiredDescribedCertificateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedCertificateTypeDef = TypedDict(
-    "_OptionalDescribedCertificateTypeDef",
-    {
-        "CertificateId": str,
-        "Usage": CertificateUsageTypeType,
-        "Status": CertificateStatusTypeType,
-        "Certificate": str,
-        "CertificateChain": str,
-        "ActiveDate": datetime,
-        "InactiveDate": datetime,
-        "Serial": str,
-        "NotBeforeDate": datetime,
-        "NotAfterDate": datetime,
-        "Type": CertificateTypeType,
-        "Description": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class DescribedCertificateTypeDef(
-    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
-):
-    pass
-
-
-_RequiredDescribedHostKeyTypeDef = TypedDict(
-    "_RequiredDescribedHostKeyTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedHostKeyTypeDef = TypedDict(
-    "_OptionalDescribedHostKeyTypeDef",
-    {
-        "HostKeyId": str,
-        "HostKeyFingerprint": str,
-        "Description": str,
-        "Type": str,
-        "DateImported": datetime,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
-    pass
-
-
-_RequiredDescribedProfileTypeDef = TypedDict(
-    "_RequiredDescribedProfileTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedProfileTypeDef = TypedDict(
-    "_OptionalDescribedProfileTypeDef",
-    {
-        "ProfileId": str,
-        "ProfileType": ProfileTypeType,
-        "As2Id": str,
-        "CertificateIds": List[str],
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
-    pass
-
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Arn": str,
-        "NextToken": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDescribedConnectorTypeDef = TypedDict(
     "_RequiredDescribedConnectorTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedConnectorTypeDef = TypedDict(
     "_OptionalDescribedConnectorTypeDef",
     {
         "ConnectorId": str,
         "Url": str,
-        "As2Config": As2ConnectorConfigOutputTypeDef,
+        "As2Config": As2ConnectorConfigTypeDef,
         "AccessRole": str,
         "LoggingRole": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "SftpConfig": SftpConnectorConfigOutputTypeDef,
     },
     total=False,
 )
 
 
 class DescribedConnectorTypeDef(
@@ -2007,21 +1896,21 @@
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
     "_OptionalDescribedUserTypeDef",
     {
         "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "UserName": str,
     },
     total=False,
 )
 
 
 class DescribedUserTypeDef(_RequiredDescribedUserTypeDef, _OptionalDescribedUserTypeDef):
@@ -2038,24 +1927,15 @@
     total=False,
 )
 
 FileLocationTypeDef = TypedDict(
     "FileLocationTypeDef",
     {
         "S3FileLocation": S3FileLocationTypeDef,
-        "EfsFileLocation": EfsFileLocationOutputTypeDef,
-    },
-    total=False,
-)
-
-InputFileLocationOutputTypeDef = TypedDict(
-    "InputFileLocationOutputTypeDef",
-    {
-        "S3FileLocation": S3InputFileLocationOutputTypeDef,
-        "EfsFileLocation": EfsFileLocationOutputTypeDef,
+        "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
@@ -2308,15 +2188,15 @@
     },
 )
 
 TagStepDetailsOutputTypeDef = TypedDict(
     "TagStepDetailsOutputTypeDef",
     {
         "Name": str,
-        "Tags": List[S3TagOutputTypeDef],
+        "Tags": List[S3TagTypeDef],
         "SourceFileLocation": str,
     },
     total=False,
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
@@ -2334,38 +2214,29 @@
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
 WorkflowDetailsOutputTypeDef = TypedDict(
     "WorkflowDetailsOutputTypeDef",
     {
-        "OnUpload": List[WorkflowDetailOutputTypeDef],
-        "OnPartialUpload": List[WorkflowDetailOutputTypeDef],
+        "OnUpload": List[WorkflowDetailTypeDef],
+        "OnPartialUpload": List[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
-DescribeAccessResponseTypeDef = TypedDict(
-    "DescribeAccessResponseTypeDef",
-    {
-        "ServerId": str,
-        "Access": DescribedAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2390,14 +2261,23 @@
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAccessResponseTypeDef = TypedDict(
+    "DescribeAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "Access": DescribedAccessTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "Connector": DescribedConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2416,49 +2296,14 @@
     {
         "Steps": List[ExecutionStepResultTypeDef],
         "OnExceptionSteps": List[ExecutionStepResultTypeDef],
     },
     total=False,
 )
 
-CopyStepDetailsOutputTypeDef = TypedDict(
-    "CopyStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "DestinationFileLocation": InputFileLocationOutputTypeDef,
-        "OverwriteExisting": OverwriteExistingType,
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
-_RequiredDecryptStepDetailsOutputTypeDef = TypedDict(
-    "_RequiredDecryptStepDetailsOutputTypeDef",
-    {
-        "Type": Literal["PGP"],
-        "DestinationFileLocation": InputFileLocationOutputTypeDef,
-    },
-)
-_OptionalDecryptStepDetailsOutputTypeDef = TypedDict(
-    "_OptionalDecryptStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "SourceFileLocation": str,
-        "OverwriteExisting": OverwriteExistingType,
-    },
-    total=False,
-)
-
-
-class DecryptStepDetailsOutputTypeDef(
-    _RequiredDecryptStepDetailsOutputTypeDef, _OptionalDecryptStepDetailsOutputTypeDef
-):
-    pass
-
-
 CopyStepDetailsTypeDef = TypedDict(
     "CopyStepDetailsTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationTypeDef,
         "OverwriteExisting": OverwriteExistingType,
         "SourceFileLocation": str,
@@ -2512,24 +2357,24 @@
     {
         "Certificate": str,
         "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
-        "IdentityProviderDetails": IdentityProviderDetailsOutputTypeDef,
+        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
         "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
         "ServerId": str,
         "State": StateType,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "UserCount": int,
         "WorkflowDetails": WorkflowDetailsOutputTypeDef,
         "StructuredLogDestinations": List[str],
     },
     total=False,
 )
 
@@ -2609,19 +2454,19 @@
     total=False,
 )
 
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "Type": WorkflowStepTypeType,
-        "CopyStepDetails": CopyStepDetailsOutputTypeDef,
-        "CustomStepDetails": CustomStepDetailsOutputTypeDef,
-        "DeleteStepDetails": DeleteStepDetailsOutputTypeDef,
+        "CopyStepDetails": CopyStepDetailsTypeDef,
+        "CustomStepDetails": CustomStepDetailsTypeDef,
+        "DeleteStepDetails": DeleteStepDetailsTypeDef,
         "TagStepDetails": TagStepDetailsOutputTypeDef,
-        "DecryptStepDetails": DecryptStepDetailsOutputTypeDef,
+        "DecryptStepDetails": DecryptStepDetailsTypeDef,
     },
     total=False,
 )
 
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
@@ -2671,15 +2516,15 @@
 _OptionalDescribedWorkflowTypeDef = TypedDict(
     "_OptionalDescribedWorkflowTypeDef",
     {
         "Description": str,
         "Steps": List[WorkflowStepOutputTypeDef],
         "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
         "WorkflowId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
```

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transfer service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transfer.type_defs import As2ConnectorConfigOutputTypeDef
+    from mypy_boto3_transfer.type_defs import As2ConnectorConfigTypeDef
 
-    data: As2ConnectorConfigOutputTypeDef = {...}
+    data: As2ConnectorConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -48,35 +48,32 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "As2ConnectorConfigOutputTypeDef",
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "SftpConnectorConfigTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
-    "CustomStepDetailsOutputTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
     "DeleteHostKeyRequestRequestTypeDef",
     "DeleteProfileRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
     "DeleteSshPublicKeyRequestRequestTypeDef",
-    "DeleteStepDetailsOutputTypeDef",
     "DeleteStepDetailsTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DescribeAccessRequestRequestTypeDef",
     "DescribeAgreementRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
@@ -85,29 +82,24 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
-    "HomeDirectoryMapEntryOutputTypeDef",
     "PosixProfileOutputTypeDef",
-    "TagOutputTypeDef",
     "SftpConnectorConfigOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "EndpointDetailsOutputTypeDef",
-    "IdentityProviderDetailsOutputTypeDef",
     "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
-    "EfsFileLocationOutputTypeDef",
     "EfsFileLocationTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
-    "S3InputFileLocationOutputTypeDef",
     "S3InputFileLocationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
     "ListCertificatesRequestRequestTypeDef",
@@ -123,29 +115,27 @@
     "ListServersRequestRequestTypeDef",
     "ListedServerTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
-    "S3TagOutputTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
-    "WorkflowDetailOutputTypeDef",
     "WorkflowDetailTypeDef",
     "CreateAccessRequestRequestTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateAccessResponseTypeDef",
     "CreateAgreementResponseTypeDef",
     "CreateConnectorResponseTypeDef",
@@ -168,33 +158,32 @@
     "UpdateHostKeyResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "UpdateServerResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DescribedAgreementTypeDef",
+    "DescribedCertificateTypeDef",
+    "DescribedHostKeyTypeDef",
+    "DescribedProfileTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConnectorRequestRequestTypeDef",
     "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
     "DescribedAccessTypeDef",
-    "DescribedAgreementTypeDef",
-    "DescribedCertificateTypeDef",
-    "DescribedHostKeyTypeDef",
-    "DescribedProfileTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribedConnectorTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
-    "InputFileLocationOutputTypeDef",
     "InputFileLocationTypeDef",
     "ListAccessesRequestListAccessesPaginateTypeDef",
     "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListProfilesRequestListProfilesPaginateTypeDef",
@@ -213,24 +202,22 @@
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
     "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
-    "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
+    "DescribeAccessResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
-    "CopyStepDetailsOutputTypeDef",
-    "DecryptStepDetailsOutputTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
     "DescribedServerTypeDef",
     "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
     "DescribedExecutionTypeDef",
@@ -240,30 +227,14 @@
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
     "DescribedWorkflowTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "DescribeWorkflowResponseTypeDef",
 )
 
-As2ConnectorConfigOutputTypeDef = TypedDict(
-    "As2ConnectorConfigOutputTypeDef",
-    {
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "MessageSubject": str,
-        "Compression": CompressionEnumType,
-        "EncryptionAlgorithm": EncryptionAlgType,
-        "SigningAlgorithm": SigningAlgType,
-        "MdnSigningAlgorithm": MdnSigningAlgType,
-        "MdnResponse": MdnResponseType,
-        "BasicAuthSecretId": str,
-    },
-    total=False,
-)
-
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "MessageSubject": str,
         "Compression": CompressionEnumType,
@@ -361,25 +332,14 @@
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": Sequence[Literal["HTTP"]],
     },
     total=False,
 )
 
-CustomStepDetailsOutputTypeDef = TypedDict(
-    "CustomStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Target": str,
-        "TimeoutSeconds": int,
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
         "Target": str,
         "TimeoutSeconds": int,
         "SourceFileLocation": str,
@@ -444,23 +404,14 @@
     {
         "ServerId": str,
         "SshPublicKeyId": str,
         "UserName": str,
     },
 )
 
-DeleteStepDetailsOutputTypeDef = TypedDict(
-    "DeleteStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
 DeleteStepDetailsTypeDef = TypedDict(
     "DeleteStepDetailsTypeDef",
     {
         "Name": str,
         "SourceFileLocation": str,
     },
     total=False,
@@ -591,22 +542,14 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
-HomeDirectoryMapEntryOutputTypeDef = TypedDict(
-    "HomeDirectoryMapEntryOutputTypeDef",
-    {
-        "Entry": str,
-        "Target": str,
-    },
-)
-
 _RequiredPosixProfileOutputTypeDef = TypedDict(
     "_RequiredPosixProfileOutputTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
@@ -619,22 +562,14 @@
 )
 
 class PosixProfileOutputTypeDef(
     _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 SftpConnectorConfigOutputTypeDef = TypedDict(
     "SftpConnectorConfigOutputTypeDef",
     {
         "UserSecretId": str,
         "TrustedHostKeys": List[str],
     },
     total=False,
@@ -657,26 +592,14 @@
         "VpcEndpointId": str,
         "VpcId": str,
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-IdentityProviderDetailsOutputTypeDef = TypedDict(
-    "IdentityProviderDetailsOutputTypeDef",
-    {
-        "Url": str,
-        "InvocationRole": str,
-        "DirectoryId": str,
-        "Function": str,
-        "SftpAuthenticationMethods": SftpAuthenticationMethodsType,
-    },
-    total=False,
-)
-
 ProtocolDetailsOutputTypeDef = TypedDict(
     "ProtocolDetailsOutputTypeDef",
     {
         "PassiveIp": str,
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": List[Literal["HTTP"]],
@@ -689,23 +612,14 @@
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
 )
 
-EfsFileLocationOutputTypeDef = TypedDict(
-    "EfsFileLocationOutputTypeDef",
-    {
-        "FileSystemId": str,
-        "Path": str,
-    },
-    total=False,
-)
-
 EfsFileLocationTypeDef = TypedDict(
     "EfsFileLocationTypeDef",
     {
         "FileSystemId": str,
         "Path": str,
     },
     total=False,
@@ -735,23 +649,14 @@
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
 )
 
-S3InputFileLocationOutputTypeDef = TypedDict(
-    "S3InputFileLocationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-    total=False,
-)
-
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
@@ -1075,22 +980,14 @@
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
     },
     total=False,
 )
 
-S3TagOutputTypeDef = TypedDict(
-    "S3TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -1267,22 +1164,14 @@
 )
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
-WorkflowDetailOutputTypeDef = TypedDict(
-    "WorkflowDetailOutputTypeDef",
-    {
-        "WorkflowId": str,
-        "ExecutionRole": str,
-    },
-)
-
 WorkflowDetailTypeDef = TypedDict(
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
@@ -1628,14 +1517,115 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+_RequiredDescribedAgreementTypeDef = TypedDict(
+    "_RequiredDescribedAgreementTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedAgreementTypeDef = TypedDict(
+    "_OptionalDescribedAgreementTypeDef",
+    {
+        "AgreementId": str,
+        "Description": str,
+        "Status": AgreementStatusTypeType,
+        "ServerId": str,
+        "LocalProfileId": str,
+        "PartnerProfileId": str,
+        "BaseDirectory": str,
+        "AccessRole": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+class DescribedAgreementTypeDef(
+    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
+):
+    pass
+
+_RequiredDescribedCertificateTypeDef = TypedDict(
+    "_RequiredDescribedCertificateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedCertificateTypeDef = TypedDict(
+    "_OptionalDescribedCertificateTypeDef",
+    {
+        "CertificateId": str,
+        "Usage": CertificateUsageTypeType,
+        "Status": CertificateStatusTypeType,
+        "Certificate": str,
+        "CertificateChain": str,
+        "ActiveDate": datetime,
+        "InactiveDate": datetime,
+        "Serial": str,
+        "NotBeforeDate": datetime,
+        "NotAfterDate": datetime,
+        "Type": CertificateTypeType,
+        "Description": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+class DescribedCertificateTypeDef(
+    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
+):
+    pass
+
+_RequiredDescribedHostKeyTypeDef = TypedDict(
+    "_RequiredDescribedHostKeyTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedHostKeyTypeDef = TypedDict(
+    "_OptionalDescribedHostKeyTypeDef",
+    {
+        "HostKeyId": str,
+        "HostKeyFingerprint": str,
+        "Description": str,
+        "Type": str,
+        "DateImported": datetime,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
+    pass
+
+_RequiredDescribedProfileTypeDef = TypedDict(
+    "_RequiredDescribedProfileTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedProfileTypeDef = TypedDict(
+    "_OptionalDescribedProfileTypeDef",
+    {
+        "ProfileId": str,
+        "ProfileType": ProfileTypeType,
+        "As2Id": str,
+        "CertificateIds": List[str],
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
+    pass
+
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
         "Usage": CertificateUsageTypeType,
         "Certificate": str,
     },
 )
@@ -1674,14 +1664,24 @@
 )
 
 class ImportHostKeyRequestRequestTypeDef(
     _RequiredImportHostKeyRequestRequestTypeDef, _OptionalImportHostKeyRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Arn": str,
+        "NextToken": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1780,150 +1780,39 @@
 ):
     pass
 
 DescribedAccessTypeDef = TypedDict(
     "DescribedAccessTypeDef",
     {
         "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "ExternalId": str,
     },
     total=False,
 )
 
-_RequiredDescribedAgreementTypeDef = TypedDict(
-    "_RequiredDescribedAgreementTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedAgreementTypeDef = TypedDict(
-    "_OptionalDescribedAgreementTypeDef",
-    {
-        "AgreementId": str,
-        "Description": str,
-        "Status": AgreementStatusTypeType,
-        "ServerId": str,
-        "LocalProfileId": str,
-        "PartnerProfileId": str,
-        "BaseDirectory": str,
-        "AccessRole": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-class DescribedAgreementTypeDef(
-    _RequiredDescribedAgreementTypeDef, _OptionalDescribedAgreementTypeDef
-):
-    pass
-
-_RequiredDescribedCertificateTypeDef = TypedDict(
-    "_RequiredDescribedCertificateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedCertificateTypeDef = TypedDict(
-    "_OptionalDescribedCertificateTypeDef",
-    {
-        "CertificateId": str,
-        "Usage": CertificateUsageTypeType,
-        "Status": CertificateStatusTypeType,
-        "Certificate": str,
-        "CertificateChain": str,
-        "ActiveDate": datetime,
-        "InactiveDate": datetime,
-        "Serial": str,
-        "NotBeforeDate": datetime,
-        "NotAfterDate": datetime,
-        "Type": CertificateTypeType,
-        "Description": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-class DescribedCertificateTypeDef(
-    _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
-):
-    pass
-
-_RequiredDescribedHostKeyTypeDef = TypedDict(
-    "_RequiredDescribedHostKeyTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedHostKeyTypeDef = TypedDict(
-    "_OptionalDescribedHostKeyTypeDef",
-    {
-        "HostKeyId": str,
-        "HostKeyFingerprint": str,
-        "Description": str,
-        "Type": str,
-        "DateImported": datetime,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-class DescribedHostKeyTypeDef(_RequiredDescribedHostKeyTypeDef, _OptionalDescribedHostKeyTypeDef):
-    pass
-
-_RequiredDescribedProfileTypeDef = TypedDict(
-    "_RequiredDescribedProfileTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedProfileTypeDef = TypedDict(
-    "_OptionalDescribedProfileTypeDef",
-    {
-        "ProfileId": str,
-        "ProfileType": ProfileTypeType,
-        "As2Id": str,
-        "CertificateIds": List[str],
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
-    pass
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Arn": str,
-        "NextToken": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDescribedConnectorTypeDef = TypedDict(
     "_RequiredDescribedConnectorTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedConnectorTypeDef = TypedDict(
     "_OptionalDescribedConnectorTypeDef",
     {
         "ConnectorId": str,
         "Url": str,
-        "As2Config": As2ConnectorConfigOutputTypeDef,
+        "As2Config": As2ConnectorConfigTypeDef,
         "AccessRole": str,
         "LoggingRole": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "SftpConfig": SftpConnectorConfigOutputTypeDef,
     },
     total=False,
 )
 
 class DescribedConnectorTypeDef(
     _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
@@ -1936,21 +1825,21 @@
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
     "_OptionalDescribedUserTypeDef",
     {
         "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryOutputTypeDef],
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "UserName": str,
     },
     total=False,
 )
 
 class DescribedUserTypeDef(_RequiredDescribedUserTypeDef, _OptionalDescribedUserTypeDef):
     pass
@@ -1965,24 +1854,15 @@
     total=False,
 )
 
 FileLocationTypeDef = TypedDict(
     "FileLocationTypeDef",
     {
         "S3FileLocation": S3FileLocationTypeDef,
-        "EfsFileLocation": EfsFileLocationOutputTypeDef,
-    },
-    total=False,
-)
-
-InputFileLocationOutputTypeDef = TypedDict(
-    "InputFileLocationOutputTypeDef",
-    {
-        "S3FileLocation": S3InputFileLocationOutputTypeDef,
-        "EfsFileLocation": EfsFileLocationOutputTypeDef,
+        "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
@@ -2225,15 +2105,15 @@
     },
 )
 
 TagStepDetailsOutputTypeDef = TypedDict(
     "TagStepDetailsOutputTypeDef",
     {
         "Name": str,
-        "Tags": List[S3TagOutputTypeDef],
+        "Tags": List[S3TagTypeDef],
         "SourceFileLocation": str,
     },
     total=False,
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
@@ -2251,38 +2131,29 @@
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
 WorkflowDetailsOutputTypeDef = TypedDict(
     "WorkflowDetailsOutputTypeDef",
     {
-        "OnUpload": List[WorkflowDetailOutputTypeDef],
-        "OnPartialUpload": List[WorkflowDetailOutputTypeDef],
+        "OnUpload": List[WorkflowDetailTypeDef],
+        "OnPartialUpload": List[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
-DescribeAccessResponseTypeDef = TypedDict(
-    "DescribeAccessResponseTypeDef",
-    {
-        "ServerId": str,
-        "Access": DescribedAccessTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2307,14 +2178,23 @@
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAccessResponseTypeDef = TypedDict(
+    "DescribeAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "Access": DescribedAccessTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "Connector": DescribedConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2333,47 +2213,14 @@
     {
         "Steps": List[ExecutionStepResultTypeDef],
         "OnExceptionSteps": List[ExecutionStepResultTypeDef],
     },
     total=False,
 )
 
-CopyStepDetailsOutputTypeDef = TypedDict(
-    "CopyStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "DestinationFileLocation": InputFileLocationOutputTypeDef,
-        "OverwriteExisting": OverwriteExistingType,
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
-_RequiredDecryptStepDetailsOutputTypeDef = TypedDict(
-    "_RequiredDecryptStepDetailsOutputTypeDef",
-    {
-        "Type": Literal["PGP"],
-        "DestinationFileLocation": InputFileLocationOutputTypeDef,
-    },
-)
-_OptionalDecryptStepDetailsOutputTypeDef = TypedDict(
-    "_OptionalDecryptStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "SourceFileLocation": str,
-        "OverwriteExisting": OverwriteExistingType,
-    },
-    total=False,
-)
-
-class DecryptStepDetailsOutputTypeDef(
-    _RequiredDecryptStepDetailsOutputTypeDef, _OptionalDecryptStepDetailsOutputTypeDef
-):
-    pass
-
 CopyStepDetailsTypeDef = TypedDict(
     "CopyStepDetailsTypeDef",
     {
         "Name": str,
         "DestinationFileLocation": InputFileLocationTypeDef,
         "OverwriteExisting": OverwriteExistingType,
         "SourceFileLocation": str,
@@ -2425,24 +2272,24 @@
     {
         "Certificate": str,
         "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
         "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
-        "IdentityProviderDetails": IdentityProviderDetailsOutputTypeDef,
+        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
         "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
         "ServerId": str,
         "State": StateType,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "UserCount": int,
         "WorkflowDetails": WorkflowDetailsOutputTypeDef,
         "StructuredLogDestinations": List[str],
     },
     total=False,
 )
 
@@ -2518,19 +2365,19 @@
     total=False,
 )
 
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "Type": WorkflowStepTypeType,
-        "CopyStepDetails": CopyStepDetailsOutputTypeDef,
-        "CustomStepDetails": CustomStepDetailsOutputTypeDef,
-        "DeleteStepDetails": DeleteStepDetailsOutputTypeDef,
+        "CopyStepDetails": CopyStepDetailsTypeDef,
+        "CustomStepDetails": CustomStepDetailsTypeDef,
+        "DeleteStepDetails": DeleteStepDetailsTypeDef,
         "TagStepDetails": TagStepDetailsOutputTypeDef,
-        "DecryptStepDetails": DecryptStepDetailsOutputTypeDef,
+        "DecryptStepDetails": DecryptStepDetailsTypeDef,
     },
     total=False,
 )
 
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
@@ -2580,15 +2427,15 @@
 _OptionalDescribedWorkflowTypeDef = TypedDict(
     "_OptionalDescribedWorkflowTypeDef",
     {
         "Description": str,
         "Steps": List[WorkflowStepOutputTypeDef],
         "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
         "WorkflowId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
```

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.12
-Summary: Type annotations for boto3.Transfer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -404,35 +404,32 @@
 ### Typed dictionaries
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
-    As2ConnectorConfigOutputTypeDef,
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     SftpConnectorConfigTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CustomStepDetailsOutputTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
     DeleteSshPublicKeyRequestRequestTypeDef,
-    DeleteStepDetailsOutputTypeDef,
     DeleteStepDetailsTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DescribeAccessRequestRequestTypeDef,
     DescribeAgreementRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -441,29 +438,24 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
-    HomeDirectoryMapEntryOutputTypeDef,
     PosixProfileOutputTypeDef,
-    TagOutputTypeDef,
     SftpConnectorConfigOutputTypeDef,
     LoggingConfigurationTypeDef,
     EndpointDetailsOutputTypeDef,
-    IdentityProviderDetailsOutputTypeDef,
     ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
-    EfsFileLocationOutputTypeDef,
     EfsFileLocationTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    S3InputFileLocationOutputTypeDef,
     S3InputFileLocationTypeDef,
     PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
     ListCertificatesRequestRequestTypeDef,
@@ -479,29 +471,27 @@
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    S3TagOutputTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgreementRequestRequestTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    WorkflowDetailOutputTypeDef,
     WorkflowDetailTypeDef,
     CreateAccessRequestRequestTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateAccessResponseTypeDef,
     CreateAgreementResponseTypeDef,
     CreateConnectorResponseTypeDef,
@@ -524,33 +514,32 @@
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DescribedAgreementTypeDef,
+    DescribedCertificateTypeDef,
+    DescribedHostKeyTypeDef,
+    DescribedProfileTypeDef,
     ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
     DescribedAccessTypeDef,
-    DescribedAgreementTypeDef,
-    DescribedCertificateTypeDef,
-    DescribedHostKeyTypeDef,
-    DescribedProfileTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribedConnectorTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
-    InputFileLocationOutputTypeDef,
     InputFileLocationTypeDef,
     ListAccessesRequestListAccessesPaginateTypeDef,
     ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListProfilesRequestListProfilesPaginateTypeDef,
@@ -569,24 +558,22 @@
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
     WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
-    DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeAccessResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
-    CopyStepDetailsOutputTypeDef,
-    DecryptStepDetailsOutputTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
     DescribedServerTypeDef,
     CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     DescribedExecutionTypeDef,
@@ -597,15 +584,15 @@
     DescribeExecutionResponseTypeDef,
     DescribedWorkflowTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     DescribeWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigOutputTypeDef:
+def get_structure() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.12/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.28.15/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.12/setup.py` & `mypy-boto3-transfer-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Transfer 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

