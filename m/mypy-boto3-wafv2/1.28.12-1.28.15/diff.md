# Comparing `tmp/mypy-boto3-wafv2-1.28.12.tar.gz` & `tmp/mypy-boto3-wafv2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.28.15.tar", last modified: Fri Jul 28 20:43:56 2023, max compression
```

## Comparing `mypy-boto3-wafv2-1.28.12.tar` & `mypy-boto3-wafv2-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.453491 mypy-boto3-wafv2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-07-27 11:49:49.449491 mypy-boto3-wafv2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.445491 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-27 11:48:39.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94383 2023-07-27 11:48:41.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94278 2023-07-27 11:48:40.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.449491 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 11:49:49.000000 mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.453491 mypy-boto3-wafv2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 11:48:38.000000 mypy-boto3-wafv2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.306036 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-07-28 20:41:19.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    87748 2023-07-28 20:41:22.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87645 2023-07-28 20:41:20.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:56.000000 mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:56.314036 mypy-boto3-wafv2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:41:18.000000 mypy-boto3-wafv2-1.28.15/setup.py
```

### Comparing `mypy-boto3-wafv2-1.28.12/LICENSE` & `mypy-boto3-wafv2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.12/PKG-INFO` & `mypy-boto3-wafv2-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.28.12
-Summary: Type annotations for boto3.WAFV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,75 +322,58 @@
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
-    AWSManagedRulesBotControlRuleSetOutputTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
-    ActionConditionOutputTypeDef,
     ActionConditionTypeDef,
-    AddressFieldOutputTypeDef,
     AddressFieldTypeDef,
     AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
-    RequestBodyAssociatedResourceTypeConfigOutputTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
-    BodyOutputTypeDef,
     BodyTypeDef,
-    TextTransformationOutputTypeDef,
     TextTransformationTypeDef,
-    ImmunityTimePropertyOutputTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
     ResponseMetadataTypeDef,
-    LabelNameConditionOutputTypeDef,
     LabelNameConditionTypeDef,
     CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
-    CustomHTTPHeaderOutputTypeDef,
     CustomHTTPHeaderTypeDef,
-    CustomResponseBodyOutputTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
     ManagedProductDescriptorTypeDef,
     DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
-    EmailFieldOutputTypeDef,
     EmailFieldTypeDef,
-    ExcludedRuleOutputTypeDef,
     ExcludedRuleTypeDef,
-    HeaderOrderOutputTypeDef,
-    SingleHeaderOutputTypeDef,
-    SingleQueryArgumentOutputTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
-    VisibilityConfigOutputTypeDef,
-    ForwardedIPConfigOutputTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
@@ -403,21 +386,18 @@
     TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
-    IPSetForwardedIPConfigOutputTypeDef,
     IPSetForwardedIPConfigTypeDef,
     JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
-    LabelMatchStatementOutputTypeDef,
     LabelMatchStatementTypeDef,
-    LabelOutputTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
@@ -427,56 +407,47 @@
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
-    PasswordFieldOutputTypeDef,
-    UsernameFieldOutputTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
-    TagOutputTypeDef,
-    NotStatementOutputTypeDef,
     NotStatementTypeDef,
     OrStatementOutputTypeDef,
     OrStatementTypeDef,
-    PhoneNumberFieldOutputTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
-    RateLimitLabelNamespaceOutputTypeDef,
     RateLimitLabelNamespaceTypeDef,
-    RegexOutputTypeDef,
     ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     RateLimitCookieOutputTypeDef,
-    RateLimitHeaderOutputTypeDef,
-    RateLimitQueryArgumentOutputTypeDef,
-    RateLimitQueryStringOutputTypeDef,
-    RateLimitUriPathOutputTypeDef,
     RateLimitCookieTypeDef,
+    RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
     RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringOutputTypeDef,
     RateLimitQueryStringTypeDef,
+    RateLimitUriPathOutputTypeDef,
     RateLimitUriPathTypeDef,
-    CaptchaConfigOutputTypeDef,
-    ChallengeConfigOutputTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
@@ -485,96 +456,93 @@
     ListResourcesForWebACLResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
-    ConditionOutputTypeDef,
     ConditionTypeDef,
     CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
+    MobileSdkReleaseTypeDef,
+    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
+    RegexPatternSetTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
     CustomRequestHandlingOutputTypeDef,
-    CustomResponseOutputTypeDef,
     CustomRequestHandlingTypeDef,
+    CustomResponseOutputTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
-    IPSetReferenceStatementOutputTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
-    RequestInspectionOutputTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
-    MobileSdkReleaseTypeDef,
-    TagInfoForResourceTypeDef,
     RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
-    RegexPatternSetTypeDef,
     ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
     RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
     FilterOutputTypeDef,
     FilterTypeDef,
+    GetMobileSdkReleaseResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetRegexPatternSetResponseTypeDef,
     AllowActionOutputTypeDef,
     CaptchaActionOutputTypeDef,
     ChallengeActionOutputTypeDef,
     CountActionOutputTypeDef,
-    BlockActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
+    BlockActionOutputTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
     FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
-    GetMobileSdkReleaseResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetRegexPatternSetResponseTypeDef,
     AWSManagedRulesACFPRuleSetOutputTypeDef,
     AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
     RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
     LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
     OverrideActionOutputTypeDef,
+    OverrideActionTypeDef,
     DefaultActionOutputTypeDef,
     RuleActionOutputTypeDef,
-    OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
     ByteMatchStatementOutputTypeDef,
     RegexMatchStatementOutputTypeDef,
     RegexPatternSetReferenceStatementOutputTypeDef,
     SizeConstraintStatementOutputTypeDef,
```

### Comparing `mypy-boto3-wafv2-1.28.12/README.md` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-wafv2
+Version: 1.28.15
+Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 wafv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-wafv2"></a>
 
 # mypy-boto3-wafv2
 
 [![PyPI - mypy-boto3-wafv2](https://img.shields.io/pypi/v/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,75 +322,58 @@
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
-    AWSManagedRulesBotControlRuleSetOutputTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
-    ActionConditionOutputTypeDef,
     ActionConditionTypeDef,
-    AddressFieldOutputTypeDef,
     AddressFieldTypeDef,
     AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
-    RequestBodyAssociatedResourceTypeConfigOutputTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
-    BodyOutputTypeDef,
     BodyTypeDef,
-    TextTransformationOutputTypeDef,
     TextTransformationTypeDef,
-    ImmunityTimePropertyOutputTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
     ResponseMetadataTypeDef,
-    LabelNameConditionOutputTypeDef,
     LabelNameConditionTypeDef,
     CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
-    CustomHTTPHeaderOutputTypeDef,
     CustomHTTPHeaderTypeDef,
-    CustomResponseBodyOutputTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
     ManagedProductDescriptorTypeDef,
     DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
-    EmailFieldOutputTypeDef,
     EmailFieldTypeDef,
-    ExcludedRuleOutputTypeDef,
     ExcludedRuleTypeDef,
-    HeaderOrderOutputTypeDef,
-    SingleHeaderOutputTypeDef,
-    SingleQueryArgumentOutputTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
-    VisibilityConfigOutputTypeDef,
-    ForwardedIPConfigOutputTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
@@ -371,21 +386,18 @@
     TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
-    IPSetForwardedIPConfigOutputTypeDef,
     IPSetForwardedIPConfigTypeDef,
     JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
-    LabelMatchStatementOutputTypeDef,
     LabelMatchStatementTypeDef,
-    LabelOutputTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
@@ -395,56 +407,47 @@
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
-    PasswordFieldOutputTypeDef,
-    UsernameFieldOutputTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
-    TagOutputTypeDef,
-    NotStatementOutputTypeDef,
     NotStatementTypeDef,
     OrStatementOutputTypeDef,
     OrStatementTypeDef,
-    PhoneNumberFieldOutputTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
-    RateLimitLabelNamespaceOutputTypeDef,
     RateLimitLabelNamespaceTypeDef,
-    RegexOutputTypeDef,
     ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     RateLimitCookieOutputTypeDef,
-    RateLimitHeaderOutputTypeDef,
-    RateLimitQueryArgumentOutputTypeDef,
-    RateLimitQueryStringOutputTypeDef,
-    RateLimitUriPathOutputTypeDef,
     RateLimitCookieTypeDef,
+    RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
     RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringOutputTypeDef,
     RateLimitQueryStringTypeDef,
+    RateLimitUriPathOutputTypeDef,
     RateLimitUriPathTypeDef,
-    CaptchaConfigOutputTypeDef,
-    ChallengeConfigOutputTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
@@ -453,96 +456,93 @@
     ListResourcesForWebACLResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
-    ConditionOutputTypeDef,
     ConditionTypeDef,
     CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
+    MobileSdkReleaseTypeDef,
+    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
+    RegexPatternSetTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
     CustomRequestHandlingOutputTypeDef,
-    CustomResponseOutputTypeDef,
     CustomRequestHandlingTypeDef,
+    CustomResponseOutputTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
-    IPSetReferenceStatementOutputTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
-    RequestInspectionOutputTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
-    MobileSdkReleaseTypeDef,
-    TagInfoForResourceTypeDef,
     RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
-    RegexPatternSetTypeDef,
     ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
     RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
     FilterOutputTypeDef,
     FilterTypeDef,
+    GetMobileSdkReleaseResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetRegexPatternSetResponseTypeDef,
     AllowActionOutputTypeDef,
     CaptchaActionOutputTypeDef,
     ChallengeActionOutputTypeDef,
     CountActionOutputTypeDef,
-    BlockActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
+    BlockActionOutputTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
     FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
-    GetMobileSdkReleaseResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetRegexPatternSetResponseTypeDef,
     AWSManagedRulesACFPRuleSetOutputTypeDef,
     AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
     RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
     LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
     OverrideActionOutputTypeDef,
+    OverrideActionTypeDef,
     DefaultActionOutputTypeDef,
     RuleActionOutputTypeDef,
-    OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
     ByteMatchStatementOutputTypeDef,
     RegexMatchStatementOutputTypeDef,
     RegexPatternSetReferenceStatementOutputTypeDef,
     SizeConstraintStatementOutputTypeDef,
```

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.WAFV2 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,75 +53,58 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "APIKeySummaryTypeDef",
-    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
-    "ActionConditionOutputTypeDef",
     "ActionConditionTypeDef",
-    "AddressFieldOutputTypeDef",
     "AddressFieldTypeDef",
     "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
-    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
-    "BodyOutputTypeDef",
     "BodyTypeDef",
-    "TextTransformationOutputTypeDef",
     "TextTransformationTypeDef",
-    "ImmunityTimePropertyOutputTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
     "ResponseMetadataTypeDef",
-    "LabelNameConditionOutputTypeDef",
     "LabelNameConditionTypeDef",
     "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
-    "CustomHTTPHeaderOutputTypeDef",
     "CustomHTTPHeaderTypeDef",
-    "CustomResponseBodyOutputTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DescribeAllManagedProductsRequestRequestTypeDef",
     "ManagedProductDescriptorTypeDef",
     "DescribeManagedProductsByVendorRequestRequestTypeDef",
     "DescribeManagedRuleGroupRequestRequestTypeDef",
     "LabelSummaryTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
-    "EmailFieldOutputTypeDef",
     "EmailFieldTypeDef",
-    "ExcludedRuleOutputTypeDef",
     "ExcludedRuleTypeDef",
-    "HeaderOrderOutputTypeDef",
-    "SingleHeaderOutputTypeDef",
-    "SingleQueryArgumentOutputTypeDef",
     "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
-    "VisibilityConfigOutputTypeDef",
-    "ForwardedIPConfigOutputTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     "GetDecryptedAPIKeyRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
@@ -134,21 +117,18 @@
     "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
-    "IPSetForwardedIPConfigOutputTypeDef",
     "IPSetForwardedIPConfigTypeDef",
     "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
-    "LabelMatchStatementOutputTypeDef",
     "LabelMatchStatementTypeDef",
-    "LabelOutputTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
     "ManagedRuleGroupSummaryTypeDef",
     "ListIPSetsRequestRequestTypeDef",
@@ -158,56 +138,47 @@
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
-    "PasswordFieldOutputTypeDef",
-    "UsernameFieldOutputTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
-    "TagOutputTypeDef",
-    "NotStatementOutputTypeDef",
     "NotStatementTypeDef",
     "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
-    "PhoneNumberFieldOutputTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
-    "RateLimitLabelNamespaceOutputTypeDef",
     "RateLimitLabelNamespaceTypeDef",
-    "RegexOutputTypeDef",
     "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
     "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
     "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
     "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
     "RateLimitCookieOutputTypeDef",
-    "RateLimitHeaderOutputTypeDef",
-    "RateLimitQueryArgumentOutputTypeDef",
-    "RateLimitQueryStringOutputTypeDef",
-    "RateLimitUriPathOutputTypeDef",
     "RateLimitCookieTypeDef",
+    "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
+    "RateLimitQueryArgumentOutputTypeDef",
     "RateLimitQueryArgumentTypeDef",
+    "RateLimitQueryStringOutputTypeDef",
     "RateLimitQueryStringTypeDef",
+    "RateLimitUriPathOutputTypeDef",
     "RateLimitUriPathTypeDef",
-    "CaptchaConfigOutputTypeDef",
-    "ChallengeConfigOutputTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
     "CheckCapacityResponseTypeDef",
     "CreateAPIKeyResponseTypeDef",
     "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyResponseTypeDef",
@@ -216,96 +187,93 @@
     "ListResourcesForWebACLResponseTypeDef",
     "PutManagedRuleSetVersionsResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
-    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
+    "MobileSdkReleaseTypeDef",
+    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
+    "RegexPatternSetTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "CustomRequestHandlingOutputTypeDef",
-    "CustomResponseOutputTypeDef",
     "CustomRequestHandlingTypeDef",
+    "CustomResponseOutputTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
     "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "HeadersOutputTypeDef",
     "HeadersTypeDef",
-    "IPSetReferenceStatementOutputTypeDef",
     "IPSetReferenceStatementTypeDef",
     "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
-    "RequestInspectionOutputTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
-    "MobileSdkReleaseTypeDef",
-    "TagInfoForResourceTypeDef",
     "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
-    "RegexPatternSetTypeDef",
     "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
     "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
     "FilterOutputTypeDef",
     "FilterTypeDef",
+    "GetMobileSdkReleaseResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetRegexPatternSetResponseTypeDef",
     "AllowActionOutputTypeDef",
     "CaptchaActionOutputTypeDef",
     "ChallengeActionOutputTypeDef",
     "CountActionOutputTypeDef",
-    "BlockActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
+    "BlockActionOutputTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
     "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
-    "GetMobileSdkReleaseResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetRegexPatternSetResponseTypeDef",
     "AWSManagedRulesACFPRuleSetOutputTypeDef",
     "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
     "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
     "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
     "OverrideActionOutputTypeDef",
+    "OverrideActionTypeDef",
     "DefaultActionOutputTypeDef",
     "RuleActionOutputTypeDef",
-    "OverrideActionTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
     "ByteMatchStatementOutputTypeDef",
     "RegexMatchStatementOutputTypeDef",
     "RegexPatternSetReferenceStatementOutputTypeDef",
     "SizeConstraintStatementOutputTypeDef",
@@ -358,49 +326,28 @@
         "APIKey": str,
         "CreationTimestamp": datetime,
         "Version": int,
     },
     total=False,
 )
 
-AWSManagedRulesBotControlRuleSetOutputTypeDef = TypedDict(
-    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
-    {
-        "InspectionLevel": InspectionLevelType,
-    },
-)
-
 AWSManagedRulesBotControlRuleSetTypeDef = TypedDict(
     "AWSManagedRulesBotControlRuleSetTypeDef",
     {
         "InspectionLevel": InspectionLevelType,
     },
 )
 
-ActionConditionOutputTypeDef = TypedDict(
-    "ActionConditionOutputTypeDef",
-    {
-        "Action": ActionValueType,
-    },
-)
-
 ActionConditionTypeDef = TypedDict(
     "ActionConditionTypeDef",
     {
         "Action": ActionValueType,
     },
 )
 
-AddressFieldOutputTypeDef = TypedDict(
-    "AddressFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -410,79 +357,49 @@
         "Statements": List["StatementOutputTypeDef"],
     },
 )
 
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 AssociateWebACLRequestRequestTypeDef = TypedDict(
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "ResourceArn": str,
     },
 )
 
-RequestBodyAssociatedResourceTypeConfigOutputTypeDef = TypedDict(
-    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
-    {
-        "DefaultSizeInspectionLimit": SizeInspectionLimitType,
-    },
-)
-
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
-BodyOutputTypeDef = TypedDict(
-    "BodyOutputTypeDef",
-    {
-        "OversizeHandling": OversizeHandlingType,
-    },
-    total=False,
-)
-
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
 
-TextTransformationOutputTypeDef = TypedDict(
-    "TextTransformationOutputTypeDef",
-    {
-        "Priority": int,
-        "Type": TextTransformationTypeType,
-    },
-)
-
 TextTransformationTypeDef = TypedDict(
     "TextTransformationTypeDef",
     {
         "Priority": int,
         "Type": TextTransformationTypeType,
     },
 )
 
-ImmunityTimePropertyOutputTypeDef = TypedDict(
-    "ImmunityTimePropertyOutputTypeDef",
-    {
-        "ImmunityTime": int,
-    },
-)
-
 ImmunityTimePropertyTypeDef = TypedDict(
     "ImmunityTimePropertyTypeDef",
     {
         "ImmunityTime": int,
     },
 )
 
@@ -513,21 +430,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-LabelNameConditionOutputTypeDef = TypedDict(
-    "LabelNameConditionOutputTypeDef",
-    {
-        "LabelName": str,
-    },
-)
-
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
@@ -636,38 +546,22 @@
         "Description": str,
         "LockToken": str,
         "ARN": str,
     },
     total=False,
 )
 
-CustomHTTPHeaderOutputTypeDef = TypedDict(
-    "CustomHTTPHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 CustomHTTPHeaderTypeDef = TypedDict(
     "CustomHTTPHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CustomResponseBodyOutputTypeDef = TypedDict(
-    "CustomResponseBodyOutputTypeDef",
-    {
-        "ContentType": ResponseContentTypeType,
-        "Content": str,
-    },
-)
-
 DeleteFirewallManagerRuleGroupsRequestRequestTypeDef = TypedDict(
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "WebACLLockToken": str,
     },
 )
@@ -792,63 +686,28 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-EmailFieldOutputTypeDef = TypedDict(
-    "EmailFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
 EmailFieldTypeDef = TypedDict(
     "EmailFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
-ExcludedRuleOutputTypeDef = TypedDict(
-    "ExcludedRuleOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "Name": str,
     },
 )
 
-HeaderOrderOutputTypeDef = TypedDict(
-    "HeaderOrderOutputTypeDef",
-    {
-        "OversizeHandling": OversizeHandlingType,
-    },
-)
-
-SingleHeaderOutputTypeDef = TypedDict(
-    "SingleHeaderOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
-SingleQueryArgumentOutputTypeDef = TypedDict(
-    "SingleQueryArgumentOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 HeaderOrderTypeDef = TypedDict(
     "HeaderOrderTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
@@ -862,31 +721,14 @@
 SingleQueryArgumentTypeDef = TypedDict(
     "SingleQueryArgumentTypeDef",
     {
         "Name": str,
     },
 )
 
-VisibilityConfigOutputTypeDef = TypedDict(
-    "VisibilityConfigOutputTypeDef",
-    {
-        "SampledRequestsEnabled": bool,
-        "CloudWatchMetricsEnabled": bool,
-        "MetricName": str,
-    },
-)
-
-ForwardedIPConfigOutputTypeDef = TypedDict(
-    "ForwardedIPConfigOutputTypeDef",
-    {
-        "HeaderName": str,
-        "FallbackBehavior": FallbackBehaviorType,
-    },
-)
-
 ForwardedIPConfigTypeDef = TypedDict(
     "ForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
     },
 )
@@ -1081,23 +923,14 @@
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
     total=False,
 )
 
-IPSetForwardedIPConfigOutputTypeDef = TypedDict(
-    "IPSetForwardedIPConfigOutputTypeDef",
-    {
-        "HeaderName": str,
-        "FallbackBehavior": FallbackBehaviorType,
-        "Position": ForwardedIPPositionType,
-    },
-)
-
 IPSetForwardedIPConfigTypeDef = TypedDict(
     "IPSetForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
@@ -1117,37 +950,22 @@
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
 )
 
-LabelMatchStatementOutputTypeDef = TypedDict(
-    "LabelMatchStatementOutputTypeDef",
-    {
-        "Scope": LabelMatchScopeType,
-        "Key": str,
-    },
-)
-
 LabelMatchStatementTypeDef = TypedDict(
     "LabelMatchStatementTypeDef",
     {
         "Scope": LabelMatchScopeType,
         "Key": str,
     },
 )
 
-LabelOutputTypeDef = TypedDict(
-    "LabelOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 LabelTypeDef = TypedDict(
     "LabelTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1462,28 +1280,14 @@
 
 class ListWebACLsRequestRequestTypeDef(
     _RequiredListWebACLsRequestRequestTypeDef, _OptionalListWebACLsRequestRequestTypeDef
 ):
     pass
 
 
-PasswordFieldOutputTypeDef = TypedDict(
-    "PasswordFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
-UsernameFieldOutputTypeDef = TypedDict(
-    "UsernameFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
 PasswordFieldTypeDef = TypedDict(
     "PasswordFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1503,29 +1307,14 @@
         "PublishTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ExpiryTimestamp": datetime,
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
-NotStatementOutputTypeDef = TypedDict(
-    "NotStatementOutputTypeDef",
-    {
-        "Statement": "StatementOutputTypeDef",
-    },
-)
-
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
         "Statement": "StatementTypeDef",
     },
 )
 
@@ -1535,22 +1324,15 @@
         "Statements": List["StatementOutputTypeDef"],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence[Dict[str, Any]],
-    },
-)
-
-PhoneNumberFieldOutputTypeDef = TypedDict(
-    "PhoneNumberFieldOutputTypeDef",
-    {
-        "Identifier": str,
+        "Statements": Sequence["StatementTypeDef"],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
@@ -1570,36 +1352,21 @@
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-RateLimitLabelNamespaceOutputTypeDef = TypedDict(
-    "RateLimitLabelNamespaceOutputTypeDef",
-    {
-        "Namespace": str,
-    },
-)
-
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
-RegexOutputTypeDef = TypedDict(
-    "RegexOutputTypeDef",
-    {
-        "RegexString": str,
-    },
-    total=False,
-)
-
 ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
     "ResponseInspectionBodyContainsOutputTypeDef",
     {
         "SuccessStrings": List[str],
         "FailureStrings": List[str],
     },
 )
@@ -1708,17 +1475,15 @@
         "ExpiryTimestamp": Union[datetime, str],
     },
 )
 
 AssociationConfigOutputTypeDef = TypedDict(
     "AssociationConfigOutputTypeDef",
     {
-        "RequestBody": Dict[
-            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigOutputTypeDef
-        ],
+        "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
     },
     total=False,
 )
 
 AssociationConfigTypeDef = TypedDict(
     "AssociationConfigTypeDef",
     {
@@ -1729,100 +1494,84 @@
     total=False,
 )
 
 RateLimitCookieOutputTypeDef = TypedDict(
     "RateLimitCookieOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderOutputTypeDef = TypedDict(
-    "RateLimitHeaderOutputTypeDef",
+RateLimitCookieTypeDef = TypedDict(
+    "RateLimitCookieTypeDef",
     {
         "Name": str,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryArgumentOutputTypeDef = TypedDict(
-    "RateLimitQueryArgumentOutputTypeDef",
+RateLimitHeaderOutputTypeDef = TypedDict(
+    "RateLimitHeaderOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
-    },
-)
-
-RateLimitQueryStringOutputTypeDef = TypedDict(
-    "RateLimitQueryStringOutputTypeDef",
-    {
-        "TextTransformations": List[TextTransformationOutputTypeDef],
-    },
-)
-
-RateLimitUriPathOutputTypeDef = TypedDict(
-    "RateLimitUriPathOutputTypeDef",
-    {
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-RateLimitCookieTypeDef = TypedDict(
-    "RateLimitCookieTypeDef",
+RateLimitHeaderTypeDef = TypedDict(
+    "RateLimitHeaderTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderTypeDef = TypedDict(
-    "RateLimitHeaderTypeDef",
+RateLimitQueryArgumentOutputTypeDef = TypedDict(
+    "RateLimitQueryArgumentOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": Sequence[TextTransformationTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 RateLimitQueryArgumentTypeDef = TypedDict(
     "RateLimitQueryArgumentTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryStringTypeDef = TypedDict(
-    "RateLimitQueryStringTypeDef",
+RateLimitQueryStringOutputTypeDef = TypedDict(
+    "RateLimitQueryStringOutputTypeDef",
     {
-        "TextTransformations": Sequence[TextTransformationTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-RateLimitUriPathTypeDef = TypedDict(
-    "RateLimitUriPathTypeDef",
+RateLimitQueryStringTypeDef = TypedDict(
+    "RateLimitQueryStringTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-CaptchaConfigOutputTypeDef = TypedDict(
-    "CaptchaConfigOutputTypeDef",
+RateLimitUriPathOutputTypeDef = TypedDict(
+    "RateLimitUriPathOutputTypeDef",
     {
-        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
-    total=False,
 )
 
-ChallengeConfigOutputTypeDef = TypedDict(
-    "ChallengeConfigOutputTypeDef",
+RateLimitUriPathTypeDef = TypedDict(
+    "RateLimitUriPathTypeDef",
     {
-        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
-    total=False,
 )
 
 CaptchaConfigTypeDef = TypedDict(
     "CaptchaConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
@@ -1950,23 +1699,14 @@
     "UpdateWebACLResponseTypeDef",
     {
         "NextLockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "ActionCondition": ActionConditionOutputTypeDef,
-        "LabelNameCondition": LabelNameConditionOutputTypeDef,
-    },
-    total=False,
-)
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
@@ -2011,14 +1751,34 @@
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
 
+MobileSdkReleaseTypeDef = TypedDict(
+    "MobileSdkReleaseTypeDef",
+    {
+        "ReleaseVersion": str,
+        "Timestamp": datetime,
+        "ReleaseNotes": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+TagInfoForResourceTypeDef = TypedDict(
+    "TagInfoForResourceTypeDef",
+    {
+        "ResourceARN": str,
+        "TagList": List[TagTypeDef],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2061,14 +1821,26 @@
 class CreateRegexPatternSetRequestRequestTypeDef(
     _RequiredCreateRegexPatternSetRequestRequestTypeDef,
     _OptionalCreateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
 
+RegexPatternSetTypeDef = TypedDict(
+    "RegexPatternSetTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "ARN": str,
+        "Description": str,
+        "RegularExpressionList": List[RegexTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "RegularExpressionList": Sequence[RegexTypeDef],
@@ -2141,47 +1913,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomRequestHandlingOutputTypeDef = TypedDict(
     "CustomRequestHandlingOutputTypeDef",
     {
-        "InsertHeaders": List[CustomHTTPHeaderOutputTypeDef],
+        "InsertHeaders": List[CustomHTTPHeaderTypeDef],
+    },
+)
+
+CustomRequestHandlingTypeDef = TypedDict(
+    "CustomRequestHandlingTypeDef",
+    {
+        "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
 _RequiredCustomResponseOutputTypeDef = TypedDict(
     "_RequiredCustomResponseOutputTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseOutputTypeDef = TypedDict(
     "_OptionalCustomResponseOutputTypeDef",
     {
         "CustomResponseBodyKey": str,
-        "ResponseHeaders": List[CustomHTTPHeaderOutputTypeDef],
+        "ResponseHeaders": List[CustomHTTPHeaderTypeDef],
     },
     total=False,
 )
 
 
 class CustomResponseOutputTypeDef(
     _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
 ):
     pass
 
 
-CustomRequestHandlingTypeDef = TypedDict(
-    "CustomRequestHandlingTypeDef",
-    {
-        "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
-    },
-)
-
 _RequiredCustomResponseTypeDef = TypedDict(
     "_RequiredCustomResponseTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseTypeDef = TypedDict(
@@ -2214,15 +1986,15 @@
     },
 )
 
 GeoMatchStatementOutputTypeDef = TypedDict(
     "GeoMatchStatementOutputTypeDef",
     {
         "CountryCodes": List[CountryCodeType],
-        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
@@ -2288,35 +2060,14 @@
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
-_RequiredIPSetReferenceStatementOutputTypeDef = TypedDict(
-    "_RequiredIPSetReferenceStatementOutputTypeDef",
-    {
-        "ARN": str,
-    },
-)
-_OptionalIPSetReferenceStatementOutputTypeDef = TypedDict(
-    "_OptionalIPSetReferenceStatementOutputTypeDef",
-    {
-        "IPSetForwardedIPConfig": IPSetForwardedIPConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class IPSetReferenceStatementOutputTypeDef(
-    _RequiredIPSetReferenceStatementOutputTypeDef, _OptionalIPSetReferenceStatementOutputTypeDef
-):
-    pass
-
-
 _RequiredIPSetReferenceStatementTypeDef = TypedDict(
     "_RequiredIPSetReferenceStatementTypeDef",
     {
         "ARN": str,
     },
 )
 _OptionalIPSetReferenceStatementTypeDef = TypedDict(
@@ -2409,23 +2160,14 @@
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RequestInspectionOutputTypeDef = TypedDict(
-    "RequestInspectionOutputTypeDef",
-    {
-        "PayloadType": PayloadTypeType,
-        "UsernameField": UsernameFieldOutputTypeDef,
-        "PasswordField": PasswordFieldOutputTypeDef,
-    },
-)
-
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
     },
@@ -2451,48 +2193,28 @@
 )
 
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
 
-MobileSdkReleaseTypeDef = TypedDict(
-    "MobileSdkReleaseTypeDef",
-    {
-        "ReleaseVersion": str,
-        "Timestamp": datetime,
-        "ReleaseNotes": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-TagInfoForResourceTypeDef = TypedDict(
-    "TagInfoForResourceTypeDef",
-    {
-        "ResourceARN": str,
-        "TagList": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPOutputTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
     "_OptionalRequestInspectionACFPOutputTypeDef",
     {
-        "UsernameField": UsernameFieldOutputTypeDef,
-        "PasswordField": PasswordFieldOutputTypeDef,
-        "EmailField": EmailFieldOutputTypeDef,
-        "PhoneNumberFields": List[PhoneNumberFieldOutputTypeDef],
-        "AddressFields": List[AddressFieldOutputTypeDef],
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "EmailField": EmailFieldTypeDef,
+        "PhoneNumberFields": List[PhoneNumberFieldTypeDef],
+        "AddressFields": List[AddressFieldTypeDef],
     },
     total=False,
 )
 
 
 class RequestInspectionACFPOutputTypeDef(
     _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
@@ -2547,26 +2269,14 @@
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-RegexPatternSetTypeDef = TypedDict(
-    "RegexPatternSetTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "ARN": str,
-        "Description": str,
-        "RegularExpressionList": List[RegexOutputTypeDef],
-    },
-    total=False,
-)
-
 ResponseInspectionOutputTypeDef = TypedDict(
     "ResponseInspectionOutputTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
         "Header": ResponseInspectionHeaderOutputTypeDef,
         "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
         "Json": ResponseInspectionJsonOutputTypeDef,
@@ -2591,15 +2301,15 @@
         "Header": RateLimitHeaderOutputTypeDef,
         "Cookie": RateLimitCookieOutputTypeDef,
         "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
         "QueryString": RateLimitQueryStringOutputTypeDef,
         "HTTPMethod": Dict[str, Any],
         "ForwardedIP": Dict[str, Any],
         "IP": Dict[str, Any],
-        "LabelNamespace": RateLimitLabelNamespaceOutputTypeDef,
+        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
         "UriPath": RateLimitUriPathOutputTypeDef,
     },
     total=False,
 )
 
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
@@ -2618,27 +2328,53 @@
 )
 
 FilterOutputTypeDef = TypedDict(
     "FilterOutputTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionOutputTypeDef],
+        "Conditions": List[ConditionTypeDef],
     },
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
         "Conditions": Sequence[ConditionTypeDef],
     },
 )
 
+GetMobileSdkReleaseResponseTypeDef = TypedDict(
+    "GetMobileSdkReleaseResponseTypeDef",
+    {
+        "MobileSdkRelease": MobileSdkReleaseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegexPatternSetResponseTypeDef = TypedDict(
+    "GetRegexPatternSetResponseTypeDef",
+    {
+        "RegexPatternSet": RegexPatternSetTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AllowActionOutputTypeDef = TypedDict(
     "AllowActionOutputTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
     total=False,
 )
@@ -2663,22 +2399,14 @@
     "CountActionOutputTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
     total=False,
 )
 
-BlockActionOutputTypeDef = TypedDict(
-    "BlockActionOutputTypeDef",
-    {
-        "CustomResponse": CustomResponseOutputTypeDef,
-    },
-    total=False,
-)
-
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
@@ -2703,14 +2431,22 @@
     "CountActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
 
+BlockActionOutputTypeDef = TypedDict(
+    "BlockActionOutputTypeDef",
+    {
+        "CustomResponse": CustomResponseOutputTypeDef,
+    },
+    total=False,
+)
+
 BlockActionTypeDef = TypedDict(
     "BlockActionTypeDef",
     {
         "CustomResponse": CustomResponseTypeDef,
     },
     total=False,
 )
@@ -2726,15 +2462,15 @@
     "_OptionalSampledHTTPRequestTypeDef",
     {
         "Timestamp": datetime,
         "Action": str,
         "RuleNameWithinRuleGroup": str,
         "RequestHeadersInserted": List[HTTPHeaderTypeDef],
         "ResponseCodeSent": int,
-        "Labels": List[LabelOutputTypeDef],
+        "Labels": List[LabelTypeDef],
         "CaptchaResponse": CaptchaResponseTypeDef,
         "ChallengeResponse": ChallengeResponseTypeDef,
         "OverriddenAction": str,
     },
     total=False,
 )
 
@@ -2744,25 +2480,25 @@
 ):
     pass
 
 
 FieldToMatchOutputTypeDef = TypedDict(
     "FieldToMatchOutputTypeDef",
     {
-        "SingleHeader": SingleHeaderOutputTypeDef,
-        "SingleQueryArgument": SingleQueryArgumentOutputTypeDef,
+        "SingleHeader": SingleHeaderTypeDef,
+        "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Dict[str, Any],
         "UriPath": Dict[str, Any],
         "QueryString": Dict[str, Any],
-        "Body": BodyOutputTypeDef,
+        "Body": BodyTypeDef,
         "Method": Dict[str, Any],
         "JsonBody": JsonBodyOutputTypeDef,
         "Headers": HeadersOutputTypeDef,
         "Cookies": CookiesOutputTypeDef,
-        "HeaderOrder": HeaderOrderOutputTypeDef,
+        "HeaderOrder": HeaderOrderTypeDef,
     },
     total=False,
 )
 
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
@@ -2786,40 +2522,14 @@
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMobileSdkReleaseResponseTypeDef = TypedDict(
-    "GetMobileSdkReleaseResponseTypeDef",
-    {
-        "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRegexPatternSetResponseTypeDef = TypedDict(
-    "GetRegexPatternSetResponseTypeDef",
-    {
-        "RegexPatternSet": RegexPatternSetTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPOutputTypeDef,
     },
@@ -2846,15 +2556,15 @@
     {
         "LoginPath": str,
     },
 )
 _OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
     "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
     {
-        "RequestInspection": RequestInspectionOutputTypeDef,
+        "RequestInspection": RequestInspectionTypeDef,
         "ResponseInspection": ResponseInspectionOutputTypeDef,
         "EnableRegexInPath": bool,
     },
     total=False,
 )
 
 
@@ -2918,15 +2628,15 @@
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementOutputTypeDef = TypedDict(
     "_OptionalRateBasedStatementOutputTypeDef",
     {
         "ScopeDownStatement": "StatementOutputTypeDef",
-        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
         "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
     },
     total=False,
 )
 
 
 class RateBasedStatementOutputTypeDef(
@@ -2980,14 +2690,23 @@
     {
         "Count": CountActionOutputTypeDef,
         "None": Dict[str, Any],
     },
     total=False,
 )
 
+OverrideActionTypeDef = TypedDict(
+    "OverrideActionTypeDef",
+    {
+        "Count": CountActionTypeDef,
+        "None": Mapping[str, Any],
+    },
+    total=False,
+)
+
 DefaultActionOutputTypeDef = TypedDict(
     "DefaultActionOutputTypeDef",
     {
         "Block": BlockActionOutputTypeDef,
         "Allow": AllowActionOutputTypeDef,
     },
     total=False,
@@ -3001,23 +2720,14 @@
         "Count": CountActionOutputTypeDef,
         "Captcha": CaptchaActionOutputTypeDef,
         "Challenge": ChallengeActionOutputTypeDef,
     },
     total=False,
 )
 
-OverrideActionTypeDef = TypedDict(
-    "OverrideActionTypeDef",
-    {
-        "Count": CountActionTypeDef,
-        "None": Mapping[str, Any],
-    },
-    total=False,
-)
-
 DefaultActionTypeDef = TypedDict(
     "DefaultActionTypeDef",
     {
         "Block": BlockActionTypeDef,
         "Allow": AllowActionTypeDef,
     },
     total=False,
@@ -3046,52 +2756,52 @@
 )
 
 ByteMatchStatementOutputTypeDef = TypedDict(
     "ByteMatchStatementOutputTypeDef",
     {
         "SearchString": bytes,
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 RegexMatchStatementOutputTypeDef = TypedDict(
     "RegexMatchStatementOutputTypeDef",
     {
         "RegexString": str,
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
     "RegexPatternSetReferenceStatementOutputTypeDef",
     {
         "ARN": str,
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 SizeConstraintStatementOutputTypeDef = TypedDict(
     "SizeConstraintStatementOutputTypeDef",
     {
         "FieldToMatch": FieldToMatchOutputTypeDef,
         "ComparisonOperator": ComparisonOperatorType,
         "Size": int,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 _RequiredSqliMatchStatementOutputTypeDef = TypedDict(
     "_RequiredSqliMatchStatementOutputTypeDef",
     {
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 _OptionalSqliMatchStatementOutputTypeDef = TypedDict(
     "_OptionalSqliMatchStatementOutputTypeDef",
     {
         "SensitivityLevel": SensitivityLevelType,
     },
@@ -3105,15 +2815,15 @@
     pass
 
 
 XssMatchStatementOutputTypeDef = TypedDict(
     "XssMatchStatementOutputTypeDef",
     {
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": Union[str, bytes, IO[Any], StreamingBody],
@@ -3182,17 +2892,17 @@
 )
 
 ManagedRuleGroupConfigOutputTypeDef = TypedDict(
     "ManagedRuleGroupConfigOutputTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
-        "UsernameField": UsernameFieldOutputTypeDef,
-        "PasswordField": PasswordFieldOutputTypeDef,
-        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetOutputTypeDef,
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
     },
     total=False,
 )
 
 ManagedRuleGroupConfigTypeDef = TypedDict(
@@ -3267,25 +2977,25 @@
 
 _RequiredRuleOutputTypeDef = TypedDict(
     "_RequiredRuleOutputTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementOutputTypeDef",
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalRuleOutputTypeDef = TypedDict(
     "_OptionalRuleOutputTypeDef",
     {
         "Action": RuleActionOutputTypeDef,
         "OverrideAction": OverrideActionOutputTypeDef,
-        "RuleLabels": List[LabelOutputTypeDef],
-        "CaptchaConfig": CaptchaConfigOutputTypeDef,
-        "ChallengeConfig": ChallengeConfigOutputTypeDef,
+        "RuleLabels": List[LabelTypeDef],
+        "CaptchaConfig": CaptchaConfigTypeDef,
+        "ChallengeConfig": ChallengeConfigTypeDef,
     },
     total=False,
 )
 
 
 class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
     pass
@@ -3373,15 +3083,15 @@
         "Name": str,
     },
 )
 _OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementOutputTypeDef",
     {
         "Version": str,
-        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
         "ScopeDownStatement": Dict[str, Any],
         "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
         "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
     },
     total=False,
 )
 
@@ -3397,15 +3107,15 @@
     {
         "ARN": str,
     },
 )
 _OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
     "_OptionalRuleGroupReferenceStatementOutputTypeDef",
     {
-        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
         "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
     },
     total=False,
 )
 
 
 class RuleGroupReferenceStatementOutputTypeDef(
@@ -3418,24 +3128,24 @@
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "Name": str,
         "Id": str,
         "Capacity": int,
         "ARN": str,
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
     "_OptionalRuleGroupTypeDef",
     {
         "Description": str,
         "Rules": List[RuleOutputTypeDef],
         "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "AvailableLabels": List[LabelSummaryTypeDef],
         "ConsumedLabels": List[LabelSummaryTypeDef],
     },
     total=False,
 )
 
 
@@ -3644,22 +3354,22 @@
     {
         "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
         "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
         "XssMatchStatement": XssMatchStatementOutputTypeDef,
         "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
         "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
         "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
         "RateBasedStatement": Dict[str, Any],
         "AndStatement": Dict[str, Any],
         "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
         "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementOutputTypeDef,
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
     },
     total=False,
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
@@ -3695,41 +3405,41 @@
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
         "OverrideAction": OverrideActionOutputTypeDef,
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
         "DefaultAction": DefaultActionOutputTypeDef,
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
         "Rules": List[RuleOutputTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
-        "CaptchaConfig": CaptchaConfigOutputTypeDef,
-        "ChallengeConfig": ChallengeConfigOutputTypeDef,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
+        "CaptchaConfig": CaptchaConfigTypeDef,
+        "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
         "AssociationConfig": AssociationConfigOutputTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -52,75 +52,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "APIKeySummaryTypeDef",
-    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
-    "ActionConditionOutputTypeDef",
     "ActionConditionTypeDef",
-    "AddressFieldOutputTypeDef",
     "AddressFieldTypeDef",
     "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
-    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
-    "BodyOutputTypeDef",
     "BodyTypeDef",
-    "TextTransformationOutputTypeDef",
     "TextTransformationTypeDef",
-    "ImmunityTimePropertyOutputTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
     "ResponseMetadataTypeDef",
-    "LabelNameConditionOutputTypeDef",
     "LabelNameConditionTypeDef",
     "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
-    "CustomHTTPHeaderOutputTypeDef",
     "CustomHTTPHeaderTypeDef",
-    "CustomResponseBodyOutputTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DescribeAllManagedProductsRequestRequestTypeDef",
     "ManagedProductDescriptorTypeDef",
     "DescribeManagedProductsByVendorRequestRequestTypeDef",
     "DescribeManagedRuleGroupRequestRequestTypeDef",
     "LabelSummaryTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
-    "EmailFieldOutputTypeDef",
     "EmailFieldTypeDef",
-    "ExcludedRuleOutputTypeDef",
     "ExcludedRuleTypeDef",
-    "HeaderOrderOutputTypeDef",
-    "SingleHeaderOutputTypeDef",
-    "SingleQueryArgumentOutputTypeDef",
     "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
-    "VisibilityConfigOutputTypeDef",
-    "ForwardedIPConfigOutputTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     "GetDecryptedAPIKeyRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
@@ -133,21 +116,18 @@
     "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
-    "IPSetForwardedIPConfigOutputTypeDef",
     "IPSetForwardedIPConfigTypeDef",
     "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
-    "LabelMatchStatementOutputTypeDef",
     "LabelMatchStatementTypeDef",
-    "LabelOutputTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
     "ManagedRuleGroupSummaryTypeDef",
     "ListIPSetsRequestRequestTypeDef",
@@ -157,56 +137,47 @@
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
-    "PasswordFieldOutputTypeDef",
-    "UsernameFieldOutputTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
-    "TagOutputTypeDef",
-    "NotStatementOutputTypeDef",
     "NotStatementTypeDef",
     "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
-    "PhoneNumberFieldOutputTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
-    "RateLimitLabelNamespaceOutputTypeDef",
     "RateLimitLabelNamespaceTypeDef",
-    "RegexOutputTypeDef",
     "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
     "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
     "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
     "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
     "RateLimitCookieOutputTypeDef",
-    "RateLimitHeaderOutputTypeDef",
-    "RateLimitQueryArgumentOutputTypeDef",
-    "RateLimitQueryStringOutputTypeDef",
-    "RateLimitUriPathOutputTypeDef",
     "RateLimitCookieTypeDef",
+    "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
+    "RateLimitQueryArgumentOutputTypeDef",
     "RateLimitQueryArgumentTypeDef",
+    "RateLimitQueryStringOutputTypeDef",
     "RateLimitQueryStringTypeDef",
+    "RateLimitUriPathOutputTypeDef",
     "RateLimitUriPathTypeDef",
-    "CaptchaConfigOutputTypeDef",
-    "ChallengeConfigOutputTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
     "CheckCapacityResponseTypeDef",
     "CreateAPIKeyResponseTypeDef",
     "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyResponseTypeDef",
@@ -215,96 +186,93 @@
     "ListResourcesForWebACLResponseTypeDef",
     "PutManagedRuleSetVersionsResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
-    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
+    "MobileSdkReleaseTypeDef",
+    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
+    "RegexPatternSetTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "CustomRequestHandlingOutputTypeDef",
-    "CustomResponseOutputTypeDef",
     "CustomRequestHandlingTypeDef",
+    "CustomResponseOutputTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
     "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "HeadersOutputTypeDef",
     "HeadersTypeDef",
-    "IPSetReferenceStatementOutputTypeDef",
     "IPSetReferenceStatementTypeDef",
     "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
-    "RequestInspectionOutputTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
-    "MobileSdkReleaseTypeDef",
-    "TagInfoForResourceTypeDef",
     "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
-    "RegexPatternSetTypeDef",
     "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
     "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
     "FilterOutputTypeDef",
     "FilterTypeDef",
+    "GetMobileSdkReleaseResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetRegexPatternSetResponseTypeDef",
     "AllowActionOutputTypeDef",
     "CaptchaActionOutputTypeDef",
     "ChallengeActionOutputTypeDef",
     "CountActionOutputTypeDef",
-    "BlockActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
+    "BlockActionOutputTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
     "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
-    "GetMobileSdkReleaseResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "GetRegexPatternSetResponseTypeDef",
     "AWSManagedRulesACFPRuleSetOutputTypeDef",
     "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
     "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
     "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
     "OverrideActionOutputTypeDef",
+    "OverrideActionTypeDef",
     "DefaultActionOutputTypeDef",
     "RuleActionOutputTypeDef",
-    "OverrideActionTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
     "ByteMatchStatementOutputTypeDef",
     "RegexMatchStatementOutputTypeDef",
     "RegexPatternSetReferenceStatementOutputTypeDef",
     "SizeConstraintStatementOutputTypeDef",
@@ -357,49 +325,28 @@
         "APIKey": str,
         "CreationTimestamp": datetime,
         "Version": int,
     },
     total=False,
 )
 
-AWSManagedRulesBotControlRuleSetOutputTypeDef = TypedDict(
-    "AWSManagedRulesBotControlRuleSetOutputTypeDef",
-    {
-        "InspectionLevel": InspectionLevelType,
-    },
-)
-
 AWSManagedRulesBotControlRuleSetTypeDef = TypedDict(
     "AWSManagedRulesBotControlRuleSetTypeDef",
     {
         "InspectionLevel": InspectionLevelType,
     },
 )
 
-ActionConditionOutputTypeDef = TypedDict(
-    "ActionConditionOutputTypeDef",
-    {
-        "Action": ActionValueType,
-    },
-)
-
 ActionConditionTypeDef = TypedDict(
     "ActionConditionTypeDef",
     {
         "Action": ActionValueType,
     },
 )
 
-AddressFieldOutputTypeDef = TypedDict(
-    "AddressFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -409,79 +356,49 @@
         "Statements": List["StatementOutputTypeDef"],
     },
 )
 
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 AssociateWebACLRequestRequestTypeDef = TypedDict(
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "ResourceArn": str,
     },
 )
 
-RequestBodyAssociatedResourceTypeConfigOutputTypeDef = TypedDict(
-    "RequestBodyAssociatedResourceTypeConfigOutputTypeDef",
-    {
-        "DefaultSizeInspectionLimit": SizeInspectionLimitType,
-    },
-)
-
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
-BodyOutputTypeDef = TypedDict(
-    "BodyOutputTypeDef",
-    {
-        "OversizeHandling": OversizeHandlingType,
-    },
-    total=False,
-)
-
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
 
-TextTransformationOutputTypeDef = TypedDict(
-    "TextTransformationOutputTypeDef",
-    {
-        "Priority": int,
-        "Type": TextTransformationTypeType,
-    },
-)
-
 TextTransformationTypeDef = TypedDict(
     "TextTransformationTypeDef",
     {
         "Priority": int,
         "Type": TextTransformationTypeType,
     },
 )
 
-ImmunityTimePropertyOutputTypeDef = TypedDict(
-    "ImmunityTimePropertyOutputTypeDef",
-    {
-        "ImmunityTime": int,
-    },
-)
-
 ImmunityTimePropertyTypeDef = TypedDict(
     "ImmunityTimePropertyTypeDef",
     {
         "ImmunityTime": int,
     },
 )
 
@@ -512,21 +429,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-LabelNameConditionOutputTypeDef = TypedDict(
-    "LabelNameConditionOutputTypeDef",
-    {
-        "LabelName": str,
-    },
-)
-
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
@@ -635,38 +545,22 @@
         "Description": str,
         "LockToken": str,
         "ARN": str,
     },
     total=False,
 )
 
-CustomHTTPHeaderOutputTypeDef = TypedDict(
-    "CustomHTTPHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 CustomHTTPHeaderTypeDef = TypedDict(
     "CustomHTTPHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CustomResponseBodyOutputTypeDef = TypedDict(
-    "CustomResponseBodyOutputTypeDef",
-    {
-        "ContentType": ResponseContentTypeType,
-        "Content": str,
-    },
-)
-
 DeleteFirewallManagerRuleGroupsRequestRequestTypeDef = TypedDict(
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "WebACLLockToken": str,
     },
 )
@@ -789,63 +683,28 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-EmailFieldOutputTypeDef = TypedDict(
-    "EmailFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
 EmailFieldTypeDef = TypedDict(
     "EmailFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
-ExcludedRuleOutputTypeDef = TypedDict(
-    "ExcludedRuleOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "Name": str,
     },
 )
 
-HeaderOrderOutputTypeDef = TypedDict(
-    "HeaderOrderOutputTypeDef",
-    {
-        "OversizeHandling": OversizeHandlingType,
-    },
-)
-
-SingleHeaderOutputTypeDef = TypedDict(
-    "SingleHeaderOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
-SingleQueryArgumentOutputTypeDef = TypedDict(
-    "SingleQueryArgumentOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 HeaderOrderTypeDef = TypedDict(
     "HeaderOrderTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
@@ -859,31 +718,14 @@
 SingleQueryArgumentTypeDef = TypedDict(
     "SingleQueryArgumentTypeDef",
     {
         "Name": str,
     },
 )
 
-VisibilityConfigOutputTypeDef = TypedDict(
-    "VisibilityConfigOutputTypeDef",
-    {
-        "SampledRequestsEnabled": bool,
-        "CloudWatchMetricsEnabled": bool,
-        "MetricName": str,
-    },
-)
-
-ForwardedIPConfigOutputTypeDef = TypedDict(
-    "ForwardedIPConfigOutputTypeDef",
-    {
-        "HeaderName": str,
-        "FallbackBehavior": FallbackBehaviorType,
-    },
-)
-
 ForwardedIPConfigTypeDef = TypedDict(
     "ForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
     },
 )
@@ -1074,23 +916,14 @@
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
     total=False,
 )
 
-IPSetForwardedIPConfigOutputTypeDef = TypedDict(
-    "IPSetForwardedIPConfigOutputTypeDef",
-    {
-        "HeaderName": str,
-        "FallbackBehavior": FallbackBehaviorType,
-        "Position": ForwardedIPPositionType,
-    },
-)
-
 IPSetForwardedIPConfigTypeDef = TypedDict(
     "IPSetForwardedIPConfigTypeDef",
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
@@ -1110,37 +943,22 @@
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
 )
 
-LabelMatchStatementOutputTypeDef = TypedDict(
-    "LabelMatchStatementOutputTypeDef",
-    {
-        "Scope": LabelMatchScopeType,
-        "Key": str,
-    },
-)
-
 LabelMatchStatementTypeDef = TypedDict(
     "LabelMatchStatementTypeDef",
     {
         "Scope": LabelMatchScopeType,
         "Key": str,
     },
 )
 
-LabelOutputTypeDef = TypedDict(
-    "LabelOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 LabelTypeDef = TypedDict(
     "LabelTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1431,28 +1249,14 @@
 )
 
 class ListWebACLsRequestRequestTypeDef(
     _RequiredListWebACLsRequestRequestTypeDef, _OptionalListWebACLsRequestRequestTypeDef
 ):
     pass
 
-PasswordFieldOutputTypeDef = TypedDict(
-    "PasswordFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
-UsernameFieldOutputTypeDef = TypedDict(
-    "UsernameFieldOutputTypeDef",
-    {
-        "Identifier": str,
-    },
-)
-
 PasswordFieldTypeDef = TypedDict(
     "PasswordFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -1472,29 +1276,14 @@
         "PublishTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ExpiryTimestamp": datetime,
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
-NotStatementOutputTypeDef = TypedDict(
-    "NotStatementOutputTypeDef",
-    {
-        "Statement": "StatementOutputTypeDef",
-    },
-)
-
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
         "Statement": "StatementTypeDef",
     },
 )
 
@@ -1504,22 +1293,15 @@
         "Statements": List["StatementOutputTypeDef"],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence[Dict[str, Any]],
-    },
-)
-
-PhoneNumberFieldOutputTypeDef = TypedDict(
-    "PhoneNumberFieldOutputTypeDef",
-    {
-        "Identifier": str,
+        "Statements": Sequence["StatementTypeDef"],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
@@ -1539,36 +1321,21 @@
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-RateLimitLabelNamespaceOutputTypeDef = TypedDict(
-    "RateLimitLabelNamespaceOutputTypeDef",
-    {
-        "Namespace": str,
-    },
-)
-
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
-RegexOutputTypeDef = TypedDict(
-    "RegexOutputTypeDef",
-    {
-        "RegexString": str,
-    },
-    total=False,
-)
-
 ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
     "ResponseInspectionBodyContainsOutputTypeDef",
     {
         "SuccessStrings": List[str],
         "FailureStrings": List[str],
     },
 )
@@ -1675,17 +1442,15 @@
         "ExpiryTimestamp": Union[datetime, str],
     },
 )
 
 AssociationConfigOutputTypeDef = TypedDict(
     "AssociationConfigOutputTypeDef",
     {
-        "RequestBody": Dict[
-            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigOutputTypeDef
-        ],
+        "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
     },
     total=False,
 )
 
 AssociationConfigTypeDef = TypedDict(
     "AssociationConfigTypeDef",
     {
@@ -1696,100 +1461,84 @@
     total=False,
 )
 
 RateLimitCookieOutputTypeDef = TypedDict(
     "RateLimitCookieOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderOutputTypeDef = TypedDict(
-    "RateLimitHeaderOutputTypeDef",
+RateLimitCookieTypeDef = TypedDict(
+    "RateLimitCookieTypeDef",
     {
         "Name": str,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryArgumentOutputTypeDef = TypedDict(
-    "RateLimitQueryArgumentOutputTypeDef",
+RateLimitHeaderOutputTypeDef = TypedDict(
+    "RateLimitHeaderOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryStringOutputTypeDef = TypedDict(
-    "RateLimitQueryStringOutputTypeDef",
-    {
-        "TextTransformations": List[TextTransformationOutputTypeDef],
-    },
-)
-
-RateLimitUriPathOutputTypeDef = TypedDict(
-    "RateLimitUriPathOutputTypeDef",
-    {
-        "TextTransformations": List[TextTransformationOutputTypeDef],
-    },
-)
-
-RateLimitCookieTypeDef = TypedDict(
-    "RateLimitCookieTypeDef",
+RateLimitHeaderTypeDef = TypedDict(
+    "RateLimitHeaderTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderTypeDef = TypedDict(
-    "RateLimitHeaderTypeDef",
+RateLimitQueryArgumentOutputTypeDef = TypedDict(
+    "RateLimitQueryArgumentOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": Sequence[TextTransformationTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 RateLimitQueryArgumentTypeDef = TypedDict(
     "RateLimitQueryArgumentTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryStringTypeDef = TypedDict(
-    "RateLimitQueryStringTypeDef",
+RateLimitQueryStringOutputTypeDef = TypedDict(
+    "RateLimitQueryStringOutputTypeDef",
     {
-        "TextTransformations": Sequence[TextTransformationTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-RateLimitUriPathTypeDef = TypedDict(
-    "RateLimitUriPathTypeDef",
+RateLimitQueryStringTypeDef = TypedDict(
+    "RateLimitQueryStringTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-CaptchaConfigOutputTypeDef = TypedDict(
-    "CaptchaConfigOutputTypeDef",
+RateLimitUriPathOutputTypeDef = TypedDict(
+    "RateLimitUriPathOutputTypeDef",
     {
-        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
-    total=False,
 )
 
-ChallengeConfigOutputTypeDef = TypedDict(
-    "ChallengeConfigOutputTypeDef",
+RateLimitUriPathTypeDef = TypedDict(
+    "RateLimitUriPathTypeDef",
     {
-        "ImmunityTimeProperty": ImmunityTimePropertyOutputTypeDef,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
-    total=False,
 )
 
 CaptchaConfigTypeDef = TypedDict(
     "CaptchaConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
@@ -1917,23 +1666,14 @@
     "UpdateWebACLResponseTypeDef",
     {
         "NextLockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "ActionCondition": ActionConditionOutputTypeDef,
-        "LabelNameCondition": LabelNameConditionOutputTypeDef,
-    },
-    total=False,
-)
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
@@ -1976,14 +1716,34 @@
 )
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
+MobileSdkReleaseTypeDef = TypedDict(
+    "MobileSdkReleaseTypeDef",
+    {
+        "ReleaseVersion": str,
+        "Timestamp": datetime,
+        "ReleaseNotes": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+TagInfoForResourceTypeDef = TypedDict(
+    "TagInfoForResourceTypeDef",
+    {
+        "ResourceARN": str,
+        "TagList": List[TagTypeDef],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2024,14 +1784,26 @@
 
 class CreateRegexPatternSetRequestRequestTypeDef(
     _RequiredCreateRegexPatternSetRequestRequestTypeDef,
     _OptionalCreateRegexPatternSetRequestRequestTypeDef,
 ):
     pass
 
+RegexPatternSetTypeDef = TypedDict(
+    "RegexPatternSetTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "ARN": str,
+        "Description": str,
+        "RegularExpressionList": List[RegexTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "RegularExpressionList": Sequence[RegexTypeDef],
@@ -2102,45 +1874,45 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomRequestHandlingOutputTypeDef = TypedDict(
     "CustomRequestHandlingOutputTypeDef",
     {
-        "InsertHeaders": List[CustomHTTPHeaderOutputTypeDef],
+        "InsertHeaders": List[CustomHTTPHeaderTypeDef],
+    },
+)
+
+CustomRequestHandlingTypeDef = TypedDict(
+    "CustomRequestHandlingTypeDef",
+    {
+        "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
 _RequiredCustomResponseOutputTypeDef = TypedDict(
     "_RequiredCustomResponseOutputTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseOutputTypeDef = TypedDict(
     "_OptionalCustomResponseOutputTypeDef",
     {
         "CustomResponseBodyKey": str,
-        "ResponseHeaders": List[CustomHTTPHeaderOutputTypeDef],
+        "ResponseHeaders": List[CustomHTTPHeaderTypeDef],
     },
     total=False,
 )
 
 class CustomResponseOutputTypeDef(
     _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
 ):
     pass
 
-CustomRequestHandlingTypeDef = TypedDict(
-    "CustomRequestHandlingTypeDef",
-    {
-        "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
-    },
-)
-
 _RequiredCustomResponseTypeDef = TypedDict(
     "_RequiredCustomResponseTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseTypeDef = TypedDict(
@@ -2171,15 +1943,15 @@
     },
 )
 
 GeoMatchStatementOutputTypeDef = TypedDict(
     "GeoMatchStatementOutputTypeDef",
     {
         "CountryCodes": List[CountryCodeType],
-        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
@@ -2245,33 +2017,14 @@
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
 )
 
-_RequiredIPSetReferenceStatementOutputTypeDef = TypedDict(
-    "_RequiredIPSetReferenceStatementOutputTypeDef",
-    {
-        "ARN": str,
-    },
-)
-_OptionalIPSetReferenceStatementOutputTypeDef = TypedDict(
-    "_OptionalIPSetReferenceStatementOutputTypeDef",
-    {
-        "IPSetForwardedIPConfig": IPSetForwardedIPConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class IPSetReferenceStatementOutputTypeDef(
-    _RequiredIPSetReferenceStatementOutputTypeDef, _OptionalIPSetReferenceStatementOutputTypeDef
-):
-    pass
-
 _RequiredIPSetReferenceStatementTypeDef = TypedDict(
     "_RequiredIPSetReferenceStatementTypeDef",
     {
         "ARN": str,
     },
 )
 _OptionalIPSetReferenceStatementTypeDef = TypedDict(
@@ -2358,23 +2111,14 @@
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RequestInspectionOutputTypeDef = TypedDict(
-    "RequestInspectionOutputTypeDef",
-    {
-        "PayloadType": PayloadTypeType,
-        "UsernameField": UsernameFieldOutputTypeDef,
-        "PasswordField": PasswordFieldOutputTypeDef,
-    },
-)
-
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
     },
@@ -2398,48 +2142,28 @@
     },
     total=False,
 )
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
-MobileSdkReleaseTypeDef = TypedDict(
-    "MobileSdkReleaseTypeDef",
-    {
-        "ReleaseVersion": str,
-        "Timestamp": datetime,
-        "ReleaseNotes": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-TagInfoForResourceTypeDef = TypedDict(
-    "TagInfoForResourceTypeDef",
-    {
-        "ResourceARN": str,
-        "TagList": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPOutputTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
     "_OptionalRequestInspectionACFPOutputTypeDef",
     {
-        "UsernameField": UsernameFieldOutputTypeDef,
-        "PasswordField": PasswordFieldOutputTypeDef,
-        "EmailField": EmailFieldOutputTypeDef,
-        "PhoneNumberFields": List[PhoneNumberFieldOutputTypeDef],
-        "AddressFields": List[AddressFieldOutputTypeDef],
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "EmailField": EmailFieldTypeDef,
+        "PhoneNumberFields": List[PhoneNumberFieldTypeDef],
+        "AddressFields": List[AddressFieldTypeDef],
     },
     total=False,
 )
 
 class RequestInspectionACFPOutputTypeDef(
     _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
 ):
@@ -2488,26 +2212,14 @@
 
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
-RegexPatternSetTypeDef = TypedDict(
-    "RegexPatternSetTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "ARN": str,
-        "Description": str,
-        "RegularExpressionList": List[RegexOutputTypeDef],
-    },
-    total=False,
-)
-
 ResponseInspectionOutputTypeDef = TypedDict(
     "ResponseInspectionOutputTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
         "Header": ResponseInspectionHeaderOutputTypeDef,
         "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
         "Json": ResponseInspectionJsonOutputTypeDef,
@@ -2532,15 +2244,15 @@
         "Header": RateLimitHeaderOutputTypeDef,
         "Cookie": RateLimitCookieOutputTypeDef,
         "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
         "QueryString": RateLimitQueryStringOutputTypeDef,
         "HTTPMethod": Dict[str, Any],
         "ForwardedIP": Dict[str, Any],
         "IP": Dict[str, Any],
-        "LabelNamespace": RateLimitLabelNamespaceOutputTypeDef,
+        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
         "UriPath": RateLimitUriPathOutputTypeDef,
     },
     total=False,
 )
 
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
@@ -2559,27 +2271,53 @@
 )
 
 FilterOutputTypeDef = TypedDict(
     "FilterOutputTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionOutputTypeDef],
+        "Conditions": List[ConditionTypeDef],
     },
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
         "Conditions": Sequence[ConditionTypeDef],
     },
 )
 
+GetMobileSdkReleaseResponseTypeDef = TypedDict(
+    "GetMobileSdkReleaseResponseTypeDef",
+    {
+        "MobileSdkRelease": MobileSdkReleaseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegexPatternSetResponseTypeDef = TypedDict(
+    "GetRegexPatternSetResponseTypeDef",
+    {
+        "RegexPatternSet": RegexPatternSetTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AllowActionOutputTypeDef = TypedDict(
     "AllowActionOutputTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
     total=False,
 )
@@ -2604,22 +2342,14 @@
     "CountActionOutputTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
     total=False,
 )
 
-BlockActionOutputTypeDef = TypedDict(
-    "BlockActionOutputTypeDef",
-    {
-        "CustomResponse": CustomResponseOutputTypeDef,
-    },
-    total=False,
-)
-
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
@@ -2644,14 +2374,22 @@
     "CountActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
 
+BlockActionOutputTypeDef = TypedDict(
+    "BlockActionOutputTypeDef",
+    {
+        "CustomResponse": CustomResponseOutputTypeDef,
+    },
+    total=False,
+)
+
 BlockActionTypeDef = TypedDict(
     "BlockActionTypeDef",
     {
         "CustomResponse": CustomResponseTypeDef,
     },
     total=False,
 )
@@ -2667,15 +2405,15 @@
     "_OptionalSampledHTTPRequestTypeDef",
     {
         "Timestamp": datetime,
         "Action": str,
         "RuleNameWithinRuleGroup": str,
         "RequestHeadersInserted": List[HTTPHeaderTypeDef],
         "ResponseCodeSent": int,
-        "Labels": List[LabelOutputTypeDef],
+        "Labels": List[LabelTypeDef],
         "CaptchaResponse": CaptchaResponseTypeDef,
         "ChallengeResponse": ChallengeResponseTypeDef,
         "OverriddenAction": str,
     },
     total=False,
 )
 
@@ -2683,25 +2421,25 @@
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
 FieldToMatchOutputTypeDef = TypedDict(
     "FieldToMatchOutputTypeDef",
     {
-        "SingleHeader": SingleHeaderOutputTypeDef,
-        "SingleQueryArgument": SingleQueryArgumentOutputTypeDef,
+        "SingleHeader": SingleHeaderTypeDef,
+        "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Dict[str, Any],
         "UriPath": Dict[str, Any],
         "QueryString": Dict[str, Any],
-        "Body": BodyOutputTypeDef,
+        "Body": BodyTypeDef,
         "Method": Dict[str, Any],
         "JsonBody": JsonBodyOutputTypeDef,
         "Headers": HeadersOutputTypeDef,
         "Cookies": CookiesOutputTypeDef,
-        "HeaderOrder": HeaderOrderOutputTypeDef,
+        "HeaderOrder": HeaderOrderTypeDef,
     },
     total=False,
 )
 
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
@@ -2725,40 +2463,14 @@
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMobileSdkReleaseResponseTypeDef = TypedDict(
-    "GetMobileSdkReleaseResponseTypeDef",
-    {
-        "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRegexPatternSetResponseTypeDef = TypedDict(
-    "GetRegexPatternSetResponseTypeDef",
-    {
-        "RegexPatternSet": RegexPatternSetTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPOutputTypeDef,
     },
@@ -2783,15 +2495,15 @@
     {
         "LoginPath": str,
     },
 )
 _OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
     "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
     {
-        "RequestInspection": RequestInspectionOutputTypeDef,
+        "RequestInspection": RequestInspectionTypeDef,
         "ResponseInspection": ResponseInspectionOutputTypeDef,
         "EnableRegexInPath": bool,
     },
     total=False,
 )
 
 class AWSManagedRulesATPRuleSetOutputTypeDef(
@@ -2849,15 +2561,15 @@
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementOutputTypeDef = TypedDict(
     "_OptionalRateBasedStatementOutputTypeDef",
     {
         "ScopeDownStatement": "StatementOutputTypeDef",
-        "ForwardedIPConfig": ForwardedIPConfigOutputTypeDef,
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
         "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
     },
     total=False,
 )
 
 class RateBasedStatementOutputTypeDef(
     _RequiredRateBasedStatementOutputTypeDef, _OptionalRateBasedStatementOutputTypeDef
@@ -2907,14 +2619,23 @@
     {
         "Count": CountActionOutputTypeDef,
         "None": Dict[str, Any],
     },
     total=False,
 )
 
+OverrideActionTypeDef = TypedDict(
+    "OverrideActionTypeDef",
+    {
+        "Count": CountActionTypeDef,
+        "None": Mapping[str, Any],
+    },
+    total=False,
+)
+
 DefaultActionOutputTypeDef = TypedDict(
     "DefaultActionOutputTypeDef",
     {
         "Block": BlockActionOutputTypeDef,
         "Allow": AllowActionOutputTypeDef,
     },
     total=False,
@@ -2928,23 +2649,14 @@
         "Count": CountActionOutputTypeDef,
         "Captcha": CaptchaActionOutputTypeDef,
         "Challenge": ChallengeActionOutputTypeDef,
     },
     total=False,
 )
 
-OverrideActionTypeDef = TypedDict(
-    "OverrideActionTypeDef",
-    {
-        "Count": CountActionTypeDef,
-        "None": Mapping[str, Any],
-    },
-    total=False,
-)
-
 DefaultActionTypeDef = TypedDict(
     "DefaultActionTypeDef",
     {
         "Block": BlockActionTypeDef,
         "Allow": AllowActionTypeDef,
     },
     total=False,
@@ -2973,52 +2685,52 @@
 )
 
 ByteMatchStatementOutputTypeDef = TypedDict(
     "ByteMatchStatementOutputTypeDef",
     {
         "SearchString": bytes,
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 RegexMatchStatementOutputTypeDef = TypedDict(
     "RegexMatchStatementOutputTypeDef",
     {
         "RegexString": str,
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
     "RegexPatternSetReferenceStatementOutputTypeDef",
     {
         "ARN": str,
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 SizeConstraintStatementOutputTypeDef = TypedDict(
     "SizeConstraintStatementOutputTypeDef",
     {
         "FieldToMatch": FieldToMatchOutputTypeDef,
         "ComparisonOperator": ComparisonOperatorType,
         "Size": int,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 _RequiredSqliMatchStatementOutputTypeDef = TypedDict(
     "_RequiredSqliMatchStatementOutputTypeDef",
     {
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 _OptionalSqliMatchStatementOutputTypeDef = TypedDict(
     "_OptionalSqliMatchStatementOutputTypeDef",
     {
         "SensitivityLevel": SensitivityLevelType,
     },
@@ -3030,15 +2742,15 @@
 ):
     pass
 
 XssMatchStatementOutputTypeDef = TypedDict(
     "XssMatchStatementOutputTypeDef",
     {
         "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationOutputTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": Union[str, bytes, IO[Any], StreamingBody],
@@ -3105,17 +2817,17 @@
 )
 
 ManagedRuleGroupConfigOutputTypeDef = TypedDict(
     "ManagedRuleGroupConfigOutputTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
-        "UsernameField": UsernameFieldOutputTypeDef,
-        "PasswordField": PasswordFieldOutputTypeDef,
-        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetOutputTypeDef,
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
     },
     total=False,
 )
 
 ManagedRuleGroupConfigTypeDef = TypedDict(
@@ -3186,25 +2898,25 @@
 
 _RequiredRuleOutputTypeDef = TypedDict(
     "_RequiredRuleOutputTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementOutputTypeDef",
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalRuleOutputTypeDef = TypedDict(
     "_OptionalRuleOutputTypeDef",
     {
         "Action": RuleActionOutputTypeDef,
         "OverrideAction": OverrideActionOutputTypeDef,
-        "RuleLabels": List[LabelOutputTypeDef],
-        "CaptchaConfig": CaptchaConfigOutputTypeDef,
-        "ChallengeConfig": ChallengeConfigOutputTypeDef,
+        "RuleLabels": List[LabelTypeDef],
+        "CaptchaConfig": CaptchaConfigTypeDef,
+        "ChallengeConfig": ChallengeConfigTypeDef,
     },
     total=False,
 )
 
 class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
     pass
 
@@ -3288,15 +3000,15 @@
         "Name": str,
     },
 )
 _OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementOutputTypeDef",
     {
         "Version": str,
-        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
         "ScopeDownStatement": Dict[str, Any],
         "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
         "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
     },
     total=False,
 )
 
@@ -3310,15 +3022,15 @@
     {
         "ARN": str,
     },
 )
 _OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
     "_OptionalRuleGroupReferenceStatementOutputTypeDef",
     {
-        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
         "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
     },
     total=False,
 )
 
 class RuleGroupReferenceStatementOutputTypeDef(
     _RequiredRuleGroupReferenceStatementOutputTypeDef,
@@ -3329,24 +3041,24 @@
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "Name": str,
         "Id": str,
         "Capacity": int,
         "ARN": str,
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
     "_OptionalRuleGroupTypeDef",
     {
         "Description": str,
         "Rules": List[RuleOutputTypeDef],
         "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "AvailableLabels": List[LabelSummaryTypeDef],
         "ConsumedLabels": List[LabelSummaryTypeDef],
     },
     total=False,
 )
 
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
@@ -3541,22 +3253,22 @@
     {
         "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
         "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
         "XssMatchStatement": XssMatchStatementOutputTypeDef,
         "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
         "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
         "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
         "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
         "RateBasedStatement": Dict[str, Any],
         "AndStatement": Dict[str, Any],
         "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
         "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementOutputTypeDef,
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
         "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
     },
     total=False,
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
@@ -3592,41 +3304,41 @@
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
         "OverrideAction": OverrideActionOutputTypeDef,
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
         "DefaultAction": DefaultActionOutputTypeDef,
-        "VisibilityConfig": VisibilityConfigOutputTypeDef,
+        "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
         "Rules": List[RuleOutputTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyOutputTypeDef],
-        "CaptchaConfig": CaptchaConfigOutputTypeDef,
-        "ChallengeConfig": ChallengeConfigOutputTypeDef,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
+        "CaptchaConfig": CaptchaConfigTypeDef,
+        "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
         "AssociationConfig": AssociationConfigOutputTypeDef,
     },
     total=False,
 )
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
```

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/PKG-INFO` & `mypy-boto3-wafv2-1.28.15/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-wafv2
-Version: 1.28.12
-Summary: Type annotations for boto3.WAFV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 wafv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-wafv2"></a>
 
 # mypy-boto3-wafv2
 
 [![PyPI - mypy-boto3-wafv2](https://img.shields.io/pypi/v/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,75 +290,58 @@
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
-    AWSManagedRulesBotControlRuleSetOutputTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
-    ActionConditionOutputTypeDef,
     ActionConditionTypeDef,
-    AddressFieldOutputTypeDef,
     AddressFieldTypeDef,
     AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
-    RequestBodyAssociatedResourceTypeConfigOutputTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
-    BodyOutputTypeDef,
     BodyTypeDef,
-    TextTransformationOutputTypeDef,
     TextTransformationTypeDef,
-    ImmunityTimePropertyOutputTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
     ResponseMetadataTypeDef,
-    LabelNameConditionOutputTypeDef,
     LabelNameConditionTypeDef,
     CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
-    CustomHTTPHeaderOutputTypeDef,
     CustomHTTPHeaderTypeDef,
-    CustomResponseBodyOutputTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
     ManagedProductDescriptorTypeDef,
     DescribeManagedProductsByVendorRequestRequestTypeDef,
     DescribeManagedRuleGroupRequestRequestTypeDef,
     LabelSummaryTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
-    EmailFieldOutputTypeDef,
     EmailFieldTypeDef,
-    ExcludedRuleOutputTypeDef,
     ExcludedRuleTypeDef,
-    HeaderOrderOutputTypeDef,
-    SingleHeaderOutputTypeDef,
-    SingleQueryArgumentOutputTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
-    VisibilityConfigOutputTypeDef,
-    ForwardedIPConfigOutputTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
@@ -403,21 +354,18 @@
     TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
-    IPSetForwardedIPConfigOutputTypeDef,
     IPSetForwardedIPConfigTypeDef,
     JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
-    LabelMatchStatementOutputTypeDef,
     LabelMatchStatementTypeDef,
-    LabelOutputTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
     ManagedRuleGroupSummaryTypeDef,
     ListIPSetsRequestRequestTypeDef,
@@ -427,56 +375,47 @@
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
-    PasswordFieldOutputTypeDef,
-    UsernameFieldOutputTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
-    TagOutputTypeDef,
-    NotStatementOutputTypeDef,
     NotStatementTypeDef,
     OrStatementOutputTypeDef,
     OrStatementTypeDef,
-    PhoneNumberFieldOutputTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
-    RateLimitLabelNamespaceOutputTypeDef,
     RateLimitLabelNamespaceTypeDef,
-    RegexOutputTypeDef,
     ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     RateLimitCookieOutputTypeDef,
-    RateLimitHeaderOutputTypeDef,
-    RateLimitQueryArgumentOutputTypeDef,
-    RateLimitQueryStringOutputTypeDef,
-    RateLimitUriPathOutputTypeDef,
     RateLimitCookieTypeDef,
+    RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
     RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringOutputTypeDef,
     RateLimitQueryStringTypeDef,
+    RateLimitUriPathOutputTypeDef,
     RateLimitUriPathTypeDef,
-    CaptchaConfigOutputTypeDef,
-    ChallengeConfigOutputTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
@@ -485,96 +424,93 @@
     ListResourcesForWebACLResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
-    ConditionOutputTypeDef,
     ConditionTypeDef,
     CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
+    MobileSdkReleaseTypeDef,
+    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
+    RegexPatternSetTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
     CustomRequestHandlingOutputTypeDef,
-    CustomResponseOutputTypeDef,
     CustomRequestHandlingTypeDef,
+    CustomResponseOutputTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
     GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
-    IPSetReferenceStatementOutputTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
-    RequestInspectionOutputTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
-    MobileSdkReleaseTypeDef,
-    TagInfoForResourceTypeDef,
     RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
-    RegexPatternSetTypeDef,
     ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
     RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
     FilterOutputTypeDef,
     FilterTypeDef,
+    GetMobileSdkReleaseResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetRegexPatternSetResponseTypeDef,
     AllowActionOutputTypeDef,
     CaptchaActionOutputTypeDef,
     ChallengeActionOutputTypeDef,
     CountActionOutputTypeDef,
-    BlockActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
+    BlockActionOutputTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
     FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
-    GetMobileSdkReleaseResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetRegexPatternSetResponseTypeDef,
     AWSManagedRulesACFPRuleSetOutputTypeDef,
     AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
     RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
     LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
     OverrideActionOutputTypeDef,
+    OverrideActionTypeDef,
     DefaultActionOutputTypeDef,
     RuleActionOutputTypeDef,
-    OverrideActionTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
     ByteMatchStatementOutputTypeDef,
     RegexMatchStatementOutputTypeDef,
     RegexPatternSetReferenceStatementOutputTypeDef,
     SizeConstraintStatementOutputTypeDef,
```

### Comparing `mypy-boto3-wafv2-1.28.12/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.28.15/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.12/setup.py` & `mypy-boto3-wafv2-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFV2 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

