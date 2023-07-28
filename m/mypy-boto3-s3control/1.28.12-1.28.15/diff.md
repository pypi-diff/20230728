# Comparing `tmp/mypy-boto3-s3control-1.28.12.tar.gz` & `tmp/mypy-boto3-s3control-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3control-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
+gzip compressed data, was "mypy-boto3-s3control-1.28.15.tar", last modified: Fri Jul 28 20:43:38 2023, max compression
```

## Comparing `mypy-boto3-s3control-1.28.12.tar` & `mypy-boto3-s3control-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24322 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43055 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98307 2023-07-27 11:45:19.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98192 2023-07-27 11:45:18.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22529 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43055 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-28 20:37:44.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85262 2023-07-28 20:37:46.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85163 2023-07-28 20:37:45.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:38.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:37.000000 mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:38.185788 mypy-boto3-s3control-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:37:43.000000 mypy-boto3-s3control-1.28.15/setup.py
```

### Comparing `mypy-boto3-s3control-1.28.12/LICENSE` & `mypy-boto3-s3control-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/PKG-INFO` & `mypy-boto3-s3control-1.28.15/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-s3control
-Version: 1.28.12
-Summary: Type annotations for boto3.S3Control 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 s3control type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,164 +332,130 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
-    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
-    VpcConfigurationOutputTypeDef,
-    ActivityMetricsOutputTypeDef,
-    AdvancedCostOptimizationMetricsOutputTypeDef,
-    AdvancedDataProtectionMetricsOutputTypeDef,
-    DetailedStatusCodesMetricsOutputTypeDef,
+    VpcConfigurationTypeDef,
     ActivityMetricsTypeDef,
     AdvancedCostOptimizationMetricsTypeDef,
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
-    DeleteMultiRegionAccessPointInputOutputTypeDef,
-    PutMultiRegionAccessPointPolicyInputOutputTypeDef,
-    AwsLambdaTransformationOutputTypeDef,
+    DeleteMultiRegionAccessPointInputTypeDef,
+    PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
-    CloudWatchMetricsOutputTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
     ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    VpcConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
-    PublicAccessBlockConfigurationOutputTypeDef,
-    RegionOutputTypeDef,
     RegionTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
-    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteMultiRegionAccessPointInputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
     ExcludeOutputTypeDef,
     ExcludeTypeDef,
-    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
-    SSEKMSEncryptionOutputTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    S3TagOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    MultiRegionAccessPointRouteOutputTypeDef,
+    MultiRegionAccessPointRouteTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
-    StorageLensTagOutputTypeDef,
+    StorageLensTagTypeDef,
     IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
-    JobReportOutputTypeDef,
     JobManifestGeneratorFilterOutputTypeDef,
     JobManifestGeneratorFilterTypeDef,
-    JobManifestLocationOutputTypeDef,
     JobManifestLocationTypeDef,
     JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
-    LambdaInvokeOperationOutputTypeDef,
-    S3InitiateRestoreObjectOperationOutputTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
-    NoncurrentVersionExpirationOutputTypeDef,
-    NoncurrentVersionTransitionOutputTypeDef,
-    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
+    TransitionOutputTypeDef,
     TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
-    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
-    MultiRegionAccessPointRouteTypeDef,
-    SelectionCriteriaOutputTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
-    PutMultiRegionAccessPointPolicyInputTypeDef,
-    StorageLensTagTypeDef,
-    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
-    S3ObjectOwnerOutputTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataOutputTypeDef,
     S3ObjectMetadataTypeDef,
-    S3GranteeOutputTypeDef,
     S3GranteeTypeDef,
-    S3ObjectLockLegalHoldOutputTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionOutputTypeDef,
     S3RetentionTypeDef,
-    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
-    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StorageLensAwsOrgOutputTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
-    ObjectLambdaContentTransformationOutputTypeDef,
+    DeleteMultiRegionAccessPointRequestRequestTypeDef,
+    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
     ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
@@ -531,125 +465,113 @@
     GetAccessPointPolicyResultTypeDef,
     GetBucketPolicyResultTypeDef,
     GetBucketResultTypeDef,
     GetBucketVersioningResultTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
-    PutPublicAccessBlockRequestRequestTypeDef,
     CreateAccessPointRequestRequestTypeDef,
+    GetAccessPointForObjectLambdaResultTypeDef,
+    GetAccessPointResultTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    PutPublicAccessBlockRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
+    GetBucketTaggingResultTypeDef,
+    GetJobTaggingResultTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     PutJobTaggingRequestRequestTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
     ReplicationRuleAndOperatorTypeDef,
+    S3SetObjectTaggingOperationOutputTypeDef,
     S3SetObjectTaggingOperationTypeDef,
     TaggingTypeDef,
-    GetAccessPointForObjectLambdaResultTypeDef,
-    GetAccessPointResultTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
     CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
-    DeleteMultiRegionAccessPointRequestRequestTypeDef,
     GeneratedManifestEncryptionOutputTypeDef,
     GeneratedManifestEncryptionTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
-    GetBucketTaggingResultTypeDef,
-    GetJobTaggingResultTypeDef,
-    LifecycleRuleAndOperatorOutputTypeDef,
-    ReplicationRuleAndOperatorOutputTypeDef,
-    S3SetObjectTaggingOperationOutputTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
+    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
+    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
-    MetricsOutputTypeDef,
-    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
-    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    PrefixLevelStorageMetricsOutputTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
-    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
-    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
-    S3GrantOutputTypeDef,
     S3GrantTypeDef,
-    S3SetObjectLegalHoldOperationOutputTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationOutputTypeDef,
     S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
-    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
     LifecycleRuleFilterTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
-    LifecycleRuleFilterOutputTypeDef,
-    ReplicationRuleFilterOutputTypeDef,
     JobListDescriptorTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
-    PrefixLevelOutputTypeDef,
     PrefixLevelTypeDef,
     S3AccessControlListOutputTypeDef,
-    S3CopyObjectOperationOutputTypeDef,
     S3AccessControlListTypeDef,
+    S3CopyObjectOperationOutputTypeDef,
     S3CopyObjectOperationTypeDef,
     S3BucketDestinationOutputTypeDef,
     S3BucketDestinationTypeDef,
     ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
+    LifecycleRuleOutputTypeDef,
     LifecycleRuleTypeDef,
     S3JobManifestGeneratorOutputTypeDef,
     S3JobManifestGeneratorTypeDef,
-    LifecycleRuleOutputTypeDef,
     ListJobsResultTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     AsyncOperationTypeDef,
-    BucketLevelOutputTypeDef,
     BucketLevelTypeDef,
     S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
     StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
     CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
+    GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
     JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
-    GetBucketLifecycleConfigurationResultTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
-    AccountLevelOutputTypeDef,
     AccountLevelTypeDef,
     S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
     StorageLensConfigurationOutputTypeDef,
@@ -660,15 +582,15 @@
     PutStorageLensConfigurationRequestRequestTypeDef,
     JobDescriptorTypeDef,
     CreateJobRequestRequestTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.12/README.md` & `mypy-boto3-s3control-1.28.15/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-s3control
+Version: 1.28.15
+Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 s3control type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,164 +364,130 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
-    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
-    VpcConfigurationOutputTypeDef,
-    ActivityMetricsOutputTypeDef,
-    AdvancedCostOptimizationMetricsOutputTypeDef,
-    AdvancedDataProtectionMetricsOutputTypeDef,
-    DetailedStatusCodesMetricsOutputTypeDef,
+    VpcConfigurationTypeDef,
     ActivityMetricsTypeDef,
     AdvancedCostOptimizationMetricsTypeDef,
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
-    DeleteMultiRegionAccessPointInputOutputTypeDef,
-    PutMultiRegionAccessPointPolicyInputOutputTypeDef,
-    AwsLambdaTransformationOutputTypeDef,
+    DeleteMultiRegionAccessPointInputTypeDef,
+    PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
-    CloudWatchMetricsOutputTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
     ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    VpcConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
-    PublicAccessBlockConfigurationOutputTypeDef,
-    RegionOutputTypeDef,
     RegionTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
-    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteMultiRegionAccessPointInputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
     ExcludeOutputTypeDef,
     ExcludeTypeDef,
-    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
-    SSEKMSEncryptionOutputTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    S3TagOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    MultiRegionAccessPointRouteOutputTypeDef,
+    MultiRegionAccessPointRouteTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
-    StorageLensTagOutputTypeDef,
+    StorageLensTagTypeDef,
     IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
-    JobReportOutputTypeDef,
     JobManifestGeneratorFilterOutputTypeDef,
     JobManifestGeneratorFilterTypeDef,
-    JobManifestLocationOutputTypeDef,
     JobManifestLocationTypeDef,
     JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
-    LambdaInvokeOperationOutputTypeDef,
-    S3InitiateRestoreObjectOperationOutputTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
-    NoncurrentVersionExpirationOutputTypeDef,
-    NoncurrentVersionTransitionOutputTypeDef,
-    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
+    TransitionOutputTypeDef,
     TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
-    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
-    MultiRegionAccessPointRouteTypeDef,
-    SelectionCriteriaOutputTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
-    PutMultiRegionAccessPointPolicyInputTypeDef,
-    StorageLensTagTypeDef,
-    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
-    S3ObjectOwnerOutputTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataOutputTypeDef,
     S3ObjectMetadataTypeDef,
-    S3GranteeOutputTypeDef,
     S3GranteeTypeDef,
-    S3ObjectLockLegalHoldOutputTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionOutputTypeDef,
     S3RetentionTypeDef,
-    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
-    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StorageLensAwsOrgOutputTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
-    ObjectLambdaContentTransformationOutputTypeDef,
+    DeleteMultiRegionAccessPointRequestRequestTypeDef,
+    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
     ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
@@ -499,125 +497,113 @@
     GetAccessPointPolicyResultTypeDef,
     GetBucketPolicyResultTypeDef,
     GetBucketResultTypeDef,
     GetBucketVersioningResultTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
-    PutPublicAccessBlockRequestRequestTypeDef,
     CreateAccessPointRequestRequestTypeDef,
+    GetAccessPointForObjectLambdaResultTypeDef,
+    GetAccessPointResultTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    PutPublicAccessBlockRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
+    GetBucketTaggingResultTypeDef,
+    GetJobTaggingResultTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     PutJobTaggingRequestRequestTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
     ReplicationRuleAndOperatorTypeDef,
+    S3SetObjectTaggingOperationOutputTypeDef,
     S3SetObjectTaggingOperationTypeDef,
     TaggingTypeDef,
-    GetAccessPointForObjectLambdaResultTypeDef,
-    GetAccessPointResultTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
     CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
-    DeleteMultiRegionAccessPointRequestRequestTypeDef,
     GeneratedManifestEncryptionOutputTypeDef,
     GeneratedManifestEncryptionTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
-    GetBucketTaggingResultTypeDef,
-    GetJobTaggingResultTypeDef,
-    LifecycleRuleAndOperatorOutputTypeDef,
-    ReplicationRuleAndOperatorOutputTypeDef,
-    S3SetObjectTaggingOperationOutputTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
+    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
+    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
-    MetricsOutputTypeDef,
-    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
-    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    PrefixLevelStorageMetricsOutputTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
-    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
-    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
-    S3GrantOutputTypeDef,
     S3GrantTypeDef,
-    S3SetObjectLegalHoldOperationOutputTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationOutputTypeDef,
     S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
-    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
     LifecycleRuleFilterTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
-    LifecycleRuleFilterOutputTypeDef,
-    ReplicationRuleFilterOutputTypeDef,
     JobListDescriptorTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
-    PrefixLevelOutputTypeDef,
     PrefixLevelTypeDef,
     S3AccessControlListOutputTypeDef,
-    S3CopyObjectOperationOutputTypeDef,
     S3AccessControlListTypeDef,
+    S3CopyObjectOperationOutputTypeDef,
     S3CopyObjectOperationTypeDef,
     S3BucketDestinationOutputTypeDef,
     S3BucketDestinationTypeDef,
     ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
+    LifecycleRuleOutputTypeDef,
     LifecycleRuleTypeDef,
     S3JobManifestGeneratorOutputTypeDef,
     S3JobManifestGeneratorTypeDef,
-    LifecycleRuleOutputTypeDef,
     ListJobsResultTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     AsyncOperationTypeDef,
-    BucketLevelOutputTypeDef,
     BucketLevelTypeDef,
     S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
     StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
     CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
+    GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
     JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
-    GetBucketLifecycleConfigurationResultTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
-    AccountLevelOutputTypeDef,
     AccountLevelTypeDef,
     S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
     StorageLensConfigurationOutputTypeDef,
@@ -628,15 +614,15 @@
     PutStorageLensConfigurationRequestRequestTypeDef,
     JobDescriptorTypeDef,
     CreateJobRequestRequestTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.py` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.pyi` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__main__.py` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Control 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.S3Control 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
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

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.py` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.pyi` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.py` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.pyi` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.py` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.pyi` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.py` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for s3control service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadOutputTypeDef
+    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadTypeDef
 
-    data: AbortIncompleteMultipartUploadOutputTypeDef = {...}
+    data: AbortIncompleteMultipartUploadTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -65,164 +65,130 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
-    "VpcConfigurationOutputTypeDef",
-    "ActivityMetricsOutputTypeDef",
-    "AdvancedCostOptimizationMetricsOutputTypeDef",
-    "AdvancedDataProtectionMetricsOutputTypeDef",
-    "DetailedStatusCodesMetricsOutputTypeDef",
+    "VpcConfigurationTypeDef",
     "ActivityMetricsTypeDef",
     "AdvancedCostOptimizationMetricsTypeDef",
     "AdvancedDataProtectionMetricsTypeDef",
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
-    "DeleteMultiRegionAccessPointInputOutputTypeDef",
-    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
-    "AwsLambdaTransformationOutputTypeDef",
+    "DeleteMultiRegionAccessPointInputTypeDef",
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
     "AwsLambdaTransformationTypeDef",
-    "CloudWatchMetricsOutputTypeDef",
     "CloudWatchMetricsTypeDef",
     "ObjectLambdaAccessPointAliasTypeDef",
     "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
-    "VpcConfigurationTypeDef",
     "CreateBucketConfigurationTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
-    "PublicAccessBlockConfigurationOutputTypeDef",
-    "RegionOutputTypeDef",
     "RegionTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyRequestRequestTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteBucketLifecycleConfigurationRequestRequestTypeDef",
     "DeleteBucketPolicyRequestRequestTypeDef",
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteJobTaggingRequestRequestTypeDef",
-    "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteMultiRegionAccessPointInputTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     "ExcludeOutputTypeDef",
     "ExcludeTypeDef",
-    "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
-    "SSEKMSEncryptionOutputTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetAccessPointPolicyStatusRequestRequestTypeDef",
     "GetAccessPointRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
     "GetBucketRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "S3TagOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "GetJobTaggingRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef",
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    "MultiRegionAccessPointRouteOutputTypeDef",
+    "MultiRegionAccessPointRouteTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
-    "StorageLensTagOutputTypeDef",
+    "StorageLensTagTypeDef",
     "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
-    "JobReportOutputTypeDef",
     "JobManifestGeneratorFilterOutputTypeDef",
     "JobManifestGeneratorFilterTypeDef",
-    "JobManifestLocationOutputTypeDef",
     "JobManifestLocationTypeDef",
     "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
-    "LambdaInvokeOperationOutputTypeDef",
-    "S3InitiateRestoreObjectOperationOutputTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
     "LifecycleExpirationOutputTypeDef",
     "LifecycleExpirationTypeDef",
-    "NoncurrentVersionExpirationOutputTypeDef",
-    "NoncurrentVersionTransitionOutputTypeDef",
-    "TransitionOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
+    "TransitionOutputTypeDef",
     "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
-    "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "ProposedMultiRegionAccessPointPolicyTypeDef",
     "MultiRegionAccessPointRegionalResponseTypeDef",
     "RegionReportTypeDef",
-    "MultiRegionAccessPointRouteTypeDef",
-    "SelectionCriteriaOutputTypeDef",
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
-    "StorageLensTagTypeDef",
-    "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
-    "S3ObjectOwnerOutputTypeDef",
     "S3ObjectOwnerTypeDef",
     "S3ObjectMetadataOutputTypeDef",
     "S3ObjectMetadataTypeDef",
-    "S3GranteeOutputTypeDef",
     "S3GranteeTypeDef",
-    "S3ObjectLockLegalHoldOutputTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
     "S3RetentionOutputTypeDef",
     "S3RetentionTypeDef",
-    "SSEKMSOutputTypeDef",
     "SSEKMSTypeDef",
-    "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
-    "StorageLensAwsOrgOutputTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
-    "ObjectLambdaContentTransformationOutputTypeDef",
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
     "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointForObjectLambdaResultTypeDef",
     "CreateAccessPointResultTypeDef",
     "CreateBucketResultTypeDef",
     "CreateJobResultTypeDef",
     "CreateMultiRegionAccessPointResultTypeDef",
@@ -232,125 +198,113 @@
     "GetAccessPointPolicyResultTypeDef",
     "GetBucketPolicyResultTypeDef",
     "GetBucketResultTypeDef",
     "GetBucketVersioningResultTypeDef",
     "PutMultiRegionAccessPointPolicyResultTypeDef",
     "UpdateJobPriorityResultTypeDef",
     "UpdateJobStatusResultTypeDef",
-    "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    "GetAccessPointResultTypeDef",
+    "GetPublicAccessBlockOutputTypeDef",
+    "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
+    "GetBucketTaggingResultTypeDef",
+    "GetJobTaggingResultTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "PutJobTaggingRequestRequestTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
+    "S3SetObjectTaggingOperationOutputTypeDef",
     "S3SetObjectTaggingOperationTypeDef",
     "TaggingTypeDef",
-    "GetAccessPointForObjectLambdaResultTypeDef",
-    "GetAccessPointResultTypeDef",
-    "GetPublicAccessBlockOutputTypeDef",
     "CreateMultiRegionAccessPointInputOutputTypeDef",
     "CreateMultiRegionAccessPointInputTypeDef",
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     "GeneratedManifestEncryptionOutputTypeDef",
     "GeneratedManifestEncryptionTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
-    "GetBucketTaggingResultTypeDef",
-    "GetJobTaggingResultTypeDef",
-    "LifecycleRuleAndOperatorOutputTypeDef",
-    "ReplicationRuleAndOperatorOutputTypeDef",
-    "S3SetObjectTaggingOperationOutputTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
-    "MetricsOutputTypeDef",
-    "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    "PrefixLevelStorageMetricsOutputTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
-    "S3GrantOutputTypeDef",
     "S3GrantTypeDef",
-    "S3SetObjectLegalHoldOperationOutputTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
     "S3SetObjectRetentionOperationOutputTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
     "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
-    "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
     "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
-    "LifecycleRuleFilterOutputTypeDef",
-    "ReplicationRuleFilterOutputTypeDef",
     "JobListDescriptorTypeDef",
-    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
-    "PrefixLevelOutputTypeDef",
     "PrefixLevelTypeDef",
     "S3AccessControlListOutputTypeDef",
-    "S3CopyObjectOperationOutputTypeDef",
     "S3AccessControlListTypeDef",
+    "S3CopyObjectOperationOutputTypeDef",
     "S3CopyObjectOperationTypeDef",
     "S3BucketDestinationOutputTypeDef",
     "S3BucketDestinationTypeDef",
     "ObjectLambdaConfigurationOutputTypeDef",
     "ObjectLambdaConfigurationTypeDef",
+    "LifecycleRuleOutputTypeDef",
     "LifecycleRuleTypeDef",
     "S3JobManifestGeneratorOutputTypeDef",
     "S3JobManifestGeneratorTypeDef",
-    "LifecycleRuleOutputTypeDef",
     "ListJobsResultTypeDef",
     "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "AsyncOperationTypeDef",
-    "BucketLevelOutputTypeDef",
     "BucketLevelTypeDef",
     "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
     "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
+    "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
     "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
-    "GetBucketLifecycleConfigurationResultTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
-    "AccountLevelOutputTypeDef",
     "AccountLevelTypeDef",
     "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
     "StorageLensConfigurationOutputTypeDef",
@@ -360,83 +314,36 @@
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
     "JobDescriptorTypeDef",
     "CreateJobRequestRequestTypeDef",
     "DescribeJobResultTypeDef",
 )
 
-AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
-    "AbortIncompleteMultipartUploadOutputTypeDef",
-    {
-        "DaysAfterInitiation": int,
-    },
-    total=False,
-)
-
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
-AccessControlTranslationOutputTypeDef = TypedDict(
-    "AccessControlTranslationOutputTypeDef",
-    {
-        "Owner": Literal["Destination"],
-    },
-)
-
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
+VpcConfigurationTypeDef = TypedDict(
+    "VpcConfigurationTypeDef",
     {
         "VpcId": str,
     },
 )
 
-ActivityMetricsOutputTypeDef = TypedDict(
-    "ActivityMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
-AdvancedCostOptimizationMetricsOutputTypeDef = TypedDict(
-    "AdvancedCostOptimizationMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
-AdvancedDataProtectionMetricsOutputTypeDef = TypedDict(
-    "AdvancedDataProtectionMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
-DetailedStatusCodesMetricsOutputTypeDef = TypedDict(
-    "DetailedStatusCodesMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
 ActivityMetricsTypeDef = TypedDict(
     "ActivityMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
     total=False,
 )
@@ -472,50 +379,29 @@
         "Message": str,
         "Resource": str,
         "RequestId": str,
     },
     total=False,
 )
 
-DeleteMultiRegionAccessPointInputOutputTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointInputOutputTypeDef",
+DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointInputTypeDef",
     {
         "Name": str,
     },
 )
 
-PutMultiRegionAccessPointPolicyInputOutputTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
+PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
     {
         "Name": str,
         "Policy": str,
     },
 )
 
-_RequiredAwsLambdaTransformationOutputTypeDef = TypedDict(
-    "_RequiredAwsLambdaTransformationOutputTypeDef",
-    {
-        "FunctionArn": str,
-    },
-)
-_OptionalAwsLambdaTransformationOutputTypeDef = TypedDict(
-    "_OptionalAwsLambdaTransformationOutputTypeDef",
-    {
-        "FunctionPayload": str,
-    },
-    total=False,
-)
-
-
-class AwsLambdaTransformationOutputTypeDef(
-    _RequiredAwsLambdaTransformationOutputTypeDef, _OptionalAwsLambdaTransformationOutputTypeDef
-):
-    pass
-
-
 _RequiredAwsLambdaTransformationTypeDef = TypedDict(
     "_RequiredAwsLambdaTransformationTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalAwsLambdaTransformationTypeDef = TypedDict(
@@ -529,21 +415,14 @@
 
 class AwsLambdaTransformationTypeDef(
     _RequiredAwsLambdaTransformationTypeDef, _OptionalAwsLambdaTransformationTypeDef
 ):
     pass
 
 
-CloudWatchMetricsOutputTypeDef = TypedDict(
-    "CloudWatchMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-)
-
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
@@ -574,21 +453,14 @@
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
-VpcConfigurationTypeDef = TypedDict(
-    "VpcConfigurationTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
@@ -619,44 +491,14 @@
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
-    "PublicAccessBlockConfigurationOutputTypeDef",
-    {
-        "BlockPublicAcls": bool,
-        "IgnorePublicAcls": bool,
-        "BlockPublicPolicy": bool,
-        "RestrictPublicBuckets": bool,
-    },
-    total=False,
-)
-
-_RequiredRegionOutputTypeDef = TypedDict(
-    "_RequiredRegionOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalRegionOutputTypeDef = TypedDict(
-    "_OptionalRegionOutputTypeDef",
-    {
-        "BucketAccountId": str,
-    },
-    total=False,
-)
-
-
-class RegionOutputTypeDef(_RequiredRegionOutputTypeDef, _OptionalRegionOutputTypeDef):
-    pass
-
-
 _RequiredRegionTypeDef = TypedDict(
     "_RequiredRegionTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalRegionTypeDef = TypedDict(
@@ -748,35 +590,21 @@
     "DeleteJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
 
-DeleteMarkerReplicationOutputTypeDef = TypedDict(
-    "DeleteMarkerReplicationOutputTypeDef",
-    {
-        "Status": DeleteMarkerReplicationStatusType,
-    },
-)
-
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
 )
 
-DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointInputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 DeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "DeletePublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -808,22 +636,14 @@
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     {
         "AccountId": str,
         "RequestTokenARN": str,
     },
 )
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "ReplicaKmsKeyID": str,
-    },
-    total=False,
-)
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
     total=False,
 )
@@ -850,35 +670,21 @@
     {
         "Buckets": Sequence[str],
         "Regions": Sequence[str],
     },
     total=False,
 )
 
-ExistingObjectReplicationOutputTypeDef = TypedDict(
-    "ExistingObjectReplicationOutputTypeDef",
-    {
-        "Status": ExistingObjectReplicationStatusType,
-    },
-)
-
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
         "Status": ExistingObjectReplicationStatusType,
     },
 )
 
-SSEKMSEncryptionOutputTypeDef = TypedDict(
-    "SSEKMSEncryptionOutputTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-
 SSEKMSEncryptionTypeDef = TypedDict(
     "SSEKMSEncryptionTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -982,22 +788,14 @@
     "GetBucketTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-S3TagOutputTypeDef = TypedDict(
-    "S3TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 GetBucketVersioningRequestRequestTypeDef = TypedDict(
     "GetBucketVersioningRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -1038,33 +836,32 @@
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
         "AccountId": str,
         "Mrap": str,
     },
 )
 
-_RequiredMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
-    "_RequiredMultiRegionAccessPointRouteOutputTypeDef",
+_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_RequiredMultiRegionAccessPointRouteTypeDef",
     {
         "TrafficDialPercentage": int,
     },
 )
-_OptionalMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
-    "_OptionalMultiRegionAccessPointRouteOutputTypeDef",
+_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_OptionalMultiRegionAccessPointRouteTypeDef",
     {
         "Bucket": str,
         "Region": str,
     },
     total=False,
 )
 
 
-class MultiRegionAccessPointRouteOutputTypeDef(
-    _RequiredMultiRegionAccessPointRouteOutputTypeDef,
-    _OptionalMultiRegionAccessPointRouteOutputTypeDef,
+class MultiRegionAccessPointRouteTypeDef(
+    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
 ):
     pass
 
 
 GetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "GetPublicAccessBlockRequestRequestTypeDef",
     {
@@ -1084,16 +881,16 @@
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
         "ConfigId": str,
         "AccountId": str,
     },
 )
 
-StorageLensTagOutputTypeDef = TypedDict(
-    "StorageLensTagOutputTypeDef",
+StorageLensTagTypeDef = TypedDict(
+    "StorageLensTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 IncludeOutputTypeDef = TypedDict(
@@ -1119,36 +916,14 @@
     {
         "FailureCode": str,
         "FailureReason": str,
     },
     total=False,
 )
 
-_RequiredJobReportOutputTypeDef = TypedDict(
-    "_RequiredJobReportOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalJobReportOutputTypeDef = TypedDict(
-    "_OptionalJobReportOutputTypeDef",
-    {
-        "Bucket": str,
-        "Format": Literal["Report_CSV_20180820"],
-        "Prefix": str,
-        "ReportScope": JobReportScopeType,
-    },
-    total=False,
-)
-
-
-class JobReportOutputTypeDef(_RequiredJobReportOutputTypeDef, _OptionalJobReportOutputTypeDef):
-    pass
-
-
 JobManifestGeneratorFilterOutputTypeDef = TypedDict(
     "JobManifestGeneratorFilterOutputTypeDef",
     {
         "EligibleForReplication": bool,
         "CreatedAfter": datetime,
         "CreatedBefore": datetime,
         "ObjectReplicationStatuses": List[ReplicationStatusType],
@@ -1163,36 +938,14 @@
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
     },
     total=False,
 )
 
-_RequiredJobManifestLocationOutputTypeDef = TypedDict(
-    "_RequiredJobManifestLocationOutputTypeDef",
-    {
-        "ObjectArn": str,
-        "ETag": str,
-    },
-)
-_OptionalJobManifestLocationOutputTypeDef = TypedDict(
-    "_OptionalJobManifestLocationOutputTypeDef",
-    {
-        "ObjectVersionId": str,
-    },
-    total=False,
-)
-
-
-class JobManifestLocationOutputTypeDef(
-    _RequiredJobManifestLocationOutputTypeDef, _OptionalJobManifestLocationOutputTypeDef
-):
-    pass
-
-
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
 )
@@ -1247,31 +1000,14 @@
 )
 
 
 class JobManifestSpecTypeDef(_RequiredJobManifestSpecTypeDef, _OptionalJobManifestSpecTypeDef):
     pass
 
 
-LambdaInvokeOperationOutputTypeDef = TypedDict(
-    "LambdaInvokeOperationOutputTypeDef",
-    {
-        "FunctionArn": str,
-    },
-    total=False,
-)
-
-S3InitiateRestoreObjectOperationOutputTypeDef = TypedDict(
-    "S3InitiateRestoreObjectOperationOutputTypeDef",
-    {
-        "ExpirationInDays": int,
-        "GlacierJobTier": S3GlacierJobTierType,
-    },
-    total=False,
-)
-
 LambdaInvokeOperationTypeDef = TypedDict(
     "LambdaInvokeOperationTypeDef",
     {
         "FunctionArn": str,
     },
     total=False,
 )
@@ -1309,25 +1045,25 @@
         "Date": Union[datetime, str],
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
-NoncurrentVersionExpirationOutputTypeDef = TypedDict(
-    "NoncurrentVersionExpirationOutputTypeDef",
+NoncurrentVersionExpirationTypeDef = TypedDict(
+    "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
     total=False,
 )
 
-NoncurrentVersionTransitionOutputTypeDef = TypedDict(
-    "NoncurrentVersionTransitionOutputTypeDef",
+NoncurrentVersionTransitionTypeDef = TypedDict(
+    "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
@@ -1337,32 +1073,14 @@
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-NoncurrentVersionExpirationTypeDef = TypedDict(
-    "NoncurrentVersionExpirationTypeDef",
-    {
-        "NoncurrentDays": int,
-        "NewerNoncurrentVersions": int,
-    },
-    total=False,
-)
-
-NoncurrentVersionTransitionTypeDef = TypedDict(
-    "NoncurrentVersionTransitionTypeDef",
-    {
-        "NoncurrentDays": int,
-        "StorageClass": TransitionStorageClassType,
-    },
-    total=False,
-)
-
 TransitionTypeDef = TypedDict(
     "TransitionTypeDef",
     {
         "Date": Union[datetime, str],
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
@@ -1559,22 +1277,14 @@
 class ListStorageLensConfigurationsRequestRequestTypeDef(
     _RequiredListStorageLensConfigurationsRequestRequestTypeDef,
     _OptionalListStorageLensConfigurationsRequestRequestTypeDef,
 ):
     pass
 
 
-ReplicationTimeValueOutputTypeDef = TypedDict(
-    "ReplicationTimeValueOutputTypeDef",
-    {
-        "Minutes": int,
-    },
-    total=False,
-)
-
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
@@ -1602,46 +1312,14 @@
         "Bucket": str,
         "Region": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
-_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_RequiredMultiRegionAccessPointRouteTypeDef",
-    {
-        "TrafficDialPercentage": int,
-    },
-)
-_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_OptionalMultiRegionAccessPointRouteTypeDef",
-    {
-        "Bucket": str,
-        "Region": str,
-    },
-    total=False,
-)
-
-
-class MultiRegionAccessPointRouteTypeDef(
-    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
-):
-    pass
-
-
-SelectionCriteriaOutputTypeDef = TypedDict(
-    "SelectionCriteriaOutputTypeDef",
-    {
-        "Delimiter": str,
-        "MaxDepth": int,
-        "MinStorageBytesPercentage": float,
-    },
-    total=False,
-)
-
 SelectionCriteriaTypeDef = TypedDict(
     "SelectionCriteriaTypeDef",
     {
         "Delimiter": str,
         "MaxDepth": int,
         "MinStorageBytesPercentage": float,
     },
@@ -1694,53 +1372,21 @@
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
 )
 
-PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
-    {
-        "Name": str,
-        "Policy": str,
-    },
-)
-
-StorageLensTagTypeDef = TypedDict(
-    "StorageLensTagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-ReplicaModificationsOutputTypeDef = TypedDict(
-    "ReplicaModificationsOutputTypeDef",
-    {
-        "Status": ReplicaModificationsStatusType,
-    },
-)
-
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
 )
 
-S3ObjectOwnerOutputTypeDef = TypedDict(
-    "S3ObjectOwnerOutputTypeDef",
-    {
-        "ID": str,
-        "DisplayName": str,
-    },
-    total=False,
-)
-
 S3ObjectOwnerTypeDef = TypedDict(
     "S3ObjectOwnerTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
@@ -1778,41 +1424,24 @@
         "HttpExpiresDate": Union[datetime, str],
         "RequesterCharged": bool,
         "SSEAlgorithm": S3SSEAlgorithmType,
     },
     total=False,
 )
 
-S3GranteeOutputTypeDef = TypedDict(
-    "S3GranteeOutputTypeDef",
-    {
-        "TypeIdentifier": S3GranteeTypeIdentifierType,
-        "Identifier": str,
-        "DisplayName": str,
-    },
-    total=False,
-)
-
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-S3ObjectLockLegalHoldOutputTypeDef = TypedDict(
-    "S3ObjectLockLegalHoldOutputTypeDef",
-    {
-        "Status": S3ObjectLockLegalHoldStatusType,
-    },
-)
-
 S3ObjectLockLegalHoldTypeDef = TypedDict(
     "S3ObjectLockLegalHoldTypeDef",
     {
         "Status": S3ObjectLockLegalHoldStatusType,
     },
 )
 
@@ -1830,49 +1459,28 @@
     {
         "RetainUntilDate": Union[datetime, str],
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
-SSEKMSOutputTypeDef = TypedDict(
-    "SSEKMSOutputTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
-SseKmsEncryptedObjectsOutputTypeDef = TypedDict(
-    "SseKmsEncryptedObjectsOutputTypeDef",
-    {
-        "Status": SseKmsEncryptedObjectsStatusType,
-    },
-)
-
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
-StorageLensAwsOrgOutputTypeDef = TypedDict(
-    "StorageLensAwsOrgOutputTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
 StorageLensAwsOrgTypeDef = TypedDict(
     "StorageLensAwsOrgTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -1915,33 +1523,43 @@
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
 )
 _OptionalAccessPointTypeDef = TypedDict(
     "_OptionalAccessPointTypeDef",
     {
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "VpcConfiguration": VpcConfigurationTypeDef,
         "AccessPointArn": str,
         "Alias": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
 
 class AccessPointTypeDef(_RequiredAccessPointTypeDef, _OptionalAccessPointTypeDef):
     pass
 
 
-ObjectLambdaContentTransformationOutputTypeDef = TypedDict(
-    "ObjectLambdaContentTransformationOutputTypeDef",
+DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     {
-        "AwsLambda": AwsLambdaTransformationOutputTypeDef,
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": DeleteMultiRegionAccessPointInputTypeDef,
+    },
+)
+
+PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
-    total=False,
 )
 
 ObjectLambdaContentTransformationTypeDef = TypedDict(
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
@@ -2094,22 +1712,14 @@
         "JobId": str,
         "Status": JobStatusType,
         "StatusUpdateReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
-    "PutPublicAccessBlockRequestRequestTypeDef",
-    {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "AccountId": str,
-    },
-)
-
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Bucket": str,
     },
@@ -2127,14 +1737,58 @@
 
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
 
+GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    {
+        "Name": str,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "CreationDate": datetime,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessPointResultTypeDef = TypedDict(
+    "GetAccessPointResultTypeDef",
+    {
+        "Name": str,
+        "Bucket": str,
+        "NetworkOrigin": NetworkOriginType,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "CreationDate": datetime,
+        "Alias": str,
+        "AccessPointArn": str,
+        "Endpoints": Dict[str, str],
+        "BucketAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicAccessBlockOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputTypeDef",
+    {
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
+    "PutPublicAccessBlockRequestRequestTypeDef",
+    {
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "AccountId": str,
+    },
+)
+
 _RequiredCreateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBucketRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalCreateBucketRequestRequestTypeDef = TypedDict(
@@ -2156,14 +1810,41 @@
 
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
 
+GetBucketTaggingResultTypeDef = TypedDict(
+    "GetBucketTaggingResultTypeDef",
+    {
+        "TagSet": List[S3TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobTaggingResultTypeDef = TypedDict(
+    "GetJobTaggingResultTypeDef",
+    {
+        "Tags": List[S3TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[S3TagTypeDef],
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+    },
+    total=False,
+)
+
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": Sequence[S3TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
@@ -2176,23 +1857,40 @@
     {
         "AccountId": str,
         "JobId": str,
         "Tags": Sequence[S3TagTypeDef],
     },
 )
 
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[S3TagTypeDef],
+    },
+    total=False,
+)
+
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": Sequence[S3TagTypeDef],
     },
     total=False,
 )
 
+S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
+    "S3SetObjectTaggingOperationOutputTypeDef",
+    {
+        "TagSet": List[S3TagTypeDef],
+    },
+    total=False,
+)
+
 S3SetObjectTaggingOperationTypeDef = TypedDict(
     "S3SetObjectTaggingOperationTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
     total=False,
 )
@@ -2200,61 +1898,25 @@
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
 )
 
-GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointForObjectLambdaResultTypeDef",
-    {
-        "Name": str,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "CreationDate": datetime,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccessPointResultTypeDef = TypedDict(
-    "GetAccessPointResultTypeDef",
-    {
-        "Name": str,
-        "Bucket": str,
-        "NetworkOrigin": NetworkOriginType,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "CreationDate": datetime,
-        "Alias": str,
-        "AccessPointArn": str,
-        "Endpoints": Dict[str, str],
-        "BucketAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPublicAccessBlockOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputTypeDef",
-    {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
     "_RequiredCreateMultiRegionAccessPointInputOutputTypeDef",
     {
         "Name": str,
-        "Regions": List[RegionOutputTypeDef],
+        "Regions": List[RegionTypeDef],
     },
 )
 _OptionalCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
     "_OptionalCreateMultiRegionAccessPointInputOutputTypeDef",
     {
-        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
+        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class CreateMultiRegionAccessPointInputOutputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputOutputTypeDef,
@@ -2282,28 +1944,19 @@
 class CreateMultiRegionAccessPointInputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputTypeDef,
     _OptionalCreateMultiRegionAccessPointInputTypeDef,
 ):
     pass
 
 
-DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": DeleteMultiRegionAccessPointInputTypeDef,
-    },
-)
-
 GeneratedManifestEncryptionOutputTypeDef = TypedDict(
     "GeneratedManifestEncryptionOutputTypeDef",
     {
         "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSEncryptionOutputTypeDef,
+        "SSEKMS": SSEKMSEncryptionTypeDef,
     },
     total=False,
 )
 
 GeneratedManifestEncryptionTypeDef = TypedDict(
     "GeneratedManifestEncryptionTypeDef",
     {
@@ -2333,89 +1986,63 @@
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     {
         "Established": PolicyStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBucketTaggingResultTypeDef = TypedDict(
-    "GetBucketTaggingResultTypeDef",
-    {
-        "TagSet": List[S3TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobTaggingResultTypeDef = TypedDict(
-    "GetJobTaggingResultTypeDef",
+GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
+    "GetMultiRegionAccessPointRoutesResultTypeDef",
     {
-        "Tags": List[S3TagOutputTypeDef],
+        "Mrap": str,
+        "Routes": List[MultiRegionAccessPointRouteTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[S3TagOutputTypeDef],
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
-ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
-    "ReplicationRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[S3TagOutputTypeDef],
-    },
-    total=False,
-)
-
-S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
-    "S3SetObjectTaggingOperationOutputTypeDef",
+SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
-        "TagSet": List[S3TagOutputTypeDef],
+        "AccountId": str,
+        "Mrap": str,
+        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
     },
-    total=False,
 )
 
-GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
-    "GetMultiRegionAccessPointRoutesResultTypeDef",
+GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
+    "GetStorageLensConfigurationTaggingResultTypeDef",
     {
-        "Mrap": str,
-        "Routes": List[MultiRegionAccessPointRouteOutputTypeDef],
+        "Tags": List[StorageLensTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
-    "GetStorageLensConfigurationTaggingResultTypeDef",
+PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
-        "Tags": List[StorageLensTagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ConfigId": str,
+        "AccountId": str,
+        "Tags": Sequence[StorageLensTagTypeDef],
     },
 )
 
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
-        "Location": JobManifestLocationOutputTypeDef,
+        "Location": JobManifestLocationTypeDef,
     },
     total=False,
 )
 
 JobManifestOutputTypeDef = TypedDict(
     "JobManifestOutputTypeDef",
     {
         "Spec": JobManifestSpecOutputTypeDef,
-        "Location": JobManifestLocationOutputTypeDef,
+        "Location": JobManifestLocationTypeDef,
     },
 )
 
 JobManifestTypeDef = TypedDict(
     "JobManifestTypeDef",
     {
         "Spec": JobManifestSpecTypeDef,
@@ -2470,41 +2097,14 @@
     {
         "NextToken": str,
         "StorageLensConfigurationList": List[ListStorageLensConfigurationEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricsOutputTypeDef = TypedDict(
-    "_RequiredMetricsOutputTypeDef",
-    {
-        "Status": MetricsStatusType,
-    },
-)
-_OptionalMetricsOutputTypeDef = TypedDict(
-    "_OptionalMetricsOutputTypeDef",
-    {
-        "EventThreshold": ReplicationTimeValueOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class MetricsOutputTypeDef(_RequiredMetricsOutputTypeDef, _OptionalMetricsOutputTypeDef):
-    pass
-
-
-ReplicationTimeOutputTypeDef = TypedDict(
-    "ReplicationTimeOutputTypeDef",
-    {
-        "Status": ReplicationTimeStatusType,
-        "Time": ReplicationTimeValueOutputTypeDef,
-    },
-)
-
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
     },
 )
 _OptionalMetricsTypeDef = TypedDict(
@@ -2547,39 +2147,21 @@
 
 MultiRegionAccessPointReportTypeDef = TypedDict(
     "MultiRegionAccessPointReportTypeDef",
     {
         "Name": str,
         "Alias": str,
         "CreatedAt": datetime,
-        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
+        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
         "Status": MultiRegionAccessPointStatusType,
         "Regions": List[RegionReportTypeDef],
     },
     total=False,
 )
 
-SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "Mrap": str,
-        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
-    },
-)
-
-PrefixLevelStorageMetricsOutputTypeDef = TypedDict(
-    "PrefixLevelStorageMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-        "SelectionCriteria": SelectionCriteriaOutputTypeDef,
-    },
-    total=False,
-)
-
 PrefixLevelStorageMetricsTypeDef = TypedDict(
     "PrefixLevelStorageMetricsTypeDef",
     {
         "IsEnabled": bool,
         "SelectionCriteria": SelectionCriteriaTypeDef,
     },
     total=False,
@@ -2605,57 +2187,23 @@
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
 
-PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
-    },
-)
-
-PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
-    {
-        "ConfigId": str,
-        "AccountId": str,
-        "Tags": Sequence[StorageLensTagTypeDef],
-    },
-)
-
-S3GrantOutputTypeDef = TypedDict(
-    "S3GrantOutputTypeDef",
-    {
-        "Grantee": S3GranteeOutputTypeDef,
-        "Permission": S3PermissionType,
-    },
-    total=False,
-)
-
 S3GrantTypeDef = TypedDict(
     "S3GrantTypeDef",
     {
         "Grantee": S3GranteeTypeDef,
         "Permission": S3PermissionType,
     },
     total=False,
 )
 
-S3SetObjectLegalHoldOperationOutputTypeDef = TypedDict(
-    "S3SetObjectLegalHoldOperationOutputTypeDef",
-    {
-        "LegalHold": S3ObjectLockLegalHoldOutputTypeDef,
-    },
-)
-
 S3SetObjectLegalHoldOperationTypeDef = TypedDict(
     "S3SetObjectLegalHoldOperationTypeDef",
     {
         "LegalHold": S3ObjectLockLegalHoldTypeDef,
     },
 )
 
@@ -2702,37 +2250,28 @@
     pass
 
 
 StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
     "StorageLensDataExportEncryptionOutputTypeDef",
     {
         "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSOutputTypeDef,
+        "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
 StorageLensDataExportEncryptionTypeDef = TypedDict(
     "StorageLensDataExportEncryptionTypeDef",
     {
         "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
-SourceSelectionCriteriaOutputTypeDef = TypedDict(
-    "SourceSelectionCriteriaOutputTypeDef",
-    {
-        "SseKmsEncryptedObjects": SseKmsEncryptedObjectsOutputTypeDef,
-        "ReplicaModifications": ReplicaModificationsOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
     total=False,
@@ -2747,15 +2286,15 @@
     },
 )
 
 ObjectLambdaTransformationConfigurationOutputTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationOutputTypeDef",
     {
         "Actions": List[ObjectLambdaTransformationConfigurationActionType],
-        "ContentTransformation": ObjectLambdaContentTransformationOutputTypeDef,
+        "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
     },
 )
 
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
@@ -2768,26 +2307,48 @@
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagTypeDef,
+        "And": LifecycleRuleAndOperatorOutputTypeDef,
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+    },
+    total=False,
+)
+
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": LifecycleRuleAndOperatorTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagTypeDef,
+        "And": ReplicationRuleAndOperatorOutputTypeDef,
+    },
+    total=False,
+)
+
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
@@ -2803,16 +2364,16 @@
     },
 )
 
 AsyncRequestParametersTypeDef = TypedDict(
     "AsyncRequestParametersTypeDef",
     {
         "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
-        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputOutputTypeDef,
-        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputOutputTypeDef,
+        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
+        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
     total=False,
 )
 
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
@@ -2866,36 +2427,14 @@
 
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
 
-LifecycleRuleFilterOutputTypeDef = TypedDict(
-    "LifecycleRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagOutputTypeDef,
-        "And": LifecycleRuleAndOperatorOutputTypeDef,
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
-ReplicationRuleFilterOutputTypeDef = TypedDict(
-    "ReplicationRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagOutputTypeDef,
-        "And": ReplicationRuleAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2903,40 +2442,14 @@
         "CreationTime": datetime,
         "TerminationDate": datetime,
         "ProgressSummary": JobProgressSummaryTypeDef,
     },
     total=False,
 )
 
-_RequiredDestinationOutputTypeDef = TypedDict(
-    "_RequiredDestinationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalDestinationOutputTypeDef = TypedDict(
-    "_OptionalDestinationOutputTypeDef",
-    {
-        "Account": str,
-        "ReplicationTime": ReplicationTimeOutputTypeDef,
-        "AccessControlTranslation": AccessControlTranslationOutputTypeDef,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "Metrics": MetricsOutputTypeDef,
-        "StorageClass": ReplicationStorageClassType,
-    },
-    total=False,
-)
-
-
-class DestinationOutputTypeDef(
-    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
-):
-    pass
-
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDestinationTypeDef = TypedDict(
@@ -2987,59 +2500,73 @@
     {
         "AccessPoints": List[MultiRegionAccessPointReportTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PrefixLevelOutputTypeDef = TypedDict(
-    "PrefixLevelOutputTypeDef",
-    {
-        "StorageMetrics": PrefixLevelStorageMetricsOutputTypeDef,
-    },
-)
-
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
     },
 )
 
 _RequiredS3AccessControlListOutputTypeDef = TypedDict(
     "_RequiredS3AccessControlListOutputTypeDef",
     {
-        "Owner": S3ObjectOwnerOutputTypeDef,
+        "Owner": S3ObjectOwnerTypeDef,
     },
 )
 _OptionalS3AccessControlListOutputTypeDef = TypedDict(
     "_OptionalS3AccessControlListOutputTypeDef",
     {
-        "Grants": List[S3GrantOutputTypeDef],
+        "Grants": List[S3GrantTypeDef],
     },
     total=False,
 )
 
 
 class S3AccessControlListOutputTypeDef(
     _RequiredS3AccessControlListOutputTypeDef, _OptionalS3AccessControlListOutputTypeDef
 ):
     pass
 
 
+_RequiredS3AccessControlListTypeDef = TypedDict(
+    "_RequiredS3AccessControlListTypeDef",
+    {
+        "Owner": S3ObjectOwnerTypeDef,
+    },
+)
+_OptionalS3AccessControlListTypeDef = TypedDict(
+    "_OptionalS3AccessControlListTypeDef",
+    {
+        "Grants": Sequence[S3GrantTypeDef],
+    },
+    total=False,
+)
+
+
+class S3AccessControlListTypeDef(
+    _RequiredS3AccessControlListTypeDef, _OptionalS3AccessControlListTypeDef
+):
+    pass
+
+
 S3CopyObjectOperationOutputTypeDef = TypedDict(
     "S3CopyObjectOperationOutputTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
-        "AccessControlGrants": List[S3GrantOutputTypeDef],
+        "AccessControlGrants": List[S3GrantTypeDef],
         "MetadataDirective": S3MetadataDirectiveType,
         "ModifiedSinceConstraint": datetime,
         "NewObjectMetadata": S3ObjectMetadataOutputTypeDef,
-        "NewObjectTagging": List[S3TagOutputTypeDef],
+        "NewObjectTagging": List[S3TagTypeDef],
         "RedirectLocation": str,
         "RequesterPays": bool,
         "StorageClass": S3StorageClassType,
         "UnModifiedSinceConstraint": datetime,
         "SSEAwsKmsKeyId": str,
         "TargetKeyPrefix": str,
         "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
@@ -3047,35 +2574,14 @@
         "ObjectLockRetainUntilDate": datetime,
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
-_RequiredS3AccessControlListTypeDef = TypedDict(
-    "_RequiredS3AccessControlListTypeDef",
-    {
-        "Owner": S3ObjectOwnerTypeDef,
-    },
-)
-_OptionalS3AccessControlListTypeDef = TypedDict(
-    "_OptionalS3AccessControlListTypeDef",
-    {
-        "Grants": Sequence[S3GrantTypeDef],
-    },
-    total=False,
-)
-
-
-class S3AccessControlListTypeDef(
-    _RequiredS3AccessControlListTypeDef, _OptionalS3AccessControlListTypeDef
-):
-    pass
-
-
 S3CopyObjectOperationTypeDef = TypedDict(
     "S3CopyObjectOperationTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
         "AccessControlGrants": Sequence[S3GrantTypeDef],
         "MetadataDirective": S3MetadataDirectiveType,
@@ -3189,14 +2695,41 @@
 
 class ObjectLambdaConfigurationTypeDef(
     _RequiredObjectLambdaConfigurationTypeDef, _OptionalObjectLambdaConfigurationTypeDef
 ):
     pass
 
 
+_RequiredLifecycleRuleOutputTypeDef = TypedDict(
+    "_RequiredLifecycleRuleOutputTypeDef",
+    {
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalLifecycleRuleOutputTypeDef = TypedDict(
+    "_OptionalLifecycleRuleOutputTypeDef",
+    {
+        "Expiration": LifecycleExpirationOutputTypeDef,
+        "ID": str,
+        "Filter": LifecycleRuleFilterOutputTypeDef,
+        "Transitions": List[TransitionOutputTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
+    },
+    total=False,
+)
+
+
+class LifecycleRuleOutputTypeDef(
+    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredLifecycleRuleTypeDef = TypedDict(
     "_RequiredLifecycleRuleTypeDef",
     {
         "Status": ExpirationStatusType,
     },
 )
 _OptionalLifecycleRuleTypeDef = TypedDict(
@@ -3262,68 +2795,41 @@
 
 class S3JobManifestGeneratorTypeDef(
     _RequiredS3JobManifestGeneratorTypeDef, _OptionalS3JobManifestGeneratorTypeDef
 ):
     pass
 
 
-_RequiredLifecycleRuleOutputTypeDef = TypedDict(
-    "_RequiredLifecycleRuleOutputTypeDef",
-    {
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalLifecycleRuleOutputTypeDef = TypedDict(
-    "_OptionalLifecycleRuleOutputTypeDef",
-    {
-        "Expiration": LifecycleExpirationOutputTypeDef,
-        "ID": str,
-        "Filter": LifecycleRuleFilterOutputTypeDef,
-        "Transitions": List[TransitionOutputTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionOutputTypeDef],
-        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
-        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class LifecycleRuleOutputTypeDef(
-    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
-):
-    pass
-
-
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredReplicationRuleOutputTypeDef = TypedDict(
     "_RequiredReplicationRuleOutputTypeDef",
     {
         "Status": ReplicationRuleStatusType,
-        "Destination": DestinationOutputTypeDef,
+        "Destination": DestinationTypeDef,
         "Bucket": str,
     },
 )
 _OptionalReplicationRuleOutputTypeDef = TypedDict(
     "_OptionalReplicationRuleOutputTypeDef",
     {
         "ID": str,
         "Priority": int,
         "Prefix": str,
         "Filter": ReplicationRuleFilterOutputTypeDef,
-        "SourceSelectionCriteria": SourceSelectionCriteriaOutputTypeDef,
-        "ExistingObjectReplication": ExistingObjectReplicationOutputTypeDef,
-        "DeleteMarkerReplication": DeleteMarkerReplicationOutputTypeDef,
+        "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
+        "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
+        "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
     total=False,
 )
 
 
 class ReplicationRuleOutputTypeDef(
     _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
@@ -3367,26 +2873,14 @@
         "RequestParameters": AsyncRequestParametersTypeDef,
         "RequestStatus": str,
         "ResponseDetails": AsyncResponseDetailsTypeDef,
     },
     total=False,
 )
 
-BucketLevelOutputTypeDef = TypedDict(
-    "BucketLevelOutputTypeDef",
-    {
-        "ActivityMetrics": ActivityMetricsOutputTypeDef,
-        "PrefixLevel": PrefixLevelOutputTypeDef,
-        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
-        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
-        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
-    },
-    total=False,
-)
-
 BucketLevelTypeDef = TypedDict(
     "BucketLevelTypeDef",
     {
         "ActivityMetrics": ActivityMetricsTypeDef,
         "PrefixLevel": PrefixLevelTypeDef,
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
@@ -3413,15 +2907,15 @@
     total=False,
 )
 
 StorageLensDataExportOutputTypeDef = TypedDict(
     "StorageLensDataExportOutputTypeDef",
     {
         "S3BucketDestination": S3BucketDestinationOutputTypeDef,
-        "CloudWatchMetrics": CloudWatchMetricsOutputTypeDef,
+        "CloudWatchMetrics": CloudWatchMetricsTypeDef,
     },
     total=False,
 )
 
 StorageLensDataExportTypeDef = TypedDict(
     "StorageLensDataExportTypeDef",
     {
@@ -3453,14 +2947,22 @@
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
+GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationResultTypeDef",
+    {
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
     total=False,
 )
@@ -3477,22 +2979,14 @@
     "JobManifestGeneratorTypeDef",
     {
         "S3JobManifestGenerator": S3JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
-GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationResultTypeDef",
-    {
-        "Rules": List[LifecycleRuleOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ReplicationConfigurationOutputTypeDef = TypedDict(
     "ReplicationConfigurationOutputTypeDef",
     {
         "Role": str,
         "Rules": List[ReplicationRuleOutputTypeDef],
     },
 )
@@ -3509,38 +3003,14 @@
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAccountLevelOutputTypeDef = TypedDict(
-    "_RequiredAccountLevelOutputTypeDef",
-    {
-        "BucketLevel": BucketLevelOutputTypeDef,
-    },
-)
-_OptionalAccountLevelOutputTypeDef = TypedDict(
-    "_OptionalAccountLevelOutputTypeDef",
-    {
-        "ActivityMetrics": ActivityMetricsOutputTypeDef,
-        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
-        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
-        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AccountLevelOutputTypeDef(
-    _RequiredAccountLevelOutputTypeDef, _OptionalAccountLevelOutputTypeDef
-):
-    pass
-
-
 _RequiredAccountLevelTypeDef = TypedDict(
     "_RequiredAccountLevelTypeDef",
     {
         "BucketLevel": BucketLevelTypeDef,
     },
 )
 _OptionalAccountLevelTypeDef = TypedDict(
@@ -3615,25 +3085,25 @@
     },
 )
 
 _RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationOutputTypeDef",
     {
         "Id": str,
-        "AccountLevel": AccountLevelOutputTypeDef,
+        "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
 )
 _OptionalStorageLensConfigurationOutputTypeDef = TypedDict(
     "_OptionalStorageLensConfigurationOutputTypeDef",
     {
         "Include": IncludeOutputTypeDef,
         "Exclude": ExcludeOutputTypeDef,
         "DataExport": StorageLensDataExportOutputTypeDef,
-        "AwsOrg": StorageLensAwsOrgOutputTypeDef,
+        "AwsOrg": StorageLensAwsOrgTypeDef,
         "StorageLensArn": str,
     },
     total=False,
 )
 
 
 class StorageLensConfigurationOutputTypeDef(
@@ -3668,21 +3138,21 @@
 ):
     pass
 
 
 JobOperationOutputTypeDef = TypedDict(
     "JobOperationOutputTypeDef",
     {
-        "LambdaInvoke": LambdaInvokeOperationOutputTypeDef,
+        "LambdaInvoke": LambdaInvokeOperationTypeDef,
         "S3PutObjectCopy": S3CopyObjectOperationOutputTypeDef,
         "S3PutObjectAcl": S3SetObjectAclOperationOutputTypeDef,
         "S3PutObjectTagging": S3SetObjectTaggingOperationOutputTypeDef,
         "S3DeleteObjectTagging": Dict[str, Any],
-        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationOutputTypeDef,
-        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationOutputTypeDef,
+        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationTypeDef,
+        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationTypeDef,
         "S3PutObjectRetention": S3SetObjectRetentionOperationOutputTypeDef,
         "S3ReplicateObject": Dict[str, Any],
     },
     total=False,
 )
 
 JobOperationTypeDef = TypedDict(
@@ -3743,15 +3213,15 @@
         "Status": JobStatusType,
         "Manifest": JobManifestOutputTypeDef,
         "Operation": JobOperationOutputTypeDef,
         "Priority": int,
         "ProgressSummary": JobProgressSummaryTypeDef,
         "StatusUpdateReason": str,
         "FailureReasons": List[JobFailureTypeDef],
-        "Report": JobReportOutputTypeDef,
+        "Report": JobReportTypeDef,
         "CreationTime": datetime,
         "TerminationDate": datetime,
         "RoleArn": str,
         "SuspendedDate": datetime,
         "SuspendedCause": str,
         "ManifestGenerator": JobManifestGeneratorOutputTypeDef,
         "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
```

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.pyi` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for s3control service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadOutputTypeDef
+    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadTypeDef
 
-    data: AbortIncompleteMultipartUploadOutputTypeDef = {...}
+    data: AbortIncompleteMultipartUploadTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,164 +64,130 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
-    "VpcConfigurationOutputTypeDef",
-    "ActivityMetricsOutputTypeDef",
-    "AdvancedCostOptimizationMetricsOutputTypeDef",
-    "AdvancedDataProtectionMetricsOutputTypeDef",
-    "DetailedStatusCodesMetricsOutputTypeDef",
+    "VpcConfigurationTypeDef",
     "ActivityMetricsTypeDef",
     "AdvancedCostOptimizationMetricsTypeDef",
     "AdvancedDataProtectionMetricsTypeDef",
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
-    "DeleteMultiRegionAccessPointInputOutputTypeDef",
-    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
-    "AwsLambdaTransformationOutputTypeDef",
+    "DeleteMultiRegionAccessPointInputTypeDef",
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
     "AwsLambdaTransformationTypeDef",
-    "CloudWatchMetricsOutputTypeDef",
     "CloudWatchMetricsTypeDef",
     "ObjectLambdaAccessPointAliasTypeDef",
     "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
-    "VpcConfigurationTypeDef",
     "CreateBucketConfigurationTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
-    "PublicAccessBlockConfigurationOutputTypeDef",
-    "RegionOutputTypeDef",
     "RegionTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyRequestRequestTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteBucketLifecycleConfigurationRequestRequestTypeDef",
     "DeleteBucketPolicyRequestRequestTypeDef",
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteJobTaggingRequestRequestTypeDef",
-    "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteMultiRegionAccessPointInputTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     "ExcludeOutputTypeDef",
     "ExcludeTypeDef",
-    "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
-    "SSEKMSEncryptionOutputTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetAccessPointPolicyStatusRequestRequestTypeDef",
     "GetAccessPointRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
     "GetBucketRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "S3TagOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "GetJobTaggingRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef",
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    "MultiRegionAccessPointRouteOutputTypeDef",
+    "MultiRegionAccessPointRouteTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
-    "StorageLensTagOutputTypeDef",
+    "StorageLensTagTypeDef",
     "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
-    "JobReportOutputTypeDef",
     "JobManifestGeneratorFilterOutputTypeDef",
     "JobManifestGeneratorFilterTypeDef",
-    "JobManifestLocationOutputTypeDef",
     "JobManifestLocationTypeDef",
     "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
-    "LambdaInvokeOperationOutputTypeDef",
-    "S3InitiateRestoreObjectOperationOutputTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
     "LifecycleExpirationOutputTypeDef",
     "LifecycleExpirationTypeDef",
-    "NoncurrentVersionExpirationOutputTypeDef",
-    "NoncurrentVersionTransitionOutputTypeDef",
-    "TransitionOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
+    "TransitionOutputTypeDef",
     "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
-    "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "ProposedMultiRegionAccessPointPolicyTypeDef",
     "MultiRegionAccessPointRegionalResponseTypeDef",
     "RegionReportTypeDef",
-    "MultiRegionAccessPointRouteTypeDef",
-    "SelectionCriteriaOutputTypeDef",
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
-    "StorageLensTagTypeDef",
-    "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
-    "S3ObjectOwnerOutputTypeDef",
     "S3ObjectOwnerTypeDef",
     "S3ObjectMetadataOutputTypeDef",
     "S3ObjectMetadataTypeDef",
-    "S3GranteeOutputTypeDef",
     "S3GranteeTypeDef",
-    "S3ObjectLockLegalHoldOutputTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
     "S3RetentionOutputTypeDef",
     "S3RetentionTypeDef",
-    "SSEKMSOutputTypeDef",
     "SSEKMSTypeDef",
-    "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
-    "StorageLensAwsOrgOutputTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
-    "ObjectLambdaContentTransformationOutputTypeDef",
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
     "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointForObjectLambdaResultTypeDef",
     "CreateAccessPointResultTypeDef",
     "CreateBucketResultTypeDef",
     "CreateJobResultTypeDef",
     "CreateMultiRegionAccessPointResultTypeDef",
@@ -231,125 +197,113 @@
     "GetAccessPointPolicyResultTypeDef",
     "GetBucketPolicyResultTypeDef",
     "GetBucketResultTypeDef",
     "GetBucketVersioningResultTypeDef",
     "PutMultiRegionAccessPointPolicyResultTypeDef",
     "UpdateJobPriorityResultTypeDef",
     "UpdateJobStatusResultTypeDef",
-    "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    "GetAccessPointResultTypeDef",
+    "GetPublicAccessBlockOutputTypeDef",
+    "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
+    "GetBucketTaggingResultTypeDef",
+    "GetJobTaggingResultTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "PutJobTaggingRequestRequestTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
+    "S3SetObjectTaggingOperationOutputTypeDef",
     "S3SetObjectTaggingOperationTypeDef",
     "TaggingTypeDef",
-    "GetAccessPointForObjectLambdaResultTypeDef",
-    "GetAccessPointResultTypeDef",
-    "GetPublicAccessBlockOutputTypeDef",
     "CreateMultiRegionAccessPointInputOutputTypeDef",
     "CreateMultiRegionAccessPointInputTypeDef",
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     "GeneratedManifestEncryptionOutputTypeDef",
     "GeneratedManifestEncryptionTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
-    "GetBucketTaggingResultTypeDef",
-    "GetJobTaggingResultTypeDef",
-    "LifecycleRuleAndOperatorOutputTypeDef",
-    "ReplicationRuleAndOperatorOutputTypeDef",
-    "S3SetObjectTaggingOperationOutputTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
-    "MetricsOutputTypeDef",
-    "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    "PrefixLevelStorageMetricsOutputTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
-    "S3GrantOutputTypeDef",
     "S3GrantTypeDef",
-    "S3SetObjectLegalHoldOperationOutputTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
     "S3SetObjectRetentionOperationOutputTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
     "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
-    "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
     "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
-    "LifecycleRuleFilterOutputTypeDef",
-    "ReplicationRuleFilterOutputTypeDef",
     "JobListDescriptorTypeDef",
-    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
-    "PrefixLevelOutputTypeDef",
     "PrefixLevelTypeDef",
     "S3AccessControlListOutputTypeDef",
-    "S3CopyObjectOperationOutputTypeDef",
     "S3AccessControlListTypeDef",
+    "S3CopyObjectOperationOutputTypeDef",
     "S3CopyObjectOperationTypeDef",
     "S3BucketDestinationOutputTypeDef",
     "S3BucketDestinationTypeDef",
     "ObjectLambdaConfigurationOutputTypeDef",
     "ObjectLambdaConfigurationTypeDef",
+    "LifecycleRuleOutputTypeDef",
     "LifecycleRuleTypeDef",
     "S3JobManifestGeneratorOutputTypeDef",
     "S3JobManifestGeneratorTypeDef",
-    "LifecycleRuleOutputTypeDef",
     "ListJobsResultTypeDef",
     "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "AsyncOperationTypeDef",
-    "BucketLevelOutputTypeDef",
     "BucketLevelTypeDef",
     "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
     "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
+    "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
     "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
-    "GetBucketLifecycleConfigurationResultTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
-    "AccountLevelOutputTypeDef",
     "AccountLevelTypeDef",
     "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
     "StorageLensConfigurationOutputTypeDef",
@@ -359,83 +313,36 @@
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
     "JobDescriptorTypeDef",
     "CreateJobRequestRequestTypeDef",
     "DescribeJobResultTypeDef",
 )
 
-AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
-    "AbortIncompleteMultipartUploadOutputTypeDef",
-    {
-        "DaysAfterInitiation": int,
-    },
-    total=False,
-)
-
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
-AccessControlTranslationOutputTypeDef = TypedDict(
-    "AccessControlTranslationOutputTypeDef",
-    {
-        "Owner": Literal["Destination"],
-    },
-)
-
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
+VpcConfigurationTypeDef = TypedDict(
+    "VpcConfigurationTypeDef",
     {
         "VpcId": str,
     },
 )
 
-ActivityMetricsOutputTypeDef = TypedDict(
-    "ActivityMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
-AdvancedCostOptimizationMetricsOutputTypeDef = TypedDict(
-    "AdvancedCostOptimizationMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
-AdvancedDataProtectionMetricsOutputTypeDef = TypedDict(
-    "AdvancedDataProtectionMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
-DetailedStatusCodesMetricsOutputTypeDef = TypedDict(
-    "DetailedStatusCodesMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-    total=False,
-)
-
 ActivityMetricsTypeDef = TypedDict(
     "ActivityMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
     total=False,
 )
@@ -471,48 +378,29 @@
         "Message": str,
         "Resource": str,
         "RequestId": str,
     },
     total=False,
 )
 
-DeleteMultiRegionAccessPointInputOutputTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointInputOutputTypeDef",
+DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointInputTypeDef",
     {
         "Name": str,
     },
 )
 
-PutMultiRegionAccessPointPolicyInputOutputTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
+PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
     {
         "Name": str,
         "Policy": str,
     },
 )
 
-_RequiredAwsLambdaTransformationOutputTypeDef = TypedDict(
-    "_RequiredAwsLambdaTransformationOutputTypeDef",
-    {
-        "FunctionArn": str,
-    },
-)
-_OptionalAwsLambdaTransformationOutputTypeDef = TypedDict(
-    "_OptionalAwsLambdaTransformationOutputTypeDef",
-    {
-        "FunctionPayload": str,
-    },
-    total=False,
-)
-
-class AwsLambdaTransformationOutputTypeDef(
-    _RequiredAwsLambdaTransformationOutputTypeDef, _OptionalAwsLambdaTransformationOutputTypeDef
-):
-    pass
-
 _RequiredAwsLambdaTransformationTypeDef = TypedDict(
     "_RequiredAwsLambdaTransformationTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalAwsLambdaTransformationTypeDef = TypedDict(
@@ -524,21 +412,14 @@
 )
 
 class AwsLambdaTransformationTypeDef(
     _RequiredAwsLambdaTransformationTypeDef, _OptionalAwsLambdaTransformationTypeDef
 ):
     pass
 
-CloudWatchMetricsOutputTypeDef = TypedDict(
-    "CloudWatchMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-    },
-)
-
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
@@ -569,21 +450,14 @@
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
-VpcConfigurationTypeDef = TypedDict(
-    "VpcConfigurationTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
@@ -612,42 +486,14 @@
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
-    "PublicAccessBlockConfigurationOutputTypeDef",
-    {
-        "BlockPublicAcls": bool,
-        "IgnorePublicAcls": bool,
-        "BlockPublicPolicy": bool,
-        "RestrictPublicBuckets": bool,
-    },
-    total=False,
-)
-
-_RequiredRegionOutputTypeDef = TypedDict(
-    "_RequiredRegionOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalRegionOutputTypeDef = TypedDict(
-    "_OptionalRegionOutputTypeDef",
-    {
-        "BucketAccountId": str,
-    },
-    total=False,
-)
-
-class RegionOutputTypeDef(_RequiredRegionOutputTypeDef, _OptionalRegionOutputTypeDef):
-    pass
-
 _RequiredRegionTypeDef = TypedDict(
     "_RequiredRegionTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalRegionTypeDef = TypedDict(
@@ -737,35 +583,21 @@
     "DeleteJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
 
-DeleteMarkerReplicationOutputTypeDef = TypedDict(
-    "DeleteMarkerReplicationOutputTypeDef",
-    {
-        "Status": DeleteMarkerReplicationStatusType,
-    },
-)
-
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
 )
 
-DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointInputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 DeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "DeletePublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -797,22 +629,14 @@
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     {
         "AccountId": str,
         "RequestTokenARN": str,
     },
 )
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "ReplicaKmsKeyID": str,
-    },
-    total=False,
-)
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
     total=False,
 )
@@ -839,35 +663,21 @@
     {
         "Buckets": Sequence[str],
         "Regions": Sequence[str],
     },
     total=False,
 )
 
-ExistingObjectReplicationOutputTypeDef = TypedDict(
-    "ExistingObjectReplicationOutputTypeDef",
-    {
-        "Status": ExistingObjectReplicationStatusType,
-    },
-)
-
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
         "Status": ExistingObjectReplicationStatusType,
     },
 )
 
-SSEKMSEncryptionOutputTypeDef = TypedDict(
-    "SSEKMSEncryptionOutputTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-
 SSEKMSEncryptionTypeDef = TypedDict(
     "SSEKMSEncryptionTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -971,22 +781,14 @@
     "GetBucketTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-S3TagOutputTypeDef = TypedDict(
-    "S3TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 GetBucketVersioningRequestRequestTypeDef = TypedDict(
     "GetBucketVersioningRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -1027,32 +829,31 @@
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
         "AccountId": str,
         "Mrap": str,
     },
 )
 
-_RequiredMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
-    "_RequiredMultiRegionAccessPointRouteOutputTypeDef",
+_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_RequiredMultiRegionAccessPointRouteTypeDef",
     {
         "TrafficDialPercentage": int,
     },
 )
-_OptionalMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
-    "_OptionalMultiRegionAccessPointRouteOutputTypeDef",
+_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_OptionalMultiRegionAccessPointRouteTypeDef",
     {
         "Bucket": str,
         "Region": str,
     },
     total=False,
 )
 
-class MultiRegionAccessPointRouteOutputTypeDef(
-    _RequiredMultiRegionAccessPointRouteOutputTypeDef,
-    _OptionalMultiRegionAccessPointRouteOutputTypeDef,
+class MultiRegionAccessPointRouteTypeDef(
+    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
 ):
     pass
 
 GetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "GetPublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -1071,16 +872,16 @@
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
         "ConfigId": str,
         "AccountId": str,
     },
 )
 
-StorageLensTagOutputTypeDef = TypedDict(
-    "StorageLensTagOutputTypeDef",
+StorageLensTagTypeDef = TypedDict(
+    "StorageLensTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 IncludeOutputTypeDef = TypedDict(
@@ -1106,34 +907,14 @@
     {
         "FailureCode": str,
         "FailureReason": str,
     },
     total=False,
 )
 
-_RequiredJobReportOutputTypeDef = TypedDict(
-    "_RequiredJobReportOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalJobReportOutputTypeDef = TypedDict(
-    "_OptionalJobReportOutputTypeDef",
-    {
-        "Bucket": str,
-        "Format": Literal["Report_CSV_20180820"],
-        "Prefix": str,
-        "ReportScope": JobReportScopeType,
-    },
-    total=False,
-)
-
-class JobReportOutputTypeDef(_RequiredJobReportOutputTypeDef, _OptionalJobReportOutputTypeDef):
-    pass
-
 JobManifestGeneratorFilterOutputTypeDef = TypedDict(
     "JobManifestGeneratorFilterOutputTypeDef",
     {
         "EligibleForReplication": bool,
         "CreatedAfter": datetime,
         "CreatedBefore": datetime,
         "ObjectReplicationStatuses": List[ReplicationStatusType],
@@ -1148,34 +929,14 @@
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
     },
     total=False,
 )
 
-_RequiredJobManifestLocationOutputTypeDef = TypedDict(
-    "_RequiredJobManifestLocationOutputTypeDef",
-    {
-        "ObjectArn": str,
-        "ETag": str,
-    },
-)
-_OptionalJobManifestLocationOutputTypeDef = TypedDict(
-    "_OptionalJobManifestLocationOutputTypeDef",
-    {
-        "ObjectVersionId": str,
-    },
-    total=False,
-)
-
-class JobManifestLocationOutputTypeDef(
-    _RequiredJobManifestLocationOutputTypeDef, _OptionalJobManifestLocationOutputTypeDef
-):
-    pass
-
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
 )
@@ -1224,31 +985,14 @@
     },
     total=False,
 )
 
 class JobManifestSpecTypeDef(_RequiredJobManifestSpecTypeDef, _OptionalJobManifestSpecTypeDef):
     pass
 
-LambdaInvokeOperationOutputTypeDef = TypedDict(
-    "LambdaInvokeOperationOutputTypeDef",
-    {
-        "FunctionArn": str,
-    },
-    total=False,
-)
-
-S3InitiateRestoreObjectOperationOutputTypeDef = TypedDict(
-    "S3InitiateRestoreObjectOperationOutputTypeDef",
-    {
-        "ExpirationInDays": int,
-        "GlacierJobTier": S3GlacierJobTierType,
-    },
-    total=False,
-)
-
 LambdaInvokeOperationTypeDef = TypedDict(
     "LambdaInvokeOperationTypeDef",
     {
         "FunctionArn": str,
     },
     total=False,
 )
@@ -1286,25 +1030,25 @@
         "Date": Union[datetime, str],
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
-NoncurrentVersionExpirationOutputTypeDef = TypedDict(
-    "NoncurrentVersionExpirationOutputTypeDef",
+NoncurrentVersionExpirationTypeDef = TypedDict(
+    "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
     total=False,
 )
 
-NoncurrentVersionTransitionOutputTypeDef = TypedDict(
-    "NoncurrentVersionTransitionOutputTypeDef",
+NoncurrentVersionTransitionTypeDef = TypedDict(
+    "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
@@ -1314,32 +1058,14 @@
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-NoncurrentVersionExpirationTypeDef = TypedDict(
-    "NoncurrentVersionExpirationTypeDef",
-    {
-        "NoncurrentDays": int,
-        "NewerNoncurrentVersions": int,
-    },
-    total=False,
-)
-
-NoncurrentVersionTransitionTypeDef = TypedDict(
-    "NoncurrentVersionTransitionTypeDef",
-    {
-        "NoncurrentDays": int,
-        "StorageClass": TransitionStorageClassType,
-    },
-    total=False,
-)
-
 TransitionTypeDef = TypedDict(
     "TransitionTypeDef",
     {
         "Date": Union[datetime, str],
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
@@ -1520,22 +1246,14 @@
 
 class ListStorageLensConfigurationsRequestRequestTypeDef(
     _RequiredListStorageLensConfigurationsRequestRequestTypeDef,
     _OptionalListStorageLensConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-ReplicationTimeValueOutputTypeDef = TypedDict(
-    "ReplicationTimeValueOutputTypeDef",
-    {
-        "Minutes": int,
-    },
-    total=False,
-)
-
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
@@ -1563,44 +1281,14 @@
         "Bucket": str,
         "Region": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
-_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_RequiredMultiRegionAccessPointRouteTypeDef",
-    {
-        "TrafficDialPercentage": int,
-    },
-)
-_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_OptionalMultiRegionAccessPointRouteTypeDef",
-    {
-        "Bucket": str,
-        "Region": str,
-    },
-    total=False,
-)
-
-class MultiRegionAccessPointRouteTypeDef(
-    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
-):
-    pass
-
-SelectionCriteriaOutputTypeDef = TypedDict(
-    "SelectionCriteriaOutputTypeDef",
-    {
-        "Delimiter": str,
-        "MaxDepth": int,
-        "MinStorageBytesPercentage": float,
-    },
-    total=False,
-)
-
 SelectionCriteriaTypeDef = TypedDict(
     "SelectionCriteriaTypeDef",
     {
         "Delimiter": str,
         "MaxDepth": int,
         "MinStorageBytesPercentage": float,
     },
@@ -1651,53 +1339,21 @@
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
 )
 
-PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
-    {
-        "Name": str,
-        "Policy": str,
-    },
-)
-
-StorageLensTagTypeDef = TypedDict(
-    "StorageLensTagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-ReplicaModificationsOutputTypeDef = TypedDict(
-    "ReplicaModificationsOutputTypeDef",
-    {
-        "Status": ReplicaModificationsStatusType,
-    },
-)
-
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
 )
 
-S3ObjectOwnerOutputTypeDef = TypedDict(
-    "S3ObjectOwnerOutputTypeDef",
-    {
-        "ID": str,
-        "DisplayName": str,
-    },
-    total=False,
-)
-
 S3ObjectOwnerTypeDef = TypedDict(
     "S3ObjectOwnerTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
@@ -1735,41 +1391,24 @@
         "HttpExpiresDate": Union[datetime, str],
         "RequesterCharged": bool,
         "SSEAlgorithm": S3SSEAlgorithmType,
     },
     total=False,
 )
 
-S3GranteeOutputTypeDef = TypedDict(
-    "S3GranteeOutputTypeDef",
-    {
-        "TypeIdentifier": S3GranteeTypeIdentifierType,
-        "Identifier": str,
-        "DisplayName": str,
-    },
-    total=False,
-)
-
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-S3ObjectLockLegalHoldOutputTypeDef = TypedDict(
-    "S3ObjectLockLegalHoldOutputTypeDef",
-    {
-        "Status": S3ObjectLockLegalHoldStatusType,
-    },
-)
-
 S3ObjectLockLegalHoldTypeDef = TypedDict(
     "S3ObjectLockLegalHoldTypeDef",
     {
         "Status": S3ObjectLockLegalHoldStatusType,
     },
 )
 
@@ -1787,49 +1426,28 @@
     {
         "RetainUntilDate": Union[datetime, str],
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
-SSEKMSOutputTypeDef = TypedDict(
-    "SSEKMSOutputTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
-SseKmsEncryptedObjectsOutputTypeDef = TypedDict(
-    "SseKmsEncryptedObjectsOutputTypeDef",
-    {
-        "Status": SseKmsEncryptedObjectsStatusType,
-    },
-)
-
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
-StorageLensAwsOrgOutputTypeDef = TypedDict(
-    "StorageLensAwsOrgOutputTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
 StorageLensAwsOrgTypeDef = TypedDict(
     "StorageLensAwsOrgTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -1870,31 +1488,41 @@
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
 )
 _OptionalAccessPointTypeDef = TypedDict(
     "_OptionalAccessPointTypeDef",
     {
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "VpcConfiguration": VpcConfigurationTypeDef,
         "AccessPointArn": str,
         "Alias": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
 class AccessPointTypeDef(_RequiredAccessPointTypeDef, _OptionalAccessPointTypeDef):
     pass
 
-ObjectLambdaContentTransformationOutputTypeDef = TypedDict(
-    "ObjectLambdaContentTransformationOutputTypeDef",
+DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     {
-        "AwsLambda": AwsLambdaTransformationOutputTypeDef,
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": DeleteMultiRegionAccessPointInputTypeDef,
+    },
+)
+
+PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
-    total=False,
 )
 
 ObjectLambdaContentTransformationTypeDef = TypedDict(
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
@@ -2045,22 +1673,14 @@
         "JobId": str,
         "Status": JobStatusType,
         "StatusUpdateReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
-    "PutPublicAccessBlockRequestRequestTypeDef",
-    {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "AccountId": str,
-    },
-)
-
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Bucket": str,
     },
@@ -2076,14 +1696,58 @@
 )
 
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
+GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    {
+        "Name": str,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "CreationDate": datetime,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessPointResultTypeDef = TypedDict(
+    "GetAccessPointResultTypeDef",
+    {
+        "Name": str,
+        "Bucket": str,
+        "NetworkOrigin": NetworkOriginType,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "CreationDate": datetime,
+        "Alias": str,
+        "AccessPointArn": str,
+        "Endpoints": Dict[str, str],
+        "BucketAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicAccessBlockOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputTypeDef",
+    {
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
+    "PutPublicAccessBlockRequestRequestTypeDef",
+    {
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "AccountId": str,
+    },
+)
+
 _RequiredCreateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBucketRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalCreateBucketRequestRequestTypeDef = TypedDict(
@@ -2103,14 +1767,41 @@
 )
 
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
+GetBucketTaggingResultTypeDef = TypedDict(
+    "GetBucketTaggingResultTypeDef",
+    {
+        "TagSet": List[S3TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobTaggingResultTypeDef = TypedDict(
+    "GetJobTaggingResultTypeDef",
+    {
+        "Tags": List[S3TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[S3TagTypeDef],
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+    },
+    total=False,
+)
+
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": Sequence[S3TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
@@ -2123,23 +1814,40 @@
     {
         "AccountId": str,
         "JobId": str,
         "Tags": Sequence[S3TagTypeDef],
     },
 )
 
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[S3TagTypeDef],
+    },
+    total=False,
+)
+
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": Sequence[S3TagTypeDef],
     },
     total=False,
 )
 
+S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
+    "S3SetObjectTaggingOperationOutputTypeDef",
+    {
+        "TagSet": List[S3TagTypeDef],
+    },
+    total=False,
+)
+
 S3SetObjectTaggingOperationTypeDef = TypedDict(
     "S3SetObjectTaggingOperationTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
     total=False,
 )
@@ -2147,61 +1855,25 @@
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
 )
 
-GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointForObjectLambdaResultTypeDef",
-    {
-        "Name": str,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "CreationDate": datetime,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccessPointResultTypeDef = TypedDict(
-    "GetAccessPointResultTypeDef",
-    {
-        "Name": str,
-        "Bucket": str,
-        "NetworkOrigin": NetworkOriginType,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "CreationDate": datetime,
-        "Alias": str,
-        "AccessPointArn": str,
-        "Endpoints": Dict[str, str],
-        "BucketAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPublicAccessBlockOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputTypeDef",
-    {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
     "_RequiredCreateMultiRegionAccessPointInputOutputTypeDef",
     {
         "Name": str,
-        "Regions": List[RegionOutputTypeDef],
+        "Regions": List[RegionTypeDef],
     },
 )
 _OptionalCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
     "_OptionalCreateMultiRegionAccessPointInputOutputTypeDef",
     {
-        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
+        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
     },
     total=False,
 )
 
 class CreateMultiRegionAccessPointInputOutputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputOutputTypeDef,
     _OptionalCreateMultiRegionAccessPointInputOutputTypeDef,
@@ -2225,28 +1897,19 @@
 
 class CreateMultiRegionAccessPointInputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputTypeDef,
     _OptionalCreateMultiRegionAccessPointInputTypeDef,
 ):
     pass
 
-DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": DeleteMultiRegionAccessPointInputTypeDef,
-    },
-)
-
 GeneratedManifestEncryptionOutputTypeDef = TypedDict(
     "GeneratedManifestEncryptionOutputTypeDef",
     {
         "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSEncryptionOutputTypeDef,
+        "SSEKMS": SSEKMSEncryptionTypeDef,
     },
     total=False,
 )
 
 GeneratedManifestEncryptionTypeDef = TypedDict(
     "GeneratedManifestEncryptionTypeDef",
     {
@@ -2276,89 +1939,63 @@
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     {
         "Established": PolicyStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBucketTaggingResultTypeDef = TypedDict(
-    "GetBucketTaggingResultTypeDef",
-    {
-        "TagSet": List[S3TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobTaggingResultTypeDef = TypedDict(
-    "GetJobTaggingResultTypeDef",
+GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
+    "GetMultiRegionAccessPointRoutesResultTypeDef",
     {
-        "Tags": List[S3TagOutputTypeDef],
+        "Mrap": str,
+        "Routes": List[MultiRegionAccessPointRouteTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[S3TagOutputTypeDef],
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
-ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
-    "ReplicationRuleAndOperatorOutputTypeDef",
+SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
-        "Prefix": str,
-        "Tags": List[S3TagOutputTypeDef],
+        "AccountId": str,
+        "Mrap": str,
+        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
     },
-    total=False,
 )
 
-S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
-    "S3SetObjectTaggingOperationOutputTypeDef",
-    {
-        "TagSet": List[S3TagOutputTypeDef],
-    },
-    total=False,
-)
-
-GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
-    "GetMultiRegionAccessPointRoutesResultTypeDef",
+GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
+    "GetStorageLensConfigurationTaggingResultTypeDef",
     {
-        "Mrap": str,
-        "Routes": List[MultiRegionAccessPointRouteOutputTypeDef],
+        "Tags": List[StorageLensTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
-    "GetStorageLensConfigurationTaggingResultTypeDef",
+PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
-        "Tags": List[StorageLensTagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ConfigId": str,
+        "AccountId": str,
+        "Tags": Sequence[StorageLensTagTypeDef],
     },
 )
 
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
-        "Location": JobManifestLocationOutputTypeDef,
+        "Location": JobManifestLocationTypeDef,
     },
     total=False,
 )
 
 JobManifestOutputTypeDef = TypedDict(
     "JobManifestOutputTypeDef",
     {
         "Spec": JobManifestSpecOutputTypeDef,
-        "Location": JobManifestLocationOutputTypeDef,
+        "Location": JobManifestLocationTypeDef,
     },
 )
 
 JobManifestTypeDef = TypedDict(
     "JobManifestTypeDef",
     {
         "Spec": JobManifestSpecTypeDef,
@@ -2411,39 +2048,14 @@
     {
         "NextToken": str,
         "StorageLensConfigurationList": List[ListStorageLensConfigurationEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricsOutputTypeDef = TypedDict(
-    "_RequiredMetricsOutputTypeDef",
-    {
-        "Status": MetricsStatusType,
-    },
-)
-_OptionalMetricsOutputTypeDef = TypedDict(
-    "_OptionalMetricsOutputTypeDef",
-    {
-        "EventThreshold": ReplicationTimeValueOutputTypeDef,
-    },
-    total=False,
-)
-
-class MetricsOutputTypeDef(_RequiredMetricsOutputTypeDef, _OptionalMetricsOutputTypeDef):
-    pass
-
-ReplicationTimeOutputTypeDef = TypedDict(
-    "ReplicationTimeOutputTypeDef",
-    {
-        "Status": ReplicationTimeStatusType,
-        "Time": ReplicationTimeValueOutputTypeDef,
-    },
-)
-
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
     },
 )
 _OptionalMetricsTypeDef = TypedDict(
@@ -2484,39 +2096,21 @@
 
 MultiRegionAccessPointReportTypeDef = TypedDict(
     "MultiRegionAccessPointReportTypeDef",
     {
         "Name": str,
         "Alias": str,
         "CreatedAt": datetime,
-        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
+        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
         "Status": MultiRegionAccessPointStatusType,
         "Regions": List[RegionReportTypeDef],
     },
     total=False,
 )
 
-SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "Mrap": str,
-        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
-    },
-)
-
-PrefixLevelStorageMetricsOutputTypeDef = TypedDict(
-    "PrefixLevelStorageMetricsOutputTypeDef",
-    {
-        "IsEnabled": bool,
-        "SelectionCriteria": SelectionCriteriaOutputTypeDef,
-    },
-    total=False,
-)
-
 PrefixLevelStorageMetricsTypeDef = TypedDict(
     "PrefixLevelStorageMetricsTypeDef",
     {
         "IsEnabled": bool,
         "SelectionCriteria": SelectionCriteriaTypeDef,
     },
     total=False,
@@ -2540,57 +2134,23 @@
 
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
-PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
-    },
-)
-
-PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
-    {
-        "ConfigId": str,
-        "AccountId": str,
-        "Tags": Sequence[StorageLensTagTypeDef],
-    },
-)
-
-S3GrantOutputTypeDef = TypedDict(
-    "S3GrantOutputTypeDef",
-    {
-        "Grantee": S3GranteeOutputTypeDef,
-        "Permission": S3PermissionType,
-    },
-    total=False,
-)
-
 S3GrantTypeDef = TypedDict(
     "S3GrantTypeDef",
     {
         "Grantee": S3GranteeTypeDef,
         "Permission": S3PermissionType,
     },
     total=False,
 )
 
-S3SetObjectLegalHoldOperationOutputTypeDef = TypedDict(
-    "S3SetObjectLegalHoldOperationOutputTypeDef",
-    {
-        "LegalHold": S3ObjectLockLegalHoldOutputTypeDef,
-    },
-)
-
 S3SetObjectLegalHoldOperationTypeDef = TypedDict(
     "S3SetObjectLegalHoldOperationTypeDef",
     {
         "LegalHold": S3ObjectLockLegalHoldTypeDef,
     },
 )
 
@@ -2633,37 +2193,28 @@
 ):
     pass
 
 StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
     "StorageLensDataExportEncryptionOutputTypeDef",
     {
         "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSOutputTypeDef,
+        "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
 StorageLensDataExportEncryptionTypeDef = TypedDict(
     "StorageLensDataExportEncryptionTypeDef",
     {
         "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
-SourceSelectionCriteriaOutputTypeDef = TypedDict(
-    "SourceSelectionCriteriaOutputTypeDef",
-    {
-        "SseKmsEncryptedObjects": SseKmsEncryptedObjectsOutputTypeDef,
-        "ReplicaModifications": ReplicaModificationsOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
     total=False,
@@ -2678,15 +2229,15 @@
     },
 )
 
 ObjectLambdaTransformationConfigurationOutputTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationOutputTypeDef",
     {
         "Actions": List[ObjectLambdaTransformationConfigurationActionType],
-        "ContentTransformation": ObjectLambdaContentTransformationOutputTypeDef,
+        "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
     },
 )
 
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
@@ -2699,26 +2250,48 @@
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagTypeDef,
+        "And": LifecycleRuleAndOperatorOutputTypeDef,
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+    },
+    total=False,
+)
+
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": LifecycleRuleAndOperatorTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagTypeDef,
+        "And": ReplicationRuleAndOperatorOutputTypeDef,
+    },
+    total=False,
+)
+
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
@@ -2734,16 +2307,16 @@
     },
 )
 
 AsyncRequestParametersTypeDef = TypedDict(
     "AsyncRequestParametersTypeDef",
     {
         "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
-        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputOutputTypeDef,
-        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputOutputTypeDef,
+        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
+        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
     total=False,
 )
 
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
@@ -2793,36 +2366,14 @@
 )
 
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
-LifecycleRuleFilterOutputTypeDef = TypedDict(
-    "LifecycleRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagOutputTypeDef,
-        "And": LifecycleRuleAndOperatorOutputTypeDef,
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
-ReplicationRuleFilterOutputTypeDef = TypedDict(
-    "ReplicationRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagOutputTypeDef,
-        "And": ReplicationRuleAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2830,38 +2381,14 @@
         "CreationTime": datetime,
         "TerminationDate": datetime,
         "ProgressSummary": JobProgressSummaryTypeDef,
     },
     total=False,
 )
 
-_RequiredDestinationOutputTypeDef = TypedDict(
-    "_RequiredDestinationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalDestinationOutputTypeDef = TypedDict(
-    "_OptionalDestinationOutputTypeDef",
-    {
-        "Account": str,
-        "ReplicationTime": ReplicationTimeOutputTypeDef,
-        "AccessControlTranslation": AccessControlTranslationOutputTypeDef,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "Metrics": MetricsOutputTypeDef,
-        "StorageClass": ReplicationStorageClassType,
-    },
-    total=False,
-)
-
-class DestinationOutputTypeDef(
-    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
-):
-    pass
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDestinationTypeDef = TypedDict(
@@ -2910,57 +2437,69 @@
     {
         "AccessPoints": List[MultiRegionAccessPointReportTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PrefixLevelOutputTypeDef = TypedDict(
-    "PrefixLevelOutputTypeDef",
-    {
-        "StorageMetrics": PrefixLevelStorageMetricsOutputTypeDef,
-    },
-)
-
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
     },
 )
 
 _RequiredS3AccessControlListOutputTypeDef = TypedDict(
     "_RequiredS3AccessControlListOutputTypeDef",
     {
-        "Owner": S3ObjectOwnerOutputTypeDef,
+        "Owner": S3ObjectOwnerTypeDef,
     },
 )
 _OptionalS3AccessControlListOutputTypeDef = TypedDict(
     "_OptionalS3AccessControlListOutputTypeDef",
     {
-        "Grants": List[S3GrantOutputTypeDef],
+        "Grants": List[S3GrantTypeDef],
     },
     total=False,
 )
 
 class S3AccessControlListOutputTypeDef(
     _RequiredS3AccessControlListOutputTypeDef, _OptionalS3AccessControlListOutputTypeDef
 ):
     pass
 
+_RequiredS3AccessControlListTypeDef = TypedDict(
+    "_RequiredS3AccessControlListTypeDef",
+    {
+        "Owner": S3ObjectOwnerTypeDef,
+    },
+)
+_OptionalS3AccessControlListTypeDef = TypedDict(
+    "_OptionalS3AccessControlListTypeDef",
+    {
+        "Grants": Sequence[S3GrantTypeDef],
+    },
+    total=False,
+)
+
+class S3AccessControlListTypeDef(
+    _RequiredS3AccessControlListTypeDef, _OptionalS3AccessControlListTypeDef
+):
+    pass
+
 S3CopyObjectOperationOutputTypeDef = TypedDict(
     "S3CopyObjectOperationOutputTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
-        "AccessControlGrants": List[S3GrantOutputTypeDef],
+        "AccessControlGrants": List[S3GrantTypeDef],
         "MetadataDirective": S3MetadataDirectiveType,
         "ModifiedSinceConstraint": datetime,
         "NewObjectMetadata": S3ObjectMetadataOutputTypeDef,
-        "NewObjectTagging": List[S3TagOutputTypeDef],
+        "NewObjectTagging": List[S3TagTypeDef],
         "RedirectLocation": str,
         "RequesterPays": bool,
         "StorageClass": S3StorageClassType,
         "UnModifiedSinceConstraint": datetime,
         "SSEAwsKmsKeyId": str,
         "TargetKeyPrefix": str,
         "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
@@ -2968,33 +2507,14 @@
         "ObjectLockRetainUntilDate": datetime,
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
-_RequiredS3AccessControlListTypeDef = TypedDict(
-    "_RequiredS3AccessControlListTypeDef",
-    {
-        "Owner": S3ObjectOwnerTypeDef,
-    },
-)
-_OptionalS3AccessControlListTypeDef = TypedDict(
-    "_OptionalS3AccessControlListTypeDef",
-    {
-        "Grants": Sequence[S3GrantTypeDef],
-    },
-    total=False,
-)
-
-class S3AccessControlListTypeDef(
-    _RequiredS3AccessControlListTypeDef, _OptionalS3AccessControlListTypeDef
-):
-    pass
-
 S3CopyObjectOperationTypeDef = TypedDict(
     "S3CopyObjectOperationTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
         "AccessControlGrants": Sequence[S3GrantTypeDef],
         "MetadataDirective": S3MetadataDirectiveType,
@@ -3100,14 +2620,39 @@
 )
 
 class ObjectLambdaConfigurationTypeDef(
     _RequiredObjectLambdaConfigurationTypeDef, _OptionalObjectLambdaConfigurationTypeDef
 ):
     pass
 
+_RequiredLifecycleRuleOutputTypeDef = TypedDict(
+    "_RequiredLifecycleRuleOutputTypeDef",
+    {
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalLifecycleRuleOutputTypeDef = TypedDict(
+    "_OptionalLifecycleRuleOutputTypeDef",
+    {
+        "Expiration": LifecycleExpirationOutputTypeDef,
+        "ID": str,
+        "Filter": LifecycleRuleFilterOutputTypeDef,
+        "Transitions": List[TransitionOutputTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
+    },
+    total=False,
+)
+
+class LifecycleRuleOutputTypeDef(
+    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
+):
+    pass
+
 _RequiredLifecycleRuleTypeDef = TypedDict(
     "_RequiredLifecycleRuleTypeDef",
     {
         "Status": ExpirationStatusType,
     },
 )
 _OptionalLifecycleRuleTypeDef = TypedDict(
@@ -3167,66 +2712,41 @@
 )
 
 class S3JobManifestGeneratorTypeDef(
     _RequiredS3JobManifestGeneratorTypeDef, _OptionalS3JobManifestGeneratorTypeDef
 ):
     pass
 
-_RequiredLifecycleRuleOutputTypeDef = TypedDict(
-    "_RequiredLifecycleRuleOutputTypeDef",
-    {
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalLifecycleRuleOutputTypeDef = TypedDict(
-    "_OptionalLifecycleRuleOutputTypeDef",
-    {
-        "Expiration": LifecycleExpirationOutputTypeDef,
-        "ID": str,
-        "Filter": LifecycleRuleFilterOutputTypeDef,
-        "Transitions": List[TransitionOutputTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionOutputTypeDef],
-        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
-        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
-    },
-    total=False,
-)
-
-class LifecycleRuleOutputTypeDef(
-    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
-):
-    pass
-
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredReplicationRuleOutputTypeDef = TypedDict(
     "_RequiredReplicationRuleOutputTypeDef",
     {
         "Status": ReplicationRuleStatusType,
-        "Destination": DestinationOutputTypeDef,
+        "Destination": DestinationTypeDef,
         "Bucket": str,
     },
 )
 _OptionalReplicationRuleOutputTypeDef = TypedDict(
     "_OptionalReplicationRuleOutputTypeDef",
     {
         "ID": str,
         "Priority": int,
         "Prefix": str,
         "Filter": ReplicationRuleFilterOutputTypeDef,
-        "SourceSelectionCriteria": SourceSelectionCriteriaOutputTypeDef,
-        "ExistingObjectReplication": ExistingObjectReplicationOutputTypeDef,
-        "DeleteMarkerReplication": DeleteMarkerReplicationOutputTypeDef,
+        "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
+        "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
+        "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
     total=False,
 )
 
 class ReplicationRuleOutputTypeDef(
     _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
 ):
@@ -3266,26 +2786,14 @@
         "RequestParameters": AsyncRequestParametersTypeDef,
         "RequestStatus": str,
         "ResponseDetails": AsyncResponseDetailsTypeDef,
     },
     total=False,
 )
 
-BucketLevelOutputTypeDef = TypedDict(
-    "BucketLevelOutputTypeDef",
-    {
-        "ActivityMetrics": ActivityMetricsOutputTypeDef,
-        "PrefixLevel": PrefixLevelOutputTypeDef,
-        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
-        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
-        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
-    },
-    total=False,
-)
-
 BucketLevelTypeDef = TypedDict(
     "BucketLevelTypeDef",
     {
         "ActivityMetrics": ActivityMetricsTypeDef,
         "PrefixLevel": PrefixLevelTypeDef,
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
@@ -3312,15 +2820,15 @@
     total=False,
 )
 
 StorageLensDataExportOutputTypeDef = TypedDict(
     "StorageLensDataExportOutputTypeDef",
     {
         "S3BucketDestination": S3BucketDestinationOutputTypeDef,
-        "CloudWatchMetrics": CloudWatchMetricsOutputTypeDef,
+        "CloudWatchMetrics": CloudWatchMetricsTypeDef,
     },
     total=False,
 )
 
 StorageLensDataExportTypeDef = TypedDict(
     "StorageLensDataExportTypeDef",
     {
@@ -3352,14 +2860,22 @@
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
+GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationResultTypeDef",
+    {
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
     total=False,
 )
@@ -3376,22 +2892,14 @@
     "JobManifestGeneratorTypeDef",
     {
         "S3JobManifestGenerator": S3JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
-GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationResultTypeDef",
-    {
-        "Rules": List[LifecycleRuleOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ReplicationConfigurationOutputTypeDef = TypedDict(
     "ReplicationConfigurationOutputTypeDef",
     {
         "Role": str,
         "Rules": List[ReplicationRuleOutputTypeDef],
     },
 )
@@ -3408,36 +2916,14 @@
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAccountLevelOutputTypeDef = TypedDict(
-    "_RequiredAccountLevelOutputTypeDef",
-    {
-        "BucketLevel": BucketLevelOutputTypeDef,
-    },
-)
-_OptionalAccountLevelOutputTypeDef = TypedDict(
-    "_OptionalAccountLevelOutputTypeDef",
-    {
-        "ActivityMetrics": ActivityMetricsOutputTypeDef,
-        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
-        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
-        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
-    },
-    total=False,
-)
-
-class AccountLevelOutputTypeDef(
-    _RequiredAccountLevelOutputTypeDef, _OptionalAccountLevelOutputTypeDef
-):
-    pass
-
 _RequiredAccountLevelTypeDef = TypedDict(
     "_RequiredAccountLevelTypeDef",
     {
         "BucketLevel": BucketLevelTypeDef,
     },
 )
 _OptionalAccountLevelTypeDef = TypedDict(
@@ -3508,25 +2994,25 @@
     },
 )
 
 _RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationOutputTypeDef",
     {
         "Id": str,
-        "AccountLevel": AccountLevelOutputTypeDef,
+        "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
 )
 _OptionalStorageLensConfigurationOutputTypeDef = TypedDict(
     "_OptionalStorageLensConfigurationOutputTypeDef",
     {
         "Include": IncludeOutputTypeDef,
         "Exclude": ExcludeOutputTypeDef,
         "DataExport": StorageLensDataExportOutputTypeDef,
-        "AwsOrg": StorageLensAwsOrgOutputTypeDef,
+        "AwsOrg": StorageLensAwsOrgTypeDef,
         "StorageLensArn": str,
     },
     total=False,
 )
 
 class StorageLensConfigurationOutputTypeDef(
     _RequiredStorageLensConfigurationOutputTypeDef, _OptionalStorageLensConfigurationOutputTypeDef
@@ -3557,21 +3043,21 @@
     _RequiredStorageLensConfigurationTypeDef, _OptionalStorageLensConfigurationTypeDef
 ):
     pass
 
 JobOperationOutputTypeDef = TypedDict(
     "JobOperationOutputTypeDef",
     {
-        "LambdaInvoke": LambdaInvokeOperationOutputTypeDef,
+        "LambdaInvoke": LambdaInvokeOperationTypeDef,
         "S3PutObjectCopy": S3CopyObjectOperationOutputTypeDef,
         "S3PutObjectAcl": S3SetObjectAclOperationOutputTypeDef,
         "S3PutObjectTagging": S3SetObjectTaggingOperationOutputTypeDef,
         "S3DeleteObjectTagging": Dict[str, Any],
-        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationOutputTypeDef,
-        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationOutputTypeDef,
+        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationTypeDef,
+        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationTypeDef,
         "S3PutObjectRetention": S3SetObjectRetentionOperationOutputTypeDef,
         "S3ReplicateObject": Dict[str, Any],
     },
     total=False,
 )
 
 JobOperationTypeDef = TypedDict(
@@ -3630,15 +3116,15 @@
         "Status": JobStatusType,
         "Manifest": JobManifestOutputTypeDef,
         "Operation": JobOperationOutputTypeDef,
         "Priority": int,
         "ProgressSummary": JobProgressSummaryTypeDef,
         "StatusUpdateReason": str,
         "FailureReasons": List[JobFailureTypeDef],
-        "Report": JobReportOutputTypeDef,
+        "Report": JobReportTypeDef,
         "CreationTime": datetime,
         "TerminationDate": datetime,
         "RoleArn": str,
         "SuspendedDate": datetime,
         "SuspendedCause": str,
         "ManifestGenerator": JobManifestGeneratorOutputTypeDef,
         "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
```

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/PKG-INFO` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.28.12
-Summary: Type annotations for boto3.S3Control 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,164 +364,130 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
-    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
-    VpcConfigurationOutputTypeDef,
-    ActivityMetricsOutputTypeDef,
-    AdvancedCostOptimizationMetricsOutputTypeDef,
-    AdvancedDataProtectionMetricsOutputTypeDef,
-    DetailedStatusCodesMetricsOutputTypeDef,
+    VpcConfigurationTypeDef,
     ActivityMetricsTypeDef,
     AdvancedCostOptimizationMetricsTypeDef,
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
-    DeleteMultiRegionAccessPointInputOutputTypeDef,
-    PutMultiRegionAccessPointPolicyInputOutputTypeDef,
-    AwsLambdaTransformationOutputTypeDef,
+    DeleteMultiRegionAccessPointInputTypeDef,
+    PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
-    CloudWatchMetricsOutputTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
     ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    VpcConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
-    PublicAccessBlockConfigurationOutputTypeDef,
-    RegionOutputTypeDef,
     RegionTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
-    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteMultiRegionAccessPointInputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
     ExcludeOutputTypeDef,
     ExcludeTypeDef,
-    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
-    SSEKMSEncryptionOutputTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    S3TagOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    MultiRegionAccessPointRouteOutputTypeDef,
+    MultiRegionAccessPointRouteTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
-    StorageLensTagOutputTypeDef,
+    StorageLensTagTypeDef,
     IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
-    JobReportOutputTypeDef,
     JobManifestGeneratorFilterOutputTypeDef,
     JobManifestGeneratorFilterTypeDef,
-    JobManifestLocationOutputTypeDef,
     JobManifestLocationTypeDef,
     JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
-    LambdaInvokeOperationOutputTypeDef,
-    S3InitiateRestoreObjectOperationOutputTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
-    NoncurrentVersionExpirationOutputTypeDef,
-    NoncurrentVersionTransitionOutputTypeDef,
-    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
+    TransitionOutputTypeDef,
     TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
-    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
-    MultiRegionAccessPointRouteTypeDef,
-    SelectionCriteriaOutputTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
-    PutMultiRegionAccessPointPolicyInputTypeDef,
-    StorageLensTagTypeDef,
-    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
-    S3ObjectOwnerOutputTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataOutputTypeDef,
     S3ObjectMetadataTypeDef,
-    S3GranteeOutputTypeDef,
     S3GranteeTypeDef,
-    S3ObjectLockLegalHoldOutputTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionOutputTypeDef,
     S3RetentionTypeDef,
-    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
-    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StorageLensAwsOrgOutputTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
-    ObjectLambdaContentTransformationOutputTypeDef,
+    DeleteMultiRegionAccessPointRequestRequestTypeDef,
+    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
     ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
@@ -531,125 +497,113 @@
     GetAccessPointPolicyResultTypeDef,
     GetBucketPolicyResultTypeDef,
     GetBucketResultTypeDef,
     GetBucketVersioningResultTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
-    PutPublicAccessBlockRequestRequestTypeDef,
     CreateAccessPointRequestRequestTypeDef,
+    GetAccessPointForObjectLambdaResultTypeDef,
+    GetAccessPointResultTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    PutPublicAccessBlockRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
+    GetBucketTaggingResultTypeDef,
+    GetJobTaggingResultTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     PutJobTaggingRequestRequestTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
     ReplicationRuleAndOperatorTypeDef,
+    S3SetObjectTaggingOperationOutputTypeDef,
     S3SetObjectTaggingOperationTypeDef,
     TaggingTypeDef,
-    GetAccessPointForObjectLambdaResultTypeDef,
-    GetAccessPointResultTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
     CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
-    DeleteMultiRegionAccessPointRequestRequestTypeDef,
     GeneratedManifestEncryptionOutputTypeDef,
     GeneratedManifestEncryptionTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
-    GetBucketTaggingResultTypeDef,
-    GetJobTaggingResultTypeDef,
-    LifecycleRuleAndOperatorOutputTypeDef,
-    ReplicationRuleAndOperatorOutputTypeDef,
-    S3SetObjectTaggingOperationOutputTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
+    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
+    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
-    MetricsOutputTypeDef,
-    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
-    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    PrefixLevelStorageMetricsOutputTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
-    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
-    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
-    S3GrantOutputTypeDef,
     S3GrantTypeDef,
-    S3SetObjectLegalHoldOperationOutputTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationOutputTypeDef,
     S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
-    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
     LifecycleRuleFilterTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
-    LifecycleRuleFilterOutputTypeDef,
-    ReplicationRuleFilterOutputTypeDef,
     JobListDescriptorTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
-    PrefixLevelOutputTypeDef,
     PrefixLevelTypeDef,
     S3AccessControlListOutputTypeDef,
-    S3CopyObjectOperationOutputTypeDef,
     S3AccessControlListTypeDef,
+    S3CopyObjectOperationOutputTypeDef,
     S3CopyObjectOperationTypeDef,
     S3BucketDestinationOutputTypeDef,
     S3BucketDestinationTypeDef,
     ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
+    LifecycleRuleOutputTypeDef,
     LifecycleRuleTypeDef,
     S3JobManifestGeneratorOutputTypeDef,
     S3JobManifestGeneratorTypeDef,
-    LifecycleRuleOutputTypeDef,
     ListJobsResultTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     AsyncOperationTypeDef,
-    BucketLevelOutputTypeDef,
     BucketLevelTypeDef,
     S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
     StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
     CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
+    GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
     JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
-    GetBucketLifecycleConfigurationResultTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
-    AccountLevelOutputTypeDef,
     AccountLevelTypeDef,
     S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
     StorageLensConfigurationOutputTypeDef,
@@ -660,15 +614,15 @@
     PutStorageLensConfigurationRequestRequestTypeDef,
     JobDescriptorTypeDef,
     CreateJobRequestRequestTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/SOURCES.txt` & `mypy-boto3-s3control-1.28.15/mypy_boto3_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.12/setup.py` & `mypy-boto3-s3control-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3control",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Control 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

