# Comparing `tmp/mypy-boto3-vpc-lattice-1.28.12.tar.gz` & `tmp/mypy-boto3-vpc-lattice-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
+gzip compressed data, was "mypy-boto3-vpc-lattice-1.28.15.tar", last modified: Fri Jul 28 20:43:55 2023, max compression
```

## Comparing `mypy-boto3-vpc-lattice-1.28.12.tar` & `mypy-boto3-vpc-lattice-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19143 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38846 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-07-27 11:48:20.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-27 11:48:20.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53229 2023-07-27 11:48:21.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53170 2023-07-27 11:48:20.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 11:49:48.000000 mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.065487 mypy-boto3-vpc-lattice-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-27 11:48:19.000000 mypy-boto3-vpc-lattice-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18820 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.290022 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38846 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49473 2023-07-28 20:41:03.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-07-28 20:41:02.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:01.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:55.000000 mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:55.298023 mypy-boto3-vpc-lattice-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-28 20:41:00.000000 mypy-boto3-vpc-lattice-1.28.15/setup.py
```

### Comparing `mypy-boto3-vpc-lattice-1.28.12/LICENSE` & `mypy-boto3-vpc-lattice-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.12
-Summary: Type annotations for boto3.VPCLattice 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,32 +386,27 @@
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
-    TargetOutputTypeDef,
-    FixedResponseActionOutputTypeDef,
     FixedResponseActionTypeDef,
-    WeightedTargetGroupOutputTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
-    HeaderMatchTypeOutputTypeDef,
     HeaderMatchTypeTypeDef,
-    MatcherOutputTypeDef,
     MatcherTypeDef,
     PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
@@ -421,15 +416,14 @@
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PathMatchTypeOutputTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
@@ -463,17 +457,15 @@
     DeregisterTargetsRequestRequestTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
     ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
-    HeaderMatchOutputTypeDef,
     HeaderMatchTypeDef,
-    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
     ListListenersRequestListListenersPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
@@ -482,34 +474,32 @@
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
-    PathMatchOutputTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    TargetGroupConfigOutputTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
     HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
     UpdateListenerResponseTypeDef,
     CreateListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
+    CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
-    CreateTargetGroupRequestRequestTypeDef,
     RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
     UpdateRuleResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
```

### Comparing `mypy-boto3-vpc-lattice-1.28.12/README.md` & `mypy-boto3-vpc-lattice-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,32 +354,27 @@
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
-    TargetOutputTypeDef,
-    FixedResponseActionOutputTypeDef,
     FixedResponseActionTypeDef,
-    WeightedTargetGroupOutputTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
-    HeaderMatchTypeOutputTypeDef,
     HeaderMatchTypeTypeDef,
-    MatcherOutputTypeDef,
     MatcherTypeDef,
     PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
@@ -389,15 +384,14 @@
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PathMatchTypeOutputTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
@@ -431,17 +425,15 @@
     DeregisterTargetsRequestRequestTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
     ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
-    HeaderMatchOutputTypeDef,
     HeaderMatchTypeDef,
-    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
     ListListenersRequestListListenersPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
@@ -450,34 +442,32 @@
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
-    PathMatchOutputTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    TargetGroupConfigOutputTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
     HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
     UpdateListenerResponseTypeDef,
     CreateListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
+    CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
-    CreateTargetGroupRequestRequestTypeDef,
     RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
     UpdateRuleResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
```

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.py` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__init__.pyi` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/__main__.py` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VPCLattice 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.VPCLattice 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.py` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/client.pyi` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.py` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/literals.pyi` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.py` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/paginator.pyi` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.py` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,32 +55,27 @@
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
-    "TargetOutputTypeDef",
-    "FixedResponseActionOutputTypeDef",
     "FixedResponseActionTypeDef",
-    "WeightedTargetGroupOutputTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
-    "HeaderMatchTypeOutputTypeDef",
     "HeaderMatchTypeTypeDef",
-    "MatcherOutputTypeDef",
     "MatcherTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
@@ -90,15 +85,14 @@
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
-    "PathMatchTypeOutputTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     "UpdateServiceNetworkRequestRequestTypeDef",
@@ -132,17 +126,15 @@
     "DeregisterTargetsRequestRequestTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
     "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
-    "HeaderMatchOutputTypeDef",
     "HeaderMatchTypeDef",
-    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
@@ -151,34 +143,32 @@
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
-    "PathMatchOutputTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
     "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
-    "TargetGroupConfigOutputTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
     "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
     "UpdateListenerResponseTypeDef",
     "CreateListenerRequestRequestTypeDef",
     "UpdateListenerRequestRequestTypeDef",
+    "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
-    "CreateTargetGroupRequestRequestTypeDef",
     "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
     "UpdateRuleResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
@@ -452,68 +442,21 @@
         "failureMessage": str,
         "id": str,
         "port": int,
     },
     total=False,
 )
 
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "port": int,
-    },
-    total=False,
-)
-
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
-    pass
-
-
-FixedResponseActionOutputTypeDef = TypedDict(
-    "FixedResponseActionOutputTypeDef",
-    {
-        "statusCode": int,
-    },
-)
-
 FixedResponseActionTypeDef = TypedDict(
     "FixedResponseActionTypeDef",
     {
         "statusCode": int,
     },
 )
 
-_RequiredWeightedTargetGroupOutputTypeDef = TypedDict(
-    "_RequiredWeightedTargetGroupOutputTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalWeightedTargetGroupOutputTypeDef = TypedDict(
-    "_OptionalWeightedTargetGroupOutputTypeDef",
-    {
-        "weight": int,
-    },
-    total=False,
-)
-
-
-class WeightedTargetGroupOutputTypeDef(
-    _RequiredWeightedTargetGroupOutputTypeDef, _OptionalWeightedTargetGroupOutputTypeDef
-):
-    pass
-
-
 _RequiredWeightedTargetGroupTypeDef = TypedDict(
     "_RequiredWeightedTargetGroupTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalWeightedTargetGroupTypeDef = TypedDict(
@@ -600,42 +543,24 @@
 GetTargetGroupRequestRequestTypeDef = TypedDict(
     "GetTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
-HeaderMatchTypeOutputTypeDef = TypedDict(
-    "HeaderMatchTypeOutputTypeDef",
-    {
-        "contains": str,
-        "exact": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
 HeaderMatchTypeTypeDef = TypedDict(
     "HeaderMatchTypeTypeDef",
     {
         "contains": str,
         "exact": str,
         "prefix": str,
     },
     total=False,
 )
 
-MatcherOutputTypeDef = TypedDict(
-    "MatcherOutputTypeDef",
-    {
-        "httpCode": str,
-    },
-    total=False,
-)
-
 MatcherTypeDef = TypedDict(
     "MatcherTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
@@ -861,23 +786,14 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
     },
     total=False,
 )
 
-PathMatchTypeOutputTypeDef = TypedDict(
-    "PathMatchTypeOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
         "exact": str,
         "prefix": str,
     },
     total=False,
@@ -1321,65 +1237,43 @@
         "targets": Sequence[TargetTypeDef],
     },
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetOutputTypeDef],
+        "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetOutputTypeDef],
+        "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ForwardActionOutputTypeDef = TypedDict(
     "ForwardActionOutputTypeDef",
     {
-        "targetGroups": List[WeightedTargetGroupOutputTypeDef],
+        "targetGroups": List[WeightedTargetGroupTypeDef],
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 
-_RequiredHeaderMatchOutputTypeDef = TypedDict(
-    "_RequiredHeaderMatchOutputTypeDef",
-    {
-        "match": HeaderMatchTypeOutputTypeDef,
-        "name": str,
-    },
-)
-_OptionalHeaderMatchOutputTypeDef = TypedDict(
-    "_OptionalHeaderMatchOutputTypeDef",
-    {
-        "caseSensitive": bool,
-    },
-    total=False,
-)
-
-
-class HeaderMatchOutputTypeDef(
-    _RequiredHeaderMatchOutputTypeDef, _OptionalHeaderMatchOutputTypeDef
-):
-    pass
-
-
 _RequiredHeaderMatchTypeDef = TypedDict(
     "_RequiredHeaderMatchTypeDef",
     {
         "match": HeaderMatchTypeTypeDef,
         "name": str,
     },
 )
@@ -1392,31 +1286,14 @@
 )
 
 
 class HeaderMatchTypeDef(_RequiredHeaderMatchTypeDef, _OptionalHeaderMatchTypeDef):
     pass
 
 
-HealthCheckConfigOutputTypeDef = TypedDict(
-    "HealthCheckConfigOutputTypeDef",
-    {
-        "enabled": bool,
-        "healthCheckIntervalSeconds": int,
-        "healthCheckTimeoutSeconds": int,
-        "healthyThresholdCount": int,
-        "matcher": MatcherOutputTypeDef,
-        "path": str,
-        "port": int,
-        "protocol": TargetGroupProtocolType,
-        "protocolVersion": HealthCheckProtocolVersionType,
-        "unhealthyThresholdCount": int,
-    },
-    total=False,
-)
-
 HealthCheckConfigTypeDef = TypedDict(
     "HealthCheckConfigTypeDef",
     {
         "enabled": bool,
         "healthCheckIntervalSeconds": int,
         "healthCheckTimeoutSeconds": int,
         "healthyThresholdCount": int,
@@ -1618,33 +1495,14 @@
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPathMatchOutputTypeDef = TypedDict(
-    "_RequiredPathMatchOutputTypeDef",
-    {
-        "match": PathMatchTypeOutputTypeDef,
-    },
-)
-_OptionalPathMatchOutputTypeDef = TypedDict(
-    "_OptionalPathMatchOutputTypeDef",
-    {
-        "caseSensitive": bool,
-    },
-    total=False,
-)
-
-
-class PathMatchOutputTypeDef(_RequiredPathMatchOutputTypeDef, _OptionalPathMatchOutputTypeDef):
-    pass
-
-
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
     },
 )
 _OptionalPathMatchTypeDef = TypedDict(
@@ -1677,54 +1535,29 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleActionOutputTypeDef = TypedDict(
     "RuleActionOutputTypeDef",
     {
-        "fixedResponse": FixedResponseActionOutputTypeDef,
+        "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionOutputTypeDef,
     },
     total=False,
 )
 
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
     },
     total=False,
 )
 
-_RequiredTargetGroupConfigOutputTypeDef = TypedDict(
-    "_RequiredTargetGroupConfigOutputTypeDef",
-    {
-        "port": int,
-        "protocol": TargetGroupProtocolType,
-        "vpcIdentifier": str,
-    },
-)
-_OptionalTargetGroupConfigOutputTypeDef = TypedDict(
-    "_OptionalTargetGroupConfigOutputTypeDef",
-    {
-        "healthCheck": HealthCheckConfigOutputTypeDef,
-        "ipAddressType": IpAddressTypeType,
-        "protocolVersion": TargetGroupProtocolVersionType,
-    },
-    total=False,
-)
-
-
-class TargetGroupConfigOutputTypeDef(
-    _RequiredTargetGroupConfigOutputTypeDef, _OptionalTargetGroupConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredTargetGroupConfigTypeDef = TypedDict(
     "_RequiredTargetGroupConfigTypeDef",
     {
         "port": int,
         "protocol": TargetGroupProtocolType,
         "vpcIdentifier": str,
     },
@@ -1753,17 +1586,17 @@
         "targetGroupIdentifier": str,
     },
 )
 
 HttpMatchOutputTypeDef = TypedDict(
     "HttpMatchOutputTypeDef",
     {
-        "headerMatches": List[HeaderMatchOutputTypeDef],
+        "headerMatches": List[HeaderMatchTypeDef],
         "method": str,
-        "pathMatch": PathMatchOutputTypeDef,
+        "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
 HttpMatchTypeDef = TypedDict(
     "HttpMatchTypeDef",
     {
@@ -1852,32 +1685,56 @@
     {
         "defaultAction": RuleActionTypeDef,
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
 
+_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTargetGroupRequestRequestTypeDef",
+    {
+        "name": str,
+        "type": TargetGroupTypeType,
+    },
+)
+_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTargetGroupRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "config": TargetGroupConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateTargetGroupRequestRequestTypeDef(
+    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
+):
+    pass
+
+
 CreateTargetGroupResponseTypeDef = TypedDict(
     "CreateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigOutputTypeDef,
+        "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigOutputTypeDef,
+        "config": TargetGroupConfigTypeDef,
         "createdAt": datetime,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
@@ -1887,47 +1744,23 @@
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigOutputTypeDef,
+        "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTargetGroupRequestRequestTypeDef",
-    {
-        "name": str,
-        "type": TargetGroupTypeType,
-    },
-)
-_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTargetGroupRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "config": TargetGroupConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateTargetGroupRequestRequestTypeDef(
-    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
-):
-    pass
-
-
 RuleMatchOutputTypeDef = TypedDict(
     "RuleMatchOutputTypeDef",
     {
         "httpMatch": HttpMatchOutputTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice/type_defs.pyi` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -54,32 +54,27 @@
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
-    "TargetOutputTypeDef",
-    "FixedResponseActionOutputTypeDef",
     "FixedResponseActionTypeDef",
-    "WeightedTargetGroupOutputTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
-    "HeaderMatchTypeOutputTypeDef",
     "HeaderMatchTypeTypeDef",
-    "MatcherOutputTypeDef",
     "MatcherTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
@@ -89,15 +84,14 @@
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
-    "PathMatchTypeOutputTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     "UpdateServiceNetworkRequestRequestTypeDef",
@@ -131,17 +125,15 @@
     "DeregisterTargetsRequestRequestTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
     "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
-    "HeaderMatchOutputTypeDef",
     "HeaderMatchTypeDef",
-    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
@@ -150,34 +142,32 @@
     "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
-    "PathMatchOutputTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
     "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
-    "TargetGroupConfigOutputTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
     "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
     "UpdateListenerResponseTypeDef",
     "CreateListenerRequestRequestTypeDef",
     "UpdateListenerRequestRequestTypeDef",
+    "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
-    "CreateTargetGroupRequestRequestTypeDef",
     "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
     "UpdateRuleResponseTypeDef",
     "CreateRuleRequestRequestTypeDef",
@@ -439,64 +429,21 @@
         "failureMessage": str,
         "id": str,
         "port": int,
     },
     total=False,
 )
 
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "port": int,
-    },
-    total=False,
-)
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
-    pass
-
-FixedResponseActionOutputTypeDef = TypedDict(
-    "FixedResponseActionOutputTypeDef",
-    {
-        "statusCode": int,
-    },
-)
-
 FixedResponseActionTypeDef = TypedDict(
     "FixedResponseActionTypeDef",
     {
         "statusCode": int,
     },
 )
 
-_RequiredWeightedTargetGroupOutputTypeDef = TypedDict(
-    "_RequiredWeightedTargetGroupOutputTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalWeightedTargetGroupOutputTypeDef = TypedDict(
-    "_OptionalWeightedTargetGroupOutputTypeDef",
-    {
-        "weight": int,
-    },
-    total=False,
-)
-
-class WeightedTargetGroupOutputTypeDef(
-    _RequiredWeightedTargetGroupOutputTypeDef, _OptionalWeightedTargetGroupOutputTypeDef
-):
-    pass
-
 _RequiredWeightedTargetGroupTypeDef = TypedDict(
     "_RequiredWeightedTargetGroupTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalWeightedTargetGroupTypeDef = TypedDict(
@@ -581,42 +528,24 @@
 GetTargetGroupRequestRequestTypeDef = TypedDict(
     "GetTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
-HeaderMatchTypeOutputTypeDef = TypedDict(
-    "HeaderMatchTypeOutputTypeDef",
-    {
-        "contains": str,
-        "exact": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
 HeaderMatchTypeTypeDef = TypedDict(
     "HeaderMatchTypeTypeDef",
     {
         "contains": str,
         "exact": str,
         "prefix": str,
     },
     total=False,
 )
 
-MatcherOutputTypeDef = TypedDict(
-    "MatcherOutputTypeDef",
-    {
-        "httpCode": str,
-    },
-    total=False,
-)
-
 MatcherTypeDef = TypedDict(
     "MatcherTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
@@ -836,23 +765,14 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
     },
     total=False,
 )
 
-PathMatchTypeOutputTypeDef = TypedDict(
-    "PathMatchTypeOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
         "exact": str,
         "prefix": str,
     },
     total=False,
@@ -1292,63 +1212,43 @@
         "targets": Sequence[TargetTypeDef],
     },
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetOutputTypeDef],
+        "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
-        "successful": List[TargetOutputTypeDef],
+        "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ForwardActionOutputTypeDef = TypedDict(
     "ForwardActionOutputTypeDef",
     {
-        "targetGroups": List[WeightedTargetGroupOutputTypeDef],
+        "targetGroups": List[WeightedTargetGroupTypeDef],
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 
-_RequiredHeaderMatchOutputTypeDef = TypedDict(
-    "_RequiredHeaderMatchOutputTypeDef",
-    {
-        "match": HeaderMatchTypeOutputTypeDef,
-        "name": str,
-    },
-)
-_OptionalHeaderMatchOutputTypeDef = TypedDict(
-    "_OptionalHeaderMatchOutputTypeDef",
-    {
-        "caseSensitive": bool,
-    },
-    total=False,
-)
-
-class HeaderMatchOutputTypeDef(
-    _RequiredHeaderMatchOutputTypeDef, _OptionalHeaderMatchOutputTypeDef
-):
-    pass
-
 _RequiredHeaderMatchTypeDef = TypedDict(
     "_RequiredHeaderMatchTypeDef",
     {
         "match": HeaderMatchTypeTypeDef,
         "name": str,
     },
 )
@@ -1359,31 +1259,14 @@
     },
     total=False,
 )
 
 class HeaderMatchTypeDef(_RequiredHeaderMatchTypeDef, _OptionalHeaderMatchTypeDef):
     pass
 
-HealthCheckConfigOutputTypeDef = TypedDict(
-    "HealthCheckConfigOutputTypeDef",
-    {
-        "enabled": bool,
-        "healthCheckIntervalSeconds": int,
-        "healthCheckTimeoutSeconds": int,
-        "healthyThresholdCount": int,
-        "matcher": MatcherOutputTypeDef,
-        "path": str,
-        "port": int,
-        "protocol": TargetGroupProtocolType,
-        "protocolVersion": HealthCheckProtocolVersionType,
-        "unhealthyThresholdCount": int,
-    },
-    total=False,
-)
-
 HealthCheckConfigTypeDef = TypedDict(
     "HealthCheckConfigTypeDef",
     {
         "enabled": bool,
         "healthCheckIntervalSeconds": int,
         "healthCheckTimeoutSeconds": int,
         "healthyThresholdCount": int,
@@ -1577,31 +1460,14 @@
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPathMatchOutputTypeDef = TypedDict(
-    "_RequiredPathMatchOutputTypeDef",
-    {
-        "match": PathMatchTypeOutputTypeDef,
-    },
-)
-_OptionalPathMatchOutputTypeDef = TypedDict(
-    "_OptionalPathMatchOutputTypeDef",
-    {
-        "caseSensitive": bool,
-    },
-    total=False,
-)
-
-class PathMatchOutputTypeDef(_RequiredPathMatchOutputTypeDef, _OptionalPathMatchOutputTypeDef):
-    pass
-
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
     },
 )
 _OptionalPathMatchTypeDef = TypedDict(
@@ -1632,52 +1498,29 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleActionOutputTypeDef = TypedDict(
     "RuleActionOutputTypeDef",
     {
-        "fixedResponse": FixedResponseActionOutputTypeDef,
+        "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionOutputTypeDef,
     },
     total=False,
 )
 
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
     },
     total=False,
 )
 
-_RequiredTargetGroupConfigOutputTypeDef = TypedDict(
-    "_RequiredTargetGroupConfigOutputTypeDef",
-    {
-        "port": int,
-        "protocol": TargetGroupProtocolType,
-        "vpcIdentifier": str,
-    },
-)
-_OptionalTargetGroupConfigOutputTypeDef = TypedDict(
-    "_OptionalTargetGroupConfigOutputTypeDef",
-    {
-        "healthCheck": HealthCheckConfigOutputTypeDef,
-        "ipAddressType": IpAddressTypeType,
-        "protocolVersion": TargetGroupProtocolVersionType,
-    },
-    total=False,
-)
-
-class TargetGroupConfigOutputTypeDef(
-    _RequiredTargetGroupConfigOutputTypeDef, _OptionalTargetGroupConfigOutputTypeDef
-):
-    pass
-
 _RequiredTargetGroupConfigTypeDef = TypedDict(
     "_RequiredTargetGroupConfigTypeDef",
     {
         "port": int,
         "protocol": TargetGroupProtocolType,
         "vpcIdentifier": str,
     },
@@ -1704,17 +1547,17 @@
         "targetGroupIdentifier": str,
     },
 )
 
 HttpMatchOutputTypeDef = TypedDict(
     "HttpMatchOutputTypeDef",
     {
-        "headerMatches": List[HeaderMatchOutputTypeDef],
+        "headerMatches": List[HeaderMatchTypeDef],
         "method": str,
-        "pathMatch": PathMatchOutputTypeDef,
+        "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
 HttpMatchTypeDef = TypedDict(
     "HttpMatchTypeDef",
     {
@@ -1801,32 +1644,54 @@
     {
         "defaultAction": RuleActionTypeDef,
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
 
+_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTargetGroupRequestRequestTypeDef",
+    {
+        "name": str,
+        "type": TargetGroupTypeType,
+    },
+)
+_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTargetGroupRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "config": TargetGroupConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateTargetGroupRequestRequestTypeDef(
+    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
+):
+    pass
+
 CreateTargetGroupResponseTypeDef = TypedDict(
     "CreateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigOutputTypeDef,
+        "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigOutputTypeDef,
+        "config": TargetGroupConfigTypeDef,
         "createdAt": datetime,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
@@ -1836,45 +1701,23 @@
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
-        "config": TargetGroupConfigOutputTypeDef,
+        "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTargetGroupRequestRequestTypeDef",
-    {
-        "name": str,
-        "type": TargetGroupTypeType,
-    },
-)
-_OptionalCreateTargetGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTargetGroupRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "config": TargetGroupConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateTargetGroupRequestRequestTypeDef(
-    _RequiredCreateTargetGroupRequestRequestTypeDef, _OptionalCreateTargetGroupRequestRequestTypeDef
-):
-    pass
-
 RuleMatchOutputTypeDef = TypedDict(
     "RuleMatchOutputTypeDef",
     {
         "httpMatch": HttpMatchOutputTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/PKG-INFO` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.28.12
-Summary: Type annotations for boto3.VPCLattice 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,32 +386,27 @@
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
-    TargetOutputTypeDef,
-    FixedResponseActionOutputTypeDef,
     FixedResponseActionTypeDef,
-    WeightedTargetGroupOutputTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
-    HeaderMatchTypeOutputTypeDef,
     HeaderMatchTypeTypeDef,
-    MatcherOutputTypeDef,
     MatcherTypeDef,
     PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
@@ -421,15 +416,14 @@
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PathMatchTypeOutputTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
@@ -463,17 +457,15 @@
     DeregisterTargetsRequestRequestTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
     ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
-    HeaderMatchOutputTypeDef,
     HeaderMatchTypeDef,
-    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
     ListListenersRequestListListenersPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
@@ -482,34 +474,32 @@
     ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
-    PathMatchOutputTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     RuleActionOutputTypeDef,
     RuleActionTypeDef,
-    TargetGroupConfigOutputTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
     HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
     UpdateListenerResponseTypeDef,
     CreateListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
+    CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
-    CreateTargetGroupRequestRequestTypeDef,
     RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
     UpdateRuleResponseTypeDef,
     CreateRuleRequestRequestTypeDef,
```

### Comparing `mypy-boto3-vpc-lattice-1.28.12/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt` & `mypy-boto3-vpc-lattice-1.28.15/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.28.12/setup.py` & `mypy-boto3-vpc-lattice-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-vpc-lattice",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VPCLattice 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.VPCLattice 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

