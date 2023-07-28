# Comparing `tmp/mypy-boto3-waf-regional-1.28.12.tar.gz` & `tmp/mypy-boto3-waf-regional-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-regional-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-regional-1.28.15.tar", last modified: Fri Jul 28 20:43:55 2023, max compression
```

## Comparing `mypy-boto3-waf-regional-1.28.12.tar` & `mypy-boto3-waf-regional-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.193489 mypy-boto3-waf-regional-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-27 11:49:49.189489 mypy-boto3-waf-regional-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.185489 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-27 11:48:28.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-27 11:48:28.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-27 11:48:28.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59977 2023-07-27 11:48:29.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59924 2023-07-27 11:48:29.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.189489 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 11:49:49.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 11:49:48.000000 mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.193489 mypy-boto3-waf-regional-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 11:48:27.000000 mypy-boto3-waf-regional-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.638027 mypy-boto3-waf-regional-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-07-28 20:43:55.634027 mypy-boto3-waf-regional-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.630027 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57158 2023-07-28 20:41:10.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57107 2023-07-28 20:41:09.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.634027 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:55.000000 mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:55.638027 mypy-boto3-waf-regional-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:41:08.000000 mypy-boto3-waf-regional-1.28.15/setup.py
```

### Comparing `mypy-boto3-waf-regional-1.28.12/LICENSE` & `mypy-boto3-waf-regional-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.12/PKG-INFO` & `mypy-boto3-waf-regional-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.12
-Summary: Type annotations for boto3.WAFRegional 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,23 +311,19 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
-    ExcludedRuleOutputTypeDef,
-    WafActionOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     ByteMatchSetSummaryTypeDef,
-    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
@@ -349,15 +345,14 @@
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
-    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
@@ -373,15 +368,14 @@
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
-    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
@@ -401,29 +395,23 @@
     SqlInjectionMatchSetSummaryTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    TagOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     ActivatedRuleOutputTypeDef,
     ActivatedRuleTypeDef,
     ByteMatchTupleOutputTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    RegexMatchTupleOutputTypeDef,
-    SizeConstraintOutputTypeDef,
-    SqlInjectionMatchTupleOutputTypeDef,
-    XssMatchTupleOutputTypeDef,
     ByteMatchTupleTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     RegexMatchTupleTypeDef,
     SizeConstraintTypeDef,
     SqlInjectionMatchTupleTypeDef,
     XssMatchTupleTypeDef,
     CreateWebACLMigrationStackResponseTypeDef,
     DeleteByteMatchSetResponseTypeDef,
@@ -456,14 +444,15 @@
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
+    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
@@ -484,71 +473,70 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
-    TagInfoForResourceTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
     WebACLTypeDef,
     RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
+    ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
-    RegexMatchSetTypeDef,
-    SizeConstraintSetTypeDef,
-    SqlInjectionMatchSetTypeDef,
-    XssMatchSetTypeDef,
-    ByteMatchSetUpdateTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
+    RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
+    SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
+    SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
+    XssMatchSetTypeDef,
     XssMatchSetUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGeoMatchSetResponseTypeDef,
     GetGeoMatchSetResponseTypeDef,
     UpdateGeoMatchSetRequestRequestTypeDef,
     SampledHTTPRequestTypeDef,
     CreateIPSetResponseTypeDef,
     GetIPSetResponseTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
+    UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
+    UpdateRegexMatchSetRequestRequestTypeDef,
     CreateSizeConstraintSetResponseTypeDef,
     GetSizeConstraintSetResponseTypeDef,
+    UpdateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetResponseTypeDef,
     GetSqlInjectionMatchSetResponseTypeDef,
+    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
-    UpdateByteMatchSetRequestRequestTypeDef,
-    UpdateRegexMatchSetRequestRequestTypeDef,
-    UpdateSizeConstraintSetRequestRequestTypeDef,
-    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleOutputTypeDef:
+def get_structure() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-regional-1.28.12/README.md` & `mypy-boto3-waf-regional-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,23 +279,19 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
-    ExcludedRuleOutputTypeDef,
-    WafActionOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     ByteMatchSetSummaryTypeDef,
-    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
@@ -317,15 +313,14 @@
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
-    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
@@ -341,15 +336,14 @@
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
-    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
@@ -369,29 +363,23 @@
     SqlInjectionMatchSetSummaryTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    TagOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     ActivatedRuleOutputTypeDef,
     ActivatedRuleTypeDef,
     ByteMatchTupleOutputTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    RegexMatchTupleOutputTypeDef,
-    SizeConstraintOutputTypeDef,
-    SqlInjectionMatchTupleOutputTypeDef,
-    XssMatchTupleOutputTypeDef,
     ByteMatchTupleTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     RegexMatchTupleTypeDef,
     SizeConstraintTypeDef,
     SqlInjectionMatchTupleTypeDef,
     XssMatchTupleTypeDef,
     CreateWebACLMigrationStackResponseTypeDef,
     DeleteByteMatchSetResponseTypeDef,
@@ -424,14 +412,15 @@
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
+    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
@@ -452,71 +441,70 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
-    TagInfoForResourceTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
     WebACLTypeDef,
     RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
+    ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
-    RegexMatchSetTypeDef,
-    SizeConstraintSetTypeDef,
-    SqlInjectionMatchSetTypeDef,
-    XssMatchSetTypeDef,
-    ByteMatchSetUpdateTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
+    RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
+    SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
+    SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
+    XssMatchSetTypeDef,
     XssMatchSetUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGeoMatchSetResponseTypeDef,
     GetGeoMatchSetResponseTypeDef,
     UpdateGeoMatchSetRequestRequestTypeDef,
     SampledHTTPRequestTypeDef,
     CreateIPSetResponseTypeDef,
     GetIPSetResponseTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
+    UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
+    UpdateRegexMatchSetRequestRequestTypeDef,
     CreateSizeConstraintSetResponseTypeDef,
     GetSizeConstraintSetResponseTypeDef,
+    UpdateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetResponseTypeDef,
     GetSqlInjectionMatchSetResponseTypeDef,
+    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
-    UpdateByteMatchSetRequestRequestTypeDef,
-    UpdateRegexMatchSetRequestRequestTypeDef,
-    UpdateSizeConstraintSetRequestRequestTypeDef,
-    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleOutputTypeDef:
+def get_structure() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/__main__.py` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFRegional 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.WAFRegional 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional\nOther"
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

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.py` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/client.pyi` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.py` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/literals.pyi` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.py` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for waf-regional service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf_regional.type_defs import ExcludedRuleOutputTypeDef
+    from mypy_boto3_waf_regional.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleOutputTypeDef = {...}
+    data: ExcludedRuleTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,23 +40,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ExcludedRuleOutputTypeDef",
-    "WafActionOutputTypeDef",
-    "WafOverrideActionOutputTypeDef",
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "ByteMatchSetSummaryTypeDef",
-    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
@@ -78,15 +74,14 @@
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
-    "GeoMatchConstraintOutputTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
@@ -102,15 +97,14 @@
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
-    "IPSetDescriptorOutputTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
@@ -130,29 +124,23 @@
     "SqlInjectionMatchSetSummaryTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
-    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
-    "TagOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ActivatedRuleOutputTypeDef",
     "ActivatedRuleTypeDef",
     "ByteMatchTupleOutputTypeDef",
-    "LoggingConfigurationOutputTypeDef",
-    "RegexMatchTupleOutputTypeDef",
-    "SizeConstraintOutputTypeDef",
-    "SqlInjectionMatchTupleOutputTypeDef",
-    "XssMatchTupleOutputTypeDef",
     "ByteMatchTupleTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "RegexMatchTupleTypeDef",
     "SizeConstraintTypeDef",
     "SqlInjectionMatchTupleTypeDef",
     "XssMatchTupleTypeDef",
     "CreateWebACLMigrationStackResponseTypeDef",
     "DeleteByteMatchSetResponseTypeDef",
@@ -185,14 +173,15 @@
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
+    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
@@ -213,90 +202,68 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
-    "TagInfoForResourceTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     "WebACLTypeDef",
     "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
+    "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
-    "RegexMatchSetTypeDef",
-    "SizeConstraintSetTypeDef",
-    "SqlInjectionMatchSetTypeDef",
-    "XssMatchSetTypeDef",
-    "ByteMatchSetUpdateTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
+    "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
+    "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
+    "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
+    "XssMatchSetTypeDef",
     "XssMatchSetUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateGeoMatchSetResponseTypeDef",
     "GetGeoMatchSetResponseTypeDef",
     "UpdateGeoMatchSetRequestRequestTypeDef",
     "SampledHTTPRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "GetIPSetResponseTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
+    "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
+    "UpdateRegexMatchSetRequestRequestTypeDef",
     "CreateSizeConstraintSetResponseTypeDef",
     "GetSizeConstraintSetResponseTypeDef",
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetResponseTypeDef",
     "GetSqlInjectionMatchSetResponseTypeDef",
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateXssMatchSetResponseTypeDef",
     "GetXssMatchSetResponseTypeDef",
-    "UpdateByteMatchSetRequestRequestTypeDef",
-    "UpdateRegexMatchSetRequestRequestTypeDef",
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "UpdateXssMatchSetRequestRequestTypeDef",
     "GetSampledRequestsResponseTypeDef",
 )
 
-ExcludedRuleOutputTypeDef = TypedDict(
-    "ExcludedRuleOutputTypeDef",
-    {
-        "RuleId": str,
-    },
-)
-
-WafActionOutputTypeDef = TypedDict(
-    "WafActionOutputTypeDef",
-    {
-        "Type": WafActionTypeType,
-    },
-)
-
-WafOverrideActionOutputTypeDef = TypedDict(
-    "WafOverrideActionOutputTypeDef",
-    {
-        "Type": WafOverrideActionTypeType,
-    },
-)
-
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -326,35 +293,14 @@
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
 
-_RequiredFieldToMatchOutputTypeDef = TypedDict(
-    "_RequiredFieldToMatchOutputTypeDef",
-    {
-        "Type": MatchFieldTypeType,
-    },
-)
-_OptionalFieldToMatchOutputTypeDef = TypedDict(
-    "_OptionalFieldToMatchOutputTypeDef",
-    {
-        "Data": str,
-    },
-    total=False,
-)
-
-
-class FieldToMatchOutputTypeDef(
-    _RequiredFieldToMatchOutputTypeDef, _OptionalFieldToMatchOutputTypeDef
-):
-    pass
-
-
 _RequiredFieldToMatchTypeDef = TypedDict(
     "_RequiredFieldToMatchTypeDef",
     {
         "Type": MatchFieldTypeType,
     },
 )
 _OptionalFieldToMatchTypeDef = TypedDict(
@@ -615,22 +561,14 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GeoMatchConstraintOutputTypeDef = TypedDict(
-    "GeoMatchConstraintOutputTypeDef",
-    {
-        "Type": Literal["Country"],
-        "Value": GeoMatchConstraintValueType,
-    },
-)
-
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
         "Value": GeoMatchConstraintValueType,
     },
 )
@@ -806,22 +744,14 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-IPSetDescriptorOutputTypeDef = TypedDict(
-    "IPSetDescriptorOutputTypeDef",
-    {
-        "Type": IPSetDescriptorTypeType,
-        "Value": str,
-    },
-)
-
 IPSetDescriptorTypeDef = TypedDict(
     "IPSetDescriptorTypeDef",
     {
         "Type": IPSetDescriptorTypeType,
         "Value": str,
     },
 )
@@ -1076,23 +1006,14 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
     },
 )
 
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
-    {
-        "Negated": bool,
-        "Type": PredicateTypeType,
-        "DataId": str,
-    },
-)
-
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
         "DataId": str,
     },
@@ -1110,22 +1031,14 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1136,18 +1049,18 @@
         "Priority": int,
         "RuleId": str,
     },
 )
 _OptionalActivatedRuleOutputTypeDef = TypedDict(
     "_OptionalActivatedRuleOutputTypeDef",
     {
-        "Action": WafActionOutputTypeDef,
-        "OverrideAction": WafOverrideActionOutputTypeDef,
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
         "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
     },
     total=False,
 )
 
 
 class ActivatedRuleOutputTypeDef(
     _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
@@ -1177,88 +1090,53 @@
 class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
     pass
 
 
 ByteMatchTupleOutputTypeDef = TypedDict(
     "ByteMatchTupleOutputTypeDef",
     {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
         "TargetString": bytes,
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
+ByteMatchTupleTypeDef = TypedDict(
+    "ByteMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
 _RequiredLoggingConfigurationOutputTypeDef = TypedDict(
     "_RequiredLoggingConfigurationOutputTypeDef",
     {
         "ResourceArn": str,
         "LogDestinationConfigs": List[str],
     },
 )
 _OptionalLoggingConfigurationOutputTypeDef = TypedDict(
     "_OptionalLoggingConfigurationOutputTypeDef",
     {
-        "RedactedFields": List[FieldToMatchOutputTypeDef],
+        "RedactedFields": List[FieldToMatchTypeDef],
     },
     total=False,
 )
 
 
 class LoggingConfigurationOutputTypeDef(
     _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
 ):
     pass
 
 
-RegexMatchTupleOutputTypeDef = TypedDict(
-    "RegexMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-        "RegexPatternSetId": str,
-    },
-)
-
-SizeConstraintOutputTypeDef = TypedDict(
-    "SizeConstraintOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
-    },
-)
-
-SqlInjectionMatchTupleOutputTypeDef = TypedDict(
-    "SqlInjectionMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-    },
-)
-
-XssMatchTupleOutputTypeDef = TypedDict(
-    "XssMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-    },
-)
-
-ByteMatchTupleTypeDef = TypedDict(
-    "ByteMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
         "LogDestinationConfigs": Sequence[str],
     },
 )
@@ -1654,14 +1532,23 @@
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
 
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
@@ -1700,15 +1587,15 @@
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
-        "GeoMatchConstraints": List[GeoMatchConstraintOutputTypeDef],
+        "GeoMatchConstraints": List[GeoMatchConstraintTypeDef],
     },
 )
 _OptionalGeoMatchSetTypeDef = TypedDict(
     "_OptionalGeoMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1777,15 +1664,15 @@
     total=False,
 )
 
 _RequiredIPSetTypeDef = TypedDict(
     "_RequiredIPSetTypeDef",
     {
         "IPSetId": str,
-        "IPSetDescriptors": List[IPSetDescriptorOutputTypeDef],
+        "IPSetDescriptors": List[IPSetDescriptorTypeDef],
     },
 )
 _OptionalIPSetTypeDef = TypedDict(
     "_OptionalIPSetTypeDef",
     {
         "Name": str,
     },
@@ -1895,15 +1782,15 @@
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
-        "MatchPredicates": List[PredicateOutputTypeDef],
+        "MatchPredicates": List[PredicateTypeDef],
         "RateKey": Literal["IP"],
         "RateLimit": int,
     },
 )
 _OptionalRateBasedRuleTypeDef = TypedDict(
     "_OptionalRateBasedRuleTypeDef",
     {
@@ -1918,15 +1805,15 @@
     pass
 
 
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "RuleId": str,
-        "Predicates": List[PredicateOutputTypeDef],
+        "Predicates": List[PredicateTypeDef],
     },
 )
 _OptionalRuleTypeDef = TypedDict(
     "_OptionalRuleTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1952,37 +1839,28 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
-TagInfoForResourceTypeDef = TypedDict(
-    "TagInfoForResourceTypeDef",
-    {
-        "ResourceARN": str,
-        "TagList": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
         "ActivatedRules": List[ActivatedRuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
-        "DefaultAction": WafActionOutputTypeDef,
+        "DefaultAction": WafActionTypeDef,
         "Rules": List[ActivatedRuleOutputTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
@@ -2029,14 +1907,22 @@
 )
 
 
 class ByteMatchSetTypeDef(_RequiredByteMatchSetTypeDef, _OptionalByteMatchSetTypeDef):
     pass
 
 
+ByteMatchSetUpdateTypeDef = TypedDict(
+    "ByteMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ByteMatchTuple": ByteMatchTupleTypeDef,
+    },
+)
+
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2054,29 +1940,44 @@
     "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    {
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+    },
+)
+
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
-        "RegexMatchTuples": List[RegexMatchTupleOutputTypeDef],
+        "RegexMatchTuples": List[RegexMatchTupleTypeDef],
     },
     total=False,
 )
 
+RegexMatchSetUpdateTypeDef = TypedDict(
+    "RegexMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "RegexMatchTuple": RegexMatchTupleTypeDef,
+    },
+)
+
 _RequiredSizeConstraintSetTypeDef = TypedDict(
     "_RequiredSizeConstraintSetTypeDef",
     {
         "SizeConstraintSetId": str,
-        "SizeConstraints": List[SizeConstraintOutputTypeDef],
+        "SizeConstraints": List[SizeConstraintTypeDef],
     },
 )
 _OptionalSizeConstraintSetTypeDef = TypedDict(
     "_OptionalSizeConstraintSetTypeDef",
     {
         "Name": str,
     },
@@ -2086,19 +1987,27 @@
 
 class SizeConstraintSetTypeDef(
     _RequiredSizeConstraintSetTypeDef, _OptionalSizeConstraintSetTypeDef
 ):
     pass
 
 
+SizeConstraintSetUpdateTypeDef = TypedDict(
+    "SizeConstraintSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SizeConstraint": SizeConstraintTypeDef,
+    },
+)
+
 _RequiredSqlInjectionMatchSetTypeDef = TypedDict(
     "_RequiredSqlInjectionMatchSetTypeDef",
     {
         "SqlInjectionMatchSetId": str,
-        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleOutputTypeDef],
+        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleTypeDef],
     },
 )
 _OptionalSqlInjectionMatchSetTypeDef = TypedDict(
     "_OptionalSqlInjectionMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -2108,19 +2017,27 @@
 
 class SqlInjectionMatchSetTypeDef(
     _RequiredSqlInjectionMatchSetTypeDef, _OptionalSqlInjectionMatchSetTypeDef
 ):
     pass
 
 
+SqlInjectionMatchSetUpdateTypeDef = TypedDict(
+    "SqlInjectionMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
+    },
+)
+
 _RequiredXssMatchSetTypeDef = TypedDict(
     "_RequiredXssMatchSetTypeDef",
     {
         "XssMatchSetId": str,
-        "XssMatchTuples": List[XssMatchTupleOutputTypeDef],
+        "XssMatchTuples": List[XssMatchTupleTypeDef],
     },
 )
 _OptionalXssMatchSetTypeDef = TypedDict(
     "_OptionalXssMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -2128,58 +2045,28 @@
 )
 
 
 class XssMatchSetTypeDef(_RequiredXssMatchSetTypeDef, _OptionalXssMatchSetTypeDef):
     pass
 
 
-ByteMatchSetUpdateTypeDef = TypedDict(
-    "ByteMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ByteMatchTuple": ByteMatchTupleTypeDef,
-    },
-)
-
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
-    {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-    },
-)
-
-RegexMatchSetUpdateTypeDef = TypedDict(
-    "RegexMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "RegexMatchTuple": RegexMatchTupleTypeDef,
-    },
-)
-
-SizeConstraintSetUpdateTypeDef = TypedDict(
-    "SizeConstraintSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "SizeConstraint": SizeConstraintTypeDef,
-    },
-)
-
-SqlInjectionMatchSetUpdateTypeDef = TypedDict(
-    "SqlInjectionMatchSetUpdateTypeDef",
+XssMatchSetUpdateTypeDef = TypedDict(
+    "XssMatchSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
-        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
+        "XssMatchTuple": XssMatchTupleTypeDef,
     },
 )
 
-XssMatchSetUpdateTypeDef = TypedDict(
-    "XssMatchSetUpdateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Action": ChangeActionType,
-        "XssMatchTuple": XssMatchTupleTypeDef,
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
@@ -2304,23 +2191,14 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2379,14 +2257,23 @@
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateByteMatchSetRequestRequestTypeDef",
+    {
+        "ByteMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
+    },
+)
+
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2396,14 +2283,23 @@
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateRegexMatchSetRequestRequestTypeDef",
+    {
+        "RegexMatchSetId": str,
+        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
+        "ChangeToken": str,
+    },
+)
+
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2413,14 +2309,23 @@
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
+    {
+        "SizeConstraintSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
+    },
+)
+
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2430,14 +2335,23 @@
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
+    {
+        "SqlInjectionMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
+    },
+)
+
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2447,50 +2361,14 @@
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateByteMatchSetRequestRequestTypeDef",
-    {
-        "ByteMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
-    },
-)
-
-UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateRegexMatchSetRequestRequestTypeDef",
-    {
-        "RegexMatchSetId": str,
-        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
-        "ChangeToken": str,
-    },
-)
-
-UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
-    {
-        "SizeConstraintSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
-    },
-)
-
-UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
-    {
-        "SqlInjectionMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
-    },
-)
-
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
         "Updates": Sequence[XssMatchSetUpdateTypeDef],
     },
```

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional/type_defs.pyi` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for waf-regional service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf_regional.type_defs import ExcludedRuleOutputTypeDef
+    from mypy_boto3_waf_regional.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleOutputTypeDef = {...}
+    data: ExcludedRuleTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -39,23 +39,19 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ExcludedRuleOutputTypeDef",
-    "WafActionOutputTypeDef",
-    "WafOverrideActionOutputTypeDef",
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "ByteMatchSetSummaryTypeDef",
-    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
@@ -77,15 +73,14 @@
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
     "DisassociateWebACLRequestRequestTypeDef",
-    "GeoMatchConstraintOutputTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
@@ -101,15 +96,14 @@
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
-    "IPSetDescriptorOutputTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
     "ListIPSetsRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
@@ -129,29 +123,23 @@
     "SqlInjectionMatchSetSummaryTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
-    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
-    "TagOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ActivatedRuleOutputTypeDef",
     "ActivatedRuleTypeDef",
     "ByteMatchTupleOutputTypeDef",
-    "LoggingConfigurationOutputTypeDef",
-    "RegexMatchTupleOutputTypeDef",
-    "SizeConstraintOutputTypeDef",
-    "SqlInjectionMatchTupleOutputTypeDef",
-    "XssMatchTupleOutputTypeDef",
     "ByteMatchTupleTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "RegexMatchTupleTypeDef",
     "SizeConstraintTypeDef",
     "SqlInjectionMatchTupleTypeDef",
     "XssMatchTupleTypeDef",
     "CreateWebACLMigrationStackResponseTypeDef",
     "DeleteByteMatchSetResponseTypeDef",
@@ -184,14 +172,15 @@
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
+    "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
@@ -212,90 +201,68 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
-    "TagInfoForResourceTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     "WebACLTypeDef",
     "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
+    "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
-    "RegexMatchSetTypeDef",
-    "SizeConstraintSetTypeDef",
-    "SqlInjectionMatchSetTypeDef",
-    "XssMatchSetTypeDef",
-    "ByteMatchSetUpdateTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
+    "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
+    "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
+    "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
+    "XssMatchSetTypeDef",
     "XssMatchSetUpdateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateGeoMatchSetResponseTypeDef",
     "GetGeoMatchSetResponseTypeDef",
     "UpdateGeoMatchSetRequestRequestTypeDef",
     "SampledHTTPRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "GetIPSetResponseTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
+    "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
+    "UpdateRegexMatchSetRequestRequestTypeDef",
     "CreateSizeConstraintSetResponseTypeDef",
     "GetSizeConstraintSetResponseTypeDef",
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetResponseTypeDef",
     "GetSqlInjectionMatchSetResponseTypeDef",
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateXssMatchSetResponseTypeDef",
     "GetXssMatchSetResponseTypeDef",
-    "UpdateByteMatchSetRequestRequestTypeDef",
-    "UpdateRegexMatchSetRequestRequestTypeDef",
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     "UpdateXssMatchSetRequestRequestTypeDef",
     "GetSampledRequestsResponseTypeDef",
 )
 
-ExcludedRuleOutputTypeDef = TypedDict(
-    "ExcludedRuleOutputTypeDef",
-    {
-        "RuleId": str,
-    },
-)
-
-WafActionOutputTypeDef = TypedDict(
-    "WafActionOutputTypeDef",
-    {
-        "Type": WafActionTypeType,
-    },
-)
-
-WafOverrideActionOutputTypeDef = TypedDict(
-    "WafOverrideActionOutputTypeDef",
-    {
-        "Type": WafOverrideActionTypeType,
-    },
-)
-
 ExcludedRuleTypeDef = TypedDict(
     "ExcludedRuleTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -325,33 +292,14 @@
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
 
-_RequiredFieldToMatchOutputTypeDef = TypedDict(
-    "_RequiredFieldToMatchOutputTypeDef",
-    {
-        "Type": MatchFieldTypeType,
-    },
-)
-_OptionalFieldToMatchOutputTypeDef = TypedDict(
-    "_OptionalFieldToMatchOutputTypeDef",
-    {
-        "Data": str,
-    },
-    total=False,
-)
-
-class FieldToMatchOutputTypeDef(
-    _RequiredFieldToMatchOutputTypeDef, _OptionalFieldToMatchOutputTypeDef
-):
-    pass
-
 _RequiredFieldToMatchTypeDef = TypedDict(
     "_RequiredFieldToMatchTypeDef",
     {
         "Type": MatchFieldTypeType,
     },
 )
 _OptionalFieldToMatchTypeDef = TypedDict(
@@ -606,22 +554,14 @@
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GeoMatchConstraintOutputTypeDef = TypedDict(
-    "GeoMatchConstraintOutputTypeDef",
-    {
-        "Type": Literal["Country"],
-        "Value": GeoMatchConstraintValueType,
-    },
-)
-
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
         "Value": GeoMatchConstraintValueType,
     },
 )
@@ -795,22 +735,14 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-IPSetDescriptorOutputTypeDef = TypedDict(
-    "IPSetDescriptorOutputTypeDef",
-    {
-        "Type": IPSetDescriptorTypeType,
-        "Value": str,
-    },
-)
-
 IPSetDescriptorTypeDef = TypedDict(
     "IPSetDescriptorTypeDef",
     {
         "Type": IPSetDescriptorTypeType,
         "Value": str,
     },
 )
@@ -1061,23 +993,14 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
     },
 )
 
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
-    {
-        "Negated": bool,
-        "Type": PredicateTypeType,
-        "DataId": str,
-    },
-)
-
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
         "DataId": str,
     },
@@ -1095,22 +1018,14 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1121,18 +1036,18 @@
         "Priority": int,
         "RuleId": str,
     },
 )
 _OptionalActivatedRuleOutputTypeDef = TypedDict(
     "_OptionalActivatedRuleOutputTypeDef",
     {
-        "Action": WafActionOutputTypeDef,
-        "OverrideAction": WafOverrideActionOutputTypeDef,
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
         "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleOutputTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
     },
     total=False,
 )
 
 class ActivatedRuleOutputTypeDef(
     _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
 ):
@@ -1158,86 +1073,51 @@
 
 class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
     pass
 
 ByteMatchTupleOutputTypeDef = TypedDict(
     "ByteMatchTupleOutputTypeDef",
     {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "FieldToMatch": FieldToMatchTypeDef,
         "TargetString": bytes,
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
+ByteMatchTupleTypeDef = TypedDict(
+    "ByteMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
 _RequiredLoggingConfigurationOutputTypeDef = TypedDict(
     "_RequiredLoggingConfigurationOutputTypeDef",
     {
         "ResourceArn": str,
         "LogDestinationConfigs": List[str],
     },
 )
 _OptionalLoggingConfigurationOutputTypeDef = TypedDict(
     "_OptionalLoggingConfigurationOutputTypeDef",
     {
-        "RedactedFields": List[FieldToMatchOutputTypeDef],
+        "RedactedFields": List[FieldToMatchTypeDef],
     },
     total=False,
 )
 
 class LoggingConfigurationOutputTypeDef(
     _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
 ):
     pass
 
-RegexMatchTupleOutputTypeDef = TypedDict(
-    "RegexMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-        "RegexPatternSetId": str,
-    },
-)
-
-SizeConstraintOutputTypeDef = TypedDict(
-    "SizeConstraintOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
-    },
-)
-
-SqlInjectionMatchTupleOutputTypeDef = TypedDict(
-    "SqlInjectionMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-    },
-)
-
-XssMatchTupleOutputTypeDef = TypedDict(
-    "XssMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformation": TextTransformationType,
-    },
-)
-
-ByteMatchTupleTypeDef = TypedDict(
-    "ByteMatchTupleTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
         "LogDestinationConfigs": Sequence[str],
     },
 )
@@ -1623,14 +1503,23 @@
 )
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
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
@@ -1669,15 +1558,15 @@
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
-        "GeoMatchConstraints": List[GeoMatchConstraintOutputTypeDef],
+        "GeoMatchConstraints": List[GeoMatchConstraintTypeDef],
     },
 )
 _OptionalGeoMatchSetTypeDef = TypedDict(
     "_OptionalGeoMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1744,15 +1633,15 @@
     total=False,
 )
 
 _RequiredIPSetTypeDef = TypedDict(
     "_RequiredIPSetTypeDef",
     {
         "IPSetId": str,
-        "IPSetDescriptors": List[IPSetDescriptorOutputTypeDef],
+        "IPSetDescriptors": List[IPSetDescriptorTypeDef],
     },
 )
 _OptionalIPSetTypeDef = TypedDict(
     "_OptionalIPSetTypeDef",
     {
         "Name": str,
     },
@@ -1860,15 +1749,15 @@
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
-        "MatchPredicates": List[PredicateOutputTypeDef],
+        "MatchPredicates": List[PredicateTypeDef],
         "RateKey": Literal["IP"],
         "RateLimit": int,
     },
 )
 _OptionalRateBasedRuleTypeDef = TypedDict(
     "_OptionalRateBasedRuleTypeDef",
     {
@@ -1881,15 +1770,15 @@
 class RateBasedRuleTypeDef(_RequiredRateBasedRuleTypeDef, _OptionalRateBasedRuleTypeDef):
     pass
 
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "RuleId": str,
-        "Predicates": List[PredicateOutputTypeDef],
+        "Predicates": List[PredicateTypeDef],
     },
 )
 _OptionalRuleTypeDef = TypedDict(
     "_OptionalRuleTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1913,37 +1802,28 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
-TagInfoForResourceTypeDef = TypedDict(
-    "TagInfoForResourceTypeDef",
-    {
-        "ResourceARN": str,
-        "TagList": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
         "ActivatedRules": List[ActivatedRuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
-        "DefaultAction": WafActionOutputTypeDef,
+        "DefaultAction": WafActionTypeDef,
         "Rules": List[ActivatedRuleOutputTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
@@ -1986,14 +1866,22 @@
     },
     total=False,
 )
 
 class ByteMatchSetTypeDef(_RequiredByteMatchSetTypeDef, _OptionalByteMatchSetTypeDef):
     pass
 
+ByteMatchSetUpdateTypeDef = TypedDict(
+    "ByteMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ByteMatchTuple": ByteMatchTupleTypeDef,
+    },
+)
+
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2011,29 +1899,44 @@
     "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    {
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+    },
+)
+
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
-        "RegexMatchTuples": List[RegexMatchTupleOutputTypeDef],
+        "RegexMatchTuples": List[RegexMatchTupleTypeDef],
     },
     total=False,
 )
 
+RegexMatchSetUpdateTypeDef = TypedDict(
+    "RegexMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "RegexMatchTuple": RegexMatchTupleTypeDef,
+    },
+)
+
 _RequiredSizeConstraintSetTypeDef = TypedDict(
     "_RequiredSizeConstraintSetTypeDef",
     {
         "SizeConstraintSetId": str,
-        "SizeConstraints": List[SizeConstraintOutputTypeDef],
+        "SizeConstraints": List[SizeConstraintTypeDef],
     },
 )
 _OptionalSizeConstraintSetTypeDef = TypedDict(
     "_OptionalSizeConstraintSetTypeDef",
     {
         "Name": str,
     },
@@ -2041,19 +1944,27 @@
 )
 
 class SizeConstraintSetTypeDef(
     _RequiredSizeConstraintSetTypeDef, _OptionalSizeConstraintSetTypeDef
 ):
     pass
 
+SizeConstraintSetUpdateTypeDef = TypedDict(
+    "SizeConstraintSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SizeConstraint": SizeConstraintTypeDef,
+    },
+)
+
 _RequiredSqlInjectionMatchSetTypeDef = TypedDict(
     "_RequiredSqlInjectionMatchSetTypeDef",
     {
         "SqlInjectionMatchSetId": str,
-        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleOutputTypeDef],
+        "SqlInjectionMatchTuples": List[SqlInjectionMatchTupleTypeDef],
     },
 )
 _OptionalSqlInjectionMatchSetTypeDef = TypedDict(
     "_OptionalSqlInjectionMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -2061,76 +1972,54 @@
 )
 
 class SqlInjectionMatchSetTypeDef(
     _RequiredSqlInjectionMatchSetTypeDef, _OptionalSqlInjectionMatchSetTypeDef
 ):
     pass
 
+SqlInjectionMatchSetUpdateTypeDef = TypedDict(
+    "SqlInjectionMatchSetUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
+    },
+)
+
 _RequiredXssMatchSetTypeDef = TypedDict(
     "_RequiredXssMatchSetTypeDef",
     {
         "XssMatchSetId": str,
-        "XssMatchTuples": List[XssMatchTupleOutputTypeDef],
+        "XssMatchTuples": List[XssMatchTupleTypeDef],
     },
 )
 _OptionalXssMatchSetTypeDef = TypedDict(
     "_OptionalXssMatchSetTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
 class XssMatchSetTypeDef(_RequiredXssMatchSetTypeDef, _OptionalXssMatchSetTypeDef):
     pass
 
-ByteMatchSetUpdateTypeDef = TypedDict(
-    "ByteMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ByteMatchTuple": ByteMatchTupleTypeDef,
-    },
-)
-
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
-    {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-    },
-)
-
-RegexMatchSetUpdateTypeDef = TypedDict(
-    "RegexMatchSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "RegexMatchTuple": RegexMatchTupleTypeDef,
-    },
-)
-
-SizeConstraintSetUpdateTypeDef = TypedDict(
-    "SizeConstraintSetUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "SizeConstraint": SizeConstraintTypeDef,
-    },
-)
-
-SqlInjectionMatchSetUpdateTypeDef = TypedDict(
-    "SqlInjectionMatchSetUpdateTypeDef",
+XssMatchSetUpdateTypeDef = TypedDict(
+    "XssMatchSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
-        "SqlInjectionMatchTuple": SqlInjectionMatchTupleTypeDef,
+        "XssMatchTuple": XssMatchTupleTypeDef,
     },
 )
 
-XssMatchSetUpdateTypeDef = TypedDict(
-    "XssMatchSetUpdateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Action": ChangeActionType,
-        "XssMatchTuple": XssMatchTupleTypeDef,
+        "NextMarker": str,
+        "TagInfoForResource": TagInfoForResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
@@ -2253,23 +2142,14 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "NextMarker": str,
-        "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2326,14 +2206,23 @@
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateByteMatchSetRequestRequestTypeDef",
+    {
+        "ByteMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
+    },
+)
+
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2343,14 +2232,23 @@
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateRegexMatchSetRequestRequestTypeDef",
+    {
+        "RegexMatchSetId": str,
+        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
+        "ChangeToken": str,
+    },
+)
+
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2360,14 +2258,23 @@
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
+    "UpdateSizeConstraintSetRequestRequestTypeDef",
+    {
+        "SizeConstraintSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
+    },
+)
+
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2377,14 +2284,23 @@
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
+    {
+        "SqlInjectionMatchSetId": str,
+        "ChangeToken": str,
+        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
+    },
+)
+
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2394,50 +2310,14 @@
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateByteMatchSetRequestRequestTypeDef",
-    {
-        "ByteMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[ByteMatchSetUpdateTypeDef],
-    },
-)
-
-UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateRegexMatchSetRequestRequestTypeDef",
-    {
-        "RegexMatchSetId": str,
-        "Updates": Sequence[RegexMatchSetUpdateTypeDef],
-        "ChangeToken": str,
-    },
-)
-
-UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
-    "UpdateSizeConstraintSetRequestRequestTypeDef",
-    {
-        "SizeConstraintSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SizeConstraintSetUpdateTypeDef],
-    },
-)
-
-UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
-    {
-        "SqlInjectionMatchSetId": str,
-        "ChangeToken": str,
-        "Updates": Sequence[SqlInjectionMatchSetUpdateTypeDef],
-    },
-)
-
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
         "Updates": Sequence[XssMatchSetUpdateTypeDef],
     },
```

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/PKG-INFO` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.12
-Summary: Type annotations for boto3.WAFRegional 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,23 +311,19 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
-    ExcludedRuleOutputTypeDef,
-    WafActionOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     ByteMatchSetSummaryTypeDef,
-    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
@@ -349,15 +345,14 @@
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
     DisassociateWebACLRequestRequestTypeDef,
-    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
@@ -373,15 +368,14 @@
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
-    IPSetDescriptorOutputTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
     ListIPSetsRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
@@ -401,29 +395,23 @@
     SqlInjectionMatchSetSummaryTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    TagOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     ActivatedRuleOutputTypeDef,
     ActivatedRuleTypeDef,
     ByteMatchTupleOutputTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    RegexMatchTupleOutputTypeDef,
-    SizeConstraintOutputTypeDef,
-    SqlInjectionMatchTupleOutputTypeDef,
-    XssMatchTupleOutputTypeDef,
     ByteMatchTupleTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     RegexMatchTupleTypeDef,
     SizeConstraintTypeDef,
     SqlInjectionMatchTupleTypeDef,
     XssMatchTupleTypeDef,
     CreateWebACLMigrationStackResponseTypeDef,
     DeleteByteMatchSetResponseTypeDef,
@@ -456,14 +444,15 @@
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
+    TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
@@ -484,71 +473,70 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
-    TagInfoForResourceTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
     WebACLTypeDef,
     RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
+    ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
-    RegexMatchSetTypeDef,
-    SizeConstraintSetTypeDef,
-    SqlInjectionMatchSetTypeDef,
-    XssMatchSetTypeDef,
-    ByteMatchSetUpdateTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
+    RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
+    SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
+    SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
+    XssMatchSetTypeDef,
     XssMatchSetUpdateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGeoMatchSetResponseTypeDef,
     GetGeoMatchSetResponseTypeDef,
     UpdateGeoMatchSetRequestRequestTypeDef,
     SampledHTTPRequestTypeDef,
     CreateIPSetResponseTypeDef,
     GetIPSetResponseTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
+    UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
+    UpdateRegexMatchSetRequestRequestTypeDef,
     CreateSizeConstraintSetResponseTypeDef,
     GetSizeConstraintSetResponseTypeDef,
+    UpdateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetResponseTypeDef,
     GetSqlInjectionMatchSetResponseTypeDef,
+    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
-    UpdateByteMatchSetRequestRequestTypeDef,
-    UpdateRegexMatchSetRequestRequestTypeDef,
-    UpdateSizeConstraintSetRequestRequestTypeDef,
-    UpdateSqlInjectionMatchSetRequestRequestTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleOutputTypeDef:
+def get_structure() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-regional-1.28.12/mypy_boto3_waf_regional.egg-info/SOURCES.txt` & `mypy-boto3-waf-regional-1.28.15/mypy_boto3_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.12/setup.py` & `mypy-boto3-waf-regional-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf-regional",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFRegional 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

