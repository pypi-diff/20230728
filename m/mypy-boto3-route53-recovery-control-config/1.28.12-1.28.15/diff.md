# Comparing `tmp/mypy-boto3-route53-recovery-control-config-1.28.12.tar.gz` & `tmp/mypy-boto3-route53-recovery-control-config-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-control-config-1.28.12.tar", last modified: Thu Jul 27 11:49:31 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-control-config-1.28.15.tar", last modified: Fri Jul 28 20:43:36 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-control-config-1.28.12.tar` & `mypy-boto3-route53-recovery-control-config-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:31.321223 mypy-boto3-route53-recovery-control-config-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-07-27 11:49:31.321223 mypy-boto3-route53-recovery-control-config-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:31.317223 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23819 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23778 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23406 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-27 11:44:50.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:31.321223 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-07-27 11:49:31.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-27 11:49:31.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:31.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:31.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:31.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 11:49:31.000000 mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:31.321223 mypy-boto3-route53-recovery-control-config-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-27 11:44:49.000000 mypy-boto3-route53-recovery-control-config-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.773769 mypy-boto3-route53-recovery-control-config-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-07-28 20:43:36.773769 mypy-boto3-route53-recovery-control-config-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17404 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.761768 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23819 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23778 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23185 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-28 20:37:15.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.761768 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:36.773769 mypy-boto3-route53-recovery-control-config-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-28 20:37:14.000000 mypy-boto3-route53-recovery-control-config-1.28.15/setup.py
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/LICENSE` & `mypy-boto3-route53-recovery-control-config-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/PKG-INFO` & `mypy-boto3-route53-recovery-control-config-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-control-config
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-control-config)](https://pepy.tech/project/mypy-boto3-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryControlConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[boto3.Route53RecoveryControlConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [mypy-boto3-route53-recovery-control-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,15 +387,15 @@
 
 `mypy_boto3_route53_recovery_control_config.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_route53_recovery_control_config.type_defs import (
-    RuleConfigOutputTypeDef,
+    RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
@@ -413,21 +413,22 @@
     PaginatorConfigTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListControlPanelsRequestRequestTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RuleConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
+    NewAssertionRuleTypeDef,
+    NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
     ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
@@ -443,29 +444,27 @@
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
     ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    NewAssertionRuleTypeDef,
-    NewGatingRuleTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
+    CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
-    CreateSafetyRuleRequestRequestTypeDef,
     ListSafetyRulesResponseTypeDef,
 )
 
 
-def get_structure() -> RuleConfigOutputTypeDef:
+def get_structure() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/README.md` & `mypy-boto3-route53-recovery-control-config-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-control-config)](https://pepy.tech/project/mypy-boto3-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryControlConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[boto3.Route53RecoveryControlConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [mypy-boto3-route53-recovery-control-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,15 +355,15 @@
 
 `mypy_boto3_route53_recovery_control_config.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_route53_recovery_control_config.type_defs import (
-    RuleConfigOutputTypeDef,
+    RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
@@ -381,21 +381,22 @@
     PaginatorConfigTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListControlPanelsRequestRequestTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RuleConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
+    NewAssertionRuleTypeDef,
+    NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
     ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
@@ -411,29 +412,27 @@
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
     ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    NewAssertionRuleTypeDef,
-    NewGatingRuleTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
+    CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
-    CreateSafetyRuleRequestRequestTypeDef,
     ListSafetyRulesResponseTypeDef,
 )
 
 
-def get_structure() -> RuleConfigOutputTypeDef:
+def get_structure() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/__init__.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/__init__.pyi` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/__main__.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryControlConfig 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryControlConfig 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig\nOther"
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

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/client.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/client.pyi` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/literals.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/literals.pyi` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/paginator.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/paginator.pyi` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/type_defs.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 Type annotations for route53-recovery-control-config service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_route53_recovery_control_config.type_defs import RuleConfigOutputTypeDef
+    from mypy_boto3_route53_recovery_control_config.type_defs import RuleConfigTypeDef
 
-    data: RuleConfigOutputTypeDef = {...}
+    data: RuleConfigTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import RuleTypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "RuleConfigOutputTypeDef",
+    "RuleConfigTypeDef",
     "AssertionRuleUpdateTypeDef",
     "ClusterEndpointTypeDef",
     "ControlPanelTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateControlPanelRequestRequestTypeDef",
     "CreateRoutingControlRequestRequestTypeDef",
@@ -45,21 +45,22 @@
     "PaginatorConfigTypeDef",
     "ListAssociatedRoute53HealthChecksRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListControlPanelsRequestRequestTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "ListSafetyRulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RuleConfigTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateControlPanelRequestRequestTypeDef",
     "UpdateRoutingControlRequestRequestTypeDef",
     "AssertionRuleTypeDef",
     "GatingRuleTypeDef",
+    "NewAssertionRuleTypeDef",
+    "NewGatingRuleTypeDef",
     "ClusterTypeDef",
     "CreateControlPanelResponseTypeDef",
     "DescribeControlPanelResponseTypeDef",
     "ListAssociatedRoute53HealthChecksResponseTypeDef",
     "ListControlPanelsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateControlPanelResponseTypeDef",
@@ -75,29 +76,27 @@
     "DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef",
     "UpdateSafetyRuleRequestRequestTypeDef",
     "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
     "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    "NewAssertionRuleTypeDef",
-    "NewGatingRuleTypeDef",
     "CreateSafetyRuleResponseTypeDef",
     "DescribeSafetyRuleResponseTypeDef",
     "RuleTypeDef",
     "UpdateSafetyRuleResponseTypeDef",
+    "CreateSafetyRuleRequestRequestTypeDef",
     "CreateClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "CreateSafetyRuleRequestRequestTypeDef",
     "ListSafetyRulesResponseTypeDef",
 )
 
-RuleConfigOutputTypeDef = TypedDict(
-    "RuleConfigOutputTypeDef",
+RuleConfigTypeDef = TypedDict(
+    "RuleConfigTypeDef",
     {
         "Inverted": bool,
         "Threshold": int,
         "Type": RuleTypeType,
     },
 )
 
@@ -398,23 +397,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-RuleConfigTypeDef = TypedDict(
-    "RuleConfigTypeDef",
-    {
-        "Inverted": bool,
-        "Threshold": int,
-        "Type": RuleTypeType,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -445,35 +435,58 @@
 
 AssertionRuleTypeDef = TypedDict(
     "AssertionRuleTypeDef",
     {
         "AssertedControls": List[str],
         "ControlPanelArn": str,
         "Name": str,
-        "RuleConfig": RuleConfigOutputTypeDef,
+        "RuleConfig": RuleConfigTypeDef,
         "SafetyRuleArn": str,
         "Status": StatusType,
         "WaitPeriodMs": int,
     },
 )
 
 GatingRuleTypeDef = TypedDict(
     "GatingRuleTypeDef",
     {
         "ControlPanelArn": str,
         "GatingControls": List[str],
         "Name": str,
-        "RuleConfig": RuleConfigOutputTypeDef,
+        "RuleConfig": RuleConfigTypeDef,
         "SafetyRuleArn": str,
         "Status": StatusType,
         "TargetControls": List[str],
         "WaitPeriodMs": int,
     },
 )
 
+NewAssertionRuleTypeDef = TypedDict(
+    "NewAssertionRuleTypeDef",
+    {
+        "AssertedControls": Sequence[str],
+        "ControlPanelArn": str,
+        "Name": str,
+        "RuleConfig": RuleConfigTypeDef,
+        "WaitPeriodMs": int,
+    },
+)
+
+NewGatingRuleTypeDef = TypedDict(
+    "NewGatingRuleTypeDef",
+    {
+        "ControlPanelArn": str,
+        "GatingControls": Sequence[str],
+        "Name": str,
+        "RuleConfig": RuleConfigTypeDef,
+        "TargetControls": Sequence[str],
+        "WaitPeriodMs": int,
+    },
+)
+
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterArn": str,
         "ClusterEndpoints": List[ClusterEndpointTypeDef],
         "Name": str,
         "Status": StatusType,
@@ -784,37 +797,14 @@
 class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
     _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
 ):
     pass
 
 
-NewAssertionRuleTypeDef = TypedDict(
-    "NewAssertionRuleTypeDef",
-    {
-        "AssertedControls": Sequence[str],
-        "ControlPanelArn": str,
-        "Name": str,
-        "RuleConfig": RuleConfigTypeDef,
-        "WaitPeriodMs": int,
-    },
-)
-
-NewGatingRuleTypeDef = TypedDict(
-    "NewGatingRuleTypeDef",
-    {
-        "ControlPanelArn": str,
-        "GatingControls": Sequence[str],
-        "Name": str,
-        "RuleConfig": RuleConfigTypeDef,
-        "TargetControls": Sequence[str],
-        "WaitPeriodMs": int,
-    },
-)
-
 CreateSafetyRuleResponseTypeDef = TypedDict(
     "CreateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -843,14 +833,25 @@
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateSafetyRuleRequestRequestTypeDef = TypedDict(
+    "CreateSafetyRuleRequestRequestTypeDef",
+    {
+        "AssertionRule": NewAssertionRuleTypeDef,
+        "ClientToken": str,
+        "GatingRule": NewGatingRuleTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -868,25 +869,14 @@
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSafetyRuleRequestRequestTypeDef = TypedDict(
-    "CreateSafetyRuleRequestRequestTypeDef",
-    {
-        "AssertionRule": NewAssertionRuleTypeDef,
-        "ClientToken": str,
-        "GatingRule": NewGatingRuleTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 ListSafetyRulesResponseTypeDef = TypedDict(
     "ListSafetyRulesResponseTypeDef",
     {
         "NextToken": str,
         "SafetyRules": List[RuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/type_defs.pyi` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 Type annotations for route53-recovery-control-config service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_route53_recovery_control_config.type_defs import RuleConfigOutputTypeDef
+    from mypy_boto3_route53_recovery_control_config.type_defs import RuleConfigTypeDef
 
-    data: RuleConfigOutputTypeDef = {...}
+    data: RuleConfigTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import RuleTypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "RuleConfigOutputTypeDef",
+    "RuleConfigTypeDef",
     "AssertionRuleUpdateTypeDef",
     "ClusterEndpointTypeDef",
     "ControlPanelTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateControlPanelRequestRequestTypeDef",
     "CreateRoutingControlRequestRequestTypeDef",
@@ -44,21 +44,22 @@
     "PaginatorConfigTypeDef",
     "ListAssociatedRoute53HealthChecksRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListControlPanelsRequestRequestTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "ListSafetyRulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RuleConfigTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateControlPanelRequestRequestTypeDef",
     "UpdateRoutingControlRequestRequestTypeDef",
     "AssertionRuleTypeDef",
     "GatingRuleTypeDef",
+    "NewAssertionRuleTypeDef",
+    "NewGatingRuleTypeDef",
     "ClusterTypeDef",
     "CreateControlPanelResponseTypeDef",
     "DescribeControlPanelResponseTypeDef",
     "ListAssociatedRoute53HealthChecksResponseTypeDef",
     "ListControlPanelsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateControlPanelResponseTypeDef",
@@ -74,29 +75,27 @@
     "DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef",
     "UpdateSafetyRuleRequestRequestTypeDef",
     "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
     "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    "NewAssertionRuleTypeDef",
-    "NewGatingRuleTypeDef",
     "CreateSafetyRuleResponseTypeDef",
     "DescribeSafetyRuleResponseTypeDef",
     "RuleTypeDef",
     "UpdateSafetyRuleResponseTypeDef",
+    "CreateSafetyRuleRequestRequestTypeDef",
     "CreateClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "CreateSafetyRuleRequestRequestTypeDef",
     "ListSafetyRulesResponseTypeDef",
 )
 
-RuleConfigOutputTypeDef = TypedDict(
-    "RuleConfigOutputTypeDef",
+RuleConfigTypeDef = TypedDict(
+    "RuleConfigTypeDef",
     {
         "Inverted": bool,
         "Threshold": int,
         "Type": RuleTypeType,
     },
 )
 
@@ -385,23 +384,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-RuleConfigTypeDef = TypedDict(
-    "RuleConfigTypeDef",
-    {
-        "Inverted": bool,
-        "Threshold": int,
-        "Type": RuleTypeType,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -432,35 +422,58 @@
 
 AssertionRuleTypeDef = TypedDict(
     "AssertionRuleTypeDef",
     {
         "AssertedControls": List[str],
         "ControlPanelArn": str,
         "Name": str,
-        "RuleConfig": RuleConfigOutputTypeDef,
+        "RuleConfig": RuleConfigTypeDef,
         "SafetyRuleArn": str,
         "Status": StatusType,
         "WaitPeriodMs": int,
     },
 )
 
 GatingRuleTypeDef = TypedDict(
     "GatingRuleTypeDef",
     {
         "ControlPanelArn": str,
         "GatingControls": List[str],
         "Name": str,
-        "RuleConfig": RuleConfigOutputTypeDef,
+        "RuleConfig": RuleConfigTypeDef,
         "SafetyRuleArn": str,
         "Status": StatusType,
         "TargetControls": List[str],
         "WaitPeriodMs": int,
     },
 )
 
+NewAssertionRuleTypeDef = TypedDict(
+    "NewAssertionRuleTypeDef",
+    {
+        "AssertedControls": Sequence[str],
+        "ControlPanelArn": str,
+        "Name": str,
+        "RuleConfig": RuleConfigTypeDef,
+        "WaitPeriodMs": int,
+    },
+)
+
+NewGatingRuleTypeDef = TypedDict(
+    "NewGatingRuleTypeDef",
+    {
+        "ControlPanelArn": str,
+        "GatingControls": Sequence[str],
+        "Name": str,
+        "RuleConfig": RuleConfigTypeDef,
+        "TargetControls": Sequence[str],
+        "WaitPeriodMs": int,
+    },
+)
+
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterArn": str,
         "ClusterEndpoints": List[ClusterEndpointTypeDef],
         "Name": str,
         "Status": StatusType,
@@ -753,37 +766,14 @@
 
 class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
     _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
 ):
     pass
 
-NewAssertionRuleTypeDef = TypedDict(
-    "NewAssertionRuleTypeDef",
-    {
-        "AssertedControls": Sequence[str],
-        "ControlPanelArn": str,
-        "Name": str,
-        "RuleConfig": RuleConfigTypeDef,
-        "WaitPeriodMs": int,
-    },
-)
-
-NewGatingRuleTypeDef = TypedDict(
-    "NewGatingRuleTypeDef",
-    {
-        "ControlPanelArn": str,
-        "GatingControls": Sequence[str],
-        "Name": str,
-        "RuleConfig": RuleConfigTypeDef,
-        "TargetControls": Sequence[str],
-        "WaitPeriodMs": int,
-    },
-)
-
 CreateSafetyRuleResponseTypeDef = TypedDict(
     "CreateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -812,14 +802,25 @@
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateSafetyRuleRequestRequestTypeDef = TypedDict(
+    "CreateSafetyRuleRequestRequestTypeDef",
+    {
+        "AssertionRule": NewAssertionRuleTypeDef,
+        "ClientToken": str,
+        "GatingRule": NewGatingRuleTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -837,25 +838,14 @@
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSafetyRuleRequestRequestTypeDef = TypedDict(
-    "CreateSafetyRuleRequestRequestTypeDef",
-    {
-        "AssertionRule": NewAssertionRuleTypeDef,
-        "ClientToken": str,
-        "GatingRule": NewGatingRuleTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 ListSafetyRulesResponseTypeDef = TypedDict(
     "ListSafetyRulesResponseTypeDef",
     {
         "NextToken": str,
         "SafetyRules": List[RuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/waiter.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config/waiter.pyi` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-control-config
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-control-config)](https://pepy.tech/project/mypy-boto3-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryControlConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[boto3.Route53RecoveryControlConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [mypy-boto3-route53-recovery-control-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,15 +387,15 @@
 
 `mypy_boto3_route53_recovery_control_config.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_route53_recovery_control_config.type_defs import (
-    RuleConfigOutputTypeDef,
+    RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
@@ -413,21 +413,22 @@
     PaginatorConfigTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListControlPanelsRequestRequestTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RuleConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
+    NewAssertionRuleTypeDef,
+    NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
     ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
@@ -443,29 +444,27 @@
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
     ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    NewAssertionRuleTypeDef,
-    NewGatingRuleTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
+    CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
-    CreateSafetyRuleRequestRequestTypeDef,
     ListSafetyRulesResponseTypeDef,
 )
 
 
-def get_structure() -> RuleConfigOutputTypeDef:
+def get_structure() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-control-config-1.28.15/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.28.12/setup.py` & `mypy-boto3-route53-recovery-control-config-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-control-config",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_route53_recovery_control_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryControlConfig 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Route53RecoveryControlConfig 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

