# Comparing `tmp/mypy-boto3-cloudfront-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudfront-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudfront-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudfront-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
```

## Comparing `mypy-boto3-cloudfront-1.28.12.tar` & `mypy-boto3-cloudfront-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34787 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33288 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79436 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79316 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   186569 2023-07-27 05:18:42.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   186182 2023-07-27 05:18:40.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34787 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31719 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79465 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79345 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   172819 2023-07-28 19:47:01.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172458 2023-07-28 19:46:59.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudfront-1.28.12/LICENSE` & `mypy-boto3-cloudfront-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.12/PKG-INFO` & `mypy-boto3-cloudfront-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-cloudfront
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudFront 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -422,34 +390,29 @@
     TrustedSignersTypeDef,
     CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
     QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
-    CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
-    ContentTypeProfileOutputTypeDef,
     ContentTypeProfileTypeDef,
     StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
-    ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
-    SessionStickinessConfigOutputTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
-    CustomErrorResponseOutputTypeDef,
     CustomErrorResponseTypeDef,
-    OriginCustomHeaderOutputTypeDef,
     OriginCustomHeaderTypeDef,
     OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
@@ -461,29 +424,23 @@
     DeleteOriginAccessControlRequestRequestTypeDef,
     DeleteOriginRequestPolicyRequestRequestTypeDef,
     DeletePublicKeyRequestRequestTypeDef,
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
-    LoggingConfigOutputTypeDef,
-    ViewerCertificateOutputTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
-    EmptyResponseMetadataTypeDef,
     FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
-    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
     QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
-    FunctionAssociationOutputTypeDef,
     FunctionAssociationTypeDef,
-    FunctionConfigOutputTypeDef,
     FunctionMetadataTypeDef,
     GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
@@ -493,115 +450,89 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
-    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
     KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
-    OriginAccessControlConfigOutputTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
-    PublicKeyConfigOutputTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
     PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
-    LambdaFunctionAssociationOutputTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RealtimeMetricsSubscriptionConfigOutputTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
     StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
-    OriginGroupMemberOutputTypeDef,
     OriginGroupMemberTypeDef,
-    OriginShieldOutputTypeDef,
-    S3OriginConfigOutputTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
-    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
-    QueryArgProfileOutputTypeDef,
     QueryArgProfileTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
-    ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
-    ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
-    ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
-    ResponseHeadersPolicyCustomHeaderOutputTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
-    ResponseHeadersPolicyFrameOptionsOutputTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
-    ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
-    ResponseHeadersPolicyRemoveHeaderOutputTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
-    ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-    ResponseHeadersPolicyXSSProtectionOutputTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
-    ResponseMetadataTypeDef,
-    S3OriginOutputTypeDef,
     S3OriginTypeDef,
-    StreamingLoggingConfigOutputTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
     CachePolicyCookiesConfigOutputTypeDef,
     CookiePreferenceOutputTypeDef,
@@ -614,67 +545,70 @@
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
     CachePolicyQueryStringsConfigOutputTypeDef,
     OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
     ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
-    ContinuousDeploymentSingleWeightConfigOutputTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
+    GetOriginAccessControlConfigResultTypeDef,
+    OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
+    GetPublicKeyConfigResultTypeDef,
+    PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
     CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
     CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
     CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
     EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
-    EndPointOutputTypeDef,
     EndPointTypeDef,
     FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
     RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     GetKeyGroupConfigResultTypeDef,
     KeyGroupTypeDef,
-    GetOriginAccessControlConfigResultTypeDef,
-    OriginAccessControlTypeDef,
-    GetPublicKeyConfigResultTypeDef,
-    PublicKeyTypeDef,
     InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
-    MonitoringSubscriptionOutputTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
     OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
     OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
@@ -682,15 +616,14 @@
     QueryArgProfilesTypeDef,
     ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
-    ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
     StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagsOutputTypeDef,
     TagsTypeDef,
@@ -703,47 +636,46 @@
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
-    TrafficConfigOutputTypeDef,
     TrafficConfigTypeDef,
+    CreateOriginAccessControlResultTypeDef,
+    GetOriginAccessControlResultTypeDef,
+    UpdateOriginAccessControlResultTypeDef,
+    CreatePublicKeyResultTypeDef,
+    GetPublicKeyResultTypeDef,
+    UpdatePublicKeyResultTypeDef,
     OriginOutputTypeDef,
     OriginTypeDef,
     EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
-    RealtimeLogConfigTypeDef,
     CreateRealtimeLogConfigRequestRequestTypeDef,
+    RealtimeLogConfigTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
     CreateKeyGroupResultTypeDef,
     GetKeyGroupResultTypeDef,
     KeyGroupSummaryTypeDef,
     UpdateKeyGroupResultTypeDef,
-    CreateOriginAccessControlResultTypeDef,
-    GetOriginAccessControlResultTypeDef,
-    UpdateOriginAccessControlResultTypeDef,
-    CreatePublicKeyResultTypeDef,
-    GetPublicKeyResultTypeDef,
-    UpdatePublicKeyResultTypeDef,
     InvalidationTypeDef,
     CreateInvalidationRequestRequestTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
+    CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
-    CreateMonitoringSubscriptionRequestRequestTypeDef,
     ListOriginAccessControlsResultTypeDef,
     OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
     QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
     ResponseHeadersPolicyConfigOutputTypeDef,
```

### Comparing `mypy-boto3-cloudfront-1.28.12/README.md` & `mypy-boto3-cloudfront-1.28.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-cloudfront
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,34 +422,29 @@
     TrustedSignersTypeDef,
     CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
     QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
-    CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
-    ContentTypeProfileOutputTypeDef,
     ContentTypeProfileTypeDef,
     StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
-    ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
-    SessionStickinessConfigOutputTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
-    CustomErrorResponseOutputTypeDef,
     CustomErrorResponseTypeDef,
-    OriginCustomHeaderOutputTypeDef,
     OriginCustomHeaderTypeDef,
     OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
@@ -429,29 +456,23 @@
     DeleteOriginAccessControlRequestRequestTypeDef,
     DeleteOriginRequestPolicyRequestRequestTypeDef,
     DeletePublicKeyRequestRequestTypeDef,
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
-    LoggingConfigOutputTypeDef,
-    ViewerCertificateOutputTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
-    EmptyResponseMetadataTypeDef,
     FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
-    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
     QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
-    FunctionAssociationOutputTypeDef,
     FunctionAssociationTypeDef,
-    FunctionConfigOutputTypeDef,
     FunctionMetadataTypeDef,
     GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
@@ -461,115 +482,89 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
-    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
     KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
-    OriginAccessControlConfigOutputTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
-    PublicKeyConfigOutputTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
     PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
-    LambdaFunctionAssociationOutputTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RealtimeMetricsSubscriptionConfigOutputTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
     StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
-    OriginGroupMemberOutputTypeDef,
     OriginGroupMemberTypeDef,
-    OriginShieldOutputTypeDef,
-    S3OriginConfigOutputTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
-    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
-    QueryArgProfileOutputTypeDef,
     QueryArgProfileTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
-    ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
-    ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
-    ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
-    ResponseHeadersPolicyCustomHeaderOutputTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
-    ResponseHeadersPolicyFrameOptionsOutputTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
-    ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
-    ResponseHeadersPolicyRemoveHeaderOutputTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
-    ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-    ResponseHeadersPolicyXSSProtectionOutputTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
-    ResponseMetadataTypeDef,
-    S3OriginOutputTypeDef,
     S3OriginTypeDef,
-    StreamingLoggingConfigOutputTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
     CachePolicyCookiesConfigOutputTypeDef,
     CookiePreferenceOutputTypeDef,
@@ -582,67 +577,70 @@
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
     CachePolicyQueryStringsConfigOutputTypeDef,
     OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
     ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
-    ContinuousDeploymentSingleWeightConfigOutputTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
+    GetOriginAccessControlConfigResultTypeDef,
+    OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
+    GetPublicKeyConfigResultTypeDef,
+    PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
     CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
     CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
     CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
     EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
-    EndPointOutputTypeDef,
     EndPointTypeDef,
     FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
     RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     GetKeyGroupConfigResultTypeDef,
     KeyGroupTypeDef,
-    GetOriginAccessControlConfigResultTypeDef,
-    OriginAccessControlTypeDef,
-    GetPublicKeyConfigResultTypeDef,
-    PublicKeyTypeDef,
     InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
-    MonitoringSubscriptionOutputTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
     OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
     OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
@@ -650,15 +648,14 @@
     QueryArgProfilesTypeDef,
     ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
-    ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
     StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagsOutputTypeDef,
     TagsTypeDef,
@@ -671,47 +668,46 @@
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
-    TrafficConfigOutputTypeDef,
     TrafficConfigTypeDef,
+    CreateOriginAccessControlResultTypeDef,
+    GetOriginAccessControlResultTypeDef,
+    UpdateOriginAccessControlResultTypeDef,
+    CreatePublicKeyResultTypeDef,
+    GetPublicKeyResultTypeDef,
+    UpdatePublicKeyResultTypeDef,
     OriginOutputTypeDef,
     OriginTypeDef,
     EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
-    RealtimeLogConfigTypeDef,
     CreateRealtimeLogConfigRequestRequestTypeDef,
+    RealtimeLogConfigTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
     CreateKeyGroupResultTypeDef,
     GetKeyGroupResultTypeDef,
     KeyGroupSummaryTypeDef,
     UpdateKeyGroupResultTypeDef,
-    CreateOriginAccessControlResultTypeDef,
-    GetOriginAccessControlResultTypeDef,
-    UpdateOriginAccessControlResultTypeDef,
-    CreatePublicKeyResultTypeDef,
-    GetPublicKeyResultTypeDef,
-    UpdatePublicKeyResultTypeDef,
     InvalidationTypeDef,
     CreateInvalidationRequestRequestTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
+    CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
-    CreateMonitoringSubscriptionRequestRequestTypeDef,
     ListOriginAccessControlsResultTypeDef,
     OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
     QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
     ResponseHeadersPolicyConfigOutputTypeDef,
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.py` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.pyi` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__main__.py` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFront 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudFront 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.py` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,16 @@
 
     def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
-        IfMatch: str = ...
+        IfMatch: str = ...,
+        Enabled: bool = ...
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.pyi` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,16 @@
         """
     def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
-        IfMatch: str = ...
+        IfMatch: str = ...,
+        Enabled: bool = ...
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.py` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 CachePolicyTypeType = Literal["custom", "managed"]
 CertificateSourceType = Literal["acm", "cloudfront", "iam"]
 ContinuousDeploymentPolicyTypeType = Literal["SingleHeader", "SingleWeight"]
 DistributionDeployedWaiterName = Literal["distribution_deployed"]
 EventTypeType = Literal["origin-request", "origin-response", "viewer-request", "viewer-response"]
 FormatType = Literal["URLEncoded"]
 FrameOptionsListType = Literal["DENY", "SAMEORIGIN"]
-FunctionRuntimeType = Literal["cloudfront-js-1.0"]
+FunctionRuntimeType = Literal["cloudfront-js-1.0", "cloudfront-js-2.0"]
 FunctionStageType = Literal["DEVELOPMENT", "LIVE"]
 GeoRestrictionTypeType = Literal["blacklist", "none", "whitelist"]
 HttpVersionType = Literal["http1.1", "http2", "http2and3", "http3"]
 ICPRecordalStatusType = Literal["APPROVED", "PENDING", "SUSPENDED"]
 InvalidationCompletedWaiterName = Literal["invalidation_completed"]
 ItemSelectionType = Literal["all", "none", "whitelist"]
 ListCloudFrontOriginAccessIdentitiesPaginatorName = Literal[
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.pyi` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 CachePolicyTypeType = Literal["custom", "managed"]
 CertificateSourceType = Literal["acm", "cloudfront", "iam"]
 ContinuousDeploymentPolicyTypeType = Literal["SingleHeader", "SingleWeight"]
 DistributionDeployedWaiterName = Literal["distribution_deployed"]
 EventTypeType = Literal["origin-request", "origin-response", "viewer-request", "viewer-response"]
 FormatType = Literal["URLEncoded"]
 FrameOptionsListType = Literal["DENY", "SAMEORIGIN"]
-FunctionRuntimeType = Literal["cloudfront-js-1.0"]
+FunctionRuntimeType = Literal["cloudfront-js-1.0", "cloudfront-js-2.0"]
 FunctionStageType = Literal["DEVELOPMENT", "LIVE"]
 GeoRestrictionTypeType = Literal["blacklist", "none", "whitelist"]
 HttpVersionType = Literal["http1.1", "http2", "http2and3", "http3"]
 ICPRecordalStatusType = Literal["APPROVED", "PENDING", "SUSPENDED"]
 InvalidationCompletedWaiterName = Literal["invalidation_completed"]
 ItemSelectionType = Literal["all", "none", "whitelist"]
 ListCloudFrontOriginAccessIdentitiesPaginatorName = Literal[
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.py` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,76 +40,70 @@
 __all__ = (
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
     "ListInvalidationsPaginator",
     "ListStreamingDistributionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListCloudFrontOriginAccessIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
-
 class ListDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
         """
 
-
 class ListInvalidationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
-        self, *, DistributionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
         """
 
-
 class ListStreamingDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamingDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
         """
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.pyi` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,70 +40,76 @@
 __all__ = (
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
     "ListInvalidationsPaginator",
     "ListStreamingDistributionsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListCloudFrontOriginAccessIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
+
 class ListDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
         """
 
+
 class ListInvalidationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
-        self, *, DistributionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
         """
 
+
 class ListStreamingDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamingDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
         """
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.py` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CachePolicyHeaderBehaviorType,
     CachePolicyQueryStringBehaviorType,
     CachePolicyTypeType,
     CertificateSourceType,
     ContinuousDeploymentPolicyTypeType,
     EventTypeType,
     FrameOptionsListType,
+    FunctionRuntimeType,
     FunctionStageType,
     GeoRestrictionTypeType,
     HttpVersionType,
     ICPRecordalStatusType,
     ItemSelectionType,
     MethodType,
     MinimumProtocolVersionType,
@@ -73,34 +74,29 @@
     "TrustedSignersTypeDef",
     "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
     "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
-    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
-    "ContentTypeProfileOutputTypeDef",
     "ContentTypeProfileTypeDef",
     "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
-    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
-    "SessionStickinessConfigOutputTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
-    "CustomErrorResponseOutputTypeDef",
     "CustomErrorResponseTypeDef",
-    "OriginCustomHeaderOutputTypeDef",
     "OriginCustomHeaderTypeDef",
     "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
@@ -112,29 +108,23 @@
     "DeleteOriginAccessControlRequestRequestTypeDef",
     "DeleteOriginRequestPolicyRequestRequestTypeDef",
     "DeletePublicKeyRequestRequestTypeDef",
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
-    "LoggingConfigOutputTypeDef",
-    "ViewerCertificateOutputTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
-    "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
     "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
-    "FunctionAssociationOutputTypeDef",
     "FunctionAssociationTypeDef",
-    "FunctionConfigOutputTypeDef",
     "FunctionMetadataTypeDef",
     "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
@@ -144,115 +134,89 @@
     "WaiterConfigTypeDef",
     "GetDistributionRequestRequestTypeDef",
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
-    "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
     "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
-    "OriginAccessControlConfigOutputTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
-    "PublicKeyConfigOutputTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
     "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
-    "LambdaFunctionAssociationOutputTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
     "ListDistributionsByKeyGroupRequestRequestTypeDef",
     "ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef",
     "ListDistributionsByWebACLIdRequestRequestTypeDef",
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListDistributionsRequestRequestTypeDef",
     "ListFieldLevelEncryptionConfigsRequestRequestTypeDef",
     "ListFieldLevelEncryptionProfilesRequestRequestTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListInvalidationsRequestRequestTypeDef",
     "ListKeyGroupsRequestRequestTypeDef",
     "ListOriginAccessControlsRequestRequestTypeDef",
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
     "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
-    "OriginGroupMemberOutputTypeDef",
     "OriginGroupMemberTypeDef",
-    "OriginShieldOutputTypeDef",
-    "S3OriginConfigOutputTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
-    "QueryArgProfileOutputTypeDef",
     "QueryArgProfileTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
-    "ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
-    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
-    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
-    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
-    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
-    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
-    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
-    "ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
-    "ResponseHeadersPolicyXSSProtectionOutputTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3OriginOutputTypeDef",
     "S3OriginTypeDef",
-    "StreamingLoggingConfigOutputTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
     "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
     "CachePolicyCookiesConfigOutputTypeDef",
     "CookiePreferenceOutputTypeDef",
@@ -265,67 +229,70 @@
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
     "CachePolicyQueryStringsConfigOutputTypeDef",
     "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
     "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
-    "ContinuousDeploymentSingleWeightConfigOutputTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
+    "GetOriginAccessControlConfigResultTypeDef",
+    "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
+    "GetPublicKeyConfigResultTypeDef",
+    "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
     "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
     "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
     "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
-    "EndPointOutputTypeDef",
     "EndPointTypeDef",
     "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
     "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     "GetKeyGroupConfigResultTypeDef",
     "KeyGroupTypeDef",
-    "GetOriginAccessControlConfigResultTypeDef",
-    "OriginAccessControlTypeDef",
-    "GetPublicKeyConfigResultTypeDef",
-    "PublicKeyTypeDef",
     "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
     "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
-    "MonitoringSubscriptionOutputTypeDef",
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
     "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
     "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
@@ -333,15 +300,14 @@
     "QueryArgProfilesTypeDef",
     "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
-    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
     "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "TagsOutputTypeDef",
     "TagsTypeDef",
@@ -354,47 +320,46 @@
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
     "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
-    "TrafficConfigOutputTypeDef",
     "TrafficConfigTypeDef",
+    "CreateOriginAccessControlResultTypeDef",
+    "GetOriginAccessControlResultTypeDef",
+    "UpdateOriginAccessControlResultTypeDef",
+    "CreatePublicKeyResultTypeDef",
+    "GetPublicKeyResultTypeDef",
+    "UpdatePublicKeyResultTypeDef",
     "OriginOutputTypeDef",
     "OriginTypeDef",
     "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
-    "RealtimeLogConfigTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
+    "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
     "CreateKeyGroupResultTypeDef",
     "GetKeyGroupResultTypeDef",
     "KeyGroupSummaryTypeDef",
     "UpdateKeyGroupResultTypeDef",
-    "CreateOriginAccessControlResultTypeDef",
-    "GetOriginAccessControlResultTypeDef",
-    "UpdateOriginAccessControlResultTypeDef",
-    "CreatePublicKeyResultTypeDef",
-    "GetPublicKeyResultTypeDef",
-    "UpdatePublicKeyResultTypeDef",
     "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "ListOriginAccessControlsResultTypeDef",
     "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
     "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
     "ResponseHeadersPolicyConfigOutputTypeDef",
@@ -792,22 +757,14 @@
 )
 
 
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
 
-CloudFrontOriginAccessIdentityConfigOutputTypeDef = TypedDict(
-    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "Comment": str,
-    },
-)
-
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -827,36 +784,14 @@
         "Alias": str,
         "DistributionId": str,
         "AccountId": str,
     },
     total=False,
 )
 
-_RequiredContentTypeProfileOutputTypeDef = TypedDict(
-    "_RequiredContentTypeProfileOutputTypeDef",
-    {
-        "Format": Literal["URLEncoded"],
-        "ContentType": str,
-    },
-)
-_OptionalContentTypeProfileOutputTypeDef = TypedDict(
-    "_OptionalContentTypeProfileOutputTypeDef",
-    {
-        "ProfileId": str,
-    },
-    total=False,
-)
-
-
-class ContentTypeProfileOutputTypeDef(
-    _RequiredContentTypeProfileOutputTypeDef, _OptionalContentTypeProfileOutputTypeDef
-):
-    pass
-
-
 _RequiredContentTypeProfileTypeDef = TypedDict(
     "_RequiredContentTypeProfileTypeDef",
     {
         "Format": Literal["URLEncoded"],
         "ContentType": str,
     },
 )
@@ -914,38 +849,22 @@
 
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
 
-ContinuousDeploymentSingleHeaderConfigOutputTypeDef = TypedDict(
-    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
-    {
-        "Header": str,
-        "Value": str,
-    },
-)
-
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
 
-SessionStickinessConfigOutputTypeDef = TypedDict(
-    "SessionStickinessConfigOutputTypeDef",
-    {
-        "IdleTTL": int,
-        "MaximumTTL": int,
-    },
-)
-
 SessionStickinessConfigTypeDef = TypedDict(
     "SessionStickinessConfigTypeDef",
     {
         "IdleTTL": int,
         "MaximumTTL": int,
     },
 )
@@ -958,30 +877,42 @@
     },
 )
 _OptionalCopyDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalCopyDistributionRequestRequestTypeDef",
     {
         "Staging": bool,
         "IfMatch": str,
+        "Enabled": bool,
     },
     total=False,
 )
 
 
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
 ):
     pass
 
 
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
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
-        "Runtime": Literal["cloudfront-js-1.0"],
+        "Runtime": FunctionRuntimeType,
     },
 )
 
 _RequiredKeyGroupConfigTypeDef = TypedDict(
     "_RequiredKeyGroupConfigTypeDef",
     {
         "Name": str,
@@ -1042,37 +973,14 @@
 )
 
 
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
 
-_RequiredCustomErrorResponseOutputTypeDef = TypedDict(
-    "_RequiredCustomErrorResponseOutputTypeDef",
-    {
-        "ErrorCode": int,
-    },
-)
-_OptionalCustomErrorResponseOutputTypeDef = TypedDict(
-    "_OptionalCustomErrorResponseOutputTypeDef",
-    {
-        "ResponsePagePath": str,
-        "ResponseCode": str,
-        "ErrorCachingMinTTL": int,
-    },
-    total=False,
-)
-
-
-class CustomErrorResponseOutputTypeDef(
-    _RequiredCustomErrorResponseOutputTypeDef, _OptionalCustomErrorResponseOutputTypeDef
-):
-    pass
-
-
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -1088,22 +996,14 @@
 
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
 
-OriginCustomHeaderOutputTypeDef = TypedDict(
-    "OriginCustomHeaderOutputTypeDef",
-    {
-        "HeaderName": str,
-        "HeaderValue": str,
-    },
-)
-
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
@@ -1426,38 +1326,14 @@
 
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
 
-LoggingConfigOutputTypeDef = TypedDict(
-    "LoggingConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-        "IncludeCookies": bool,
-        "Bucket": str,
-        "Prefix": str,
-    },
-)
-
-ViewerCertificateOutputTypeDef = TypedDict(
-    "ViewerCertificateOutputTypeDef",
-    {
-        "CloudFrontDefaultCertificate": bool,
-        "IAMCertificateId": str,
-        "ACMCertificateArn": str,
-        "SSLSupportMethod": SSLSupportMethodType,
-        "MinimumProtocolVersion": MinimumProtocolVersionType,
-        "Certificate": str,
-        "CertificateSource": CertificateSourceType,
-    },
-    total=False,
-)
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1499,21 +1375,14 @@
 
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFieldPatternsOutputTypeDef = TypedDict(
     "_RequiredFieldPatternsOutputTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFieldPatternsOutputTypeDef = TypedDict(
@@ -1546,22 +1415,14 @@
 )
 
 
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
 
-KinesisStreamConfigOutputTypeDef = TypedDict(
-    "KinesisStreamConfigOutputTypeDef",
-    {
-        "RoleARN": str,
-        "StreamARN": str,
-    },
-)
-
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
@@ -1604,38 +1465,22 @@
 
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
 
-FunctionAssociationOutputTypeDef = TypedDict(
-    "FunctionAssociationOutputTypeDef",
-    {
-        "FunctionARN": str,
-        "EventType": EventTypeType,
-    },
-)
-
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
 
-FunctionConfigOutputTypeDef = TypedDict(
-    "FunctionConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "Runtime": Literal["cloudfront-js-1.0"],
-    },
-)
-
 _RequiredFunctionMetadataTypeDef = TypedDict(
     "_RequiredFunctionMetadataTypeDef",
     {
         "FunctionARN": str,
         "LastModifiedTime": datetime,
     },
 )
@@ -1805,24 +1650,14 @@
 
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
 
-GetFunctionResultTypeDef = TypedDict(
-    "GetFunctionResultTypeDef",
-    {
-        "FunctionCode": StreamingBody,
-        "ETag": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -1873,38 +1708,14 @@
 GetOriginAccessControlConfigRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredOriginAccessControlConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginAccessControlConfigOutputTypeDef",
-    {
-        "Name": str,
-        "SigningProtocol": Literal["sigv4"],
-        "SigningBehavior": OriginAccessControlSigningBehaviorsType,
-        "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
-    },
-)
-_OptionalOriginAccessControlConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginAccessControlConfigOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class OriginAccessControlConfigOutputTypeDef(
-    _RequiredOriginAccessControlConfigOutputTypeDef, _OptionalOriginAccessControlConfigOutputTypeDef
-):
-    pass
-
-
 GetOriginAccessControlRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1925,37 +1736,14 @@
 GetPublicKeyConfigRequestRequestTypeDef = TypedDict(
     "GetPublicKeyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredPublicKeyConfigOutputTypeDef = TypedDict(
-    "_RequiredPublicKeyConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "Name": str,
-        "EncodedKey": str,
-    },
-)
-_OptionalPublicKeyConfigOutputTypeDef = TypedDict(
-    "_OptionalPublicKeyConfigOutputTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-
-class PublicKeyConfigOutputTypeDef(
-    _RequiredPublicKeyConfigOutputTypeDef, _OptionalPublicKeyConfigOutputTypeDef
-):
-    pass
-
-
 GetPublicKeyRequestRequestTypeDef = TypedDict(
     "GetPublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -2058,36 +1846,14 @@
 )
 
 
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
 
-_RequiredLambdaFunctionAssociationOutputTypeDef = TypedDict(
-    "_RequiredLambdaFunctionAssociationOutputTypeDef",
-    {
-        "LambdaFunctionARN": str,
-        "EventType": EventTypeType,
-    },
-)
-_OptionalLambdaFunctionAssociationOutputTypeDef = TypedDict(
-    "_OptionalLambdaFunctionAssociationOutputTypeDef",
-    {
-        "IncludeBody": bool,
-    },
-    total=False,
-)
-
-
-class LambdaFunctionAssociationOutputTypeDef(
-    _RequiredLambdaFunctionAssociationOutputTypeDef, _OptionalLambdaFunctionAssociationOutputTypeDef
-):
-    pass
-
-
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -2112,18 +1878,20 @@
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
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
 
 ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     {
@@ -2288,22 +2056,14 @@
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
 
-ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2333,36 +2093,14 @@
         "Marker": str,
         "MaxItems": str,
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "DistributionId": str,
-    },
-)
-_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
-    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInvalidationsRequestRequestTypeDef = TypedDict(
     "_RequiredListInvalidationsRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 _OptionalListInvalidationsRequestRequestTypeDef = TypedDict(
@@ -2433,22 +2171,14 @@
         "Type": ResponseHeadersPolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamingDistributionsRequestRequestTypeDef = TypedDict(
     "ListStreamingDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2457,21 +2187,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
-RealtimeMetricsSubscriptionConfigOutputTypeDef = TypedDict(
-    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
-    {
-        "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
-    },
-)
-
 RealtimeMetricsSubscriptionConfigTypeDef = TypedDict(
     "RealtimeMetricsSubscriptionConfigTypeDef",
     {
         "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
     },
 )
 
@@ -2499,56 +2222,21 @@
     "StatusCodesTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[int],
     },
 )
 
-OriginGroupMemberOutputTypeDef = TypedDict(
-    "OriginGroupMemberOutputTypeDef",
-    {
-        "OriginId": str,
-    },
-)
-
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
     },
 )
 
-_RequiredOriginShieldOutputTypeDef = TypedDict(
-    "_RequiredOriginShieldOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalOriginShieldOutputTypeDef = TypedDict(
-    "_OptionalOriginShieldOutputTypeDef",
-    {
-        "OriginShieldRegion": str,
-    },
-    total=False,
-)
-
-
-class OriginShieldOutputTypeDef(
-    _RequiredOriginShieldOutputTypeDef, _OptionalOriginShieldOutputTypeDef
-):
-    pass
-
-
-S3OriginConfigOutputTypeDef = TypedDict(
-    "S3OriginConfigOutputTypeDef",
-    {
-        "OriginAccessIdentity": str,
-    },
-)
-
 _RequiredOriginShieldTypeDef = TypedDict(
     "_RequiredOriginShieldTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOriginShieldTypeDef = TypedDict(
@@ -2567,24 +2255,14 @@
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
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
 _RequiredPublicKeySummaryTypeDef = TypedDict(
     "_RequiredPublicKeySummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatedTime": datetime,
         "EncodedKey": str,
@@ -2607,22 +2285,14 @@
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
 
-QueryArgProfileOutputTypeDef = TypedDict(
-    "QueryArgProfileOutputTypeDef",
-    {
-        "QueryArg": str,
-        "ProfileId": str,
-    },
-)
-
 QueryArgProfileTypeDef = TypedDict(
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
@@ -2715,36 +2385,14 @@
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
 
-_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
-    {
-        "SamplingRate": float,
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
@@ -2759,156 +2407,61 @@
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
 
-ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
-    {
-        "Override": bool,
-        "ContentSecurityPolicy": str,
-    },
-)
-
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
 
-ResponseHeadersPolicyContentTypeOptionsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
-    {
-        "Override": bool,
-    },
-)
-
 ResponseHeadersPolicyContentTypeOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     {
         "Override": bool,
     },
 )
 
-ResponseHeadersPolicyCustomHeaderOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
-    {
-        "Header": str,
-        "Value": str,
-        "Override": bool,
-    },
-)
-
 ResponseHeadersPolicyCustomHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     {
         "Header": str,
         "Value": str,
         "Override": bool,
     },
 )
 
-ResponseHeadersPolicyFrameOptionsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
-    {
-        "Override": bool,
-        "FrameOption": FrameOptionsListType,
-    },
-)
-
 ResponseHeadersPolicyFrameOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     {
         "Override": bool,
         "FrameOption": FrameOptionsListType,
     },
 )
 
-ResponseHeadersPolicyReferrerPolicyOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
-    {
-        "Override": bool,
-        "ReferrerPolicy": ReferrerPolicyListType,
-    },
-)
-
 ResponseHeadersPolicyReferrerPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     {
         "Override": bool,
         "ReferrerPolicy": ReferrerPolicyListType,
     },
 )
 
-ResponseHeadersPolicyRemoveHeaderOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
-    {
-        "Header": str,
-    },
-)
-
 ResponseHeadersPolicyRemoveHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     {
         "Header": str,
     },
 )
 
-_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
-    {
-        "Override": bool,
-        "AccessControlMaxAgeSec": int,
-    },
-)
-_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
-    {
-        "IncludeSubdomains": bool,
-        "Preload": bool,
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef(
-    _RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-    _OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-):
-    pass
-
-
-_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef",
-    {
-        "Override": bool,
-        "Protection": bool,
-    },
-)
-_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef",
-    {
-        "ModeBlock": bool,
-        "ReportUri": str,
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyXSSProtectionOutputTypeDef(
-    _RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef,
-    _OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef,
-):
-    pass
-
-
 _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef",
     {
         "Override": bool,
         "AccessControlMaxAgeSec": int,
     },
 )
@@ -2949,50 +2502,22 @@
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
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
-S3OriginOutputTypeDef = TypedDict(
-    "S3OriginOutputTypeDef",
-    {
-        "DomainName": str,
-        "OriginAccessIdentity": str,
-    },
-)
-
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
 
-StreamingLoggingConfigOutputTypeDef = TypedDict(
-    "StreamingLoggingConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Bucket": str,
-        "Prefix": str,
-    },
-)
-
 StreamingLoggingConfigTypeDef = TypedDict(
     "StreamingLoggingConfigTypeDef",
     {
         "Enabled": bool,
         "Bucket": str,
         "Prefix": str,
     },
@@ -3002,33 +2527,14 @@
     "TagKeysTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -3437,35 +2943,26 @@
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
 _OptionalCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
     total=False,
 )
 
 
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
 
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
@@ -3534,15 +3031,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesOutputTypeDef = TypedDict(
     "_OptionalContentTypeProfilesOutputTypeDef",
     {
-        "Items": List[ContentTypeProfileOutputTypeDef],
+        "Items": List[ContentTypeProfileTypeDef],
     },
     total=False,
 )
 
 
 class ContentTypeProfilesOutputTypeDef(
     _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
@@ -3567,36 +3064,14 @@
 
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
 
-_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
-    "_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef",
-    {
-        "Weight": float,
-    },
-)
-_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
-    "_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef",
-    {
-        "SessionStickinessConfig": SessionStickinessConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ContinuousDeploymentSingleWeightConfigOutputTypeDef(
-    _RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef,
-    _OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
@@ -3611,14 +3086,40 @@
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    {
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionResultTypeDef = TypedDict(
+    "GetFunctionResultTypeDef",
+    {
+        "FunctionCode": StreamingBody,
+        "ETag": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -3666,14 +3167,44 @@
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
+GetOriginAccessControlConfigResultTypeDef = TypedDict(
+    "GetOriginAccessControlConfigResultTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredOriginAccessControlTypeDef = TypedDict(
+    "_RequiredOriginAccessControlTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalOriginAccessControlTypeDef = TypedDict(
+    "_OptionalOriginAccessControlTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginAccessControlTypeDef(
+    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
+):
+    pass
+
+
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -3696,14 +3227,32 @@
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
+GetPublicKeyConfigResultTypeDef = TypedDict(
+    "GetPublicKeyConfigResultTypeDef",
+    {
+        "PublicKeyConfig": PublicKeyConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublicKeyTypeDef = TypedDict(
+    "PublicKeyTypeDef",
+    {
+        "Id": str,
+        "CreatedTime": datetime,
+        "PublicKeyConfig": PublicKeyConfigTypeDef,
+    },
+)
+
 _RequiredUpdatePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "Id": str,
     },
 )
@@ -3727,15 +3276,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesOutputTypeDef",
     {
-        "Items": List[CustomErrorResponseOutputTypeDef],
+        "Items": List[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
 
 class CustomErrorResponsesOutputTypeDef(
     _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
@@ -3769,15 +3318,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersOutputTypeDef = TypedDict(
     "_OptionalCustomHeadersOutputTypeDef",
     {
-        "Items": List[OriginCustomHeaderOutputTypeDef],
+        "Items": List[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
 
 class CustomHeadersOutputTypeDef(
     _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
@@ -3854,39 +3403,39 @@
     pass
 
 
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByKeyGroupResultTypeDef = TypedDict(
     "ListDistributionsByKeyGroupResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByOriginRequestPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EncryptionEntityOutputTypeDef = TypedDict(
     "EncryptionEntityOutputTypeDef",
     {
         "PublicKeyId": str,
@@ -3900,33 +3449,14 @@
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
 )
 
-_RequiredEndPointOutputTypeDef = TypedDict(
-    "_RequiredEndPointOutputTypeDef",
-    {
-        "StreamType": str,
-    },
-)
-_OptionalEndPointOutputTypeDef = TypedDict(
-    "_OptionalEndPointOutputTypeDef",
-    {
-        "KinesisStreamConfig": KinesisStreamConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EndPointOutputTypeDef(_RequiredEndPointOutputTypeDef, _OptionalEndPointOutputTypeDef):
-    pass
-
-
 _RequiredEndPointTypeDef = TypedDict(
     "_RequiredEndPointTypeDef",
     {
         "StreamType": str,
     },
 )
 _OptionalEndPointTypeDef = TypedDict(
@@ -3947,15 +3477,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsOutputTypeDef = TypedDict(
     "_OptionalFunctionAssociationsOutputTypeDef",
     {
-        "Items": List[FunctionAssociationOutputTypeDef],
+        "Items": List[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
 
 class FunctionAssociationsOutputTypeDef(
     _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
@@ -3984,15 +3514,15 @@
     pass
 
 
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
-        "FunctionConfig": FunctionConfigOutputTypeDef,
+        "FunctionConfig": FunctionConfigTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
 )
 _OptionalFunctionSummaryTypeDef = TypedDict(
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
@@ -4087,75 +3617,27 @@
 
 
 GetKeyGroupConfigResultTypeDef = TypedDict(
     "GetKeyGroupConfigResultTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KeyGroupTypeDef = TypedDict(
     "KeyGroupTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
     },
 )
 
-GetOriginAccessControlConfigResultTypeDef = TypedDict(
-    "GetOriginAccessControlConfigResultTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredOriginAccessControlTypeDef = TypedDict(
-    "_RequiredOriginAccessControlTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalOriginAccessControlTypeDef = TypedDict(
-    "_OptionalOriginAccessControlTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class OriginAccessControlTypeDef(
-    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
-):
-    pass
-
-
-GetPublicKeyConfigResultTypeDef = TypedDict(
-    "GetPublicKeyConfigResultTypeDef",
-    {
-        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PublicKeyTypeDef = TypedDict(
-    "PublicKeyTypeDef",
-    {
-        "Id": str,
-        "CreatedTime": datetime,
-        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
-    },
-)
-
 InvalidationBatchOutputTypeDef = TypedDict(
     "InvalidationBatchOutputTypeDef",
     {
         "Paths": PathsOutputTypeDef,
         "CallerReference": str,
     },
 )
@@ -4214,15 +3696,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsOutputTypeDef",
     {
-        "Items": List[LambdaFunctionAssociationOutputTypeDef],
+        "Items": List[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
 
 class LambdaFunctionAssociationsOutputTypeDef(
     _RequiredLambdaFunctionAssociationsOutputTypeDef,
@@ -4248,18 +3730,56 @@
 
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
 
-MonitoringSubscriptionOutputTypeDef = TypedDict(
-    "MonitoringSubscriptionOutputTypeDef",
+ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "DistributionId": str,
+    },
+)
+_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
+    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
+):
+    pass
+
+
+ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     {
-        "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
@@ -4307,15 +3827,15 @@
     },
 )
 
 OriginGroupMembersOutputTypeDef = TypedDict(
     "OriginGroupMembersOutputTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginGroupMemberOutputTypeDef],
+        "Items": List[OriginGroupMemberTypeDef],
     },
 )
 
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
@@ -4349,15 +3869,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalQueryArgProfilesOutputTypeDef = TypedDict(
     "_OptionalQueryArgProfilesOutputTypeDef",
     {
-        "Items": List[QueryArgProfileOutputTypeDef],
+        "Items": List[QueryArgProfileTypeDef],
     },
     total=False,
 )
 
 
 class QueryArgProfilesOutputTypeDef(
     _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
@@ -4442,15 +3962,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     {
-        "Items": List[ResponseHeadersPolicyCustomHeaderOutputTypeDef],
+        "Items": List[ResponseHeadersPolicyCustomHeaderTypeDef],
     },
     total=False,
 )
 
 
 class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
@@ -4486,15 +4006,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     {
-        "Items": List[ResponseHeadersPolicyRemoveHeaderOutputTypeDef],
+        "Items": List[ResponseHeadersPolicyRemoveHeaderTypeDef],
     },
     total=False,
 )
 
 
 class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
@@ -4521,27 +4041,14 @@
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
 
-ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
-    {
-        "XSSProtection": ResponseHeadersPolicyXSSProtectionOutputTypeDef,
-        "FrameOptions": ResponseHeadersPolicyFrameOptionsOutputTypeDef,
-        "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
-        "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
-        "ContentTypeOptions": ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
-        "StrictTransportSecurity": ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-    },
-    total=False,
-)
-
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -4555,38 +4062,38 @@
     "StreamingDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "S3Origin": S3OriginOutputTypeDef,
+        "S3Origin": S3OriginTypeDef,
         "Aliases": AliasesOutputTypeDef,
         "TrustedSigners": TrustedSignersOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
 _RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
-        "S3Origin": S3OriginOutputTypeDef,
+        "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersOutputTypeDef,
         "Enabled": bool,
     },
 )
 _OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
     "_OptionalStreamingDistributionConfigOutputTypeDef",
     {
         "Aliases": AliasesOutputTypeDef,
-        "Logging": StreamingLoggingConfigOutputTypeDef,
+        "Logging": StreamingLoggingConfigTypeDef,
         "PriceClass": PriceClassType,
     },
     total=False,
 )
 
 
 class StreamingDistributionConfigOutputTypeDef(
@@ -4630,15 +4137,15 @@
         "TagKeys": TagKeysTypeDef,
     },
 )
 
 TagsOutputTypeDef = TypedDict(
     "TagsOutputTypeDef",
     {
-        "Items": List[TagOutputTypeDef],
+        "Items": List[TagTypeDef],
     },
     total=False,
 )
 
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
@@ -4791,49 +4298,49 @@
 
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCloudFrontOriginAccessIdentitiesResultTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     {
         "CloudFrontOriginAccessIdentityList": CloudFrontOriginAccessIdentityListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigOutputTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
@@ -4871,73 +4378,107 @@
 
 class ContentTypeProfileConfigTypeDef(
     _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
 ):
     pass
 
 
-_RequiredTrafficConfigOutputTypeDef = TypedDict(
-    "_RequiredTrafficConfigOutputTypeDef",
+_RequiredTrafficConfigTypeDef = TypedDict(
+    "_RequiredTrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
-_OptionalTrafficConfigOutputTypeDef = TypedDict(
-    "_OptionalTrafficConfigOutputTypeDef",
+_OptionalTrafficConfigTypeDef = TypedDict(
+    "_OptionalTrafficConfigTypeDef",
     {
-        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigOutputTypeDef,
-        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
+        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
+        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
     total=False,
 )
 
 
-class TrafficConfigOutputTypeDef(
-    _RequiredTrafficConfigOutputTypeDef, _OptionalTrafficConfigOutputTypeDef
-):
+class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
     pass
 
 
-_RequiredTrafficConfigTypeDef = TypedDict(
-    "_RequiredTrafficConfigTypeDef",
+CreateOriginAccessControlResultTypeDef = TypedDict(
+    "CreateOriginAccessControlResultTypeDef",
     {
-        "Type": ContinuousDeploymentPolicyTypeType,
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTrafficConfigTypeDef = TypedDict(
-    "_OptionalTrafficConfigTypeDef",
+
+GetOriginAccessControlResultTypeDef = TypedDict(
+    "GetOriginAccessControlResultTypeDef",
     {
-        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
-        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateOriginAccessControlResultTypeDef = TypedDict(
+    "UpdateOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
-    pass
+CreatePublicKeyResultTypeDef = TypedDict(
+    "CreatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetPublicKeyResultTypeDef = TypedDict(
+    "GetPublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePublicKeyResultTypeDef = TypedDict(
+    "UpdatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredOriginOutputTypeDef = TypedDict(
     "_RequiredOriginOutputTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
 )
 _OptionalOriginOutputTypeDef = TypedDict(
     "_OptionalOriginOutputTypeDef",
     {
         "OriginPath": str,
         "CustomHeaders": CustomHeadersOutputTypeDef,
-        "S3OriginConfig": S3OriginConfigOutputTypeDef,
+        "S3OriginConfig": S3OriginConfigTypeDef,
         "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
         "ConnectionAttempts": int,
         "ConnectionTimeout": int,
-        "OriginShield": OriginShieldOutputTypeDef,
+        "OriginShield": OriginShieldTypeDef,
         "OriginAccessControlId": str,
     },
     total=False,
 )
 
 
 class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
@@ -5009,32 +4550,32 @@
 
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
 
-RealtimeLogConfigTypeDef = TypedDict(
-    "RealtimeLogConfigTypeDef",
+CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
+    "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
-        "ARN": str,
+        "EndPoints": Sequence[EndPointTypeDef],
+        "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
-        "EndPoints": List[EndPointOutputTypeDef],
-        "Fields": List[str],
     },
 )
 
-CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
-    "CreateRealtimeLogConfigRequestRequestTypeDef",
+RealtimeLogConfigTypeDef = TypedDict(
+    "RealtimeLogConfigTypeDef",
     {
-        "EndPoints": Sequence[EndPointTypeDef],
-        "Fields": Sequence[str],
+        "ARN": str,
         "Name": str,
         "SamplingRate": int,
+        "EndPoints": List[EndPointTypeDef],
+        "Fields": List[str],
     },
 )
 
 UpdateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
@@ -5048,24 +4589,24 @@
 
 CreateFunctionResultTypeDef = TypedDict(
     "CreateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFunctionResultTypeDef = TypedDict(
     "DescribeFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionListTypeDef = TypedDict(
     "_RequiredFunctionListTypeDef",
     {
         "MaxItems": int,
@@ -5086,15 +4627,15 @@
     pass
 
 
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestResultTypeDef = TypedDict(
     "TestResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
@@ -5107,34 +4648,34 @@
 )
 
 UpdateFunctionResultTypeDef = TypedDict(
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeyGroupResultTypeDef = TypedDict(
     "CreateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyGroupResultTypeDef = TypedDict(
     "GetKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KeyGroupSummaryTypeDef = TypedDict(
     "KeyGroupSummaryTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
@@ -5142,71 +4683,15 @@
 )
 
 UpdateKeyGroupResultTypeDef = TypedDict(
     "UpdateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateOriginAccessControlResultTypeDef = TypedDict(
-    "CreateOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetOriginAccessControlResultTypeDef = TypedDict(
-    "GetOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateOriginAccessControlResultTypeDef = TypedDict(
-    "UpdateOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePublicKeyResultTypeDef = TypedDict(
-    "CreatePublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPublicKeyResultTypeDef = TypedDict(
-    "GetPublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePublicKeyResultTypeDef = TypedDict(
-    "UpdatePublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
@@ -5224,15 +4709,15 @@
     },
 )
 
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActiveTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredActiveTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
@@ -5272,43 +4757,43 @@
 
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
 
-CreateMonitoringSubscriptionResultTypeDef = TypedDict(
-    "CreateMonitoringSubscriptionResultTypeDef",
+CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DistributionId": str,
+        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
     },
 )
 
-GetMonitoringSubscriptionResultTypeDef = TypedDict(
-    "GetMonitoringSubscriptionResultTypeDef",
+CreateMonitoringSubscriptionResultTypeDef = TypedDict(
+    "CreateMonitoringSubscriptionResultTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
+GetMonitoringSubscriptionResultTypeDef = TypedDict(
+    "GetMonitoringSubscriptionResultTypeDef",
     {
-        "DistributionId": str,
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginGroupOutputTypeDef = TypedDict(
     "OriginGroupOutputTypeDef",
     {
         "Id": str,
@@ -5326,15 +4811,15 @@
     },
 )
 
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigOutputTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
@@ -5383,16 +4868,16 @@
     },
 )
 _OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
     {
         "Comment": str,
         "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
-        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
-        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigTypeDef,
+        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
         "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
         "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     },
     total=False,
 )
 
 
@@ -5455,15 +4940,15 @@
 
 
 GetStreamingDistributionConfigResultTypeDef = TypedDict(
     "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -5493,15 +4978,15 @@
     pass
 
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": TagsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -5693,15 +5178,15 @@
 
 
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
@@ -5771,15 +5256,15 @@
         "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
         "Enabled": bool,
     },
 )
 _OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
     "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
     {
-        "TrafficConfig": TrafficConfigOutputTypeDef,
+        "TrafficConfig": TrafficConfigTypeDef,
     },
     total=False,
 )
 
 
 class ContinuousDeploymentPolicyConfigOutputTypeDef(
     _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
@@ -5900,23 +5385,23 @@
     pass
 
 
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRealtimeLogConfigResultTypeDef = TypedDict(
     "GetRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRealtimeLogConfigsTypeDef = TypedDict(
     "_RequiredRealtimeLogConfigsTypeDef",
     {
         "MaxItems": int,
@@ -5940,31 +5425,31 @@
     pass
 
 
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResultTypeDef = TypedDict(
     "ListFunctionsResultTypeDef",
     {
         "FunctionList": FunctionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFunctionResultTypeDef = TypedDict(
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyGroupListTypeDef = TypedDict(
     "_RequiredKeyGroupListTypeDef",
     {
         "MaxItems": int,
@@ -5986,23 +5471,23 @@
 
 
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvalidationResultTypeDef = TypedDict(
     "GetInvalidationResultTypeDef",
     {
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStreamingDistributionTypeDef = TypedDict(
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
@@ -6140,15 +5625,15 @@
 
 
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
@@ -6187,15 +5672,15 @@
     pass
 
 
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
@@ -6252,34 +5737,34 @@
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginRequestPolicyResultTypeDef = TypedDict(
     "GetOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicySummaryTypeDef = TypedDict(
     "OriginRequestPolicySummaryTypeDef",
     {
         "Type": OriginRequestPolicyTypeType,
@@ -6288,15 +5773,15 @@
 )
 
 UpdateOriginRequestPolicyResultTypeDef = TypedDict(
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCachePolicyRequestRequestTypeDef = TypedDict(
     "CreateCachePolicyRequestRequestTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
@@ -6335,15 +5820,15 @@
 )
 
 GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -6383,15 +5868,15 @@
 )
 
 GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
         "MaxItems": int,
@@ -6444,61 +5929,61 @@
     pass
 
 
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeyGroupsResultTypeDef = TypedDict(
     "ListKeyGroupsResultTypeDef",
     {
         "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsResultTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingDistributionResultTypeDef = TypedDict(
     "GetStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStreamingDistributionResultTypeDef = TypedDict(
     "UpdateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
@@ -6508,15 +5993,15 @@
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFieldLevelEncryptionListTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionListTypeDef",
     {
         "MaxItems": int,
@@ -6571,24 +6056,24 @@
 
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResponseHeadersPolicyResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicySummaryTypeDef = TypedDict(
     "ResponseHeadersPolicySummaryTypeDef",
     {
         "Type": ResponseHeadersPolicyTypeType,
@@ -6597,15 +6082,15 @@
 )
 
 UpdateResponseHeadersPolicyResultTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDistributionConfigOutputTypeDef = TypedDict(
     "_RequiredDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
@@ -6619,17 +6104,17 @@
     "_OptionalDistributionConfigOutputTypeDef",
     {
         "Aliases": AliasesOutputTypeDef,
         "DefaultRootObject": str,
         "OriginGroups": OriginGroupsOutputTypeDef,
         "CacheBehaviors": CacheBehaviorsOutputTypeDef,
         "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
-        "Logging": LoggingConfigOutputTypeDef,
+        "Logging": LoggingConfigTypeDef,
         "PriceClass": PriceClassType,
-        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "ViewerCertificate": ViewerCertificateTypeDef,
         "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
@@ -6655,15 +6140,15 @@
         "Origins": OriginsOutputTypeDef,
         "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
         "CacheBehaviors": CacheBehaviorsOutputTypeDef,
         "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
-        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "ViewerCertificate": ViewerCertificateTypeDef,
         "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
@@ -6731,33 +6216,33 @@
 
 CreateCachePolicyResultTypeDef = TypedDict(
     "CreateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCachePolicyResultTypeDef = TypedDict(
     "GetCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCachePolicyResultTypeDef = TypedDict(
     "UpdateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOriginRequestPolicyListTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -6789,105 +6274,105 @@
 
 CreateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionProfilesResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     {
         "FieldLevelEncryptionProfileList": FieldLevelEncryptionProfileListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionConfigsResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     {
         "FieldLevelEncryptionList": FieldLevelEncryptionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResponseHeadersPolicyListTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -6938,15 +6423,15 @@
 
 
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
         "DistributionConfig": DistributionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDistributionListTypeDef = TypedDict(
     "_RequiredDistributionListTypeDef",
     {
         "Marker": str,
@@ -7028,15 +6513,15 @@
     pass
 
 
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContinuousDeploymentPolicyListTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -7059,114 +6544,114 @@
     pass
 
 
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionWithTagsResultTypeDef = TypedDict(
     "CreateDistributionWithTagsResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionResultTypeDef = TypedDict(
     "GetDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionWithStagingConfigResultTypeDef = TypedDict(
     "UpdateDistributionWithStagingConfigResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByRealtimeLogConfigResultTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByWebACLIdResultTypeDef = TypedDict(
     "ListDistributionsByWebACLIdResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateDistributionWithTagsRequestRequestTypeDef",
     {
         "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
     },
 )
 
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListContinuousDeploymentPoliciesResultTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesResultTypeDef",
     {
         "ContinuousDeploymentPolicyList": ContinuousDeploymentPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.pyi` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CachePolicyHeaderBehaviorType,
     CachePolicyQueryStringBehaviorType,
     CachePolicyTypeType,
     CertificateSourceType,
     ContinuousDeploymentPolicyTypeType,
     EventTypeType,
     FrameOptionsListType,
+    FunctionRuntimeType,
     FunctionStageType,
     GeoRestrictionTypeType,
     HttpVersionType,
     ICPRecordalStatusType,
     ItemSelectionType,
     MethodType,
     MinimumProtocolVersionType,
@@ -72,34 +73,29 @@
     "TrustedSignersTypeDef",
     "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
     "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
-    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
-    "ContentTypeProfileOutputTypeDef",
     "ContentTypeProfileTypeDef",
     "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
-    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
-    "SessionStickinessConfigOutputTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
-    "CustomErrorResponseOutputTypeDef",
     "CustomErrorResponseTypeDef",
-    "OriginCustomHeaderOutputTypeDef",
     "OriginCustomHeaderTypeDef",
     "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
@@ -111,29 +107,23 @@
     "DeleteOriginAccessControlRequestRequestTypeDef",
     "DeleteOriginRequestPolicyRequestRequestTypeDef",
     "DeletePublicKeyRequestRequestTypeDef",
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
-    "LoggingConfigOutputTypeDef",
-    "ViewerCertificateOutputTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
-    "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
     "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
-    "FunctionAssociationOutputTypeDef",
     "FunctionAssociationTypeDef",
-    "FunctionConfigOutputTypeDef",
     "FunctionMetadataTypeDef",
     "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
@@ -143,115 +133,89 @@
     "WaiterConfigTypeDef",
     "GetDistributionRequestRequestTypeDef",
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
-    "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
     "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
-    "OriginAccessControlConfigOutputTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
-    "PublicKeyConfigOutputTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
     "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
-    "LambdaFunctionAssociationOutputTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
     "ListDistributionsByKeyGroupRequestRequestTypeDef",
     "ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef",
     "ListDistributionsByWebACLIdRequestRequestTypeDef",
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListDistributionsRequestRequestTypeDef",
     "ListFieldLevelEncryptionConfigsRequestRequestTypeDef",
     "ListFieldLevelEncryptionProfilesRequestRequestTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListInvalidationsRequestRequestTypeDef",
     "ListKeyGroupsRequestRequestTypeDef",
     "ListOriginAccessControlsRequestRequestTypeDef",
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
     "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
-    "OriginGroupMemberOutputTypeDef",
     "OriginGroupMemberTypeDef",
-    "OriginShieldOutputTypeDef",
-    "S3OriginConfigOutputTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
-    "QueryArgProfileOutputTypeDef",
     "QueryArgProfileTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
-    "ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
-    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
-    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
-    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
-    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
-    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
-    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
-    "ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
-    "ResponseHeadersPolicyXSSProtectionOutputTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3OriginOutputTypeDef",
     "S3OriginTypeDef",
-    "StreamingLoggingConfigOutputTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
     "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
     "CachePolicyCookiesConfigOutputTypeDef",
     "CookiePreferenceOutputTypeDef",
@@ -264,67 +228,70 @@
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
     "CachePolicyQueryStringsConfigOutputTypeDef",
     "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
     "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
-    "ContinuousDeploymentSingleWeightConfigOutputTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
+    "GetOriginAccessControlConfigResultTypeDef",
+    "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
+    "GetPublicKeyConfigResultTypeDef",
+    "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
     "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
     "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
     "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
-    "EndPointOutputTypeDef",
     "EndPointTypeDef",
     "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
     "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     "GetKeyGroupConfigResultTypeDef",
     "KeyGroupTypeDef",
-    "GetOriginAccessControlConfigResultTypeDef",
-    "OriginAccessControlTypeDef",
-    "GetPublicKeyConfigResultTypeDef",
-    "PublicKeyTypeDef",
     "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
     "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
-    "MonitoringSubscriptionOutputTypeDef",
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
     "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
     "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
@@ -332,15 +299,14 @@
     "QueryArgProfilesTypeDef",
     "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
-    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
     "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "TagsOutputTypeDef",
     "TagsTypeDef",
@@ -353,47 +319,46 @@
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
     "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
-    "TrafficConfigOutputTypeDef",
     "TrafficConfigTypeDef",
+    "CreateOriginAccessControlResultTypeDef",
+    "GetOriginAccessControlResultTypeDef",
+    "UpdateOriginAccessControlResultTypeDef",
+    "CreatePublicKeyResultTypeDef",
+    "GetPublicKeyResultTypeDef",
+    "UpdatePublicKeyResultTypeDef",
     "OriginOutputTypeDef",
     "OriginTypeDef",
     "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
-    "RealtimeLogConfigTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
+    "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
     "CreateKeyGroupResultTypeDef",
     "GetKeyGroupResultTypeDef",
     "KeyGroupSummaryTypeDef",
     "UpdateKeyGroupResultTypeDef",
-    "CreateOriginAccessControlResultTypeDef",
-    "GetOriginAccessControlResultTypeDef",
-    "UpdateOriginAccessControlResultTypeDef",
-    "CreatePublicKeyResultTypeDef",
-    "GetPublicKeyResultTypeDef",
-    "UpdatePublicKeyResultTypeDef",
     "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "ListOriginAccessControlsResultTypeDef",
     "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
     "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
     "ResponseHeadersPolicyConfigOutputTypeDef",
@@ -767,22 +732,14 @@
     },
     total=False,
 )
 
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
-CloudFrontOriginAccessIdentityConfigOutputTypeDef = TypedDict(
-    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "Comment": str,
-    },
-)
-
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -802,34 +759,14 @@
         "Alias": str,
         "DistributionId": str,
         "AccountId": str,
     },
     total=False,
 )
 
-_RequiredContentTypeProfileOutputTypeDef = TypedDict(
-    "_RequiredContentTypeProfileOutputTypeDef",
-    {
-        "Format": Literal["URLEncoded"],
-        "ContentType": str,
-    },
-)
-_OptionalContentTypeProfileOutputTypeDef = TypedDict(
-    "_OptionalContentTypeProfileOutputTypeDef",
-    {
-        "ProfileId": str,
-    },
-    total=False,
-)
-
-class ContentTypeProfileOutputTypeDef(
-    _RequiredContentTypeProfileOutputTypeDef, _OptionalContentTypeProfileOutputTypeDef
-):
-    pass
-
 _RequiredContentTypeProfileTypeDef = TypedDict(
     "_RequiredContentTypeProfileTypeDef",
     {
         "Format": Literal["URLEncoded"],
         "ContentType": str,
     },
 )
@@ -881,38 +818,22 @@
 )
 
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
-ContinuousDeploymentSingleHeaderConfigOutputTypeDef = TypedDict(
-    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
-    {
-        "Header": str,
-        "Value": str,
-    },
-)
-
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
 
-SessionStickinessConfigOutputTypeDef = TypedDict(
-    "SessionStickinessConfigOutputTypeDef",
-    {
-        "IdleTTL": int,
-        "MaximumTTL": int,
-    },
-)
-
 SessionStickinessConfigTypeDef = TypedDict(
     "SessionStickinessConfigTypeDef",
     {
         "IdleTTL": int,
         "MaximumTTL": int,
     },
 )
@@ -925,28 +846,40 @@
     },
 )
 _OptionalCopyDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalCopyDistributionRequestRequestTypeDef",
     {
         "Staging": bool,
         "IfMatch": str,
+        "Enabled": bool,
     },
     total=False,
 )
 
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
 ):
     pass
 
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
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
-        "Runtime": Literal["cloudfront-js-1.0"],
+        "Runtime": FunctionRuntimeType,
     },
 )
 
 _RequiredKeyGroupConfigTypeDef = TypedDict(
     "_RequiredKeyGroupConfigTypeDef",
     {
         "Name": str,
@@ -1001,35 +934,14 @@
     },
     total=False,
 )
 
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
-_RequiredCustomErrorResponseOutputTypeDef = TypedDict(
-    "_RequiredCustomErrorResponseOutputTypeDef",
-    {
-        "ErrorCode": int,
-    },
-)
-_OptionalCustomErrorResponseOutputTypeDef = TypedDict(
-    "_OptionalCustomErrorResponseOutputTypeDef",
-    {
-        "ResponsePagePath": str,
-        "ResponseCode": str,
-        "ErrorCachingMinTTL": int,
-    },
-    total=False,
-)
-
-class CustomErrorResponseOutputTypeDef(
-    _RequiredCustomErrorResponseOutputTypeDef, _OptionalCustomErrorResponseOutputTypeDef
-):
-    pass
-
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -1043,22 +955,14 @@
 )
 
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
-OriginCustomHeaderOutputTypeDef = TypedDict(
-    "OriginCustomHeaderOutputTypeDef",
-    {
-        "HeaderName": str,
-        "HeaderValue": str,
-    },
-)
-
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
@@ -1355,38 +1259,14 @@
 )
 
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
-LoggingConfigOutputTypeDef = TypedDict(
-    "LoggingConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-        "IncludeCookies": bool,
-        "Bucket": str,
-        "Prefix": str,
-    },
-)
-
-ViewerCertificateOutputTypeDef = TypedDict(
-    "ViewerCertificateOutputTypeDef",
-    {
-        "CloudFrontDefaultCertificate": bool,
-        "IAMCertificateId": str,
-        "ACMCertificateArn": str,
-        "SSLSupportMethod": SSLSupportMethodType,
-        "MinimumProtocolVersion": MinimumProtocolVersionType,
-        "Certificate": str,
-        "CertificateSource": CertificateSourceType,
-    },
-    total=False,
-)
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1426,21 +1306,14 @@
 )
 
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFieldPatternsOutputTypeDef = TypedDict(
     "_RequiredFieldPatternsOutputTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFieldPatternsOutputTypeDef = TypedDict(
@@ -1469,22 +1342,14 @@
     },
     total=False,
 )
 
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
-KinesisStreamConfigOutputTypeDef = TypedDict(
-    "KinesisStreamConfigOutputTypeDef",
-    {
-        "RoleARN": str,
-        "StreamARN": str,
-    },
-)
-
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
@@ -1523,38 +1388,22 @@
 )
 
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
-FunctionAssociationOutputTypeDef = TypedDict(
-    "FunctionAssociationOutputTypeDef",
-    {
-        "FunctionARN": str,
-        "EventType": EventTypeType,
-    },
-)
-
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
 
-FunctionConfigOutputTypeDef = TypedDict(
-    "FunctionConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "Runtime": Literal["cloudfront-js-1.0"],
-    },
-)
-
 _RequiredFunctionMetadataTypeDef = TypedDict(
     "_RequiredFunctionMetadataTypeDef",
     {
         "FunctionARN": str,
         "LastModifiedTime": datetime,
     },
 )
@@ -1716,24 +1565,14 @@
 )
 
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
-GetFunctionResultTypeDef = TypedDict(
-    "GetFunctionResultTypeDef",
-    {
-        "FunctionCode": StreamingBody,
-        "ETag": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -1782,36 +1621,14 @@
 GetOriginAccessControlConfigRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredOriginAccessControlConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginAccessControlConfigOutputTypeDef",
-    {
-        "Name": str,
-        "SigningProtocol": Literal["sigv4"],
-        "SigningBehavior": OriginAccessControlSigningBehaviorsType,
-        "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
-    },
-)
-_OptionalOriginAccessControlConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginAccessControlConfigOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class OriginAccessControlConfigOutputTypeDef(
-    _RequiredOriginAccessControlConfigOutputTypeDef, _OptionalOriginAccessControlConfigOutputTypeDef
-):
-    pass
-
 GetOriginAccessControlRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1832,35 +1649,14 @@
 GetPublicKeyConfigRequestRequestTypeDef = TypedDict(
     "GetPublicKeyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredPublicKeyConfigOutputTypeDef = TypedDict(
-    "_RequiredPublicKeyConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "Name": str,
-        "EncodedKey": str,
-    },
-)
-_OptionalPublicKeyConfigOutputTypeDef = TypedDict(
-    "_OptionalPublicKeyConfigOutputTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-class PublicKeyConfigOutputTypeDef(
-    _RequiredPublicKeyConfigOutputTypeDef, _OptionalPublicKeyConfigOutputTypeDef
-):
-    pass
-
 GetPublicKeyRequestRequestTypeDef = TypedDict(
     "GetPublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1957,34 +1753,14 @@
     },
     total=False,
 )
 
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
-_RequiredLambdaFunctionAssociationOutputTypeDef = TypedDict(
-    "_RequiredLambdaFunctionAssociationOutputTypeDef",
-    {
-        "LambdaFunctionARN": str,
-        "EventType": EventTypeType,
-    },
-)
-_OptionalLambdaFunctionAssociationOutputTypeDef = TypedDict(
-    "_OptionalLambdaFunctionAssociationOutputTypeDef",
-    {
-        "IncludeBody": bool,
-    },
-    total=False,
-)
-
-class LambdaFunctionAssociationOutputTypeDef(
-    _RequiredLambdaFunctionAssociationOutputTypeDef, _OptionalLambdaFunctionAssociationOutputTypeDef
-):
-    pass
-
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -2007,18 +1783,20 @@
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
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
 
 ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     {
@@ -2171,22 +1949,14 @@
 
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
-ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2216,34 +1986,14 @@
         "Marker": str,
         "MaxItems": str,
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "DistributionId": str,
-    },
-)
-_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
-    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListInvalidationsRequestRequestTypeDef = TypedDict(
     "_RequiredListInvalidationsRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 _OptionalListInvalidationsRequestRequestTypeDef = TypedDict(
@@ -2312,22 +2062,14 @@
         "Type": ResponseHeadersPolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamingDistributionsRequestRequestTypeDef = TypedDict(
     "ListStreamingDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2336,21 +2078,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
-RealtimeMetricsSubscriptionConfigOutputTypeDef = TypedDict(
-    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
-    {
-        "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
-    },
-)
-
 RealtimeMetricsSubscriptionConfigTypeDef = TypedDict(
     "RealtimeMetricsSubscriptionConfigTypeDef",
     {
         "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
     },
 )
 
@@ -2378,54 +2113,21 @@
     "StatusCodesTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[int],
     },
 )
 
-OriginGroupMemberOutputTypeDef = TypedDict(
-    "OriginGroupMemberOutputTypeDef",
-    {
-        "OriginId": str,
-    },
-)
-
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
     },
 )
 
-_RequiredOriginShieldOutputTypeDef = TypedDict(
-    "_RequiredOriginShieldOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalOriginShieldOutputTypeDef = TypedDict(
-    "_OptionalOriginShieldOutputTypeDef",
-    {
-        "OriginShieldRegion": str,
-    },
-    total=False,
-)
-
-class OriginShieldOutputTypeDef(
-    _RequiredOriginShieldOutputTypeDef, _OptionalOriginShieldOutputTypeDef
-):
-    pass
-
-S3OriginConfigOutputTypeDef = TypedDict(
-    "S3OriginConfigOutputTypeDef",
-    {
-        "OriginAccessIdentity": str,
-    },
-)
-
 _RequiredOriginShieldTypeDef = TypedDict(
     "_RequiredOriginShieldTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOriginShieldTypeDef = TypedDict(
@@ -2442,24 +2144,14 @@
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
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
 _RequiredPublicKeySummaryTypeDef = TypedDict(
     "_RequiredPublicKeySummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatedTime": datetime,
         "EncodedKey": str,
@@ -2480,22 +2172,14 @@
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
 
-QueryArgProfileOutputTypeDef = TypedDict(
-    "QueryArgProfileOutputTypeDef",
-    {
-        "QueryArg": str,
-        "ProfileId": str,
-    },
-)
-
 QueryArgProfileTypeDef = TypedDict(
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
@@ -2584,34 +2268,14 @@
 
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
-_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
-    {
-        "SamplingRate": float,
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
-):
-    pass
-
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
@@ -2624,152 +2288,61 @@
 
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
-ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
-    {
-        "Override": bool,
-        "ContentSecurityPolicy": str,
-    },
-)
-
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
 
-ResponseHeadersPolicyContentTypeOptionsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
-    {
-        "Override": bool,
-    },
-)
-
 ResponseHeadersPolicyContentTypeOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     {
         "Override": bool,
     },
 )
 
-ResponseHeadersPolicyCustomHeaderOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
-    {
-        "Header": str,
-        "Value": str,
-        "Override": bool,
-    },
-)
-
 ResponseHeadersPolicyCustomHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     {
         "Header": str,
         "Value": str,
         "Override": bool,
     },
 )
 
-ResponseHeadersPolicyFrameOptionsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
-    {
-        "Override": bool,
-        "FrameOption": FrameOptionsListType,
-    },
-)
-
 ResponseHeadersPolicyFrameOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     {
         "Override": bool,
         "FrameOption": FrameOptionsListType,
     },
 )
 
-ResponseHeadersPolicyReferrerPolicyOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
-    {
-        "Override": bool,
-        "ReferrerPolicy": ReferrerPolicyListType,
-    },
-)
-
 ResponseHeadersPolicyReferrerPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     {
         "Override": bool,
         "ReferrerPolicy": ReferrerPolicyListType,
     },
 )
 
-ResponseHeadersPolicyRemoveHeaderOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
-    {
-        "Header": str,
-    },
-)
-
 ResponseHeadersPolicyRemoveHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     {
         "Header": str,
     },
 )
 
-_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
-    {
-        "Override": bool,
-        "AccessControlMaxAgeSec": int,
-    },
-)
-_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
-    {
-        "IncludeSubdomains": bool,
-        "Preload": bool,
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef(
-    _RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-    _OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-):
-    pass
-
-_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef",
-    {
-        "Override": bool,
-        "Protection": bool,
-    },
-)
-_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef",
-    {
-        "ModeBlock": bool,
-        "ReportUri": str,
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyXSSProtectionOutputTypeDef(
-    _RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef,
-    _OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef,
-):
-    pass
-
 _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef",
     {
         "Override": bool,
         "AccessControlMaxAgeSec": int,
     },
 )
@@ -2806,50 +2379,22 @@
 
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
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
-S3OriginOutputTypeDef = TypedDict(
-    "S3OriginOutputTypeDef",
-    {
-        "DomainName": str,
-        "OriginAccessIdentity": str,
-    },
-)
-
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
 
-StreamingLoggingConfigOutputTypeDef = TypedDict(
-    "StreamingLoggingConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Bucket": str,
-        "Prefix": str,
-    },
-)
-
 StreamingLoggingConfigTypeDef = TypedDict(
     "StreamingLoggingConfigTypeDef",
     {
         "Enabled": bool,
         "Bucket": str,
         "Prefix": str,
     },
@@ -2859,31 +2404,14 @@
     "TagKeysTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -3254,33 +2782,24 @@
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
 _OptionalCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
     total=False,
 )
 
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
@@ -3345,15 +2864,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesOutputTypeDef = TypedDict(
     "_OptionalContentTypeProfilesOutputTypeDef",
     {
-        "Items": List[ContentTypeProfileOutputTypeDef],
+        "Items": List[ContentTypeProfileTypeDef],
     },
     total=False,
 )
 
 class ContentTypeProfilesOutputTypeDef(
     _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
 ):
@@ -3374,34 +2893,14 @@
 )
 
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
-_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
-    "_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef",
-    {
-        "Weight": float,
-    },
-)
-_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
-    "_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef",
-    {
-        "SessionStickinessConfig": SessionStickinessConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class ContinuousDeploymentSingleWeightConfigOutputTypeDef(
-    _RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef,
-    _OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef,
-):
-    pass
-
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
@@ -3414,14 +2913,40 @@
 
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    {
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionResultTypeDef = TypedDict(
+    "GetFunctionResultTypeDef",
+    {
+        "FunctionCode": StreamingBody,
+        "ETag": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -3467,14 +2992,42 @@
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
+GetOriginAccessControlConfigResultTypeDef = TypedDict(
+    "GetOriginAccessControlConfigResultTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredOriginAccessControlTypeDef = TypedDict(
+    "_RequiredOriginAccessControlTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalOriginAccessControlTypeDef = TypedDict(
+    "_OptionalOriginAccessControlTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
+    },
+    total=False,
+)
+
+class OriginAccessControlTypeDef(
+    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
+):
+    pass
+
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -3495,14 +3048,32 @@
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
+GetPublicKeyConfigResultTypeDef = TypedDict(
+    "GetPublicKeyConfigResultTypeDef",
+    {
+        "PublicKeyConfig": PublicKeyConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublicKeyTypeDef = TypedDict(
+    "PublicKeyTypeDef",
+    {
+        "Id": str,
+        "CreatedTime": datetime,
+        "PublicKeyConfig": PublicKeyConfigTypeDef,
+    },
+)
+
 _RequiredUpdatePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "Id": str,
     },
 )
@@ -3524,15 +3095,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesOutputTypeDef",
     {
-        "Items": List[CustomErrorResponseOutputTypeDef],
+        "Items": List[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
 class CustomErrorResponsesOutputTypeDef(
     _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
 ):
@@ -3562,15 +3133,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersOutputTypeDef = TypedDict(
     "_OptionalCustomHeadersOutputTypeDef",
     {
-        "Items": List[OriginCustomHeaderOutputTypeDef],
+        "Items": List[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
 class CustomHeadersOutputTypeDef(
     _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
 ):
@@ -3639,39 +3210,39 @@
 ):
     pass
 
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByKeyGroupResultTypeDef = TypedDict(
     "ListDistributionsByKeyGroupResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByOriginRequestPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EncryptionEntityOutputTypeDef = TypedDict(
     "EncryptionEntityOutputTypeDef",
     {
         "PublicKeyId": str,
@@ -3685,31 +3256,14 @@
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
 )
 
-_RequiredEndPointOutputTypeDef = TypedDict(
-    "_RequiredEndPointOutputTypeDef",
-    {
-        "StreamType": str,
-    },
-)
-_OptionalEndPointOutputTypeDef = TypedDict(
-    "_OptionalEndPointOutputTypeDef",
-    {
-        "KinesisStreamConfig": KinesisStreamConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class EndPointOutputTypeDef(_RequiredEndPointOutputTypeDef, _OptionalEndPointOutputTypeDef):
-    pass
-
 _RequiredEndPointTypeDef = TypedDict(
     "_RequiredEndPointTypeDef",
     {
         "StreamType": str,
     },
 )
 _OptionalEndPointTypeDef = TypedDict(
@@ -3728,15 +3282,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsOutputTypeDef = TypedDict(
     "_OptionalFunctionAssociationsOutputTypeDef",
     {
-        "Items": List[FunctionAssociationOutputTypeDef],
+        "Items": List[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
 class FunctionAssociationsOutputTypeDef(
     _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
 ):
@@ -3761,15 +3315,15 @@
 ):
     pass
 
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
-        "FunctionConfig": FunctionConfigOutputTypeDef,
+        "FunctionConfig": FunctionConfigTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
 )
 _OptionalFunctionSummaryTypeDef = TypedDict(
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
@@ -3856,73 +3410,27 @@
     pass
 
 GetKeyGroupConfigResultTypeDef = TypedDict(
     "GetKeyGroupConfigResultTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KeyGroupTypeDef = TypedDict(
     "KeyGroupTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
     },
 )
 
-GetOriginAccessControlConfigResultTypeDef = TypedDict(
-    "GetOriginAccessControlConfigResultTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredOriginAccessControlTypeDef = TypedDict(
-    "_RequiredOriginAccessControlTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalOriginAccessControlTypeDef = TypedDict(
-    "_OptionalOriginAccessControlTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class OriginAccessControlTypeDef(
-    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
-):
-    pass
-
-GetPublicKeyConfigResultTypeDef = TypedDict(
-    "GetPublicKeyConfigResultTypeDef",
-    {
-        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PublicKeyTypeDef = TypedDict(
-    "PublicKeyTypeDef",
-    {
-        "Id": str,
-        "CreatedTime": datetime,
-        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
-    },
-)
-
 InvalidationBatchOutputTypeDef = TypedDict(
     "InvalidationBatchOutputTypeDef",
     {
         "Paths": PathsOutputTypeDef,
         "CallerReference": str,
     },
 )
@@ -3979,15 +3487,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsOutputTypeDef",
     {
-        "Items": List[LambdaFunctionAssociationOutputTypeDef],
+        "Items": List[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
 class LambdaFunctionAssociationsOutputTypeDef(
     _RequiredLambdaFunctionAssociationsOutputTypeDef,
     _OptionalLambdaFunctionAssociationsOutputTypeDef,
@@ -4009,18 +3517,54 @@
 )
 
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
-MonitoringSubscriptionOutputTypeDef = TypedDict(
-    "MonitoringSubscriptionOutputTypeDef",
+ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     {
-        "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "DistributionId": str,
+    },
+)
+_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
+    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
+):
+    pass
+
+ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
@@ -4066,15 +3610,15 @@
     },
 )
 
 OriginGroupMembersOutputTypeDef = TypedDict(
     "OriginGroupMembersOutputTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginGroupMemberOutputTypeDef],
+        "Items": List[OriginGroupMemberTypeDef],
     },
 )
 
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
@@ -4106,15 +3650,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalQueryArgProfilesOutputTypeDef = TypedDict(
     "_OptionalQueryArgProfilesOutputTypeDef",
     {
-        "Items": List[QueryArgProfileOutputTypeDef],
+        "Items": List[QueryArgProfileTypeDef],
     },
     total=False,
 )
 
 class QueryArgProfilesOutputTypeDef(
     _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
 ):
@@ -4191,15 +3735,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     {
-        "Items": List[ResponseHeadersPolicyCustomHeaderOutputTypeDef],
+        "Items": List[ResponseHeadersPolicyCustomHeaderTypeDef],
     },
     total=False,
 )
 
 class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
@@ -4231,15 +3775,15 @@
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     {
-        "Items": List[ResponseHeadersPolicyRemoveHeaderOutputTypeDef],
+        "Items": List[ResponseHeadersPolicyRemoveHeaderTypeDef],
     },
     total=False,
 )
 
 class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
@@ -4262,27 +3806,14 @@
 
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
-ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
-    {
-        "XSSProtection": ResponseHeadersPolicyXSSProtectionOutputTypeDef,
-        "FrameOptions": ResponseHeadersPolicyFrameOptionsOutputTypeDef,
-        "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
-        "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
-        "ContentTypeOptions": ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
-        "StrictTransportSecurity": ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-    },
-    total=False,
-)
-
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -4296,38 +3827,38 @@
     "StreamingDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "S3Origin": S3OriginOutputTypeDef,
+        "S3Origin": S3OriginTypeDef,
         "Aliases": AliasesOutputTypeDef,
         "TrustedSigners": TrustedSignersOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
 _RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
-        "S3Origin": S3OriginOutputTypeDef,
+        "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersOutputTypeDef,
         "Enabled": bool,
     },
 )
 _OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
     "_OptionalStreamingDistributionConfigOutputTypeDef",
     {
         "Aliases": AliasesOutputTypeDef,
-        "Logging": StreamingLoggingConfigOutputTypeDef,
+        "Logging": StreamingLoggingConfigTypeDef,
         "PriceClass": PriceClassType,
     },
     total=False,
 )
 
 class StreamingDistributionConfigOutputTypeDef(
     _RequiredStreamingDistributionConfigOutputTypeDef,
@@ -4367,15 +3898,15 @@
         "TagKeys": TagKeysTypeDef,
     },
 )
 
 TagsOutputTypeDef = TypedDict(
     "TagsOutputTypeDef",
     {
-        "Items": List[TagOutputTypeDef],
+        "Items": List[TagTypeDef],
     },
     total=False,
 )
 
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
@@ -4516,49 +4047,49 @@
 
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCloudFrontOriginAccessIdentitiesResultTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     {
         "CloudFrontOriginAccessIdentityList": CloudFrontOriginAccessIdentityListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigOutputTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
@@ -4592,69 +4123,105 @@
 )
 
 class ContentTypeProfileConfigTypeDef(
     _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
 ):
     pass
 
-_RequiredTrafficConfigOutputTypeDef = TypedDict(
-    "_RequiredTrafficConfigOutputTypeDef",
+_RequiredTrafficConfigTypeDef = TypedDict(
+    "_RequiredTrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
-_OptionalTrafficConfigOutputTypeDef = TypedDict(
-    "_OptionalTrafficConfigOutputTypeDef",
+_OptionalTrafficConfigTypeDef = TypedDict(
+    "_OptionalTrafficConfigTypeDef",
     {
-        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigOutputTypeDef,
-        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
+        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
+        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
     total=False,
 )
 
-class TrafficConfigOutputTypeDef(
-    _RequiredTrafficConfigOutputTypeDef, _OptionalTrafficConfigOutputTypeDef
-):
+class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
     pass
 
-_RequiredTrafficConfigTypeDef = TypedDict(
-    "_RequiredTrafficConfigTypeDef",
+CreateOriginAccessControlResultTypeDef = TypedDict(
+    "CreateOriginAccessControlResultTypeDef",
     {
-        "Type": ContinuousDeploymentPolicyTypeType,
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTrafficConfigTypeDef = TypedDict(
-    "_OptionalTrafficConfigTypeDef",
+
+GetOriginAccessControlResultTypeDef = TypedDict(
+    "GetOriginAccessControlResultTypeDef",
     {
-        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
-        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
-    pass
+UpdateOriginAccessControlResultTypeDef = TypedDict(
+    "UpdateOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePublicKeyResultTypeDef = TypedDict(
+    "CreatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicKeyResultTypeDef = TypedDict(
+    "GetPublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePublicKeyResultTypeDef = TypedDict(
+    "UpdatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredOriginOutputTypeDef = TypedDict(
     "_RequiredOriginOutputTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
 )
 _OptionalOriginOutputTypeDef = TypedDict(
     "_OptionalOriginOutputTypeDef",
     {
         "OriginPath": str,
         "CustomHeaders": CustomHeadersOutputTypeDef,
-        "S3OriginConfig": S3OriginConfigOutputTypeDef,
+        "S3OriginConfig": S3OriginConfigTypeDef,
         "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
         "ConnectionAttempts": int,
         "ConnectionTimeout": int,
-        "OriginShield": OriginShieldOutputTypeDef,
+        "OriginShield": OriginShieldTypeDef,
         "OriginAccessControlId": str,
     },
     total=False,
 )
 
 class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
     pass
@@ -4718,32 +4285,32 @@
 )
 
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
-RealtimeLogConfigTypeDef = TypedDict(
-    "RealtimeLogConfigTypeDef",
+CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
+    "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
-        "ARN": str,
+        "EndPoints": Sequence[EndPointTypeDef],
+        "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
-        "EndPoints": List[EndPointOutputTypeDef],
-        "Fields": List[str],
     },
 )
 
-CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
-    "CreateRealtimeLogConfigRequestRequestTypeDef",
+RealtimeLogConfigTypeDef = TypedDict(
+    "RealtimeLogConfigTypeDef",
     {
-        "EndPoints": Sequence[EndPointTypeDef],
-        "Fields": Sequence[str],
+        "ARN": str,
         "Name": str,
         "SamplingRate": int,
+        "EndPoints": List[EndPointTypeDef],
+        "Fields": List[str],
     },
 )
 
 UpdateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
@@ -4757,24 +4324,24 @@
 
 CreateFunctionResultTypeDef = TypedDict(
     "CreateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFunctionResultTypeDef = TypedDict(
     "DescribeFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionListTypeDef = TypedDict(
     "_RequiredFunctionListTypeDef",
     {
         "MaxItems": int,
@@ -4793,15 +4360,15 @@
 class FunctionListTypeDef(_RequiredFunctionListTypeDef, _OptionalFunctionListTypeDef):
     pass
 
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestResultTypeDef = TypedDict(
     "TestResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
@@ -4814,34 +4381,34 @@
 )
 
 UpdateFunctionResultTypeDef = TypedDict(
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeyGroupResultTypeDef = TypedDict(
     "CreateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyGroupResultTypeDef = TypedDict(
     "GetKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KeyGroupSummaryTypeDef = TypedDict(
     "KeyGroupSummaryTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
@@ -4849,71 +4416,15 @@
 )
 
 UpdateKeyGroupResultTypeDef = TypedDict(
     "UpdateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateOriginAccessControlResultTypeDef = TypedDict(
-    "CreateOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetOriginAccessControlResultTypeDef = TypedDict(
-    "GetOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateOriginAccessControlResultTypeDef = TypedDict(
-    "UpdateOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePublicKeyResultTypeDef = TypedDict(
-    "CreatePublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPublicKeyResultTypeDef = TypedDict(
-    "GetPublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePublicKeyResultTypeDef = TypedDict(
-    "UpdatePublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
@@ -4931,15 +4442,15 @@
     },
 )
 
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActiveTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredActiveTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
@@ -4975,43 +4486,43 @@
 )
 
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
-CreateMonitoringSubscriptionResultTypeDef = TypedDict(
-    "CreateMonitoringSubscriptionResultTypeDef",
+CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DistributionId": str,
+        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
     },
 )
 
-GetMonitoringSubscriptionResultTypeDef = TypedDict(
-    "GetMonitoringSubscriptionResultTypeDef",
+CreateMonitoringSubscriptionResultTypeDef = TypedDict(
+    "CreateMonitoringSubscriptionResultTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
+GetMonitoringSubscriptionResultTypeDef = TypedDict(
+    "GetMonitoringSubscriptionResultTypeDef",
     {
-        "DistributionId": str,
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginGroupOutputTypeDef = TypedDict(
     "OriginGroupOutputTypeDef",
     {
         "Id": str,
@@ -5029,15 +4540,15 @@
     },
 )
 
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigOutputTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
@@ -5082,16 +4593,16 @@
     },
 )
 _OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
     {
         "Comment": str,
         "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
-        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
-        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigTypeDef,
+        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
         "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
         "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     },
     total=False,
 )
 
 class ResponseHeadersPolicyConfigOutputTypeDef(
@@ -5148,15 +4659,15 @@
     pass
 
 GetStreamingDistributionConfigResultTypeDef = TypedDict(
     "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -5184,15 +4695,15 @@
 ):
     pass
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": TagsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -5374,15 +4885,15 @@
     pass
 
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
@@ -5448,15 +4959,15 @@
         "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
         "Enabled": bool,
     },
 )
 _OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
     "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
     {
-        "TrafficConfig": TrafficConfigOutputTypeDef,
+        "TrafficConfig": TrafficConfigTypeDef,
     },
     total=False,
 )
 
 class ContinuousDeploymentPolicyConfigOutputTypeDef(
     _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
     _OptionalContinuousDeploymentPolicyConfigOutputTypeDef,
@@ -5567,23 +5078,23 @@
 ):
     pass
 
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRealtimeLogConfigResultTypeDef = TypedDict(
     "GetRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRealtimeLogConfigsTypeDef = TypedDict(
     "_RequiredRealtimeLogConfigsTypeDef",
     {
         "MaxItems": int,
@@ -5605,31 +5116,31 @@
 ):
     pass
 
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResultTypeDef = TypedDict(
     "ListFunctionsResultTypeDef",
     {
         "FunctionList": FunctionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFunctionResultTypeDef = TypedDict(
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyGroupListTypeDef = TypedDict(
     "_RequiredKeyGroupListTypeDef",
     {
         "MaxItems": int,
@@ -5649,23 +5160,23 @@
     pass
 
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvalidationResultTypeDef = TypedDict(
     "GetInvalidationResultTypeDef",
     {
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStreamingDistributionTypeDef = TypedDict(
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
@@ -5791,15 +5302,15 @@
     pass
 
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
@@ -5836,15 +5347,15 @@
 ):
     pass
 
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
@@ -5897,34 +5408,34 @@
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginRequestPolicyResultTypeDef = TypedDict(
     "GetOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicySummaryTypeDef = TypedDict(
     "OriginRequestPolicySummaryTypeDef",
     {
         "Type": OriginRequestPolicyTypeType,
@@ -5933,15 +5444,15 @@
 )
 
 UpdateOriginRequestPolicyResultTypeDef = TypedDict(
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCachePolicyRequestRequestTypeDef = TypedDict(
     "CreateCachePolicyRequestRequestTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
@@ -5978,15 +5489,15 @@
 )
 
 GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -6024,15 +5535,15 @@
 )
 
 GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
         "MaxItems": int,
@@ -6081,61 +5592,61 @@
 ):
     pass
 
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeyGroupsResultTypeDef = TypedDict(
     "ListKeyGroupsResultTypeDef",
     {
         "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsResultTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingDistributionResultTypeDef = TypedDict(
     "GetStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStreamingDistributionResultTypeDef = TypedDict(
     "UpdateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
@@ -6145,15 +5656,15 @@
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFieldLevelEncryptionListTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionListTypeDef",
     {
         "MaxItems": int,
@@ -6204,24 +5715,24 @@
 
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResponseHeadersPolicyResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicySummaryTypeDef = TypedDict(
     "ResponseHeadersPolicySummaryTypeDef",
     {
         "Type": ResponseHeadersPolicyTypeType,
@@ -6230,15 +5741,15 @@
 )
 
 UpdateResponseHeadersPolicyResultTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDistributionConfigOutputTypeDef = TypedDict(
     "_RequiredDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
@@ -6252,17 +5763,17 @@
     "_OptionalDistributionConfigOutputTypeDef",
     {
         "Aliases": AliasesOutputTypeDef,
         "DefaultRootObject": str,
         "OriginGroups": OriginGroupsOutputTypeDef,
         "CacheBehaviors": CacheBehaviorsOutputTypeDef,
         "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
-        "Logging": LoggingConfigOutputTypeDef,
+        "Logging": LoggingConfigTypeDef,
         "PriceClass": PriceClassType,
-        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "ViewerCertificate": ViewerCertificateTypeDef,
         "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
@@ -6286,15 +5797,15 @@
         "Origins": OriginsOutputTypeDef,
         "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
         "CacheBehaviors": CacheBehaviorsOutputTypeDef,
         "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
-        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "ViewerCertificate": ViewerCertificateTypeDef,
         "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
@@ -6358,33 +5869,33 @@
 
 CreateCachePolicyResultTypeDef = TypedDict(
     "CreateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCachePolicyResultTypeDef = TypedDict(
     "GetCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCachePolicyResultTypeDef = TypedDict(
     "UpdateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOriginRequestPolicyListTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -6414,105 +5925,105 @@
 
 CreateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionProfilesResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     {
         "FieldLevelEncryptionProfileList": FieldLevelEncryptionProfileListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionConfigsResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     {
         "FieldLevelEncryptionList": FieldLevelEncryptionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResponseHeadersPolicyListTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -6559,15 +6070,15 @@
     pass
 
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
         "DistributionConfig": DistributionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDistributionListTypeDef = TypedDict(
     "_RequiredDistributionListTypeDef",
     {
         "Marker": str,
@@ -6643,15 +6154,15 @@
 class CachePolicyListTypeDef(_RequiredCachePolicyListTypeDef, _OptionalCachePolicyListTypeDef):
     pass
 
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContinuousDeploymentPolicyListTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -6672,114 +6183,114 @@
 ):
     pass
 
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionWithTagsResultTypeDef = TypedDict(
     "CreateDistributionWithTagsResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionResultTypeDef = TypedDict(
     "GetDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionWithStagingConfigResultTypeDef = TypedDict(
     "UpdateDistributionWithStagingConfigResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByRealtimeLogConfigResultTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByWebACLIdResultTypeDef = TypedDict(
     "ListDistributionsByWebACLIdResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateDistributionWithTagsRequestRequestTypeDef",
     {
         "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
     },
 )
 
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListContinuousDeploymentPoliciesResultTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesResultTypeDef",
     {
         "ContinuousDeploymentPolicyList": ContinuousDeploymentPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.py` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.pyi` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/PKG-INFO` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudFront 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -422,34 +422,29 @@
     TrustedSignersTypeDef,
     CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
     QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
-    CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
-    ContentTypeProfileOutputTypeDef,
     ContentTypeProfileTypeDef,
     StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
-    ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
-    SessionStickinessConfigOutputTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
-    CustomErrorResponseOutputTypeDef,
     CustomErrorResponseTypeDef,
-    OriginCustomHeaderOutputTypeDef,
     OriginCustomHeaderTypeDef,
     OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
@@ -461,29 +456,23 @@
     DeleteOriginAccessControlRequestRequestTypeDef,
     DeleteOriginRequestPolicyRequestRequestTypeDef,
     DeletePublicKeyRequestRequestTypeDef,
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
-    LoggingConfigOutputTypeDef,
-    ViewerCertificateOutputTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
-    EmptyResponseMetadataTypeDef,
     FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
-    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
     QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
-    FunctionAssociationOutputTypeDef,
     FunctionAssociationTypeDef,
-    FunctionConfigOutputTypeDef,
     FunctionMetadataTypeDef,
     GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
@@ -493,115 +482,89 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
-    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
     KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
-    OriginAccessControlConfigOutputTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
-    PublicKeyConfigOutputTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
     PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
-    LambdaFunctionAssociationOutputTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RealtimeMetricsSubscriptionConfigOutputTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
     StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
-    OriginGroupMemberOutputTypeDef,
     OriginGroupMemberTypeDef,
-    OriginShieldOutputTypeDef,
-    S3OriginConfigOutputTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
-    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
-    QueryArgProfileOutputTypeDef,
     QueryArgProfileTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
-    ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
-    ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
-    ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
-    ResponseHeadersPolicyCustomHeaderOutputTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
-    ResponseHeadersPolicyFrameOptionsOutputTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
-    ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
-    ResponseHeadersPolicyRemoveHeaderOutputTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
-    ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
-    ResponseHeadersPolicyXSSProtectionOutputTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
-    ResponseMetadataTypeDef,
-    S3OriginOutputTypeDef,
     S3OriginTypeDef,
-    StreamingLoggingConfigOutputTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
     CachePolicyCookiesConfigOutputTypeDef,
     CookiePreferenceOutputTypeDef,
@@ -614,67 +577,70 @@
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
     CachePolicyQueryStringsConfigOutputTypeDef,
     OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
     ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
-    ContinuousDeploymentSingleWeightConfigOutputTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
+    GetOriginAccessControlConfigResultTypeDef,
+    OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
+    GetPublicKeyConfigResultTypeDef,
+    PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
     CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
     CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
     CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
     EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
-    EndPointOutputTypeDef,
     EndPointTypeDef,
     FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
     RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     GetKeyGroupConfigResultTypeDef,
     KeyGroupTypeDef,
-    GetOriginAccessControlConfigResultTypeDef,
-    OriginAccessControlTypeDef,
-    GetPublicKeyConfigResultTypeDef,
-    PublicKeyTypeDef,
     InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
-    MonitoringSubscriptionOutputTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
     OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
     OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
@@ -682,15 +648,14 @@
     QueryArgProfilesTypeDef,
     ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
-    ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
     StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagsOutputTypeDef,
     TagsTypeDef,
@@ -703,47 +668,46 @@
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
-    TrafficConfigOutputTypeDef,
     TrafficConfigTypeDef,
+    CreateOriginAccessControlResultTypeDef,
+    GetOriginAccessControlResultTypeDef,
+    UpdateOriginAccessControlResultTypeDef,
+    CreatePublicKeyResultTypeDef,
+    GetPublicKeyResultTypeDef,
+    UpdatePublicKeyResultTypeDef,
     OriginOutputTypeDef,
     OriginTypeDef,
     EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
-    RealtimeLogConfigTypeDef,
     CreateRealtimeLogConfigRequestRequestTypeDef,
+    RealtimeLogConfigTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
     CreateKeyGroupResultTypeDef,
     GetKeyGroupResultTypeDef,
     KeyGroupSummaryTypeDef,
     UpdateKeyGroupResultTypeDef,
-    CreateOriginAccessControlResultTypeDef,
-    GetOriginAccessControlResultTypeDef,
-    UpdateOriginAccessControlResultTypeDef,
-    CreatePublicKeyResultTypeDef,
-    GetPublicKeyResultTypeDef,
-    UpdatePublicKeyResultTypeDef,
     InvalidationTypeDef,
     CreateInvalidationRequestRequestTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
+    CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
-    CreateMonitoringSubscriptionRequestRequestTypeDef,
     ListOriginAccessControlsResultTypeDef,
     OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
     QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
     ResponseHeadersPolicyConfigOutputTypeDef,
```

### Comparing `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/SOURCES.txt` & `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.12/setup.py` & `mypy-boto3-cloudfront-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudfront",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFront 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

