# Comparing `tmp/mypy-boto3-elbv2-1.28.12.tar.gz` & `tmp/mypy-boto3-elbv2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elbv2-1.28.12.tar", last modified: Thu Jul 27 05:34:39 2023, max compression
+gzip compressed data, was "mypy-boto3-elbv2-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
```

## Comparing `mypy-boto3-elbv2-1.28.12.tar` & `mypy-boto3-elbv2-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20734 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19238 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33888 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33835 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47068 2023-07-27 05:21:56.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-07-27 05:21:56.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20734 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:39.000000 mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:39.964516 mypy-boto3-elbv2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-27 05:21:55.000000 mypy-boto3-elbv2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.453078 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33888 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33835 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-28 20:25:22.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43450 2023-07-28 20:25:23.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43403 2023-07-28 20:25:22.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:42:46.000000 mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.469078 mypy-boto3-elbv2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-28 20:25:21.000000 mypy-boto3-elbv2-1.28.15/setup.py
```

### Comparing `mypy-boto3-elbv2-1.28.12/LICENSE` & `mypy-boto3-elbv2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/PKG-INFO` & `mypy-boto3-elbv2-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,129 +406,118 @@
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigOutputTypeDef,
     AuthenticateOidcActionConfigOutputTypeDef,
-    FixedResponseActionConfigOutputTypeDef,
-    RedirectActionConfigOutputTypeDef,
-    AuthenticateCognitoActionConfigTypeDef,
-    AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
+    AuthenticateCognitoActionConfigTypeDef,
+    AuthenticateOidcActionConfigTypeDef,
     CertificateTypeDef,
-    CertificateOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
-    LoadBalancerAttributeOutputTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    LoadBalancerAttributeTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
-    TargetGroupAttributeOutputTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
+    TargetGroupAttributeTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
-    TargetGroupStickinessConfigOutputTypeDef,
-    TargetGroupTupleOutputTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
     HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
     HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
     HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
-    LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
-    MatcherOutputTypeDef,
-    TargetGroupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
-    QueryStringKeyValuePairOutputTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
-    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
-    SetSecurityGroupsOutputTypeDef,
-    TagOutputTypeDef,
-    TargetDescriptionOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
     RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
+    SetIpAddressTypeOutputTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
+    TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
+    ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
-    TargetGroupTypeDef,
-    ModifyTargetGroupAttributesInputRequestTypeDef,
     QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
-    TagDescriptionTypeDef,
     TargetHealthDescriptionTypeDef,
+    DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
-    ActionOutputTypeDef,
-    ActionTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    ActionOutputTypeDef,
+    ActionTypeDef,
     RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
     ListenerTypeDef,
     CreateListenerInputRequestTypeDef,
     ModifyListenerInputRequestTypeDef,
     RuleTypeDef,
```

### Comparing `mypy-boto3-elbv2-1.28.12/README.md` & `mypy-boto3-elbv2-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,129 +374,118 @@
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigOutputTypeDef,
     AuthenticateOidcActionConfigOutputTypeDef,
-    FixedResponseActionConfigOutputTypeDef,
-    RedirectActionConfigOutputTypeDef,
-    AuthenticateCognitoActionConfigTypeDef,
-    AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
+    AuthenticateCognitoActionConfigTypeDef,
+    AuthenticateOidcActionConfigTypeDef,
     CertificateTypeDef,
-    CertificateOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
-    LoadBalancerAttributeOutputTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    LoadBalancerAttributeTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
-    TargetGroupAttributeOutputTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
+    TargetGroupAttributeTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
-    TargetGroupStickinessConfigOutputTypeDef,
-    TargetGroupTupleOutputTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
     HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
     HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
     HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
-    LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
-    MatcherOutputTypeDef,
-    TargetGroupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
-    QueryStringKeyValuePairOutputTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
-    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
-    SetSecurityGroupsOutputTypeDef,
-    TagOutputTypeDef,
-    TargetDescriptionOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
     RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
+    SetIpAddressTypeOutputTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
+    TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
+    ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
-    TargetGroupTypeDef,
-    ModifyTargetGroupAttributesInputRequestTypeDef,
     QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
-    TagDescriptionTypeDef,
     TargetHealthDescriptionTypeDef,
+    DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
-    ActionOutputTypeDef,
-    ActionTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    ActionOutputTypeDef,
+    ActionTypeDef,
     RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
     ListenerTypeDef,
     CreateListenerInputRequestTypeDef,
     ModifyListenerInputRequestTypeDef,
     RuleTypeDef,
```

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.py` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__init__.pyi` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/__main__.py` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.py` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/client.pyi` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.py` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/literals.pyi` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.py` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,30 +71,30 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
         """
 
 
 class DescribeListenerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeListenerCertificatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
         """
 
 
@@ -105,15 +105,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeListenersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenerspaginator)
         """
 
 
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
 
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describerulespaginator)
         """
 
 
@@ -162,15 +162,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describesslpoliciespaginator)
         """
 
 
@@ -182,13 +182,13 @@
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/paginator.pyi` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -68,29 +68,29 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeListenerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeListenerCertificatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
         """
 
 class DescribeListenersPaginator(Paginator):
@@ -100,15 +100,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeListenersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenerspaginator)
         """
 
 class DescribeLoadBalancersPaginator(Paginator):
@@ -118,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
 class DescribeRulesPaginator(Paginator):
@@ -136,15 +136,15 @@
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describerulespaginator)
         """
 
 class DescribeSSLPoliciesPaginator(Paginator):
@@ -154,15 +154,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describesslpoliciespaginator)
         """
 
 class DescribeTargetGroupsPaginator(Paginator):
@@ -173,13 +173,13 @@
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.py` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,129 +36,118 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AuthenticateCognitoActionConfigOutputTypeDef",
     "AuthenticateOidcActionConfigOutputTypeDef",
-    "FixedResponseActionConfigOutputTypeDef",
-    "RedirectActionConfigOutputTypeDef",
-    "AuthenticateCognitoActionConfigTypeDef",
-    "AuthenticateOidcActionConfigTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
+    "AuthenticateCognitoActionConfigTypeDef",
+    "AuthenticateOidcActionConfigTypeDef",
     "CertificateTypeDef",
-    "CertificateOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
     "DeleteRuleInputRequestTypeDef",
     "DeleteTargetGroupInputRequestTypeDef",
     "TargetDescriptionTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
-    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
-    "LoadBalancerAttributeOutputTypeDef",
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    "LoadBalancerAttributeTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
-    "TargetGroupAttributeOutputTypeDef",
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    "TargetGroupAttributeTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
-    "TargetGroupStickinessConfigOutputTypeDef",
-    "TargetGroupTupleOutputTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
     "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
     "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
     "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
-    "LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
-    "MatcherOutputTypeDef",
-    "TargetGroupAttributeTypeDef",
-    "PaginatorConfigTypeDef",
     "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
-    "QueryStringKeyValuePairOutputTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
-    "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
-    "SetSecurityGroupsOutputTypeDef",
-    "TagOutputTypeDef",
-    "TargetDescriptionOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
     "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
+    "SetIpAddressTypeOutputTypeDef",
+    "SetSecurityGroupsOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
+    "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
     "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
-    "TargetGroupTypeDef",
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
     "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
-    "TagDescriptionTypeDef",
     "TargetHealthDescriptionTypeDef",
+    "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
-    "ActionOutputTypeDef",
-    "ActionTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
+    "ActionOutputTypeDef",
+    "ActionTypeDef",
     "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
-    "DescribeTagsOutputTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
     "ListenerTypeDef",
     "CreateListenerInputRequestTypeDef",
     "ModifyListenerInputRequestTypeDef",
     "RuleTypeDef",
@@ -229,57 +218,57 @@
 class AuthenticateOidcActionConfigOutputTypeDef(
     _RequiredAuthenticateOidcActionConfigOutputTypeDef,
     _OptionalAuthenticateOidcActionConfigOutputTypeDef,
 ):
     pass
 
 
-_RequiredFixedResponseActionConfigOutputTypeDef = TypedDict(
-    "_RequiredFixedResponseActionConfigOutputTypeDef",
+_RequiredFixedResponseActionConfigTypeDef = TypedDict(
+    "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
     },
 )
-_OptionalFixedResponseActionConfigOutputTypeDef = TypedDict(
-    "_OptionalFixedResponseActionConfigOutputTypeDef",
+_OptionalFixedResponseActionConfigTypeDef = TypedDict(
+    "_OptionalFixedResponseActionConfigTypeDef",
     {
         "MessageBody": str,
         "ContentType": str,
     },
     total=False,
 )
 
 
-class FixedResponseActionConfigOutputTypeDef(
-    _RequiredFixedResponseActionConfigOutputTypeDef, _OptionalFixedResponseActionConfigOutputTypeDef
+class FixedResponseActionConfigTypeDef(
+    _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
 ):
     pass
 
 
-_RequiredRedirectActionConfigOutputTypeDef = TypedDict(
-    "_RequiredRedirectActionConfigOutputTypeDef",
+_RequiredRedirectActionConfigTypeDef = TypedDict(
+    "_RequiredRedirectActionConfigTypeDef",
     {
         "StatusCode": RedirectActionStatusCodeEnumType,
     },
 )
-_OptionalRedirectActionConfigOutputTypeDef = TypedDict(
-    "_OptionalRedirectActionConfigOutputTypeDef",
+_OptionalRedirectActionConfigTypeDef = TypedDict(
+    "_OptionalRedirectActionConfigTypeDef",
     {
         "Protocol": str,
         "Port": str,
         "Host": str,
         "Path": str,
         "Query": str,
     },
     total=False,
 )
 
 
-class RedirectActionConfigOutputTypeDef(
-    _RequiredRedirectActionConfigOutputTypeDef, _OptionalRedirectActionConfigOutputTypeDef
+class RedirectActionConfigTypeDef(
+    _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
 
 _RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateCognitoActionConfigTypeDef",
     {
@@ -334,77 +323,32 @@
 
 class AuthenticateOidcActionConfigTypeDef(
     _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
 
-_RequiredFixedResponseActionConfigTypeDef = TypedDict(
-    "_RequiredFixedResponseActionConfigTypeDef",
-    {
-        "StatusCode": str,
-    },
-)
-_OptionalFixedResponseActionConfigTypeDef = TypedDict(
-    "_OptionalFixedResponseActionConfigTypeDef",
-    {
-        "MessageBody": str,
-        "ContentType": str,
-    },
-    total=False,
-)
-
-
-class FixedResponseActionConfigTypeDef(
-    _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
-):
-    pass
-
-
-_RequiredRedirectActionConfigTypeDef = TypedDict(
-    "_RequiredRedirectActionConfigTypeDef",
-    {
-        "StatusCode": RedirectActionStatusCodeEnumType,
-    },
-)
-_OptionalRedirectActionConfigTypeDef = TypedDict(
-    "_OptionalRedirectActionConfigTypeDef",
-    {
-        "Protocol": str,
-        "Port": str,
-        "Host": str,
-        "Path": str,
-        "Query": str,
-    },
-    total=False,
-)
-
-
-class RedirectActionConfigTypeDef(
-    _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
-):
-    pass
-
-
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
 )
 
-CertificateOutputTypeDef = TypedDict(
-    "CertificateOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CertificateArn": str,
-        "IsDefault": bool,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -508,18 +452,20 @@
 
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -534,36 +480,14 @@
     {
         "Name": str,
         "Max": str,
     },
     total=False,
 )
 
-_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
-    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -579,24 +503,14 @@
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
 
-DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "ListenerArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeListenersInputRequestTypeDef = TypedDict(
     "DescribeListenersInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
@@ -607,33 +521,23 @@
 DescribeLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 
-LoadBalancerAttributeOutputTypeDef = TypedDict(
-    "LoadBalancerAttributeOutputTypeDef",
+LoadBalancerAttributeTypeDef = TypedDict(
+    "LoadBalancerAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -646,45 +550,25 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-        "RuleArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRulesInputRequestTypeDef = TypedDict(
     "DescribeRulesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "RuleArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "LoadBalancerType": LoadBalancerTypeEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSSLPoliciesInputRequestTypeDef = TypedDict(
     "DescribeSSLPoliciesInputRequestTypeDef",
     {
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
         "LoadBalancerType": LoadBalancerTypeEnumType,
@@ -702,64 +586,35 @@
 DescribeTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 
-TargetGroupAttributeOutputTypeDef = TypedDict(
-    "TargetGroupAttributeOutputTypeDef",
+TargetGroupAttributeTypeDef = TypedDict(
+    "TargetGroupAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "TargetGroupArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTargetGroupsInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "TargetGroupArns": Sequence[str],
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-TargetGroupStickinessConfigOutputTypeDef = TypedDict(
-    "TargetGroupStickinessConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-        "DurationSeconds": int,
-    },
-    total=False,
-)
-
-TargetGroupTupleOutputTypeDef = TypedDict(
-    "TargetGroupTupleOutputTypeDef",
-    {
-        "TargetGroupArn": str,
-        "Weight": int,
-    },
-    total=False,
-)
-
 TargetGroupStickinessConfigTypeDef = TypedDict(
     "TargetGroupStickinessConfigTypeDef",
     {
         "Enabled": bool,
         "DurationSeconds": int,
     },
     total=False,
@@ -820,60 +675,23 @@
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-LoadBalancerAttributeTypeDef = TypedDict(
-    "LoadBalancerAttributeTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
-MatcherOutputTypeDef = TypedDict(
-    "MatcherOutputTypeDef",
-    {
-        "HttpCode": str,
-        "GrpcCode": str,
-    },
-    total=False,
-)
-
-TargetGroupAttributeTypeDef = TypedDict(
-    "TargetGroupAttributeTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
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
 PathPatternConditionConfigOutputTypeDef = TypedDict(
     "PathPatternConditionConfigOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
@@ -882,23 +700,14 @@
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-QueryStringKeyValuePairOutputTypeDef = TypedDict(
-    "QueryStringKeyValuePairOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 QueryStringKeyValuePairTypeDef = TypedDict(
     "QueryStringKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -908,25 +717,14 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
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
 SourceIpConditionConfigOutputTypeDef = TypedDict(
     "SourceIpConditionConfigOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
@@ -952,79 +750,22 @@
     "SetIpAddressTypeInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "IpAddressType": IpAddressTypeType,
     },
 )
 
-SetIpAddressTypeOutputTypeDef = TypedDict(
-    "SetIpAddressTypeOutputTypeDef",
-    {
-        "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSecurityGroupsInputRequestTypeDef = TypedDict(
     "SetSecurityGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-SetSecurityGroupsOutputTypeDef = TypedDict(
-    "SetSecurityGroupsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
-_RequiredTargetDescriptionOutputTypeDef = TypedDict(
-    "_RequiredTargetDescriptionOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalTargetDescriptionOutputTypeDef = TypedDict(
-    "_OptionalTargetDescriptionOutputTypeDef",
-    {
-        "Port": int,
-        "AvailabilityZone": str,
-    },
-    total=False,
-)
-
-
-class TargetDescriptionOutputTypeDef(
-    _RequiredTargetDescriptionOutputTypeDef, _OptionalTargetDescriptionOutputTypeDef
-):
-    pass
-
-
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -1046,36 +787,61 @@
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Certificates": List[CertificateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateOutputTypeDef],
+        "Certificates": List[CertificateTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetIpAddressTypeOutputTypeDef = TypedDict(
+    "SetIpAddressTypeOutputTypeDef",
+    {
+        "IpAddressType": IpAddressTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetSecurityGroupsOutputTypeDef = TypedDict(
+    "SetSecurityGroupsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
         "OutpostId": str,
         "LoadBalancerAddresses": List[LoadBalancerAddressTypeDef],
@@ -1206,14 +972,39 @@
 
 class ModifyTargetGroupInputRequestTypeDef(
     _RequiredModifyTargetGroupInputRequestTypeDef, _OptionalModifyTargetGroupInputRequestTypeDef
 ):
     pass
 
 
+TargetGroupTypeDef = TypedDict(
+    "TargetGroupTypeDef",
+    {
+        "TargetGroupArn": str,
+        "TargetGroupName": str,
+        "Protocol": ProtocolEnumType,
+        "Port": int,
+        "VpcId": str,
+        "HealthCheckProtocol": ProtocolEnumType,
+        "HealthCheckPort": str,
+        "HealthCheckEnabled": bool,
+        "HealthCheckIntervalSeconds": int,
+        "HealthCheckTimeoutSeconds": int,
+        "HealthyThresholdCount": int,
+        "UnhealthyThresholdCount": int,
+        "HealthCheckPath": str,
+        "Matcher": MatcherTypeDef,
+        "LoadBalancerArns": List[str],
+        "TargetType": TargetTypeEnumType,
+        "ProtocolVersion": str,
+        "IpAddressType": TargetGroupIpAddressTypeEnumType,
+    },
+    total=False,
+)
+
 DeregisterTargetsInputRequestTypeDef = TypedDict(
     "DeregisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
@@ -1244,36 +1035,125 @@
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
+    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+):
+    pass
+
+
+DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "ListenerArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+        "RuleArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "LoadBalancerType": LoadBalancerTypeEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "TargetGroupArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
         "LoadBalancerArns": Sequence[str],
@@ -1354,90 +1234,57 @@
 ):
     pass
 
 
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[TargetGroupAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
+    {
+        "TargetGroupArn": str,
+        "Attributes": Sequence[TargetGroupAttributeTypeDef],
     },
 )
 
 ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[TargetGroupAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ForwardActionConfigOutputTypeDef = TypedDict(
     "ForwardActionConfigOutputTypeDef",
     {
-        "TargetGroups": List[TargetGroupTupleOutputTypeDef],
-        "TargetGroupStickinessConfig": TargetGroupStickinessConfigOutputTypeDef,
+        "TargetGroups": List[TargetGroupTupleTypeDef],
+        "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
-    },
-)
-
-TargetGroupTypeDef = TypedDict(
-    "TargetGroupTypeDef",
-    {
-        "TargetGroupArn": str,
-        "TargetGroupName": str,
-        "Protocol": ProtocolEnumType,
-        "Port": int,
-        "VpcId": str,
-        "HealthCheckProtocol": ProtocolEnumType,
-        "HealthCheckPort": str,
-        "HealthCheckEnabled": bool,
-        "HealthCheckIntervalSeconds": int,
-        "HealthCheckTimeoutSeconds": int,
-        "HealthyThresholdCount": int,
-        "UnhealthyThresholdCount": int,
-        "HealthCheckPath": str,
-        "Matcher": MatcherOutputTypeDef,
-        "LoadBalancerArns": List[str],
-        "TargetType": TargetTypeEnumType,
-        "ProtocolVersion": str,
-        "IpAddressType": TargetGroupIpAddressTypeEnumType,
-    },
-    total=False,
-)
-
-ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
-    {
-        "TargetGroupArn": str,
-        "Attributes": Sequence[TargetGroupAttributeTypeDef],
-    },
-)
-
 QueryStringConditionConfigOutputTypeDef = TypedDict(
     "QueryStringConditionConfigOutputTypeDef",
     {
-        "Values": List[QueryStringKeyValuePairOutputTypeDef],
+        "Values": List[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
 
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
@@ -1449,33 +1296,32 @@
 SetRulePrioritiesInputRequestTypeDef = TypedDict(
     "SetRulePrioritiesInputRequestTypeDef",
     {
         "RulePriorities": Sequence[RulePriorityPairTypeDef],
     },
 )
 
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 TargetHealthDescriptionTypeDef = TypedDict(
     "TargetHealthDescriptionTypeDef",
     {
-        "Target": TargetDescriptionOutputTypeDef,
+        "Target": TargetDescriptionTypeDef,
         "HealthCheckPort": str,
         "TargetHealth": TargetHealthTypeDef,
     },
     total=False,
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
         "DNSName": str,
         "CanonicalHostedZoneId": str,
         "CreatedTime": datetime,
@@ -1493,24 +1339,49 @@
 )
 
 SetSubnetsOutputTypeDef = TypedDict(
     "SetSubnetsOutputTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSSLPoliciesOutputTypeDef = TypedDict(
     "DescribeSSLPoliciesOutputTypeDef",
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTargetGroupOutputTypeDef = TypedDict(
+    "CreateTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTargetGroupsOutputTypeDef = TypedDict(
+    "DescribeTargetGroupsOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyTargetGroupOutputTypeDef = TypedDict(
+    "ModifyTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActionOutputTypeDef = TypedDict(
     "_RequiredActionOutputTypeDef",
     {
         "Type": ActionTypeEnumType,
@@ -1519,16 +1390,16 @@
 _OptionalActionOutputTypeDef = TypedDict(
     "_OptionalActionOutputTypeDef",
     {
         "TargetGroupArn": str,
         "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
         "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
         "Order": int,
-        "RedirectConfig": RedirectActionConfigOutputTypeDef,
-        "FixedResponseConfig": FixedResponseActionConfigOutputTypeDef,
+        "RedirectConfig": RedirectActionConfigTypeDef,
+        "FixedResponseConfig": FixedResponseActionConfigTypeDef,
         "ForwardConfig": ForwardActionConfigOutputTypeDef,
     },
     total=False,
 )
 
 
 class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
@@ -1556,39 +1427,14 @@
 )
 
 
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
 
-CreateTargetGroupOutputTypeDef = TypedDict(
-    "CreateTargetGroupOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeTargetGroupsOutputTypeDef = TypedDict(
-    "DescribeTargetGroupsOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModifyTargetGroupOutputTypeDef = TypedDict(
-    "ModifyTargetGroupOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RuleConditionOutputTypeDef = TypedDict(
     "RuleConditionOutputTypeDef",
     {
         "Field": str,
         "Values": List[str],
         "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
         "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
@@ -1611,55 +1457,47 @@
         "QueryStringConfig": QueryStringConditionConfigTypeDef,
         "HttpRequestMethodConfig": HttpRequestMethodConditionConfigTypeDef,
         "SourceIpConfig": SourceIpConditionConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
-    {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerOutputTypeDef = TypedDict(
     "CreateLoadBalancerOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersOutputTypeDef = TypedDict(
     "DescribeLoadBalancersOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListenerTypeDef = TypedDict(
     "ListenerTypeDef",
     {
         "ListenerArn": str,
         "LoadBalancerArn": str,
         "Port": int,
         "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateOutputTypeDef],
+        "Certificates": List[CertificateTypeDef],
         "SslPolicy": str,
         "DefaultActions": List[ActionOutputTypeDef],
         "AlpnPolicy": List[str],
     },
     total=False,
 )
 
@@ -1774,60 +1612,60 @@
     pass
 
 
 CreateListenerOutputTypeDef = TypedDict(
     "CreateListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenersOutputTypeDef = TypedDict(
     "DescribeListenersOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyListenerOutputTypeDef = TypedDict(
     "ModifyListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleOutputTypeDef = TypedDict(
     "CreateRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRulesOutputTypeDef = TypedDict(
     "DescribeRulesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRuleOutputTypeDef = TypedDict(
     "ModifyRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetRulePrioritiesOutputTypeDef = TypedDict(
     "SetRulePrioritiesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/type_defs.pyi` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -35,129 +35,118 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AuthenticateCognitoActionConfigOutputTypeDef",
     "AuthenticateOidcActionConfigOutputTypeDef",
-    "FixedResponseActionConfigOutputTypeDef",
-    "RedirectActionConfigOutputTypeDef",
-    "AuthenticateCognitoActionConfigTypeDef",
-    "AuthenticateOidcActionConfigTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
+    "AuthenticateCognitoActionConfigTypeDef",
+    "AuthenticateOidcActionConfigTypeDef",
     "CertificateTypeDef",
-    "CertificateOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
     "DeleteRuleInputRequestTypeDef",
     "DeleteTargetGroupInputRequestTypeDef",
     "TargetDescriptionTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
-    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
-    "LoadBalancerAttributeOutputTypeDef",
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    "LoadBalancerAttributeTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
-    "TargetGroupAttributeOutputTypeDef",
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    "TargetGroupAttributeTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
-    "TargetGroupStickinessConfigOutputTypeDef",
-    "TargetGroupTupleOutputTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
     "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
     "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
     "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
-    "LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
-    "MatcherOutputTypeDef",
-    "TargetGroupAttributeTypeDef",
-    "PaginatorConfigTypeDef",
     "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
-    "QueryStringKeyValuePairOutputTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
-    "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
-    "SetSecurityGroupsOutputTypeDef",
-    "TagOutputTypeDef",
-    "TargetDescriptionOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
     "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
+    "SetIpAddressTypeOutputTypeDef",
+    "SetSecurityGroupsOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
+    "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
     "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
-    "TargetGroupTypeDef",
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
     "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
-    "TagDescriptionTypeDef",
     "TargetHealthDescriptionTypeDef",
+    "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
-    "ActionOutputTypeDef",
-    "ActionTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
+    "ActionOutputTypeDef",
+    "ActionTypeDef",
     "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
-    "DescribeTagsOutputTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
     "ListenerTypeDef",
     "CreateListenerInputRequestTypeDef",
     "ModifyListenerInputRequestTypeDef",
     "RuleTypeDef",
@@ -224,54 +213,54 @@
 
 class AuthenticateOidcActionConfigOutputTypeDef(
     _RequiredAuthenticateOidcActionConfigOutputTypeDef,
     _OptionalAuthenticateOidcActionConfigOutputTypeDef,
 ):
     pass
 
-_RequiredFixedResponseActionConfigOutputTypeDef = TypedDict(
-    "_RequiredFixedResponseActionConfigOutputTypeDef",
+_RequiredFixedResponseActionConfigTypeDef = TypedDict(
+    "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
     },
 )
-_OptionalFixedResponseActionConfigOutputTypeDef = TypedDict(
-    "_OptionalFixedResponseActionConfigOutputTypeDef",
+_OptionalFixedResponseActionConfigTypeDef = TypedDict(
+    "_OptionalFixedResponseActionConfigTypeDef",
     {
         "MessageBody": str,
         "ContentType": str,
     },
     total=False,
 )
 
-class FixedResponseActionConfigOutputTypeDef(
-    _RequiredFixedResponseActionConfigOutputTypeDef, _OptionalFixedResponseActionConfigOutputTypeDef
+class FixedResponseActionConfigTypeDef(
+    _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
 ):
     pass
 
-_RequiredRedirectActionConfigOutputTypeDef = TypedDict(
-    "_RequiredRedirectActionConfigOutputTypeDef",
+_RequiredRedirectActionConfigTypeDef = TypedDict(
+    "_RequiredRedirectActionConfigTypeDef",
     {
         "StatusCode": RedirectActionStatusCodeEnumType,
     },
 )
-_OptionalRedirectActionConfigOutputTypeDef = TypedDict(
-    "_OptionalRedirectActionConfigOutputTypeDef",
+_OptionalRedirectActionConfigTypeDef = TypedDict(
+    "_OptionalRedirectActionConfigTypeDef",
     {
         "Protocol": str,
         "Port": str,
         "Host": str,
         "Path": str,
         "Query": str,
     },
     total=False,
 )
 
-class RedirectActionConfigOutputTypeDef(
-    _RequiredRedirectActionConfigOutputTypeDef, _OptionalRedirectActionConfigOutputTypeDef
+class RedirectActionConfigTypeDef(
+    _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
 _RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateCognitoActionConfigTypeDef",
     {
         "UserPoolArn": str,
@@ -321,73 +310,32 @@
 )
 
 class AuthenticateOidcActionConfigTypeDef(
     _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
-_RequiredFixedResponseActionConfigTypeDef = TypedDict(
-    "_RequiredFixedResponseActionConfigTypeDef",
-    {
-        "StatusCode": str,
-    },
-)
-_OptionalFixedResponseActionConfigTypeDef = TypedDict(
-    "_OptionalFixedResponseActionConfigTypeDef",
-    {
-        "MessageBody": str,
-        "ContentType": str,
-    },
-    total=False,
-)
-
-class FixedResponseActionConfigTypeDef(
-    _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
-):
-    pass
-
-_RequiredRedirectActionConfigTypeDef = TypedDict(
-    "_RequiredRedirectActionConfigTypeDef",
-    {
-        "StatusCode": RedirectActionStatusCodeEnumType,
-    },
-)
-_OptionalRedirectActionConfigTypeDef = TypedDict(
-    "_OptionalRedirectActionConfigTypeDef",
-    {
-        "Protocol": str,
-        "Port": str,
-        "Host": str,
-        "Path": str,
-        "Query": str,
-    },
-    total=False,
-)
-
-class RedirectActionConfigTypeDef(
-    _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
-):
-    pass
-
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
 )
 
-CertificateOutputTypeDef = TypedDict(
-    "CertificateOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CertificateArn": str,
-        "IsDefault": bool,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -487,18 +435,20 @@
 )
 
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -513,34 +463,14 @@
     {
         "Name": str,
         "Max": str,
     },
     total=False,
 )
 
-_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
-    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -554,24 +484,14 @@
 
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
-DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "ListenerArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeListenersInputRequestTypeDef = TypedDict(
     "DescribeListenersInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
@@ -582,33 +502,23 @@
 DescribeLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 
-LoadBalancerAttributeOutputTypeDef = TypedDict(
-    "LoadBalancerAttributeOutputTypeDef",
+LoadBalancerAttributeTypeDef = TypedDict(
+    "LoadBalancerAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -621,45 +531,25 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-        "RuleArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRulesInputRequestTypeDef = TypedDict(
     "DescribeRulesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "RuleArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "LoadBalancerType": LoadBalancerTypeEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSSLPoliciesInputRequestTypeDef = TypedDict(
     "DescribeSSLPoliciesInputRequestTypeDef",
     {
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
         "LoadBalancerType": LoadBalancerTypeEnumType,
@@ -677,64 +567,35 @@
 DescribeTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 
-TargetGroupAttributeOutputTypeDef = TypedDict(
-    "TargetGroupAttributeOutputTypeDef",
+TargetGroupAttributeTypeDef = TypedDict(
+    "TargetGroupAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "TargetGroupArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTargetGroupsInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "TargetGroupArns": Sequence[str],
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-TargetGroupStickinessConfigOutputTypeDef = TypedDict(
-    "TargetGroupStickinessConfigOutputTypeDef",
-    {
-        "Enabled": bool,
-        "DurationSeconds": int,
-    },
-    total=False,
-)
-
-TargetGroupTupleOutputTypeDef = TypedDict(
-    "TargetGroupTupleOutputTypeDef",
-    {
-        "TargetGroupArn": str,
-        "Weight": int,
-    },
-    total=False,
-)
-
 TargetGroupStickinessConfigTypeDef = TypedDict(
     "TargetGroupStickinessConfigTypeDef",
     {
         "Enabled": bool,
         "DurationSeconds": int,
     },
     total=False,
@@ -795,60 +656,23 @@
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-LoadBalancerAttributeTypeDef = TypedDict(
-    "LoadBalancerAttributeTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
-MatcherOutputTypeDef = TypedDict(
-    "MatcherOutputTypeDef",
-    {
-        "HttpCode": str,
-        "GrpcCode": str,
-    },
-    total=False,
-)
-
-TargetGroupAttributeTypeDef = TypedDict(
-    "TargetGroupAttributeTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
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
 PathPatternConditionConfigOutputTypeDef = TypedDict(
     "PathPatternConditionConfigOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
@@ -857,23 +681,14 @@
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-QueryStringKeyValuePairOutputTypeDef = TypedDict(
-    "QueryStringKeyValuePairOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 QueryStringKeyValuePairTypeDef = TypedDict(
     "QueryStringKeyValuePairTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -883,25 +698,14 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
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
 SourceIpConditionConfigOutputTypeDef = TypedDict(
     "SourceIpConditionConfigOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
@@ -927,75 +731,22 @@
     "SetIpAddressTypeInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "IpAddressType": IpAddressTypeType,
     },
 )
 
-SetIpAddressTypeOutputTypeDef = TypedDict(
-    "SetIpAddressTypeOutputTypeDef",
-    {
-        "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSecurityGroupsInputRequestTypeDef = TypedDict(
     "SetSecurityGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-SetSecurityGroupsOutputTypeDef = TypedDict(
-    "SetSecurityGroupsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
-_RequiredTargetDescriptionOutputTypeDef = TypedDict(
-    "_RequiredTargetDescriptionOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalTargetDescriptionOutputTypeDef = TypedDict(
-    "_OptionalTargetDescriptionOutputTypeDef",
-    {
-        "Port": int,
-        "AvailabilityZone": str,
-    },
-    total=False,
-)
-
-class TargetDescriptionOutputTypeDef(
-    _RequiredTargetDescriptionOutputTypeDef, _OptionalTargetDescriptionOutputTypeDef
-):
-    pass
-
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -1017,36 +768,61 @@
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Certificates": List[CertificateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
-        "Certificates": List[CertificateOutputTypeDef],
+        "Certificates": List[CertificateTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetIpAddressTypeOutputTypeDef = TypedDict(
+    "SetIpAddressTypeOutputTypeDef",
+    {
+        "IpAddressType": IpAddressTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetSecurityGroupsOutputTypeDef = TypedDict(
+    "SetSecurityGroupsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
         "OutpostId": str,
         "LoadBalancerAddresses": List[LoadBalancerAddressTypeDef],
@@ -1169,14 +945,39 @@
 )
 
 class ModifyTargetGroupInputRequestTypeDef(
     _RequiredModifyTargetGroupInputRequestTypeDef, _OptionalModifyTargetGroupInputRequestTypeDef
 ):
     pass
 
+TargetGroupTypeDef = TypedDict(
+    "TargetGroupTypeDef",
+    {
+        "TargetGroupArn": str,
+        "TargetGroupName": str,
+        "Protocol": ProtocolEnumType,
+        "Port": int,
+        "VpcId": str,
+        "HealthCheckProtocol": ProtocolEnumType,
+        "HealthCheckPort": str,
+        "HealthCheckEnabled": bool,
+        "HealthCheckIntervalSeconds": int,
+        "HealthCheckTimeoutSeconds": int,
+        "HealthyThresholdCount": int,
+        "UnhealthyThresholdCount": int,
+        "HealthCheckPath": str,
+        "Matcher": MatcherTypeDef,
+        "LoadBalancerArns": List[str],
+        "TargetType": TargetTypeEnumType,
+        "ProtocolVersion": str,
+        "IpAddressType": TargetGroupIpAddressTypeEnumType,
+    },
+    total=False,
+)
+
 DeregisterTargetsInputRequestTypeDef = TypedDict(
     "DeregisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
@@ -1205,36 +1006,123 @@
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
+    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+):
+    pass
+
+DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "ListenerArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+        "RuleArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "LoadBalancerType": LoadBalancerTypeEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "TargetGroupArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
-        "Attributes": List[LoadBalancerAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[LoadBalancerAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
         "LoadBalancerArns": Sequence[str],
@@ -1311,90 +1199,57 @@
     _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef,
 ):
     pass
 
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[TargetGroupAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
+    "ModifyTargetGroupAttributesInputRequestTypeDef",
+    {
+        "TargetGroupArn": str,
+        "Attributes": Sequence[TargetGroupAttributeTypeDef],
     },
 )
 
 ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
-        "Attributes": List[TargetGroupAttributeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[TargetGroupAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ForwardActionConfigOutputTypeDef = TypedDict(
     "ForwardActionConfigOutputTypeDef",
     {
-        "TargetGroups": List[TargetGroupTupleOutputTypeDef],
-        "TargetGroupStickinessConfig": TargetGroupStickinessConfigOutputTypeDef,
+        "TargetGroups": List[TargetGroupTupleTypeDef],
+        "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "Attributes": Sequence[LoadBalancerAttributeTypeDef],
-    },
-)
-
-TargetGroupTypeDef = TypedDict(
-    "TargetGroupTypeDef",
-    {
-        "TargetGroupArn": str,
-        "TargetGroupName": str,
-        "Protocol": ProtocolEnumType,
-        "Port": int,
-        "VpcId": str,
-        "HealthCheckProtocol": ProtocolEnumType,
-        "HealthCheckPort": str,
-        "HealthCheckEnabled": bool,
-        "HealthCheckIntervalSeconds": int,
-        "HealthCheckTimeoutSeconds": int,
-        "HealthyThresholdCount": int,
-        "UnhealthyThresholdCount": int,
-        "HealthCheckPath": str,
-        "Matcher": MatcherOutputTypeDef,
-        "LoadBalancerArns": List[str],
-        "TargetType": TargetTypeEnumType,
-        "ProtocolVersion": str,
-        "IpAddressType": TargetGroupIpAddressTypeEnumType,
-    },
-    total=False,
-)
-
-ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
-    "ModifyTargetGroupAttributesInputRequestTypeDef",
-    {
-        "TargetGroupArn": str,
-        "Attributes": Sequence[TargetGroupAttributeTypeDef],
-    },
-)
-
 QueryStringConditionConfigOutputTypeDef = TypedDict(
     "QueryStringConditionConfigOutputTypeDef",
     {
-        "Values": List[QueryStringKeyValuePairOutputTypeDef],
+        "Values": List[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
 
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
@@ -1406,33 +1261,32 @@
 SetRulePrioritiesInputRequestTypeDef = TypedDict(
     "SetRulePrioritiesInputRequestTypeDef",
     {
         "RulePriorities": Sequence[RulePriorityPairTypeDef],
     },
 )
 
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 TargetHealthDescriptionTypeDef = TypedDict(
     "TargetHealthDescriptionTypeDef",
     {
-        "Target": TargetDescriptionOutputTypeDef,
+        "Target": TargetDescriptionTypeDef,
         "HealthCheckPort": str,
         "TargetHealth": TargetHealthTypeDef,
     },
     total=False,
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
         "DNSName": str,
         "CanonicalHostedZoneId": str,
         "CreatedTime": datetime,
@@ -1450,24 +1304,49 @@
 )
 
 SetSubnetsOutputTypeDef = TypedDict(
     "SetSubnetsOutputTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSSLPoliciesOutputTypeDef = TypedDict(
     "DescribeSSLPoliciesOutputTypeDef",
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTargetGroupOutputTypeDef = TypedDict(
+    "CreateTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTargetGroupsOutputTypeDef = TypedDict(
+    "DescribeTargetGroupsOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyTargetGroupOutputTypeDef = TypedDict(
+    "ModifyTargetGroupOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActionOutputTypeDef = TypedDict(
     "_RequiredActionOutputTypeDef",
     {
         "Type": ActionTypeEnumType,
@@ -1476,16 +1355,16 @@
 _OptionalActionOutputTypeDef = TypedDict(
     "_OptionalActionOutputTypeDef",
     {
         "TargetGroupArn": str,
         "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
         "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
         "Order": int,
-        "RedirectConfig": RedirectActionConfigOutputTypeDef,
-        "FixedResponseConfig": FixedResponseActionConfigOutputTypeDef,
+        "RedirectConfig": RedirectActionConfigTypeDef,
+        "FixedResponseConfig": FixedResponseActionConfigTypeDef,
         "ForwardConfig": ForwardActionConfigOutputTypeDef,
     },
     total=False,
 )
 
 class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
     pass
@@ -1509,39 +1388,14 @@
     },
     total=False,
 )
 
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
-CreateTargetGroupOutputTypeDef = TypedDict(
-    "CreateTargetGroupOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeTargetGroupsOutputTypeDef = TypedDict(
-    "DescribeTargetGroupsOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModifyTargetGroupOutputTypeDef = TypedDict(
-    "ModifyTargetGroupOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RuleConditionOutputTypeDef = TypedDict(
     "RuleConditionOutputTypeDef",
     {
         "Field": str,
         "Values": List[str],
         "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
         "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
@@ -1564,55 +1418,47 @@
         "QueryStringConfig": QueryStringConditionConfigTypeDef,
         "HttpRequestMethodConfig": HttpRequestMethodConditionConfigTypeDef,
         "SourceIpConfig": SourceIpConditionConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
-    {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerOutputTypeDef = TypedDict(
     "CreateLoadBalancerOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersOutputTypeDef = TypedDict(
     "DescribeLoadBalancersOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListenerTypeDef = TypedDict(
     "ListenerTypeDef",
     {
         "ListenerArn": str,
         "LoadBalancerArn": str,
         "Port": int,
         "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateOutputTypeDef],
+        "Certificates": List[CertificateTypeDef],
         "SslPolicy": str,
         "DefaultActions": List[ActionOutputTypeDef],
         "AlpnPolicy": List[str],
     },
     total=False,
 )
 
@@ -1719,60 +1565,60 @@
 ):
     pass
 
 CreateListenerOutputTypeDef = TypedDict(
     "CreateListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenersOutputTypeDef = TypedDict(
     "DescribeListenersOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyListenerOutputTypeDef = TypedDict(
     "ModifyListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleOutputTypeDef = TypedDict(
     "CreateRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRulesOutputTypeDef = TypedDict(
     "DescribeRulesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRuleOutputTypeDef = TypedDict(
     "ModifyRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetRulePrioritiesOutputTypeDef = TypedDict(
     "SetRulePrioritiesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.py` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2/waiter.pyi` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/PKG-INFO` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,129 +406,118 @@
 `mypy_boto3_elbv2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigOutputTypeDef,
     AuthenticateOidcActionConfigOutputTypeDef,
-    FixedResponseActionConfigOutputTypeDef,
-    RedirectActionConfigOutputTypeDef,
-    AuthenticateCognitoActionConfigTypeDef,
-    AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
+    AuthenticateCognitoActionConfigTypeDef,
+    AuthenticateOidcActionConfigTypeDef,
     CertificateTypeDef,
-    CertificateOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
-    LoadBalancerAttributeOutputTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    LoadBalancerAttributeTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
-    TargetGroupAttributeOutputTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
+    TargetGroupAttributeTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
-    TargetGroupStickinessConfigOutputTypeDef,
-    TargetGroupTupleOutputTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
     HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
     HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
     HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
-    LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
-    MatcherOutputTypeDef,
-    TargetGroupAttributeTypeDef,
-    PaginatorConfigTypeDef,
     PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
-    QueryStringKeyValuePairOutputTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
-    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
-    SetSecurityGroupsOutputTypeDef,
-    TagOutputTypeDef,
-    TargetDescriptionOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
     RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
+    SetIpAddressTypeOutputTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
+    TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
+    ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
-    TargetGroupTypeDef,
-    ModifyTargetGroupAttributesInputRequestTypeDef,
     QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
-    TagDescriptionTypeDef,
     TargetHealthDescriptionTypeDef,
+    DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
-    ActionOutputTypeDef,
-    ActionTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    ActionOutputTypeDef,
+    ActionTypeDef,
     RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
     ListenerTypeDef,
     CreateListenerInputRequestTypeDef,
     ModifyListenerInputRequestTypeDef,
     RuleTypeDef,
```

### Comparing `mypy-boto3-elbv2-1.28.12/mypy_boto3_elbv2.egg-info/SOURCES.txt` & `mypy-boto3-elbv2-1.28.15/mypy_boto3_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.28.12/setup.py` & `mypy-boto3-elbv2-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elbv2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

