# Comparing `tmp/mypy-boto3-waf-1.28.12.tar.gz` & `tmp/mypy-boto3-waf-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-1.28.15.tar", last modified: Fri Jul 28 20:43:55 2023, max compression
```

## Comparing `mypy-boto3-waf-1.28.12.tar` & `mypy-boto3-waf-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24753 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/mypy_boto3_waf/
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49342 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-27 11:48:25.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-27 11:48:25.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-07-27 11:48:24.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63705 2023-07-27 11:48:26.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63652 2023-07-27 11:48:25.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24753 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:48.000000 mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.097488 mypy-boto3-waf-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:48:22.000000 mypy-boto3-waf-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.366023 mypy-boto3-waf-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-07-28 20:43:55.362023 mypy-boto3-waf-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22889 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.358023 mypy-boto3-waf-1.28.15/mypy_boto3_waf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49342 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-28 20:41:05.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-28 20:41:05.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60886 2023-07-28 20:41:07.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60835 2023-07-28 20:41:06.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.362023 mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-07-28 20:43:55.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:55.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:55.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:55.000000 mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:55.366023 mypy-boto3-waf-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:41:04.000000 mypy-boto3-waf-1.28.15/setup.py
```

### Comparing `mypy-boto3-waf-1.28.12/LICENSE` & `mypy-boto3-waf-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/PKG-INFO` & `mypy-boto3-waf-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf
-Version: 1.28.12
-Summary: Type annotations for boto3.WAF 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WAF 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,22 +401,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
-    ExcludedRuleOutputTypeDef,
-    WafActionOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     ByteMatchSetSummaryTypeDef,
-    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
@@ -437,15 +433,14 @@
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
@@ -460,15 +455,14 @@
     TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
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
@@ -488,29 +482,23 @@
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
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
@@ -542,14 +530,15 @@
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
@@ -585,71 +574,70 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
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

### Comparing `mypy-boto3-waf-1.28.12/README.md` & `mypy-boto3-waf-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,22 +369,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
-    ExcludedRuleOutputTypeDef,
-    WafActionOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     ByteMatchSetSummaryTypeDef,
-    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
@@ -405,15 +401,14 @@
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
@@ -428,15 +423,14 @@
     TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
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
@@ -456,29 +450,23 @@
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
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
@@ -510,14 +498,15 @@
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
@@ -553,71 +542,70 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
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

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.py` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/__init__.pyi` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/__main__.py` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAF 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.WAF 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF\nOther"
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

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.py` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/client.pyi` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.py` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/literals.pyi` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.py` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/paginator.pyi` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.py` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for waf service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf.type_defs import ExcludedRuleOutputTypeDef
+    from mypy_boto3_waf.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleOutputTypeDef = {...}
+    data: ExcludedRuleTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -39,22 +39,18 @@
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
     "ByteMatchSetSummaryTypeDef",
-    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
@@ -75,15 +71,14 @@
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
-    "GeoMatchConstraintOutputTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
@@ -98,15 +93,14 @@
     "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
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
@@ -126,29 +120,23 @@
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
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
@@ -180,14 +168,15 @@
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
@@ -223,90 +212,68 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
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
 
@@ -328,35 +295,14 @@
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
@@ -610,22 +556,14 @@
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
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
@@ -796,22 +734,14 @@
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
@@ -1052,23 +982,14 @@
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
@@ -1086,22 +1007,14 @@
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
@@ -1112,18 +1025,18 @@
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
@@ -1153,88 +1066,53 @@
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
@@ -1622,14 +1500,23 @@
 
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
@@ -1668,15 +1555,15 @@
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
@@ -1871,15 +1758,15 @@
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
@@ -1998,15 +1885,15 @@
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
@@ -2021,15 +1908,15 @@
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
@@ -2055,37 +1942,28 @@
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
@@ -2132,14 +2010,22 @@
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
@@ -2157,29 +2043,44 @@
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
@@ -2189,19 +2090,27 @@
 
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
@@ -2211,19 +2120,27 @@
 
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
@@ -2231,58 +2148,28 @@
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
@@ -2407,23 +2294,14 @@
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
@@ -2482,14 +2360,23 @@
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
@@ -2499,14 +2386,23 @@
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
@@ -2516,14 +2412,23 @@
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
@@ -2533,14 +2438,23 @@
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
@@ -2550,50 +2464,14 @@
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

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf/type_defs.pyi` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for waf service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_waf.type_defs import ExcludedRuleOutputTypeDef
+    from mypy_boto3_waf.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleOutputTypeDef = {...}
+    data: ExcludedRuleTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -38,22 +38,18 @@
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
     "ByteMatchSetSummaryTypeDef",
-    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
@@ -74,15 +70,14 @@
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
-    "GeoMatchConstraintOutputTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
@@ -97,15 +92,14 @@
     "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
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
@@ -125,29 +119,23 @@
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
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
@@ -179,14 +167,15 @@
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
@@ -222,90 +211,68 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
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
 
@@ -327,33 +294,14 @@
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
@@ -601,22 +549,14 @@
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
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
@@ -785,22 +725,14 @@
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
@@ -1039,23 +971,14 @@
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
@@ -1073,22 +996,14 @@
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
@@ -1099,18 +1014,18 @@
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
@@ -1136,86 +1051,51 @@
 
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
@@ -1593,14 +1473,23 @@
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
@@ -1639,15 +1528,15 @@
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
@@ -1838,15 +1727,15 @@
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
@@ -1963,15 +1852,15 @@
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
@@ -1984,15 +1873,15 @@
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
@@ -2016,37 +1905,28 @@
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
@@ -2089,14 +1969,22 @@
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
@@ -2114,29 +2002,44 @@
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
@@ -2144,19 +2047,27 @@
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
@@ -2164,76 +2075,54 @@
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
@@ -2356,23 +2245,14 @@
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
@@ -2429,14 +2309,23 @@
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
@@ -2446,14 +2335,23 @@
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
@@ -2463,14 +2361,23 @@
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
@@ -2480,14 +2387,23 @@
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
@@ -2497,50 +2413,14 @@
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

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/PKG-INFO` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf
-Version: 1.28.12
-Summary: Type annotations for boto3.WAF 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WAF 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
 See how it helps to find and fix potential bugs:
 
@@ -401,22 +401,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
-    ExcludedRuleOutputTypeDef,
-    WafActionOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     ByteMatchSetSummaryTypeDef,
-    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
@@ -437,15 +433,14 @@
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    GeoMatchConstraintOutputTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
@@ -460,15 +455,14 @@
     TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
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
@@ -488,29 +482,23 @@
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
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
@@ -542,14 +530,15 @@
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
@@ -585,71 +574,70 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
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

### Comparing `mypy-boto3-waf-1.28.12/mypy_boto3_waf.egg-info/SOURCES.txt` & `mypy-boto3-waf-1.28.15/mypy_boto3_waf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.12/setup.py` & `mypy-boto3-waf-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_waf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAF 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.WAF 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

