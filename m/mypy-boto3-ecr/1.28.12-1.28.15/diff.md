# Comparing `tmp/mypy-boto3-ecr-1.28.12.tar.gz` & `tmp/mypy-boto3-ecr-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-1.28.12.tar", last modified: Thu Jul 27 05:34:37 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
```

## Comparing `mypy-boto3-ecr-1.28.12.tar` & `mypy-boto3-ecr-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.788523 mypy-boto3-ecr-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20369 2023-07-27 05:34:37.780523 mypy-boto3-ecr-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.780523 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33677 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33621 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-27 05:21:28.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-27 05:21:28.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-27 05:21:29.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54739 2023-07-27 05:21:28.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.780523 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20369 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:37.788523 mypy-boto3-ecr-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.377035 mypy-boto3-ecr-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20107 2023-07-28 20:42:43.373035 mypy-boto3-ecr-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.361035 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33677 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33621 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52907 2023-07-28 20:24:45.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52832 2023-07-28 20:24:45.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-28 20:24:44.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.373035 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20107 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:43.000000 mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.377035 mypy-boto3-ecr-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:24:43.000000 mypy-boto3-ecr-1.28.15/setup.py
```

### Comparing `mypy-boto3-ecr-1.28.12/LICENSE` & `mypy-boto3-ecr-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/PKG-INFO` & `mypy-boto3-ecr-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.12
-Summary: Type annotations for boto3.ECR 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,140 +390,133 @@
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
-    ImageIdentifierOutputTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
-    ImageScanningConfigurationOutputTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
-    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
-    ScanningRepositoryFilterOutputTypeDef,
     ScanningRepositoryFilterTypeDef,
-    ReplicationDestinationOutputTypeDef,
     ReplicationDestinationTypeDef,
-    RepositoryFilterOutputTypeDef,
     RepositoryFilterTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
+    PutRegistryPolicyResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
-    StartImageScanRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
+    StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
+    PutImageScanningConfigurationResponseTypeDef,
+    RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
-    PutImageScanningConfigurationResponseTypeDef,
-    RepositoryTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     RegistryScanningRuleOutputTypeDef,
-    RepositoryScanningConfigurationTypeDef,
     RegistryScanningRuleTypeDef,
+    RepositoryScanningConfigurationTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
-    ScoreDetailsTypeDef,
-    DescribeImagesResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    ScoreDetailsTypeDef,
+    DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
     RegistryScanningConfigurationTypeDef,
-    BatchGetRepositoryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationRequestRequestTypeDef,
+    BatchGetRepositoryScanningConfigurationResponseTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     DescribeRegistryResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-ecr-1.28.12/README.md` & `mypy-boto3-ecr-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,140 +358,133 @@
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
-    ImageIdentifierOutputTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
-    ImageScanningConfigurationOutputTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
-    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
-    ScanningRepositoryFilterOutputTypeDef,
     ScanningRepositoryFilterTypeDef,
-    ReplicationDestinationOutputTypeDef,
     ReplicationDestinationTypeDef,
-    RepositoryFilterOutputTypeDef,
     RepositoryFilterTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
+    PutRegistryPolicyResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
-    StartImageScanRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
+    StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
+    PutImageScanningConfigurationResponseTypeDef,
+    RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
-    PutImageScanningConfigurationResponseTypeDef,
-    RepositoryTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     RegistryScanningRuleOutputTypeDef,
-    RepositoryScanningConfigurationTypeDef,
     RegistryScanningRuleTypeDef,
+    RepositoryScanningConfigurationTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
-    ScoreDetailsTypeDef,
-    DescribeImagesResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    ScoreDetailsTypeDef,
+    DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
     RegistryScanningConfigurationTypeDef,
-    BatchGetRepositoryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationRequestRequestTypeDef,
+    BatchGetRepositoryScanningConfigurationResponseTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     DescribeRegistryResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.py` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.pyi` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__main__.py` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECR 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ECR 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.py` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.pyi` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.py` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.pyi` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.py` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.py`

 * *Files 17% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
 
@@ -96,15 +96,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagespaginator)
         """
 
 
@@ -115,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
 
@@ -134,15 +134,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describerepositoriespaginator)
         """
 
 
@@ -155,15 +155,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
 
@@ -175,13 +175,13 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.pyi` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
 class DescribeImagesPaginator(Paginator):
@@ -92,15 +92,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagespaginator)
         """
 
 class DescribePullThroughCacheRulesPaginator(Paginator):
@@ -110,15 +110,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
 class DescribeRepositoriesPaginator(Paginator):
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describerepositoriespaginator)
         """
 
 class GetLifecyclePolicyPreviewPaginator(Paginator):
@@ -148,15 +148,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
 class ListImagesPaginator(Paginator):
@@ -167,13 +167,13 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.py` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -37,148 +37,140 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
-    "ImageIdentifierOutputTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
-    "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
-    "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleRequestRequestTypeDef",
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    "DeleteRegistryPolicyResponseTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "ImageReplicationStatusTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
-    "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
-    "GetLifecyclePolicyResponseTypeDef",
-    "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
-    "ImageScanningConfigurationOutputTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
-    "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
-    "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
-    "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
-    "ScanningRepositoryFilterOutputTypeDef",
     "ScanningRepositoryFilterTypeDef",
-    "ReplicationDestinationOutputTypeDef",
     "ReplicationDestinationTypeDef",
-    "RepositoryFilterOutputTypeDef",
     "RepositoryFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
-    "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
     "ImageScanFindingTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    "DeleteLifecyclePolicyResponseTypeDef",
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    "DeleteRegistryPolicyResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetDownloadUrlForLayerResponseTypeDef",
+    "GetLifecyclePolicyResponseTypeDef",
+    "GetRegistryPolicyResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "PutImageTagMutabilityResponseTypeDef",
+    "PutLifecyclePolicyResponseTypeDef",
+    "PutRegistryPolicyResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
-    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
-    "StartImageScanRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
+    "StartImageScanRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
+    "PutImageScanningConfigurationResponseTypeDef",
+    "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
+    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
-    "PutImageScanningConfigurationResponseTypeDef",
-    "RepositoryTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "RegistryScanningRuleOutputTypeDef",
-    "RepositoryScanningConfigurationTypeDef",
     "RegistryScanningRuleTypeDef",
+    "RepositoryScanningConfigurationTypeDef",
     "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
-    "ScoreDetailsTypeDef",
-    "DescribeImagesResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
+    "ScoreDetailsTypeDef",
+    "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
     "RegistryScanningConfigurationTypeDef",
-    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
     "DescribeRegistryResponseTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
@@ -197,19 +189,17 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
         "authorizationToken": str,
         "expiresAt": datetime,
         "proxyEndpoint": str,
     },
@@ -242,22 +232,20 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -271,25 +259,27 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
     },
     total=False,
 )
 
-ImageIdentifierTypeDef = TypedDict(
-    "ImageIdentifierTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "imageDigest": str,
-        "imageTag": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ImageIdentifierOutputTypeDef = TypedDict(
-    "ImageIdentifierOutputTypeDef",
+ImageIdentifierTypeDef = TypedDict(
+    "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
@@ -322,33 +312,20 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
     },
 )
@@ -356,54 +333,39 @@
     "_OptionalCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-
-CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "encryptionType": EncryptionTypeType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "kmsKey": str,
     },
     total=False,
 )
 
-
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
-
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "scanOnPush": bool,
     },
     total=False,
 )
@@ -447,107 +409,60 @@
     "_OptionalDeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteLifecyclePolicyResponseTypeDef = TypedDict(
-    "DeleteLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
     },
 )
 _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-
-DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRegistryPolicyResponseTypeDef = TypedDict(
-    "DeleteRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -555,32 +470,40 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 ImageReplicationStatusTypeDef = TypedDict(
     "ImageReplicationStatusTypeDef",
     {
         "region": str,
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -599,24 +522,14 @@
     "DescribeImagesFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
 
-DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    {
-        "registryId": str,
-        "ecrRepositoryPrefixes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePullThroughCacheRulesRequestRequestTypeDef = TypedDict(
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     {
         "registryId": str,
         "ecrRepositoryPrefixes": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -631,56 +544,25 @@
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "encryptionType": EncryptionTypeType,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "kmsKey": str,
-    },
-    total=False,
-)
-
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
-
 GetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "GetAuthorizationTokenRequestRequestTypeDef",
     {
         "registryIds": Sequence[str],
     },
     total=False,
 )
@@ -696,31 +578,20 @@
     "_OptionalGetDownloadUrlForLayerRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
-
-GetDownloadUrlForLayerResponseTypeDef = TypedDict(
-    "GetDownloadUrlForLayerResponseTypeDef",
-    {
-        "downloadUrl": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecyclePolicyPreviewFilterTypeDef = TypedDict(
     "LifecyclePolicyPreviewFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
@@ -743,123 +614,70 @@
     "_OptionalGetLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-GetLifecyclePolicyResponseTypeDef = TypedDict(
-    "GetLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistryPolicyResponseTypeDef = TypedDict(
-    "GetRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageScanFindingsSummaryTypeDef = TypedDict(
     "ImageScanFindingsSummaryTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
     },
     total=False,
 )
 
-ImageScanningConfigurationOutputTypeDef = TypedDict(
-    "ImageScanningConfigurationOutputTypeDef",
-    {
-        "scanOnPush": bool,
-    },
-    total=False,
-)
-
 _RequiredInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredInitiateLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecyclePolicyRuleActionTypeDef = TypedDict(
     "LifecyclePolicyRuleActionTypeDef",
     {
         "type": Literal["EXPIRE"],
     },
     total=False,
 )
@@ -875,23 +693,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 VulnerablePackageTypeDef = TypedDict(
     "VulnerablePackageTypeDef",
     {
         "arch": str,
         "epoch": int,
         "filePath": str,
         "name": str,
@@ -899,24 +708,14 @@
         "release": str,
         "sourceLayerHash": str,
         "version": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -927,21 +726,19 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
-
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutImageTagMutabilityRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageTagMutabilityRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
     },
 )
@@ -949,32 +746,20 @@
     "_OptionalPutImageTagMutabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
-
-PutImageTagMutabilityResponseTypeDef = TypedDict(
-    "PutImageTagMutabilityResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageTagMutability": ImageTagMutabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutLifecyclePolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "lifecyclePolicyText": str,
     },
 )
@@ -982,116 +767,60 @@
     "_OptionalPutLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-PutLifecyclePolicyResponseTypeDef = TypedDict(
-    "PutLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutRegistryPolicyRequestRequestTypeDef = TypedDict(
     "PutRegistryPolicyRequestRequestTypeDef",
     {
         "policyText": str,
     },
 )
 
-PutRegistryPolicyResponseTypeDef = TypedDict(
-    "PutRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "url": str,
         "text": str,
     },
     total=False,
 )
 
-ScanningRepositoryFilterOutputTypeDef = TypedDict(
-    "ScanningRepositoryFilterOutputTypeDef",
-    {
-        "filter": str,
-        "filterType": Literal["WILDCARD"],
-    },
-)
-
 ScanningRepositoryFilterTypeDef = TypedDict(
     "ScanningRepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["WILDCARD"],
     },
 )
 
-ReplicationDestinationOutputTypeDef = TypedDict(
-    "ReplicationDestinationOutputTypeDef",
-    {
-        "region": str,
-        "registryId": str,
-    },
-)
-
 ReplicationDestinationTypeDef = TypedDict(
     "ReplicationDestinationTypeDef",
     {
         "region": str,
         "registryId": str,
     },
 )
 
-RepositoryFilterOutputTypeDef = TypedDict(
-    "RepositoryFilterOutputTypeDef",
-    {
-        "filter": str,
-        "filterType": Literal["PREFIX_MATCH"],
-    },
-)
-
 RepositoryFilterTypeDef = TypedDict(
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
     },
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -1100,32 +829,20 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1133,33 +850,20 @@
     {
         "registryId": str,
         "lifecyclePolicyText": str,
     },
     total=False,
 )
 
-
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
-
-StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
-    "StartLifecyclePolicyPreviewResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "status": LifecyclePolicyPreviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1178,66 +882,225 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
-
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "name": str,
         "description": str,
         "uri": str,
         "severity": FindingSeverityType,
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-GetAuthorizationTokenResponseTypeDef = TypedDict(
-    "GetAuthorizationTokenResponseTypeDef",
-    {
-        "authorizationData": List[AuthorizationDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
     },
     total=False,
 )
 
 BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
     "BatchCheckLayerAvailabilityResponseTypeDef",
     {
         "layers": List[LayerTypeDef],
         "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLifecyclePolicyResponseTypeDef = TypedDict(
+    "DeleteLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRegistryPolicyResponseTypeDef = TypedDict(
+    "DeleteRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizationTokenResponseTypeDef = TypedDict(
+    "GetAuthorizationTokenResponseTypeDef",
+    {
+        "authorizationData": List[AuthorizationDataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDownloadUrlForLayerResponseTypeDef = TypedDict(
+    "GetDownloadUrlForLayerResponseTypeDef",
+    {
+        "downloadUrl": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLifecyclePolicyResponseTypeDef = TypedDict(
+    "GetLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistryPolicyResponseTypeDef = TypedDict(
+    "GetRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImageTagMutabilityResponseTypeDef = TypedDict(
+    "PutImageTagMutabilityResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageTagMutability": ImageTagMutabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLifecyclePolicyResponseTypeDef = TypedDict(
+    "PutLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRegistryPolicyResponseTypeDef = TypedDict(
+    "PutRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "status": LifecyclePolicyPreviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1248,21 +1111,19 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBatchGetImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
@@ -1271,21 +1132,19 @@
     {
         "registryId": str,
         "acceptedMediaTypes": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchGetImageRequestRequestTypeDef(
     _RequiredBatchGetImageRequestRequestTypeDef, _OptionalBatchGetImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeImageReplicationStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1293,46 +1152,20 @@
     "_OptionalDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
-    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1342,74 +1175,70 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeImageScanFindingsRequestRequestTypeDef(
     _RequiredDescribeImageScanFindingsRequestRequestTypeDef,
     _OptionalDescribeImageScanFindingsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImageScanRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImageScanRequestRequestTypeDef",
-    {
-        "registryId": str,
-    },
-    total=False,
-)
-
-
-class StartImageScanRequestRequestTypeDef(
-    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
-):
-    pass
-
-
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierOutputTypeDef],
+        "imageIds": List[ImageIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImageScanRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
     },
 )
+_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImageScanRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+class StartImageScanRequestRequestTypeDef(
+    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
+):
+    pass
 
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
@@ -1418,21 +1247,44 @@
     "_OptionalPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutImageScanningConfigurationRequestRequestTypeDef(
     _RequiredPutImageScanningConfigurationRequestRequestTypeDef,
     _OptionalPutImageScanningConfigurationRequestRequestTypeDef,
 ):
     pass
 
+PutImageScanningConfigurationResponseTypeDef = TypedDict(
+    "PutImageScanningConfigurationResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
+    {
+        "repositoryArn": str,
+        "registryId": str,
+        "repositoryName": str,
+        "repositoryUri": str,
+        "createdAt": datetime,
+        "imageTagMutability": ImageTagMutabilityType,
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "encryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -1444,20 +1296,26 @@
         "imageTagMutability": ImageTagMutabilityType,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -1475,20 +1333,62 @@
     total=False,
 )
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
+    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+):
+    pass
+
+DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    {
+        "registryId": str,
+        "ecrRepositoryPrefixes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1499,30 +1399,28 @@
         "nextToken": str,
         "maxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef(
     _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     _OptionalDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
 ):
     pass
 
-
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1530,27 +1428,25 @@
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -1561,27 +1457,25 @@
         "nextToken": str,
         "maxResults": int,
         "filter": DescribeImagesFilterTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
-
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1589,27 +1483,25 @@
 )
 _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
@@ -1621,22 +1513,20 @@
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1647,22 +1537,20 @@
         "nextToken": str,
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
-
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -1673,39 +1561,14 @@
         "imageManifestMediaType": str,
         "artifactMediaType": str,
         "lastRecordedPullTime": datetime,
     },
     total=False,
 )
 
-PutImageScanningConfigurationResponseTypeDef = TypedDict(
-    "PutImageScanningConfigurationResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RepositoryTypeDef = TypedDict(
-    "RepositoryTypeDef",
-    {
-        "repositoryArn": str,
-        "registryId": str,
-        "repositoryName": str,
-        "repositoryUri": str,
-        "createdAt": datetime,
-        "imageTagMutability": ImageTagMutabilityType,
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-        "encryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 LifecyclePolicyPreviewResultTypeDef = TypedDict(
     "LifecyclePolicyPreviewResultTypeDef",
     {
         "imageTags": List[str],
         "imageDigest": str,
         "imagePushedAt": datetime,
         "action": LifecyclePolicyRuleActionTypeDef,
@@ -1721,27 +1584,25 @@
     },
 )
 _OptionalListImagesRequestListImagesPaginateTypeDef = TypedDict(
     "_OptionalListImagesRequestListImagesPaginateTypeDef",
     {
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
     _OptionalListImagesRequestListImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListImagesRequestRequestTypeDef = TypedDict(
@@ -1751,29 +1612,19 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListImagesFilterTypeDef,
     },
     total=False,
 )
 
-
 class ListImagesRequestRequestTypeDef(
     _RequiredListImagesRequestRequestTypeDef, _OptionalListImagesRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PackageVulnerabilityDetailsTypeDef = TypedDict(
     "PackageVulnerabilityDetailsTypeDef",
     {
         "cvss": List[CvssScoreTypeDef],
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
         "source": str,
@@ -1795,198 +1646,194 @@
     total=False,
 )
 
 RegistryScanningRuleOutputTypeDef = TypedDict(
     "RegistryScanningRuleOutputTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterOutputTypeDef],
+        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+    },
+)
+
+RegistryScanningRuleTypeDef = TypedDict(
+    "RegistryScanningRuleTypeDef",
+    {
+        "scanFrequency": ScanFrequencyType,
+        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
         "repositoryName": str,
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
-        "appliedScanFilters": List[ScanningRepositoryFilterOutputTypeDef],
+        "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
     },
     total=False,
 )
 
-RegistryScanningRuleTypeDef = TypedDict(
-    "RegistryScanningRuleTypeDef",
-    {
-        "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
-    },
-)
-
 _RequiredReplicationRuleOutputTypeDef = TypedDict(
     "_RequiredReplicationRuleOutputTypeDef",
     {
-        "destinations": List[ReplicationDestinationOutputTypeDef],
+        "destinations": List[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleOutputTypeDef = TypedDict(
     "_OptionalReplicationRuleOutputTypeDef",
     {
-        "repositoryFilters": List[RepositoryFilterOutputTypeDef],
+        "repositoryFilters": List[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
-
 class ReplicationRuleOutputTypeDef(
     _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
 ):
     pass
 
-
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "destinations": Sequence[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
         "repositoryFilters": Sequence[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
-
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "details": ResourceDetailsTypeDef,
         "id": str,
         "tags": Dict[str, str],
         "type": str,
     },
     total=False,
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierOutputTypeDef],
+        "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
     {
         "images": List[ImageTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ScoreDetailsTypeDef = TypedDict(
-    "ScoreDetailsTypeDef",
-    {
-        "cvss": CvssScoreDetailsTypeDef,
-    },
-    total=False,
-)
-
-DescribeImagesResponseTypeDef = TypedDict(
-    "DescribeImagesResponseTypeDef",
-    {
-        "imageDetails": List[ImageDetailTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScoreDetailsTypeDef = TypedDict(
+    "ScoreDetailsTypeDef",
+    {
+        "cvss": CvssScoreDetailsTypeDef,
+    },
+    total=False,
+)
+
+DescribeImagesResponseTypeDef = TypedDict(
+    "DescribeImagesResponseTypeDef",
+    {
+        "imageDetails": List[ImageDetailTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
         "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
-BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
-    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
-    {
-        "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
-        "failures": List[RepositoryScanningConfigurationFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
     {
         "scanType": ScanTypeType,
         "rules": Sequence[RegistryScanningRuleTypeDef],
     },
     total=False,
 )
 
+BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
+    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
+    {
+        "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
+        "failures": List[RepositoryScanningConfigurationFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ReplicationConfigurationOutputTypeDef = TypedDict(
     "ReplicationConfigurationOutputTypeDef",
     {
         "rules": List[ReplicationRuleOutputTypeDef],
     },
 )
 
@@ -2020,40 +1867,40 @@
 )
 
 GetRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "GetRegistryScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "scanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
         "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReplicationConfigurationResponseTypeDef = TypedDict(
     "PutReplicationConfigurationResponseTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
@@ -2073,14 +1920,14 @@
 )
 
 DescribeImageScanFindingsResponseTypeDef = TypedDict(
     "DescribeImageScanFindingsResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.pyi` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,147 +37,141 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
-    "ImageIdentifierOutputTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
-    "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
-    "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleRequestRequestTypeDef",
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    "DeleteRegistryPolicyResponseTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "ImageReplicationStatusTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
-    "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
-    "GetLifecyclePolicyResponseTypeDef",
-    "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
-    "ImageScanningConfigurationOutputTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
-    "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
-    "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
-    "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
-    "ScanningRepositoryFilterOutputTypeDef",
     "ScanningRepositoryFilterTypeDef",
-    "ReplicationDestinationOutputTypeDef",
     "ReplicationDestinationTypeDef",
-    "RepositoryFilterOutputTypeDef",
     "RepositoryFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
-    "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
     "ImageScanFindingTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    "DeleteLifecyclePolicyResponseTypeDef",
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    "DeleteRegistryPolicyResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetDownloadUrlForLayerResponseTypeDef",
+    "GetLifecyclePolicyResponseTypeDef",
+    "GetRegistryPolicyResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "PutImageTagMutabilityResponseTypeDef",
+    "PutLifecyclePolicyResponseTypeDef",
+    "PutRegistryPolicyResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
-    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
-    "StartImageScanRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
+    "StartImageScanRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
+    "PutImageScanningConfigurationResponseTypeDef",
+    "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
+    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
-    "PutImageScanningConfigurationResponseTypeDef",
-    "RepositoryTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "RegistryScanningRuleOutputTypeDef",
-    "RepositoryScanningConfigurationTypeDef",
     "RegistryScanningRuleTypeDef",
+    "RepositoryScanningConfigurationTypeDef",
     "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
-    "ScoreDetailsTypeDef",
-    "DescribeImagesResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
+    "ScoreDetailsTypeDef",
+    "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
     "RegistryScanningConfigurationTypeDef",
-    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
     "DescribeRegistryResponseTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
@@ -196,17 +190,19 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
         "authorizationToken": str,
         "expiresAt": datetime,
         "proxyEndpoint": str,
     },
@@ -239,20 +235,22 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
+
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -266,25 +264,27 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
     },
     total=False,
 )
 
-ImageIdentifierTypeDef = TypedDict(
-    "ImageIdentifierTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "imageDigest": str,
-        "imageTag": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ImageIdentifierOutputTypeDef = TypedDict(
-    "ImageIdentifierOutputTypeDef",
+ImageIdentifierTypeDef = TypedDict(
+    "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
@@ -317,30 +317,21 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
     },
@@ -349,30 +340,21 @@
     "_OptionalCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "encryptionType": EncryptionTypeType,
     },
 )
@@ -380,19 +362,21 @@
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "kmsKey": str,
     },
     total=False,
 )
 
+
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
+
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "scanOnPush": bool,
     },
     total=False,
 )
@@ -436,30 +420,21 @@
     "_OptionalDeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteLifecyclePolicyResponseTypeDef = TypedDict(
-    "DeleteLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
     },
 )
@@ -467,39 +442,21 @@
     "_OptionalDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRegistryPolicyResponseTypeDef = TypedDict(
-    "DeleteRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -507,29 +464,21 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -538,30 +487,42 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 ImageReplicationStatusTypeDef = TypedDict(
     "ImageReplicationStatusTypeDef",
     {
         "region": str,
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -580,24 +541,14 @@
     "DescribeImagesFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
 
-DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    {
-        "registryId": str,
-        "ecrRepositoryPrefixes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePullThroughCacheRulesRequestRequestTypeDef = TypedDict(
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     {
         "registryId": str,
         "ecrRepositoryPrefixes": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -612,54 +563,25 @@
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "encryptionType": EncryptionTypeType,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "kmsKey": str,
-    },
-    total=False,
-)
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
 GetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "GetAuthorizationTokenRequestRequestTypeDef",
     {
         "registryIds": Sequence[str],
     },
     total=False,
 )
@@ -675,28 +597,21 @@
     "_OptionalGetDownloadUrlForLayerRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
-GetDownloadUrlForLayerResponseTypeDef = TypedDict(
-    "GetDownloadUrlForLayerResponseTypeDef",
-    {
-        "downloadUrl": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 LifecyclePolicyPreviewFilterTypeDef = TypedDict(
     "LifecyclePolicyPreviewFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
@@ -720,39 +635,21 @@
     "_OptionalGetLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-GetLifecyclePolicyResponseTypeDef = TypedDict(
-    "GetLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistryPolicyResponseTypeDef = TypedDict(
-    "GetRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -760,76 +657,53 @@
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ImageScanFindingsSummaryTypeDef = TypedDict(
     "ImageScanFindingsSummaryTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
     },
     total=False,
 )
 
-ImageScanningConfigurationOutputTypeDef = TypedDict(
-    "ImageScanningConfigurationOutputTypeDef",
-    {
-        "scanOnPush": bool,
-    },
-    total=False,
-)
-
 _RequiredInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredInitiateLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 LifecyclePolicyRuleActionTypeDef = TypedDict(
     "LifecyclePolicyRuleActionTypeDef",
     {
         "type": Literal["EXPIRE"],
     },
     total=False,
@@ -846,23 +720,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 VulnerablePackageTypeDef = TypedDict(
     "VulnerablePackageTypeDef",
     {
         "arch": str,
         "epoch": int,
         "filePath": str,
         "name": str,
@@ -870,24 +735,14 @@
         "release": str,
         "sourceLayerHash": str,
         "version": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -898,19 +753,21 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
+
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutImageTagMutabilityRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageTagMutabilityRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
     },
 )
@@ -918,29 +775,21 @@
     "_OptionalPutImageTagMutabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
-PutImageTagMutabilityResponseTypeDef = TypedDict(
-    "PutImageTagMutabilityResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageTagMutability": ImageTagMutabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredPutLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutLifecyclePolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "lifecyclePolicyText": str,
     },
@@ -949,114 +798,62 @@
     "_OptionalPutLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-PutLifecyclePolicyResponseTypeDef = TypedDict(
-    "PutLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 PutRegistryPolicyRequestRequestTypeDef = TypedDict(
     "PutRegistryPolicyRequestRequestTypeDef",
     {
         "policyText": str,
     },
 )
 
-PutRegistryPolicyResponseTypeDef = TypedDict(
-    "PutRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "url": str,
         "text": str,
     },
     total=False,
 )
 
-ScanningRepositoryFilterOutputTypeDef = TypedDict(
-    "ScanningRepositoryFilterOutputTypeDef",
-    {
-        "filter": str,
-        "filterType": Literal["WILDCARD"],
-    },
-)
-
 ScanningRepositoryFilterTypeDef = TypedDict(
     "ScanningRepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["WILDCARD"],
     },
 )
 
-ReplicationDestinationOutputTypeDef = TypedDict(
-    "ReplicationDestinationOutputTypeDef",
-    {
-        "region": str,
-        "registryId": str,
-    },
-)
-
 ReplicationDestinationTypeDef = TypedDict(
     "ReplicationDestinationTypeDef",
     {
         "region": str,
         "registryId": str,
     },
 )
 
-RepositoryFilterOutputTypeDef = TypedDict(
-    "RepositoryFilterOutputTypeDef",
-    {
-        "filter": str,
-        "filterType": Literal["PREFIX_MATCH"],
-    },
-)
-
 RepositoryFilterTypeDef = TypedDict(
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
     },
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -1065,29 +862,21 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -1096,30 +885,21 @@
     {
         "registryId": str,
         "lifecyclePolicyText": str,
     },
     total=False,
 )
 
+
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
-StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
-    "StartLifecyclePolicyPreviewResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "status": LifecyclePolicyPreviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -1139,64 +919,227 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "name": str,
         "description": str,
         "uri": str,
         "severity": FindingSeverityType,
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-GetAuthorizationTokenResponseTypeDef = TypedDict(
-    "GetAuthorizationTokenResponseTypeDef",
-    {
-        "authorizationData": List[AuthorizationDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
     },
     total=False,
 )
 
 BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
     "BatchCheckLayerAvailabilityResponseTypeDef",
     {
         "layers": List[LayerTypeDef],
         "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLifecyclePolicyResponseTypeDef = TypedDict(
+    "DeleteLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRegistryPolicyResponseTypeDef = TypedDict(
+    "DeleteRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizationTokenResponseTypeDef = TypedDict(
+    "GetAuthorizationTokenResponseTypeDef",
+    {
+        "authorizationData": List[AuthorizationDataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDownloadUrlForLayerResponseTypeDef = TypedDict(
+    "GetDownloadUrlForLayerResponseTypeDef",
+    {
+        "downloadUrl": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLifecyclePolicyResponseTypeDef = TypedDict(
+    "GetLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistryPolicyResponseTypeDef = TypedDict(
+    "GetRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImageTagMutabilityResponseTypeDef = TypedDict(
+    "PutImageTagMutabilityResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageTagMutability": ImageTagMutabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLifecyclePolicyResponseTypeDef = TypedDict(
+    "PutLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRegistryPolicyResponseTypeDef = TypedDict(
+    "PutRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "status": LifecyclePolicyPreviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1207,19 +1150,21 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBatchGetImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
@@ -1228,19 +1173,21 @@
     {
         "registryId": str,
         "acceptedMediaTypes": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchGetImageRequestRequestTypeDef(
     _RequiredBatchGetImageRequestRequestTypeDef, _OptionalBatchGetImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeImageReplicationStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1248,41 +1195,21 @@
     "_OptionalDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
-    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
@@ -1293,70 +1220,74 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeImageScanFindingsRequestRequestTypeDef(
     _RequiredDescribeImageScanFindingsRequestRequestTypeDef,
     _OptionalDescribeImageScanFindingsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImageScanRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImageScanRequestRequestTypeDef",
-    {
-        "registryId": str,
-    },
-    total=False,
-)
-
-class StartImageScanRequestRequestTypeDef(
-    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
-):
-    pass
 
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierOutputTypeDef],
+        "imageIds": List[ImageIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImageScanRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
     },
 )
+_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImageScanRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+
+class StartImageScanRequestRequestTypeDef(
+    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
@@ -1365,20 +1296,47 @@
     "_OptionalPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutImageScanningConfigurationRequestRequestTypeDef(
     _RequiredPutImageScanningConfigurationRequestRequestTypeDef,
     _OptionalPutImageScanningConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
+PutImageScanningConfigurationResponseTypeDef = TypedDict(
+    "PutImageScanningConfigurationResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
+    {
+        "repositoryArn": str,
+        "registryId": str,
+        "repositoryName": str,
+        "repositoryUri": str,
+        "createdAt": datetime,
+        "imageTagMutability": ImageTagMutabilityType,
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "encryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
@@ -1389,19 +1347,29 @@
         "imageTagMutability": ImageTagMutabilityType,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1418,20 +1386,64 @@
     total=False,
 )
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
+    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+):
+    pass
+
+
+DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    {
+        "registryId": str,
+        "ecrRepositoryPrefixes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1442,28 +1454,30 @@
         "nextToken": str,
         "maxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef(
     _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     _OptionalDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
 ):
     pass
 
+
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1471,25 +1485,27 @@
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -1500,25 +1516,27 @@
         "nextToken": str,
         "maxResults": int,
         "filter": DescribeImagesFilterTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
+
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1526,25 +1544,27 @@
 )
 _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
@@ -1556,20 +1576,22 @@
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1580,20 +1602,22 @@
         "nextToken": str,
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
+
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -1604,39 +1628,14 @@
         "imageManifestMediaType": str,
         "artifactMediaType": str,
         "lastRecordedPullTime": datetime,
     },
     total=False,
 )
 
-PutImageScanningConfigurationResponseTypeDef = TypedDict(
-    "PutImageScanningConfigurationResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RepositoryTypeDef = TypedDict(
-    "RepositoryTypeDef",
-    {
-        "repositoryArn": str,
-        "registryId": str,
-        "repositoryName": str,
-        "repositoryUri": str,
-        "createdAt": datetime,
-        "imageTagMutability": ImageTagMutabilityType,
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-        "encryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 LifecyclePolicyPreviewResultTypeDef = TypedDict(
     "LifecyclePolicyPreviewResultTypeDef",
     {
         "imageTags": List[str],
         "imageDigest": str,
         "imagePushedAt": datetime,
         "action": LifecyclePolicyRuleActionTypeDef,
@@ -1652,25 +1651,27 @@
     },
 )
 _OptionalListImagesRequestListImagesPaginateTypeDef = TypedDict(
     "_OptionalListImagesRequestListImagesPaginateTypeDef",
     {
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
     _OptionalListImagesRequestListImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListImagesRequestRequestTypeDef = TypedDict(
@@ -1680,26 +1681,20 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListImagesFilterTypeDef,
     },
     total=False,
 )
 
+
 class ListImagesRequestRequestTypeDef(
     _RequiredListImagesRequestRequestTypeDef, _OptionalListImagesRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 PackageVulnerabilityDetailsTypeDef = TypedDict(
     "PackageVulnerabilityDetailsTypeDef",
     {
         "cvss": List[CvssScoreTypeDef],
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
@@ -1722,194 +1717,198 @@
     total=False,
 )
 
 RegistryScanningRuleOutputTypeDef = TypedDict(
     "RegistryScanningRuleOutputTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterOutputTypeDef],
+        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+    },
+)
+
+RegistryScanningRuleTypeDef = TypedDict(
+    "RegistryScanningRuleTypeDef",
+    {
+        "scanFrequency": ScanFrequencyType,
+        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
         "repositoryName": str,
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
-        "appliedScanFilters": List[ScanningRepositoryFilterOutputTypeDef],
+        "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
     },
     total=False,
 )
 
-RegistryScanningRuleTypeDef = TypedDict(
-    "RegistryScanningRuleTypeDef",
-    {
-        "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
-    },
-)
-
 _RequiredReplicationRuleOutputTypeDef = TypedDict(
     "_RequiredReplicationRuleOutputTypeDef",
     {
-        "destinations": List[ReplicationDestinationOutputTypeDef],
+        "destinations": List[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleOutputTypeDef = TypedDict(
     "_OptionalReplicationRuleOutputTypeDef",
     {
-        "repositoryFilters": List[RepositoryFilterOutputTypeDef],
+        "repositoryFilters": List[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
+
 class ReplicationRuleOutputTypeDef(
     _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
 ):
     pass
 
+
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "destinations": Sequence[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
         "repositoryFilters": Sequence[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
+
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "details": ResourceDetailsTypeDef,
         "id": str,
         "tags": Dict[str, str],
         "type": str,
     },
     total=False,
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierOutputTypeDef],
+        "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
     {
         "images": List[ImageTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ScoreDetailsTypeDef = TypedDict(
-    "ScoreDetailsTypeDef",
-    {
-        "cvss": CvssScoreDetailsTypeDef,
-    },
-    total=False,
-)
-
-DescribeImagesResponseTypeDef = TypedDict(
-    "DescribeImagesResponseTypeDef",
-    {
-        "imageDetails": List[ImageDetailTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScoreDetailsTypeDef = TypedDict(
+    "ScoreDetailsTypeDef",
+    {
+        "cvss": CvssScoreDetailsTypeDef,
+    },
+    total=False,
+)
+
+DescribeImagesResponseTypeDef = TypedDict(
+    "DescribeImagesResponseTypeDef",
+    {
+        "imageDetails": List[ImageDetailTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
         "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
-BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
-    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
-    {
-        "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
-        "failures": List[RepositoryScanningConfigurationFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
     {
         "scanType": ScanTypeType,
         "rules": Sequence[RegistryScanningRuleTypeDef],
     },
     total=False,
 )
 
+BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
+    "BatchGetRepositoryScanningConfigurationResponseTypeDef",
+    {
+        "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
+        "failures": List[RepositoryScanningConfigurationFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ReplicationConfigurationOutputTypeDef = TypedDict(
     "ReplicationConfigurationOutputTypeDef",
     {
         "rules": List[ReplicationRuleOutputTypeDef],
     },
 )
 
@@ -1943,40 +1942,40 @@
 )
 
 GetRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "GetRegistryScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "scanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
         "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReplicationConfigurationResponseTypeDef = TypedDict(
     "PutReplicationConfigurationResponseTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
@@ -1996,14 +1995,14 @@
 )
 
 DescribeImageScanFindingsResponseTypeDef = TypedDict(
     "DescribeImageScanFindingsResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierOutputTypeDef,
+        "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.py` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.pyi` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/PKG-INFO` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.12
-Summary: Type annotations for boto3.ECR 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,140 +390,133 @@
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
-    ImageIdentifierOutputTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
-    ImageScanningConfigurationOutputTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
-    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
-    ScanningRepositoryFilterOutputTypeDef,
     ScanningRepositoryFilterTypeDef,
-    ReplicationDestinationOutputTypeDef,
     ReplicationDestinationTypeDef,
-    RepositoryFilterOutputTypeDef,
     RepositoryFilterTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
+    PutRegistryPolicyResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
-    StartImageScanRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
+    StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
+    PutImageScanningConfigurationResponseTypeDef,
+    RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
-    PutImageScanningConfigurationResponseTypeDef,
-    RepositoryTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     RegistryScanningRuleOutputTypeDef,
-    RepositoryScanningConfigurationTypeDef,
     RegistryScanningRuleTypeDef,
+    RepositoryScanningConfigurationTypeDef,
     ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
-    ScoreDetailsTypeDef,
-    DescribeImagesResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
+    ScoreDetailsTypeDef,
+    DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
     RegistryScanningConfigurationTypeDef,
-    BatchGetRepositoryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationRequestRequestTypeDef,
+    BatchGetRepositoryScanningConfigurationResponseTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     DescribeRegistryResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/SOURCES.txt` & `mypy-boto3-ecr-1.28.15/mypy_boto3_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.12/setup.py` & `mypy-boto3-ecr-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECR 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ECR 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

