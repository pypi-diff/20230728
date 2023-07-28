# Comparing `tmp/mypy-boto3-dataexchange-1.28.12.tar.gz` & `tmp/mypy-boto3-dataexchange-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dataexchange-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
+gzip compressed data, was "mypy-boto3-dataexchange-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
```

## Comparing `mypy-boto3-dataexchange-1.28.12.tar` & `mypy-boto3-dataexchange-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.392537 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-07-27 05:19:59.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50714 2023-07-27 05:19:59.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.184949 mypy-boto3-dataexchange-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-28 20:42:37.180949 mypy-boto3-dataexchange-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.164949 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-28 20:22:34.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-28 20:22:34.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46564 2023-07-28 20:22:35.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46495 2023-07-28 20:22:34.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.180949 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-28 20:42:36.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:36.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:36.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:36.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:36.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:36.000000 mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.184949 mypy-boto3-dataexchange-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:22:33.000000 mypy-boto3-dataexchange-1.28.15/setup.py
```

### Comparing `mypy-boto3-dataexchange-1.28.12/LICENSE` & `mypy-boto3-dataexchange-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/PKG-INFO` & `mypy-boto3-dataexchange-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dataexchange
-Version: 1.28.12
-Summary: Type annotations for boto3.DataExchange 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DataExchange 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dataexchange)](https://pepy.tech/project/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,125 +352,114 @@
 
 `mypy_boto3_dataexchange.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dataexchange.type_defs import (
     ApiGatewayApiAssetTypeDef,
-    AssetDestinationEntryOutputTypeDef,
     AssetDestinationEntryTypeDef,
     RedshiftDataShareAssetTypeDef,
     S3SnapshotAssetTypeDef,
-    AssetSourceEntryOutputTypeDef,
     AssetSourceEntryTypeDef,
-    AutoExportRevisionDestinationEntryOutputTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
-    ExportServerSideEncryptionOutputTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateRevisionRequestRequestTypeDef,
-    CreateRevisionResponseTypeDef,
     LFTagOutputTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
-    RevisionPublishedOutputTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
-    RevisionDestinationEntryOutputTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
-    GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
-    RedshiftDataShareAssetSourceEntryOutputTypeDef,
-    KmsKeyToGrantOutputTypeDef,
     KmsKeyToGrantTypeDef,
-    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
-    ListEventActionsRequestListEventActionsPaginateTypeDef,
     ListEventActionsRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListRevisionAssetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RevokeRevisionRequestRequestTypeDef,
-    RevokeRevisionResponseTypeDef,
     SendApiAssetRequestRequestTypeDef,
-    SendApiAssetResponseTypeDef,
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
-    UpdateRevisionResponseTypeDef,
-    ImportAssetsFromS3ResponseDetailsTypeDef,
     ImportAssetsFromS3RequestDetailsTypeDef,
-    AutoExportRevisionToS3RequestDetailsOutputTypeDef,
-    ExportAssetsToS3ResponseDetailsTypeDef,
+    ImportAssetsFromS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
-    CreateDataSetResponseTypeDef,
+    ExportAssetsToS3ResponseDetailsTypeDef,
     DataSetEntryTypeDef,
+    CreateDataSetResponseTypeDef,
+    CreateRevisionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetDataSetResponseTypeDef,
+    GetRevisionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RevokeRevisionResponseTypeDef,
+    SendApiAssetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
+    UpdateRevisionResponseTypeDef,
     DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
     DatabaseLFTagPolicyTypeDef,
     TableLFTagPolicyAndPermissionsOutputTypeDef,
     TableLFTagPolicyTypeDef,
     DatabaseLFTagPolicyAndPermissionsTypeDef,
     TableLFTagPolicyAndPermissionsTypeDef,
     DetailsTypeDef,
-    EventOutputTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
     S3DataAccessAssetSourceEntryOutputTypeDef,
-    S3DataAccessAssetTypeDef,
     S3DataAccessAssetSourceEntryTypeDef,
+    S3DataAccessAssetTypeDef,
+    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
+    ListEventActionsRequestListEventActionsPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListDataSetRevisionsResponseTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     JobErrorTypeDef,
     CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
     CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
+    CreateEventActionRequestRequestTypeDef,
     CreateEventActionResponseTypeDef,
     EventActionEntryTypeDef,
     GetEventActionResponseTypeDef,
-    UpdateEventActionResponseTypeDef,
-    CreateEventActionRequestRequestTypeDef,
     UpdateEventActionRequestRequestTypeDef,
+    UpdateEventActionResponseTypeDef,
     LFTagPolicyDetailsTypeDef,
     ResponseDetailsTypeDef,
     RequestDetailsTypeDef,
     ListEventActionsResponseTypeDef,
     LakeFormationDataPermissionDetailsTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
```

### Comparing `mypy-boto3-dataexchange-1.28.12/README.md` & `mypy-boto3-dataexchange-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dataexchange)](https://pepy.tech/project/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,125 +320,114 @@
 
 `mypy_boto3_dataexchange.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dataexchange.type_defs import (
     ApiGatewayApiAssetTypeDef,
-    AssetDestinationEntryOutputTypeDef,
     AssetDestinationEntryTypeDef,
     RedshiftDataShareAssetTypeDef,
     S3SnapshotAssetTypeDef,
-    AssetSourceEntryOutputTypeDef,
     AssetSourceEntryTypeDef,
-    AutoExportRevisionDestinationEntryOutputTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
-    ExportServerSideEncryptionOutputTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateRevisionRequestRequestTypeDef,
-    CreateRevisionResponseTypeDef,
     LFTagOutputTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
-    RevisionPublishedOutputTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
-    RevisionDestinationEntryOutputTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
-    GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
-    RedshiftDataShareAssetSourceEntryOutputTypeDef,
-    KmsKeyToGrantOutputTypeDef,
     KmsKeyToGrantTypeDef,
-    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
-    ListEventActionsRequestListEventActionsPaginateTypeDef,
     ListEventActionsRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListRevisionAssetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RevokeRevisionRequestRequestTypeDef,
-    RevokeRevisionResponseTypeDef,
     SendApiAssetRequestRequestTypeDef,
-    SendApiAssetResponseTypeDef,
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
-    UpdateRevisionResponseTypeDef,
-    ImportAssetsFromS3ResponseDetailsTypeDef,
     ImportAssetsFromS3RequestDetailsTypeDef,
-    AutoExportRevisionToS3RequestDetailsOutputTypeDef,
-    ExportAssetsToS3ResponseDetailsTypeDef,
+    ImportAssetsFromS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
-    CreateDataSetResponseTypeDef,
+    ExportAssetsToS3ResponseDetailsTypeDef,
     DataSetEntryTypeDef,
+    CreateDataSetResponseTypeDef,
+    CreateRevisionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetDataSetResponseTypeDef,
+    GetRevisionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RevokeRevisionResponseTypeDef,
+    SendApiAssetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
+    UpdateRevisionResponseTypeDef,
     DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
     DatabaseLFTagPolicyTypeDef,
     TableLFTagPolicyAndPermissionsOutputTypeDef,
     TableLFTagPolicyTypeDef,
     DatabaseLFTagPolicyAndPermissionsTypeDef,
     TableLFTagPolicyAndPermissionsTypeDef,
     DetailsTypeDef,
-    EventOutputTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
     S3DataAccessAssetSourceEntryOutputTypeDef,
-    S3DataAccessAssetTypeDef,
     S3DataAccessAssetSourceEntryTypeDef,
+    S3DataAccessAssetTypeDef,
+    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
+    ListEventActionsRequestListEventActionsPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListDataSetRevisionsResponseTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     JobErrorTypeDef,
     CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
     CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
+    CreateEventActionRequestRequestTypeDef,
     CreateEventActionResponseTypeDef,
     EventActionEntryTypeDef,
     GetEventActionResponseTypeDef,
-    UpdateEventActionResponseTypeDef,
-    CreateEventActionRequestRequestTypeDef,
     UpdateEventActionRequestRequestTypeDef,
+    UpdateEventActionResponseTypeDef,
     LFTagPolicyDetailsTypeDef,
     ResponseDetailsTypeDef,
     RequestDetailsTypeDef,
     ListEventActionsResponseTypeDef,
     LakeFormationDataPermissionDetailsTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
```

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.py` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.pyi` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__main__.py` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataExchange 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.DataExchange 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange\nOther"
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

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.py` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.pyi` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.py` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.pyi` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.py` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,45 +62,45 @@
 class ListDataSetRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataSetRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
         """
 
 
 class ListDataSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, Origin: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Origin: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
         """
 
 
 class ListEventActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
     """
 
     def paginate(
-        self, *, EventSourceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EventSourceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
         """
 
 
@@ -111,28 +111,28 @@
     """
 
     def paginate(
         self,
         *,
         DataSetId: str = ...,
         RevisionId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listjobspaginator)
         """
 
 
 class ListRevisionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, RevisionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataSetId: str, RevisionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRevisionAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
         """
```

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.pyi` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -59,43 +59,43 @@
 class ListDataSetRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataSetRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
         """
 
 class ListDataSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, Origin: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Origin: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
         """
 
 class ListEventActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
     """
 
     def paginate(
-        self, *, EventSourceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EventSourceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -105,27 +105,27 @@
     """
 
     def paginate(
         self,
         *,
         DataSetId: str = ...,
         RevisionId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listjobspaginator)
         """
 
 class ListRevisionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, RevisionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataSetId: str, RevisionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRevisionAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
         """
```

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.py` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -34,128 +34,116 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApiGatewayApiAssetTypeDef",
-    "AssetDestinationEntryOutputTypeDef",
     "AssetDestinationEntryTypeDef",
     "RedshiftDataShareAssetTypeDef",
     "S3SnapshotAssetTypeDef",
-    "AssetSourceEntryOutputTypeDef",
     "AssetSourceEntryTypeDef",
-    "AutoExportRevisionDestinationEntryOutputTypeDef",
     "AutoExportRevisionDestinationEntryTypeDef",
-    "ExportServerSideEncryptionOutputTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRevisionRequestRequestTypeDef",
-    "CreateRevisionResponseTypeDef",
     "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "RevisionPublishedOutputTypeDef",
     "RevisionPublishedTypeDef",
     "ExportAssetToSignedUrlRequestDetailsTypeDef",
     "ExportAssetToSignedUrlResponseDetailsTypeDef",
     "RevisionDestinationEntryTypeDef",
-    "RevisionDestinationEntryOutputTypeDef",
     "GetAssetRequestRequestTypeDef",
     "GetDataSetRequestRequestTypeDef",
     "GetEventActionRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetRevisionRequestRequestTypeDef",
-    "GetRevisionResponseTypeDef",
     "ImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     "ImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     "ImportAssetFromSignedUrlResponseDetailsTypeDef",
     "RedshiftDataShareAssetSourceEntryTypeDef",
-    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
-    "KmsKeyToGrantOutputTypeDef",
     "KmsKeyToGrantTypeDef",
-    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDataSetRevisionsRequestRequestTypeDef",
     "RevisionEntryTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
     "ListEventActionsRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListRevisionAssetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeRevisionRequestRequestTypeDef",
-    "RevokeRevisionResponseTypeDef",
     "SendApiAssetRequestRequestTypeDef",
-    "SendApiAssetResponseTypeDef",
     "StartJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "UpdateRevisionRequestRequestTypeDef",
-    "UpdateRevisionResponseTypeDef",
-    "ImportAssetsFromS3ResponseDetailsTypeDef",
     "ImportAssetsFromS3RequestDetailsTypeDef",
-    "AutoExportRevisionToS3RequestDetailsOutputTypeDef",
-    "ExportAssetsToS3ResponseDetailsTypeDef",
+    "ImportAssetsFromS3ResponseDetailsTypeDef",
     "AutoExportRevisionToS3RequestDetailsTypeDef",
     "ExportAssetsToS3RequestDetailsTypeDef",
-    "CreateDataSetResponseTypeDef",
+    "ExportAssetsToS3ResponseDetailsTypeDef",
     "DataSetEntryTypeDef",
+    "CreateDataSetResponseTypeDef",
+    "CreateRevisionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetDataSetResponseTypeDef",
+    "GetRevisionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RevokeRevisionResponseTypeDef",
+    "SendApiAssetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
+    "UpdateRevisionResponseTypeDef",
     "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     "DatabaseLFTagPolicyTypeDef",
     "TableLFTagPolicyAndPermissionsOutputTypeDef",
     "TableLFTagPolicyTypeDef",
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
     "TableLFTagPolicyAndPermissionsTypeDef",
     "DetailsTypeDef",
-    "EventOutputTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     "S3DataAccessAssetSourceEntryOutputTypeDef",
-    "S3DataAccessAssetTypeDef",
     "S3DataAccessAssetSourceEntryTypeDef",
+    "S3DataAccessAssetTypeDef",
+    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "JobErrorTypeDef",
     "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+    "CreateEventActionRequestRequestTypeDef",
     "CreateEventActionResponseTypeDef",
     "EventActionEntryTypeDef",
     "GetEventActionResponseTypeDef",
-    "UpdateEventActionResponseTypeDef",
-    "CreateEventActionRequestRequestTypeDef",
     "UpdateEventActionRequestRequestTypeDef",
+    "UpdateEventActionResponseTypeDef",
     "LFTagPolicyDetailsTypeDef",
     "ResponseDetailsTypeDef",
     "RequestDetailsTypeDef",
     "ListEventActionsResponseTypeDef",
     "LakeFormationDataPermissionDetailsTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
@@ -182,36 +170,14 @@
         "ApiSpecificationDownloadUrlExpiresAt": datetime,
         "ProtocolType": Literal["REST"],
         "Stage": str,
     },
     total=False,
 )
 
-_RequiredAssetDestinationEntryOutputTypeDef = TypedDict(
-    "_RequiredAssetDestinationEntryOutputTypeDef",
-    {
-        "AssetId": str,
-        "Bucket": str,
-    },
-)
-_OptionalAssetDestinationEntryOutputTypeDef = TypedDict(
-    "_OptionalAssetDestinationEntryOutputTypeDef",
-    {
-        "Key": str,
-    },
-    total=False,
-)
-
-
-class AssetDestinationEntryOutputTypeDef(
-    _RequiredAssetDestinationEntryOutputTypeDef, _OptionalAssetDestinationEntryOutputTypeDef
-):
-    pass
-
-
 _RequiredAssetDestinationEntryTypeDef = TypedDict(
     "_RequiredAssetDestinationEntryTypeDef",
     {
         "AssetId": str,
         "Bucket": str,
     },
 )
@@ -219,138 +185,80 @@
     "_OptionalAssetDestinationEntryTypeDef",
     {
         "Key": str,
     },
     total=False,
 )
 
-
 class AssetDestinationEntryTypeDef(
     _RequiredAssetDestinationEntryTypeDef, _OptionalAssetDestinationEntryTypeDef
 ):
     pass
 
-
 RedshiftDataShareAssetTypeDef = TypedDict(
     "RedshiftDataShareAssetTypeDef",
     {
         "Arn": str,
     },
 )
 
 S3SnapshotAssetTypeDef = TypedDict(
     "S3SnapshotAssetTypeDef",
     {
         "Size": float,
     },
 )
 
-AssetSourceEntryOutputTypeDef = TypedDict(
-    "AssetSourceEntryOutputTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-
 AssetSourceEntryTypeDef = TypedDict(
     "AssetSourceEntryTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-_RequiredAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_RequiredAutoExportRevisionDestinationEntryOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_OptionalAutoExportRevisionDestinationEntryOutputTypeDef",
-    {
-        "KeyPattern": str,
-    },
-    total=False,
-)
-
-
-class AutoExportRevisionDestinationEntryOutputTypeDef(
-    _RequiredAutoExportRevisionDestinationEntryOutputTypeDef,
-    _OptionalAutoExportRevisionDestinationEntryOutputTypeDef,
-):
-    pass
-
-
 _RequiredAutoExportRevisionDestinationEntryTypeDef = TypedDict(
     "_RequiredAutoExportRevisionDestinationEntryTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalAutoExportRevisionDestinationEntryTypeDef = TypedDict(
     "_OptionalAutoExportRevisionDestinationEntryTypeDef",
     {
         "KeyPattern": str,
     },
     total=False,
 )
 
-
 class AutoExportRevisionDestinationEntryTypeDef(
     _RequiredAutoExportRevisionDestinationEntryTypeDef,
     _OptionalAutoExportRevisionDestinationEntryTypeDef,
 ):
     pass
 
-
-_RequiredExportServerSideEncryptionOutputTypeDef = TypedDict(
-    "_RequiredExportServerSideEncryptionOutputTypeDef",
-    {
-        "Type": ServerSideEncryptionTypesType,
-    },
-)
-_OptionalExportServerSideEncryptionOutputTypeDef = TypedDict(
-    "_OptionalExportServerSideEncryptionOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
-
-class ExportServerSideEncryptionOutputTypeDef(
-    _RequiredExportServerSideEncryptionOutputTypeDef,
-    _OptionalExportServerSideEncryptionOutputTypeDef,
-):
-    pass
-
-
 _RequiredExportServerSideEncryptionTypeDef = TypedDict(
     "_RequiredExportServerSideEncryptionTypeDef",
     {
         "Type": ServerSideEncryptionTypesType,
     },
 )
 _OptionalExportServerSideEncryptionTypeDef = TypedDict(
     "_OptionalExportServerSideEncryptionTypeDef",
     {
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class ExportServerSideEncryptionTypeDef(
     _RequiredExportServerSideEncryptionTypeDef, _OptionalExportServerSideEncryptionTypeDef
 ):
     pass
 
-
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -366,28 +274,37 @@
     "_OptionalCreateDataSetRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDataSetRequestRequestTypeDef(
     _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
 ):
     pass
 
-
 OriginDetailsTypeDef = TypedDict(
     "OriginDetailsTypeDef",
     {
         "ProductId": str,
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
 _RequiredCreateRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalCreateRevisionRequestRequestTypeDef = TypedDict(
@@ -395,40 +312,19 @@
     {
         "Comment": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRevisionRequestRequestTypeDef(
     _RequiredCreateRevisionRequestRequestTypeDef, _OptionalCreateRevisionRequestRequestTypeDef
 ):
     pass
 
-
-CreateRevisionResponseTypeDef = TypedDict(
-    "CreateRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LFTagOutputTypeDef = TypedDict(
     "LFTagOutputTypeDef",
     {
         "TagKey": str,
         "TagValues": List[str],
     },
 )
@@ -475,28 +371,14 @@
 ImportAssetFromSignedUrlJobErrorDetailsTypeDef = TypedDict(
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     {
         "AssetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RevisionPublishedOutputTypeDef = TypedDict(
-    "RevisionPublishedOutputTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-
 RevisionPublishedTypeDef = TypedDict(
     "RevisionPublishedTypeDef",
     {
         "DataSetId": str,
     },
 )
 
@@ -522,22 +404,20 @@
     {
         "SignedUrl": str,
         "SignedUrlExpiresAt": datetime,
     },
     total=False,
 )
 
-
 class ExportAssetToSignedUrlResponseDetailsTypeDef(
     _RequiredExportAssetToSignedUrlResponseDetailsTypeDef,
     _OptionalExportAssetToSignedUrlResponseDetailsTypeDef,
 ):
     pass
 
-
 _RequiredRevisionDestinationEntryTypeDef = TypedDict(
     "_RequiredRevisionDestinationEntryTypeDef",
     {
         "Bucket": str,
         "RevisionId": str,
     },
 )
@@ -545,43 +425,19 @@
     "_OptionalRevisionDestinationEntryTypeDef",
     {
         "KeyPattern": str,
     },
     total=False,
 )
 
-
 class RevisionDestinationEntryTypeDef(
     _RequiredRevisionDestinationEntryTypeDef, _OptionalRevisionDestinationEntryTypeDef
 ):
     pass
 
-
-_RequiredRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_RequiredRevisionDestinationEntryOutputTypeDef",
-    {
-        "Bucket": str,
-        "RevisionId": str,
-    },
-)
-_OptionalRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_OptionalRevisionDestinationEntryOutputTypeDef",
-    {
-        "KeyPattern": str,
-    },
-    total=False,
-)
-
-
-class RevisionDestinationEntryOutputTypeDef(
-    _RequiredRevisionDestinationEntryOutputTypeDef, _OptionalRevisionDestinationEntryOutputTypeDef
-):
-    pass
-
-
 GetAssetRequestRequestTypeDef = TypedDict(
     "GetAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -612,33 +468,14 @@
     "GetRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-GetRevisionResponseTypeDef = TypedDict(
-    "GetRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef = TypedDict(
     "_RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     {
         "ApiId": str,
         "ApiName": str,
         "ApiSpecificationMd5Hash": str,
         "DataSetId": str,
@@ -652,22 +489,20 @@
     {
         "ApiDescription": str,
         "ApiKey": str,
     },
     total=False,
 )
 
-
 class ImportAssetFromApiGatewayApiRequestDetailsTypeDef(
     _RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     _OptionalImportAssetFromApiGatewayApiRequestDetailsTypeDef,
 ):
     pass
 
-
 _RequiredImportAssetFromApiGatewayApiResponseDetailsTypeDef = TypedDict(
     "_RequiredImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     {
         "ApiId": str,
         "ApiName": str,
         "ApiSpecificationMd5Hash": str,
         "ApiSpecificationUploadUrl": str,
@@ -683,22 +518,20 @@
     {
         "ApiDescription": str,
         "ApiKey": str,
     },
     total=False,
 )
 
-
 class ImportAssetFromApiGatewayApiResponseDetailsTypeDef(
     _RequiredImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     _OptionalImportAssetFromApiGatewayApiResponseDetailsTypeDef,
 ):
     pass
 
-
 ImportAssetFromSignedUrlRequestDetailsTypeDef = TypedDict(
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     {
         "AssetName": str,
         "DataSetId": str,
         "Md5Hash": str,
         "RevisionId": str,
@@ -719,72 +552,44 @@
         "Md5Hash": str,
         "SignedUrl": str,
         "SignedUrlExpiresAt": datetime,
     },
     total=False,
 )
 
-
 class ImportAssetFromSignedUrlResponseDetailsTypeDef(
     _RequiredImportAssetFromSignedUrlResponseDetailsTypeDef,
     _OptionalImportAssetFromSignedUrlResponseDetailsTypeDef,
 ):
     pass
 
-
 RedshiftDataShareAssetSourceEntryTypeDef = TypedDict(
     "RedshiftDataShareAssetSourceEntryTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
-RedshiftDataShareAssetSourceEntryOutputTypeDef = TypedDict(
-    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
-    {
-        "DataShareArn": str,
-    },
-)
-
-KmsKeyToGrantOutputTypeDef = TypedDict(
-    "KmsKeyToGrantOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-)
-
 KmsKeyToGrantTypeDef = TypedDict(
     "KmsKeyToGrantTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
-_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
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
-class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
-    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDataSetRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetRevisionsRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalListDataSetRevisionsRequestRequestTypeDef = TypedDict(
@@ -792,22 +597,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDataSetRevisionsRequestRequestTypeDef(
     _RequiredListDataSetRevisionsRequestRequestTypeDef,
     _OptionalListDataSetRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRevisionEntryTypeDef = TypedDict(
     "_RequiredRevisionEntryTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
@@ -823,101 +626,48 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
     },
     total=False,
 )
 
-
 class RevisionEntryTypeDef(_RequiredRevisionEntryTypeDef, _OptionalRevisionEntryTypeDef):
     pass
 
-
-ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "Origin": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataSetsRequestRequestTypeDef = TypedDict(
     "ListDataSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Origin": str,
     },
     total=False,
 )
 
-ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
-    {
-        "EventSourceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEventActionsRequestRequestTypeDef = TypedDict(
     "ListEventActionsRequestRequestTypeDef",
     {
         "EventSourceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "MaxResults": int,
         "NextToken": str,
         "RevisionId": str,
     },
     total=False,
 )
 
-_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
-_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
-    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRevisionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListRevisionAssetsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
@@ -926,85 +676,36 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRevisionAssetsRequestRequestTypeDef(
     _RequiredListRevisionAssetsRequestRequestTypeDef,
     _OptionalListRevisionAssetsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
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
 RevokeRevisionRequestRequestTypeDef = TypedDict(
     "RevokeRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
         "RevocationComment": str,
     },
 )
 
-RevokeRevisionResponseTypeDef = TypedDict(
-    "RevokeRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendApiAssetRequestRequestTypeDef = TypedDict(
     "_RequiredSendApiAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -1017,30 +718,19 @@
         "RequestHeaders": Mapping[str, str],
         "Method": str,
         "Path": str,
     },
     total=False,
 )
 
-
 class SendApiAssetRequestRequestTypeDef(
     _RequiredSendApiAssetRequestRequestTypeDef, _OptionalSendApiAssetRequestRequestTypeDef
 ):
     pass
 
-
-SendApiAssetResponseTypeDef = TypedDict(
-    "SendApiAssetResponseTypeDef",
-    {
-        "Body": str,
-        "ResponseHeaders": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartJobRequestRequestTypeDef = TypedDict(
     "StartJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -1081,21 +771,19 @@
     {
         "Description": str,
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateDataSetRequestRequestTypeDef(
     _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
@@ -1104,101 +792,36 @@
     {
         "Comment": str,
         "Finalized": bool,
     },
     total=False,
 )
 
-
 class UpdateRevisionRequestRequestTypeDef(
     _RequiredUpdateRevisionRequestRequestTypeDef, _OptionalUpdateRevisionRequestRequestTypeDef
 ):
     pass
 
-
-UpdateRevisionResponseTypeDef = TypedDict(
-    "UpdateRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
-    "ImportAssetsFromS3ResponseDetailsTypeDef",
-    {
-        "AssetSources": List[AssetSourceEntryOutputTypeDef],
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
-
 ImportAssetsFromS3RequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromS3RequestDetailsTypeDef",
     {
         "AssetSources": Sequence[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
-    "_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef",
-    {
-        "RevisionDestination": AutoExportRevisionDestinationEntryOutputTypeDef,
-    },
-)
-_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
-    "_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef",
-    {
-        "Encryption": ExportServerSideEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AutoExportRevisionToS3RequestDetailsOutputTypeDef(
-    _RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef,
-    _OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef,
-):
-    pass
-
-
-_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
+ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
+    "ImportAssetsFromS3ResponseDetailsTypeDef",
     {
-        "AssetDestinations": List[AssetDestinationEntryOutputTypeDef],
+        "AssetSources": List[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
-    {
-        "Encryption": ExportServerSideEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ExportAssetsToS3ResponseDetailsTypeDef(
-    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
-):
-    pass
-
 
 _RequiredAutoExportRevisionToS3RequestDetailsTypeDef = TypedDict(
     "_RequiredAutoExportRevisionToS3RequestDetailsTypeDef",
     {
         "RevisionDestination": AutoExportRevisionDestinationEntryTypeDef,
     },
 )
@@ -1206,22 +829,20 @@
     "_OptionalAutoExportRevisionToS3RequestDetailsTypeDef",
     {
         "Encryption": ExportServerSideEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class AutoExportRevisionToS3RequestDetailsTypeDef(
     _RequiredAutoExportRevisionToS3RequestDetailsTypeDef,
     _OptionalAutoExportRevisionToS3RequestDetailsTypeDef,
 ):
     pass
 
-
 _RequiredExportAssetsToS3RequestDetailsTypeDef = TypedDict(
     "_RequiredExportAssetsToS3RequestDetailsTypeDef",
     {
         "AssetDestinations": Sequence[AssetDestinationEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -1230,65 +851,108 @@
     "_OptionalExportAssetsToS3RequestDetailsTypeDef",
     {
         "Encryption": ExportServerSideEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class ExportAssetsToS3RequestDetailsTypeDef(
     _RequiredExportAssetsToS3RequestDetailsTypeDef, _OptionalExportAssetsToS3RequestDetailsTypeDef
 ):
     pass
 
+_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
+    {
+        "AssetDestinations": List[AssetDestinationEntryTypeDef],
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
+    {
+        "Encryption": ExportServerSideEncryptionTypeDef,
+    },
+    total=False,
+)
 
-CreateDataSetResponseTypeDef = TypedDict(
-    "CreateDataSetResponseTypeDef",
+class ExportAssetsToS3ResponseDetailsTypeDef(
+    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
+):
+    pass
+
+_RequiredDataSetEntryTypeDef = TypedDict(
+    "_RequiredDataSetEntryTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
+        "UpdatedAt": datetime,
+    },
+)
+_OptionalDataSetEntryTypeDef = TypedDict(
+    "_OptionalDataSetEntryTypeDef",
+    {
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-_RequiredDataSetEntryTypeDef = TypedDict(
-    "_RequiredDataSetEntryTypeDef",
+class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
+    pass
+
+CreateDataSetResponseTypeDef = TypedDict(
+    "CreateDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
+        "OriginDetails": OriginDetailsTypeDef,
+        "SourceId": str,
+        "Tags": Dict[str, str],
         "UpdatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDataSetEntryTypeDef = TypedDict(
-    "_OptionalDataSetEntryTypeDef",
+
+CreateRevisionResponseTypeDef = TypedDict(
+    "CreateRevisionResponseTypeDef",
     {
-        "OriginDetails": OriginDetailsTypeDef,
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
         "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
-    pass
-
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetDataSetResponseTypeDef = TypedDict(
     "GetDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
@@ -1296,15 +960,69 @@
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "Tags": Dict[str, str],
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRevisionResponseTypeDef = TypedDict(
+    "GetRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RevokeRevisionResponseTypeDef = TypedDict(
+    "RevokeRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendApiAssetResponseTypeDef = TypedDict(
+    "SendApiAssetResponseTypeDef",
+    {
+        "Body": str,
+        "ResponseHeaders": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataSetResponseTypeDef = TypedDict(
     "UpdateDataSetResponseTypeDef",
     {
         "Arn": str,
@@ -1313,15 +1031,33 @@
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRevisionResponseTypeDef = TypedDict(
+    "UpdateRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatabaseLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
     "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     {
         "Expression": List[LFTagOutputTypeDef],
@@ -1367,23 +1103,15 @@
     },
 )
 
 DetailsTypeDef = TypedDict(
     "DetailsTypeDef",
     {
         "ImportAssetFromSignedUrlJobErrorDetails": ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
-        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryOutputTypeDef],
-    },
-    total=False,
-)
-
-EventOutputTypeDef = TypedDict(
-    "EventOutputTypeDef",
-    {
-        "RevisionPublished": RevisionPublishedOutputTypeDef,
+        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryTypeDef],
     },
     total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
@@ -1403,59 +1131,55 @@
     "_OptionalExportRevisionsToS3RequestDetailsTypeDef",
     {
         "Encryption": ExportServerSideEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class ExportRevisionsToS3RequestDetailsTypeDef(
     _RequiredExportRevisionsToS3RequestDetailsTypeDef,
     _OptionalExportRevisionsToS3RequestDetailsTypeDef,
 ):
     pass
 
-
 _RequiredExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_RequiredExportRevisionsToS3ResponseDetailsTypeDef",
     {
         "DataSetId": str,
-        "RevisionDestinations": List[RevisionDestinationEntryOutputTypeDef],
+        "RevisionDestinations": List[RevisionDestinationEntryTypeDef],
     },
 )
 _OptionalExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_OptionalExportRevisionsToS3ResponseDetailsTypeDef",
     {
-        "Encryption": ExportServerSideEncryptionOutputTypeDef,
+        "Encryption": ExportServerSideEncryptionTypeDef,
         "EventActionArn": str,
     },
     total=False,
 )
 
-
 class ExportRevisionsToS3ResponseDetailsTypeDef(
     _RequiredExportRevisionsToS3ResponseDetailsTypeDef,
     _OptionalExportRevisionsToS3ResponseDetailsTypeDef,
 ):
     pass
 
-
 ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     {
         "AssetSources": Sequence[RedshiftDataShareAssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
 ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef = TypedDict(
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     {
-        "AssetSources": List[RedshiftDataShareAssetSourceEntryOutputTypeDef],
+        "AssetSources": List[RedshiftDataShareAssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
 _RequiredS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetSourceEntryOutputTypeDef",
@@ -1464,106 +1188,161 @@
     },
 )
 _OptionalS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
     "_OptionalS3DataAccessAssetSourceEntryOutputTypeDef",
     {
         "KeyPrefixes": List[str],
         "Keys": List[str],
-        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
+        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
     },
     total=False,
 )
 
-
 class S3DataAccessAssetSourceEntryOutputTypeDef(
     _RequiredS3DataAccessAssetSourceEntryOutputTypeDef,
     _OptionalS3DataAccessAssetSourceEntryOutputTypeDef,
 ):
     pass
 
+_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "KeyPrefixes": Sequence[str],
+        "Keys": Sequence[str],
+        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+    },
+    total=False,
+)
+
+class S3DataAccessAssetSourceEntryTypeDef(
+    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+):
+    pass
 
 _RequiredS3DataAccessAssetTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3DataAccessAssetTypeDef = TypedDict(
     "_OptionalS3DataAccessAssetTypeDef",
     {
         "KeyPrefixes": List[str],
         "Keys": List[str],
         "S3AccessPointAlias": str,
         "S3AccessPointArn": str,
-        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
+        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
     },
     total=False,
 )
 
-
 class S3DataAccessAssetTypeDef(
     _RequiredS3DataAccessAssetTypeDef, _OptionalS3DataAccessAssetTypeDef
 ):
     pass
 
-
-_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     {
-        "Bucket": str,
+        "DataSetId": str,
     },
 )
-_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     {
-        "KeyPrefixes": Sequence[str],
-        "Keys": Sequence[str],
-        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class S3DataAccessAssetSourceEntryTypeDef(
-    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
+    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
 ):
     pass
 
+ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "Origin": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ListDataSetRevisionsResponseTypeDef = TypedDict(
-    "ListDataSetRevisionsResponseTypeDef",
+ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
     {
-        "NextToken": str,
-        "Revisions": List[RevisionEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EventSourceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
     {
-        "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsOutputTypeDef,
+        "DataSetId": str,
+        "RevisionId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
+    {
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
+    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+):
+    pass
+
+ListDataSetRevisionsResponseTypeDef = TypedDict(
+    "ListDataSetRevisionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Revisions": List[RevisionEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsTypeDef,
     },
     total=False,
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
     "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "CatalogId": str,
@@ -1577,22 +1356,20 @@
     {
         "Database": DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
         "Table": TableLFTagPolicyAndPermissionsOutputTypeDef,
     },
     total=False,
 )
 
-
 class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
     _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
 ):
     pass
 
-
 LFResourceDetailsTypeDef = TypedDict(
     "LFResourceDetailsTypeDef",
     {
         "Database": DatabaseLFTagPolicyTypeDef,
         "Table": TableLFTagPolicyTypeDef,
     },
     total=False,
@@ -1612,22 +1389,20 @@
     {
         "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
         "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
-
 class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
     _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
 ):
     pass
 
-
 _RequiredJobErrorTypeDef = TypedDict(
     "_RequiredJobErrorTypeDef",
     {
         "Code": CodeType,
         "Message": str,
     },
 )
@@ -1639,19 +1414,17 @@
         "LimitValue": float,
         "ResourceId": str,
         "ResourceType": JobErrorResourceTypesType,
     },
     total=False,
 )
 
-
 class JobErrorTypeDef(_RequiredJobErrorTypeDef, _OptionalJobErrorTypeDef):
     pass
 
-
 CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
     "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     {
         "AssetSource": S3DataAccessAssetSourceEntryOutputTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -1662,70 +1435,57 @@
     {
         "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
+CreateEventActionRequestRequestTypeDef = TypedDict(
+    "CreateEventActionRequestRequestTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "Event": EventTypeDef,
+    },
+)
+
 CreateEventActionResponseTypeDef = TypedDict(
     "CreateEventActionResponseTypeDef",
     {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
+        "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventActionEntryTypeDef = TypedDict(
     "EventActionEntryTypeDef",
     {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
+        "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
     },
 )
 
 GetEventActionResponseTypeDef = TypedDict(
     "GetEventActionResponseTypeDef",
     {
-        "Action": ActionOutputTypeDef,
-        "Arn": str,
-        "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
-        "Id": str,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateEventActionResponseTypeDef = TypedDict(
-    "UpdateEventActionResponseTypeDef",
-    {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
+        "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEventActionRequestRequestTypeDef = TypedDict(
-    "CreateEventActionRequestRequestTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "Event": EventTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateEventActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventActionRequestRequestTypeDef",
     {
         "EventActionId": str,
@@ -1735,20 +1495,31 @@
     "_OptionalUpdateEventActionRequestRequestTypeDef",
     {
         "Action": ActionTypeDef,
     },
     total=False,
 )
 
-
 class UpdateEventActionRequestRequestTypeDef(
     _RequiredUpdateEventActionRequestRequestTypeDef, _OptionalUpdateEventActionRequestRequestTypeDef
 ):
     pass
 
+UpdateEventActionResponseTypeDef = TypedDict(
+    "UpdateEventActionResponseTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Event": EventTypeDef,
+        "Id": str,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 LFTagPolicyDetailsTypeDef = TypedDict(
     "LFTagPolicyDetailsTypeDef",
     {
         "CatalogId": str,
         "ResourceType": LFResourceTypeType,
         "ResourceDetails": LFResourceDetailsTypeDef,
@@ -1796,15 +1567,15 @@
 )
 
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LakeFormationDataPermissionDetailsTypeDef = TypedDict(
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
@@ -1819,30 +1590,30 @@
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobEntryTypeDef = TypedDict(
     "_RequiredJobEntryTypeDef",
     {
         "Arn": str,
@@ -1858,19 +1629,17 @@
     "_OptionalJobEntryTypeDef",
     {
         "Errors": List[JobErrorTypeDef],
     },
     total=False,
 )
 
-
 class JobEntryTypeDef(_RequiredJobEntryTypeDef, _OptionalJobEntryTypeDef):
     pass
 
-
 CreateJobRequestRequestTypeDef = TypedDict(
     "CreateJobRequestRequestTypeDef",
     {
         "Details": RequestDetailsTypeDef,
         "Type": TypeType,
     },
 )
@@ -1887,28 +1656,26 @@
     "_OptionalLakeFormationDataPermissionAssetTypeDef",
     {
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class LakeFormationDataPermissionAssetTypeDef(
     _RequiredLakeFormationDataPermissionAssetTypeDef,
     _OptionalLakeFormationDataPermissionAssetTypeDef,
 ):
     pass
 
-
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssetDetailsTypeDef = TypedDict(
     "AssetDetailsTypeDef",
     {
         "S3SnapshotAsset": S3SnapshotAssetTypeDef,
@@ -1938,33 +1705,31 @@
     "_OptionalAssetEntryTypeDef",
     {
         "SourceId": str,
     },
     total=False,
 )
 
-
 class AssetEntryTypeDef(_RequiredAssetEntryTypeDef, _OptionalAssetEntryTypeDef):
     pass
 
-
 GetAssetResponseTypeDef = TypedDict(
     "GetAssetResponseTypeDef",
     {
         "Arn": str,
         "AssetDetails": AssetDetailsTypeDef,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssetResponseTypeDef = TypedDict(
     "UpdateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -1973,19 +1738,19 @@
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRevisionAssetsResponseTypeDef = TypedDict(
     "ListRevisionAssetsResponseTypeDef",
     {
         "Assets": List[AssetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.pyi` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,127 +34,117 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ApiGatewayApiAssetTypeDef",
-    "AssetDestinationEntryOutputTypeDef",
     "AssetDestinationEntryTypeDef",
     "RedshiftDataShareAssetTypeDef",
     "S3SnapshotAssetTypeDef",
-    "AssetSourceEntryOutputTypeDef",
     "AssetSourceEntryTypeDef",
-    "AutoExportRevisionDestinationEntryOutputTypeDef",
     "AutoExportRevisionDestinationEntryTypeDef",
-    "ExportServerSideEncryptionOutputTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRevisionRequestRequestTypeDef",
-    "CreateRevisionResponseTypeDef",
     "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "RevisionPublishedOutputTypeDef",
     "RevisionPublishedTypeDef",
     "ExportAssetToSignedUrlRequestDetailsTypeDef",
     "ExportAssetToSignedUrlResponseDetailsTypeDef",
     "RevisionDestinationEntryTypeDef",
-    "RevisionDestinationEntryOutputTypeDef",
     "GetAssetRequestRequestTypeDef",
     "GetDataSetRequestRequestTypeDef",
     "GetEventActionRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetRevisionRequestRequestTypeDef",
-    "GetRevisionResponseTypeDef",
     "ImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     "ImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     "ImportAssetFromSignedUrlResponseDetailsTypeDef",
     "RedshiftDataShareAssetSourceEntryTypeDef",
-    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
-    "KmsKeyToGrantOutputTypeDef",
     "KmsKeyToGrantTypeDef",
-    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDataSetRevisionsRequestRequestTypeDef",
     "RevisionEntryTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
     "ListEventActionsRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListRevisionAssetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeRevisionRequestRequestTypeDef",
-    "RevokeRevisionResponseTypeDef",
     "SendApiAssetRequestRequestTypeDef",
-    "SendApiAssetResponseTypeDef",
     "StartJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "UpdateRevisionRequestRequestTypeDef",
-    "UpdateRevisionResponseTypeDef",
-    "ImportAssetsFromS3ResponseDetailsTypeDef",
     "ImportAssetsFromS3RequestDetailsTypeDef",
-    "AutoExportRevisionToS3RequestDetailsOutputTypeDef",
-    "ExportAssetsToS3ResponseDetailsTypeDef",
+    "ImportAssetsFromS3ResponseDetailsTypeDef",
     "AutoExportRevisionToS3RequestDetailsTypeDef",
     "ExportAssetsToS3RequestDetailsTypeDef",
-    "CreateDataSetResponseTypeDef",
+    "ExportAssetsToS3ResponseDetailsTypeDef",
     "DataSetEntryTypeDef",
+    "CreateDataSetResponseTypeDef",
+    "CreateRevisionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetDataSetResponseTypeDef",
+    "GetRevisionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RevokeRevisionResponseTypeDef",
+    "SendApiAssetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
+    "UpdateRevisionResponseTypeDef",
     "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     "DatabaseLFTagPolicyTypeDef",
     "TableLFTagPolicyAndPermissionsOutputTypeDef",
     "TableLFTagPolicyTypeDef",
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
     "TableLFTagPolicyAndPermissionsTypeDef",
     "DetailsTypeDef",
-    "EventOutputTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     "S3DataAccessAssetSourceEntryOutputTypeDef",
-    "S3DataAccessAssetTypeDef",
     "S3DataAccessAssetSourceEntryTypeDef",
+    "S3DataAccessAssetTypeDef",
+    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "JobErrorTypeDef",
     "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+    "CreateEventActionRequestRequestTypeDef",
     "CreateEventActionResponseTypeDef",
     "EventActionEntryTypeDef",
     "GetEventActionResponseTypeDef",
-    "UpdateEventActionResponseTypeDef",
-    "CreateEventActionRequestRequestTypeDef",
     "UpdateEventActionRequestRequestTypeDef",
+    "UpdateEventActionResponseTypeDef",
     "LFTagPolicyDetailsTypeDef",
     "ResponseDetailsTypeDef",
     "RequestDetailsTypeDef",
     "ListEventActionsResponseTypeDef",
     "LakeFormationDataPermissionDetailsTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
@@ -181,34 +171,14 @@
         "ApiSpecificationDownloadUrlExpiresAt": datetime,
         "ProtocolType": Literal["REST"],
         "Stage": str,
     },
     total=False,
 )
 
-_RequiredAssetDestinationEntryOutputTypeDef = TypedDict(
-    "_RequiredAssetDestinationEntryOutputTypeDef",
-    {
-        "AssetId": str,
-        "Bucket": str,
-    },
-)
-_OptionalAssetDestinationEntryOutputTypeDef = TypedDict(
-    "_OptionalAssetDestinationEntryOutputTypeDef",
-    {
-        "Key": str,
-    },
-    total=False,
-)
-
-class AssetDestinationEntryOutputTypeDef(
-    _RequiredAssetDestinationEntryOutputTypeDef, _OptionalAssetDestinationEntryOutputTypeDef
-):
-    pass
-
 _RequiredAssetDestinationEntryTypeDef = TypedDict(
     "_RequiredAssetDestinationEntryTypeDef",
     {
         "AssetId": str,
         "Bucket": str,
     },
 )
@@ -216,108 +186,64 @@
     "_OptionalAssetDestinationEntryTypeDef",
     {
         "Key": str,
     },
     total=False,
 )
 
+
 class AssetDestinationEntryTypeDef(
     _RequiredAssetDestinationEntryTypeDef, _OptionalAssetDestinationEntryTypeDef
 ):
     pass
 
+
 RedshiftDataShareAssetTypeDef = TypedDict(
     "RedshiftDataShareAssetTypeDef",
     {
         "Arn": str,
     },
 )
 
 S3SnapshotAssetTypeDef = TypedDict(
     "S3SnapshotAssetTypeDef",
     {
         "Size": float,
     },
 )
 
-AssetSourceEntryOutputTypeDef = TypedDict(
-    "AssetSourceEntryOutputTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-
 AssetSourceEntryTypeDef = TypedDict(
     "AssetSourceEntryTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-_RequiredAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_RequiredAutoExportRevisionDestinationEntryOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_OptionalAutoExportRevisionDestinationEntryOutputTypeDef",
-    {
-        "KeyPattern": str,
-    },
-    total=False,
-)
-
-class AutoExportRevisionDestinationEntryOutputTypeDef(
-    _RequiredAutoExportRevisionDestinationEntryOutputTypeDef,
-    _OptionalAutoExportRevisionDestinationEntryOutputTypeDef,
-):
-    pass
-
 _RequiredAutoExportRevisionDestinationEntryTypeDef = TypedDict(
     "_RequiredAutoExportRevisionDestinationEntryTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalAutoExportRevisionDestinationEntryTypeDef = TypedDict(
     "_OptionalAutoExportRevisionDestinationEntryTypeDef",
     {
         "KeyPattern": str,
     },
     total=False,
 )
 
+
 class AutoExportRevisionDestinationEntryTypeDef(
     _RequiredAutoExportRevisionDestinationEntryTypeDef,
     _OptionalAutoExportRevisionDestinationEntryTypeDef,
 ):
     pass
 
-_RequiredExportServerSideEncryptionOutputTypeDef = TypedDict(
-    "_RequiredExportServerSideEncryptionOutputTypeDef",
-    {
-        "Type": ServerSideEncryptionTypesType,
-    },
-)
-_OptionalExportServerSideEncryptionOutputTypeDef = TypedDict(
-    "_OptionalExportServerSideEncryptionOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
-class ExportServerSideEncryptionOutputTypeDef(
-    _RequiredExportServerSideEncryptionOutputTypeDef,
-    _OptionalExportServerSideEncryptionOutputTypeDef,
-):
-    pass
 
 _RequiredExportServerSideEncryptionTypeDef = TypedDict(
     "_RequiredExportServerSideEncryptionTypeDef",
     {
         "Type": ServerSideEncryptionTypesType,
     },
 )
@@ -325,19 +251,21 @@
     "_OptionalExportServerSideEncryptionTypeDef",
     {
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class ExportServerSideEncryptionTypeDef(
     _RequiredExportServerSideEncryptionTypeDef, _OptionalExportServerSideEncryptionTypeDef
 ):
     pass
 
+
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -353,26 +281,39 @@
     "_OptionalCreateDataSetRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDataSetRequestRequestTypeDef(
     _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
 ):
     pass
 
+
 OriginDetailsTypeDef = TypedDict(
     "OriginDetailsTypeDef",
     {
         "ProductId": str,
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
 _RequiredCreateRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalCreateRevisionRequestRequestTypeDef = TypedDict(
@@ -380,37 +321,20 @@
     {
         "Comment": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRevisionRequestRequestTypeDef(
     _RequiredCreateRevisionRequestRequestTypeDef, _OptionalCreateRevisionRequestRequestTypeDef
 ):
     pass
 
-CreateRevisionResponseTypeDef = TypedDict(
-    "CreateRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 LFTagOutputTypeDef = TypedDict(
     "LFTagOutputTypeDef",
     {
         "TagKey": str,
         "TagValues": List[str],
     },
@@ -458,28 +382,14 @@
 ImportAssetFromSignedUrlJobErrorDetailsTypeDef = TypedDict(
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     {
         "AssetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RevisionPublishedOutputTypeDef = TypedDict(
-    "RevisionPublishedOutputTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-
 RevisionPublishedTypeDef = TypedDict(
     "RevisionPublishedTypeDef",
     {
         "DataSetId": str,
     },
 )
 
@@ -505,20 +415,22 @@
     {
         "SignedUrl": str,
         "SignedUrlExpiresAt": datetime,
     },
     total=False,
 )
 
+
 class ExportAssetToSignedUrlResponseDetailsTypeDef(
     _RequiredExportAssetToSignedUrlResponseDetailsTypeDef,
     _OptionalExportAssetToSignedUrlResponseDetailsTypeDef,
 ):
     pass
 
+
 _RequiredRevisionDestinationEntryTypeDef = TypedDict(
     "_RequiredRevisionDestinationEntryTypeDef",
     {
         "Bucket": str,
         "RevisionId": str,
     },
 )
@@ -526,38 +438,20 @@
     "_OptionalRevisionDestinationEntryTypeDef",
     {
         "KeyPattern": str,
     },
     total=False,
 )
 
+
 class RevisionDestinationEntryTypeDef(
     _RequiredRevisionDestinationEntryTypeDef, _OptionalRevisionDestinationEntryTypeDef
 ):
     pass
 
-_RequiredRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_RequiredRevisionDestinationEntryOutputTypeDef",
-    {
-        "Bucket": str,
-        "RevisionId": str,
-    },
-)
-_OptionalRevisionDestinationEntryOutputTypeDef = TypedDict(
-    "_OptionalRevisionDestinationEntryOutputTypeDef",
-    {
-        "KeyPattern": str,
-    },
-    total=False,
-)
-
-class RevisionDestinationEntryOutputTypeDef(
-    _RequiredRevisionDestinationEntryOutputTypeDef, _OptionalRevisionDestinationEntryOutputTypeDef
-):
-    pass
 
 GetAssetRequestRequestTypeDef = TypedDict(
     "GetAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
@@ -589,33 +483,14 @@
     "GetRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-GetRevisionResponseTypeDef = TypedDict(
-    "GetRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef = TypedDict(
     "_RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     {
         "ApiId": str,
         "ApiName": str,
         "ApiSpecificationMd5Hash": str,
         "DataSetId": str,
@@ -629,20 +504,22 @@
     {
         "ApiDescription": str,
         "ApiKey": str,
     },
     total=False,
 )
 
+
 class ImportAssetFromApiGatewayApiRequestDetailsTypeDef(
     _RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     _OptionalImportAssetFromApiGatewayApiRequestDetailsTypeDef,
 ):
     pass
 
+
 _RequiredImportAssetFromApiGatewayApiResponseDetailsTypeDef = TypedDict(
     "_RequiredImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     {
         "ApiId": str,
         "ApiName": str,
         "ApiSpecificationMd5Hash": str,
         "ApiSpecificationUploadUrl": str,
@@ -658,20 +535,22 @@
     {
         "ApiDescription": str,
         "ApiKey": str,
     },
     total=False,
 )
 
+
 class ImportAssetFromApiGatewayApiResponseDetailsTypeDef(
     _RequiredImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     _OptionalImportAssetFromApiGatewayApiResponseDetailsTypeDef,
 ):
     pass
 
+
 ImportAssetFromSignedUrlRequestDetailsTypeDef = TypedDict(
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     {
         "AssetName": str,
         "DataSetId": str,
         "Md5Hash": str,
         "RevisionId": str,
@@ -692,68 +571,46 @@
         "Md5Hash": str,
         "SignedUrl": str,
         "SignedUrlExpiresAt": datetime,
     },
     total=False,
 )
 
+
 class ImportAssetFromSignedUrlResponseDetailsTypeDef(
     _RequiredImportAssetFromSignedUrlResponseDetailsTypeDef,
     _OptionalImportAssetFromSignedUrlResponseDetailsTypeDef,
 ):
     pass
 
+
 RedshiftDataShareAssetSourceEntryTypeDef = TypedDict(
     "RedshiftDataShareAssetSourceEntryTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
-RedshiftDataShareAssetSourceEntryOutputTypeDef = TypedDict(
-    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
-    {
-        "DataShareArn": str,
-    },
-)
-
-KmsKeyToGrantOutputTypeDef = TypedDict(
-    "KmsKeyToGrantOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-)
-
 KmsKeyToGrantTypeDef = TypedDict(
     "KmsKeyToGrantTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
-_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
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
 
-class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
-    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDataSetRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetRevisionsRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalListDataSetRevisionsRequestRequestTypeDef = TypedDict(
@@ -761,20 +618,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDataSetRevisionsRequestRequestTypeDef(
     _RequiredListDataSetRevisionsRequestRequestTypeDef,
     _OptionalListDataSetRevisionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRevisionEntryTypeDef = TypedDict(
     "_RequiredRevisionEntryTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
@@ -790,97 +649,50 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
     },
     total=False,
 )
 
+
 class RevisionEntryTypeDef(_RequiredRevisionEntryTypeDef, _OptionalRevisionEntryTypeDef):
     pass
 
-ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "Origin": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDataSetsRequestRequestTypeDef = TypedDict(
     "ListDataSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Origin": str,
     },
     total=False,
 )
 
-ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
-    {
-        "EventSourceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEventActionsRequestRequestTypeDef = TypedDict(
     "ListEventActionsRequestRequestTypeDef",
     {
         "EventSourceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "MaxResults": int,
         "NextToken": str,
         "RevisionId": str,
     },
     total=False,
 )
 
-_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
-_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
-    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRevisionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListRevisionAssetsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
@@ -889,83 +701,38 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRevisionAssetsRequestRequestTypeDef(
     _RequiredListRevisionAssetsRequestRequestTypeDef,
     _OptionalListRevisionAssetsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
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
 RevokeRevisionRequestRequestTypeDef = TypedDict(
     "RevokeRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
         "RevocationComment": str,
     },
 )
 
-RevokeRevisionResponseTypeDef = TypedDict(
-    "RevokeRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendApiAssetRequestRequestTypeDef = TypedDict(
     "_RequiredSendApiAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -978,27 +745,20 @@
         "RequestHeaders": Mapping[str, str],
         "Method": str,
         "Path": str,
     },
     total=False,
 )
 
+
 class SendApiAssetRequestRequestTypeDef(
     _RequiredSendApiAssetRequestRequestTypeDef, _OptionalSendApiAssetRequestRequestTypeDef
 ):
     pass
 
-SendApiAssetResponseTypeDef = TypedDict(
-    "SendApiAssetResponseTypeDef",
-    {
-        "Body": str,
-        "ResponseHeaders": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 StartJobRequestRequestTypeDef = TypedDict(
     "StartJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
@@ -1040,19 +800,21 @@
     {
         "Description": str,
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateDataSetRequestRequestTypeDef(
     _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
@@ -1061,95 +823,38 @@
     {
         "Comment": str,
         "Finalized": bool,
     },
     total=False,
 )
 
+
 class UpdateRevisionRequestRequestTypeDef(
     _RequiredUpdateRevisionRequestRequestTypeDef, _OptionalUpdateRevisionRequestRequestTypeDef
 ):
     pass
 
-UpdateRevisionResponseTypeDef = TypedDict(
-    "UpdateRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
-    "ImportAssetsFromS3ResponseDetailsTypeDef",
-    {
-        "AssetSources": List[AssetSourceEntryOutputTypeDef],
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
 
 ImportAssetsFromS3RequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromS3RequestDetailsTypeDef",
     {
         "AssetSources": Sequence[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
-    "_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef",
-    {
-        "RevisionDestination": AutoExportRevisionDestinationEntryOutputTypeDef,
-    },
-)
-_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
-    "_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef",
-    {
-        "Encryption": ExportServerSideEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-class AutoExportRevisionToS3RequestDetailsOutputTypeDef(
-    _RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef,
-    _OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef,
-):
-    pass
-
-_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
+ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
+    "ImportAssetsFromS3ResponseDetailsTypeDef",
     {
-        "AssetDestinations": List[AssetDestinationEntryOutputTypeDef],
+        "AssetSources": List[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
-    {
-        "Encryption": ExportServerSideEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-class ExportAssetsToS3ResponseDetailsTypeDef(
-    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
-):
-    pass
 
 _RequiredAutoExportRevisionToS3RequestDetailsTypeDef = TypedDict(
     "_RequiredAutoExportRevisionToS3RequestDetailsTypeDef",
     {
         "RevisionDestination": AutoExportRevisionDestinationEntryTypeDef,
     },
 )
@@ -1157,20 +862,22 @@
     "_OptionalAutoExportRevisionToS3RequestDetailsTypeDef",
     {
         "Encryption": ExportServerSideEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class AutoExportRevisionToS3RequestDetailsTypeDef(
     _RequiredAutoExportRevisionToS3RequestDetailsTypeDef,
     _OptionalAutoExportRevisionToS3RequestDetailsTypeDef,
 ):
     pass
 
+
 _RequiredExportAssetsToS3RequestDetailsTypeDef = TypedDict(
     "_RequiredExportAssetsToS3RequestDetailsTypeDef",
     {
         "AssetDestinations": Sequence[AssetDestinationEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -1179,61 +886,114 @@
     "_OptionalExportAssetsToS3RequestDetailsTypeDef",
     {
         "Encryption": ExportServerSideEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class ExportAssetsToS3RequestDetailsTypeDef(
     _RequiredExportAssetsToS3RequestDetailsTypeDef, _OptionalExportAssetsToS3RequestDetailsTypeDef
 ):
     pass
 
-CreateDataSetResponseTypeDef = TypedDict(
-    "CreateDataSetResponseTypeDef",
+
+_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
+    {
+        "AssetDestinations": List[AssetDestinationEntryTypeDef],
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
+    {
+        "Encryption": ExportServerSideEncryptionTypeDef,
+    },
+    total=False,
+)
+
+
+class ExportAssetsToS3ResponseDetailsTypeDef(
+    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
+):
+    pass
+
+
+_RequiredDataSetEntryTypeDef = TypedDict(
+    "_RequiredDataSetEntryTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
+        "UpdatedAt": datetime,
+    },
+)
+_OptionalDataSetEntryTypeDef = TypedDict(
+    "_OptionalDataSetEntryTypeDef",
+    {
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-_RequiredDataSetEntryTypeDef = TypedDict(
-    "_RequiredDataSetEntryTypeDef",
+
+class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
+    pass
+
+
+CreateDataSetResponseTypeDef = TypedDict(
+    "CreateDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
+        "OriginDetails": OriginDetailsTypeDef,
+        "SourceId": str,
+        "Tags": Dict[str, str],
         "UpdatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDataSetEntryTypeDef = TypedDict(
-    "_OptionalDataSetEntryTypeDef",
+
+CreateRevisionResponseTypeDef = TypedDict(
+    "CreateRevisionResponseTypeDef",
     {
-        "OriginDetails": OriginDetailsTypeDef,
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
         "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetDataSetResponseTypeDef = TypedDict(
     "GetDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
@@ -1241,15 +1001,69 @@
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "Tags": Dict[str, str],
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRevisionResponseTypeDef = TypedDict(
+    "GetRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RevokeRevisionResponseTypeDef = TypedDict(
+    "RevokeRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendApiAssetResponseTypeDef = TypedDict(
+    "SendApiAssetResponseTypeDef",
+    {
+        "Body": str,
+        "ResponseHeaders": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataSetResponseTypeDef = TypedDict(
     "UpdateDataSetResponseTypeDef",
     {
         "Arn": str,
@@ -1258,15 +1072,33 @@
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRevisionResponseTypeDef = TypedDict(
+    "UpdateRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatabaseLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
     "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     {
         "Expression": List[LFTagOutputTypeDef],
@@ -1312,23 +1144,15 @@
     },
 )
 
 DetailsTypeDef = TypedDict(
     "DetailsTypeDef",
     {
         "ImportAssetFromSignedUrlJobErrorDetails": ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
-        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryOutputTypeDef],
-    },
-    total=False,
-)
-
-EventOutputTypeDef = TypedDict(
-    "EventOutputTypeDef",
-    {
-        "RevisionPublished": RevisionPublishedOutputTypeDef,
+        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryTypeDef],
     },
     total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
@@ -1348,55 +1172,59 @@
     "_OptionalExportRevisionsToS3RequestDetailsTypeDef",
     {
         "Encryption": ExportServerSideEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class ExportRevisionsToS3RequestDetailsTypeDef(
     _RequiredExportRevisionsToS3RequestDetailsTypeDef,
     _OptionalExportRevisionsToS3RequestDetailsTypeDef,
 ):
     pass
 
+
 _RequiredExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_RequiredExportRevisionsToS3ResponseDetailsTypeDef",
     {
         "DataSetId": str,
-        "RevisionDestinations": List[RevisionDestinationEntryOutputTypeDef],
+        "RevisionDestinations": List[RevisionDestinationEntryTypeDef],
     },
 )
 _OptionalExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_OptionalExportRevisionsToS3ResponseDetailsTypeDef",
     {
-        "Encryption": ExportServerSideEncryptionOutputTypeDef,
+        "Encryption": ExportServerSideEncryptionTypeDef,
         "EventActionArn": str,
     },
     total=False,
 )
 
+
 class ExportRevisionsToS3ResponseDetailsTypeDef(
     _RequiredExportRevisionsToS3ResponseDetailsTypeDef,
     _OptionalExportRevisionsToS3ResponseDetailsTypeDef,
 ):
     pass
 
+
 ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     {
         "AssetSources": Sequence[RedshiftDataShareAssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
 ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef = TypedDict(
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     {
-        "AssetSources": List[RedshiftDataShareAssetSourceEntryOutputTypeDef],
+        "AssetSources": List[RedshiftDataShareAssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
 _RequiredS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetSourceEntryOutputTypeDef",
@@ -1405,100 +1233,171 @@
     },
 )
 _OptionalS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
     "_OptionalS3DataAccessAssetSourceEntryOutputTypeDef",
     {
         "KeyPrefixes": List[str],
         "Keys": List[str],
-        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
+        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
     },
     total=False,
 )
 
+
 class S3DataAccessAssetSourceEntryOutputTypeDef(
     _RequiredS3DataAccessAssetSourceEntryOutputTypeDef,
     _OptionalS3DataAccessAssetSourceEntryOutputTypeDef,
 ):
     pass
 
+
+_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "KeyPrefixes": Sequence[str],
+        "Keys": Sequence[str],
+        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+    },
+    total=False,
+)
+
+
+class S3DataAccessAssetSourceEntryTypeDef(
+    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+):
+    pass
+
+
 _RequiredS3DataAccessAssetTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3DataAccessAssetTypeDef = TypedDict(
     "_OptionalS3DataAccessAssetTypeDef",
     {
         "KeyPrefixes": List[str],
         "Keys": List[str],
         "S3AccessPointAlias": str,
         "S3AccessPointArn": str,
-        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
+        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
     },
     total=False,
 )
 
+
 class S3DataAccessAssetTypeDef(
     _RequiredS3DataAccessAssetTypeDef, _OptionalS3DataAccessAssetTypeDef
 ):
     pass
 
-_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+
+_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     {
-        "Bucket": str,
+        "DataSetId": str,
     },
 )
-_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     {
-        "KeyPrefixes": Sequence[str],
-        "Keys": Sequence[str],
-        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class S3DataAccessAssetSourceEntryTypeDef(
-    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+
+class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
+    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
 ):
     pass
 
-ListDataSetRevisionsResponseTypeDef = TypedDict(
-    "ListDataSetRevisionsResponseTypeDef",
+
+ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     {
-        "NextToken": str,
-        "Revisions": List[RevisionEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Origin": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
+    {
+        "EventSourceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "DataSetId": str,
+        "RevisionId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
+_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     {
-        "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsOutputTypeDef,
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
+    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+):
+    pass
+
+
+ListDataSetRevisionsResponseTypeDef = TypedDict(
+    "ListDataSetRevisionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Revisions": List[RevisionEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsTypeDef,
     },
     total=False,
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
     "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "CatalogId": str,
@@ -1512,20 +1411,22 @@
     {
         "Database": DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
         "Table": TableLFTagPolicyAndPermissionsOutputTypeDef,
     },
     total=False,
 )
 
+
 class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
     _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
 ):
     pass
 
+
 LFResourceDetailsTypeDef = TypedDict(
     "LFResourceDetailsTypeDef",
     {
         "Database": DatabaseLFTagPolicyTypeDef,
         "Table": TableLFTagPolicyTypeDef,
     },
     total=False,
@@ -1545,20 +1446,22 @@
     {
         "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
         "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
+
 class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
     _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
 ):
     pass
 
+
 _RequiredJobErrorTypeDef = TypedDict(
     "_RequiredJobErrorTypeDef",
     {
         "Code": CodeType,
         "Message": str,
     },
 )
@@ -1570,17 +1473,19 @@
         "LimitValue": float,
         "ResourceId": str,
         "ResourceType": JobErrorResourceTypesType,
     },
     total=False,
 )
 
+
 class JobErrorTypeDef(_RequiredJobErrorTypeDef, _OptionalJobErrorTypeDef):
     pass
 
+
 CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
     "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     {
         "AssetSource": S3DataAccessAssetSourceEntryOutputTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -1591,70 +1496,57 @@
     {
         "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
+CreateEventActionRequestRequestTypeDef = TypedDict(
+    "CreateEventActionRequestRequestTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "Event": EventTypeDef,
+    },
+)
+
 CreateEventActionResponseTypeDef = TypedDict(
     "CreateEventActionResponseTypeDef",
     {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
+        "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventActionEntryTypeDef = TypedDict(
     "EventActionEntryTypeDef",
     {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
+        "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
     },
 )
 
 GetEventActionResponseTypeDef = TypedDict(
     "GetEventActionResponseTypeDef",
     {
-        "Action": ActionOutputTypeDef,
-        "Arn": str,
-        "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
-        "Id": str,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateEventActionResponseTypeDef = TypedDict(
-    "UpdateEventActionResponseTypeDef",
-    {
-        "Action": ActionOutputTypeDef,
+        "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventOutputTypeDef,
+        "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEventActionRequestRequestTypeDef = TypedDict(
-    "CreateEventActionRequestRequestTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "Event": EventTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateEventActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventActionRequestRequestTypeDef",
     {
         "EventActionId": str,
@@ -1664,19 +1556,34 @@
     "_OptionalUpdateEventActionRequestRequestTypeDef",
     {
         "Action": ActionTypeDef,
     },
     total=False,
 )
 
+
 class UpdateEventActionRequestRequestTypeDef(
     _RequiredUpdateEventActionRequestRequestTypeDef, _OptionalUpdateEventActionRequestRequestTypeDef
 ):
     pass
 
+
+UpdateEventActionResponseTypeDef = TypedDict(
+    "UpdateEventActionResponseTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Event": EventTypeDef,
+        "Id": str,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LFTagPolicyDetailsTypeDef = TypedDict(
     "LFTagPolicyDetailsTypeDef",
     {
         "CatalogId": str,
         "ResourceType": LFResourceTypeType,
         "ResourceDetails": LFResourceDetailsTypeDef,
     },
@@ -1723,15 +1630,15 @@
 )
 
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LakeFormationDataPermissionDetailsTypeDef = TypedDict(
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
@@ -1746,30 +1653,30 @@
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJobEntryTypeDef = TypedDict(
     "_RequiredJobEntryTypeDef",
     {
         "Arn": str,
@@ -1785,17 +1692,19 @@
     "_OptionalJobEntryTypeDef",
     {
         "Errors": List[JobErrorTypeDef],
     },
     total=False,
 )
 
+
 class JobEntryTypeDef(_RequiredJobEntryTypeDef, _OptionalJobEntryTypeDef):
     pass
 
+
 CreateJobRequestRequestTypeDef = TypedDict(
     "CreateJobRequestRequestTypeDef",
     {
         "Details": RequestDetailsTypeDef,
         "Type": TypeType,
     },
 )
@@ -1812,26 +1721,28 @@
     "_OptionalLakeFormationDataPermissionAssetTypeDef",
     {
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class LakeFormationDataPermissionAssetTypeDef(
     _RequiredLakeFormationDataPermissionAssetTypeDef,
     _OptionalLakeFormationDataPermissionAssetTypeDef,
 ):
     pass
 
+
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssetDetailsTypeDef = TypedDict(
     "AssetDetailsTypeDef",
     {
         "S3SnapshotAsset": S3SnapshotAssetTypeDef,
@@ -1861,31 +1772,33 @@
     "_OptionalAssetEntryTypeDef",
     {
         "SourceId": str,
     },
     total=False,
 )
 
+
 class AssetEntryTypeDef(_RequiredAssetEntryTypeDef, _OptionalAssetEntryTypeDef):
     pass
 
+
 GetAssetResponseTypeDef = TypedDict(
     "GetAssetResponseTypeDef",
     {
         "Arn": str,
         "AssetDetails": AssetDetailsTypeDef,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssetResponseTypeDef = TypedDict(
     "UpdateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -1894,19 +1807,19 @@
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRevisionAssetsResponseTypeDef = TypedDict(
     "ListRevisionAssetsResponseTypeDef",
     {
         "Assets": List[AssetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/PKG-INFO` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dataexchange
-Version: 1.28.12
-Summary: Type annotations for boto3.DataExchange 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DataExchange 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dataexchange)](https://pepy.tech/project/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,125 +352,114 @@
 
 `mypy_boto3_dataexchange.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dataexchange.type_defs import (
     ApiGatewayApiAssetTypeDef,
-    AssetDestinationEntryOutputTypeDef,
     AssetDestinationEntryTypeDef,
     RedshiftDataShareAssetTypeDef,
     S3SnapshotAssetTypeDef,
-    AssetSourceEntryOutputTypeDef,
     AssetSourceEntryTypeDef,
-    AutoExportRevisionDestinationEntryOutputTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
-    ExportServerSideEncryptionOutputTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateRevisionRequestRequestTypeDef,
-    CreateRevisionResponseTypeDef,
     LFTagOutputTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
-    RevisionPublishedOutputTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
-    RevisionDestinationEntryOutputTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
-    GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
-    RedshiftDataShareAssetSourceEntryOutputTypeDef,
-    KmsKeyToGrantOutputTypeDef,
     KmsKeyToGrantTypeDef,
-    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
-    ListEventActionsRequestListEventActionsPaginateTypeDef,
     ListEventActionsRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListRevisionAssetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RevokeRevisionRequestRequestTypeDef,
-    RevokeRevisionResponseTypeDef,
     SendApiAssetRequestRequestTypeDef,
-    SendApiAssetResponseTypeDef,
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
-    UpdateRevisionResponseTypeDef,
-    ImportAssetsFromS3ResponseDetailsTypeDef,
     ImportAssetsFromS3RequestDetailsTypeDef,
-    AutoExportRevisionToS3RequestDetailsOutputTypeDef,
-    ExportAssetsToS3ResponseDetailsTypeDef,
+    ImportAssetsFromS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
-    CreateDataSetResponseTypeDef,
+    ExportAssetsToS3ResponseDetailsTypeDef,
     DataSetEntryTypeDef,
+    CreateDataSetResponseTypeDef,
+    CreateRevisionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetDataSetResponseTypeDef,
+    GetRevisionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RevokeRevisionResponseTypeDef,
+    SendApiAssetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
+    UpdateRevisionResponseTypeDef,
     DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
     DatabaseLFTagPolicyTypeDef,
     TableLFTagPolicyAndPermissionsOutputTypeDef,
     TableLFTagPolicyTypeDef,
     DatabaseLFTagPolicyAndPermissionsTypeDef,
     TableLFTagPolicyAndPermissionsTypeDef,
     DetailsTypeDef,
-    EventOutputTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
     S3DataAccessAssetSourceEntryOutputTypeDef,
-    S3DataAccessAssetTypeDef,
     S3DataAccessAssetSourceEntryTypeDef,
+    S3DataAccessAssetTypeDef,
+    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
+    ListEventActionsRequestListEventActionsPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListDataSetRevisionsResponseTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     JobErrorTypeDef,
     CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
     CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
+    CreateEventActionRequestRequestTypeDef,
     CreateEventActionResponseTypeDef,
     EventActionEntryTypeDef,
     GetEventActionResponseTypeDef,
-    UpdateEventActionResponseTypeDef,
-    CreateEventActionRequestRequestTypeDef,
     UpdateEventActionRequestRequestTypeDef,
+    UpdateEventActionResponseTypeDef,
     LFTagPolicyDetailsTypeDef,
     ResponseDetailsTypeDef,
     RequestDetailsTypeDef,
     ListEventActionsResponseTypeDef,
     LakeFormationDataPermissionDetailsTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
```

### Comparing `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/SOURCES.txt` & `mypy-boto3-dataexchange-1.28.15/mypy_boto3_dataexchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.12/setup.py` & `mypy-boto3-dataexchange-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dataexchange",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_dataexchange"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataExchange 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.DataExchange 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

