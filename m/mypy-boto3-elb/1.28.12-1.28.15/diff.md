# Comparing `tmp/mypy-boto3-elb-1.28.12.tar.gz` & `tmp/mypy-boto3-elb-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elb-1.28.12.tar", last modified: Thu Jul 27 05:34:39 2023, max compression
+gzip compressed data, was "mypy-boto3-elb-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
```

## Comparing `mypy-boto3-elb-1.28.12.tar` & `mypy-boto3-elb-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.908516 mypy-boto3-elb-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-07-27 05:34:39.904516 mypy-boto3-elb-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.904516 mypy-boto3-elb-1.28.12/mypy_boto3_elb/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24903 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-07-27 05:21:53.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27865 2023-07-27 05:21:53.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.904516 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:39.908516 mypy-boto3-elb-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.245075 mypy-boto3-elb-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-07-28 20:42:46.233075 mypy-boto3-elb-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.225075 mypy-boto3-elb-1.28.15/mypy_boto3_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24903 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25023 2023-07-28 20:25:19.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25000 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-28 20:25:18.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.233075 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:46.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:45.000000 mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.245075 mypy-boto3-elb-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-28 20:25:17.000000 mypy-boto3-elb-1.28.15/setup.py
```

### Comparing `mypy-boto3-elb-1.28.12/LICENSE` & `mypy-boto3-elb-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/PKG-INFO` & `mypy-boto3-elb-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elb)](https://pepy.tech/project/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,108 +357,99 @@
 ### Typed dictionaries
 
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
-    AccessLogOutputTypeDef,
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    AdditionalAttributeOutputTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
-    HealthCheckOutputTypeDef,
-    ConnectionDrainingOutputTypeDef,
     ConnectionDrainingTypeDef,
-    ConnectionSettingsOutputTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
-    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
-    CrossZoneLoadBalancingOutputTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    InstanceOutputTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
-    ListenerOutputTypeDef,
     SourceSecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
-    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
-    TagOutputTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
+    CreateAccessPointOutputTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
+    ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
     LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
+    DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
-    DeregisterEndPointsOutputTypeDef,
     RegisterEndPointsOutputTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
-    ListenerDescriptionTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogOutputTypeDef:
+def get_structure() -> AccessLogTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elb-1.28.12/README.md` & `mypy-boto3-elb-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elb)](https://pepy.tech/project/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,108 +325,99 @@
 ### Typed dictionaries
 
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
-    AccessLogOutputTypeDef,
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    AdditionalAttributeOutputTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
-    HealthCheckOutputTypeDef,
-    ConnectionDrainingOutputTypeDef,
     ConnectionDrainingTypeDef,
-    ConnectionSettingsOutputTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
-    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
-    CrossZoneLoadBalancingOutputTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    InstanceOutputTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
-    ListenerOutputTypeDef,
     SourceSecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
-    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
-    TagOutputTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
+    CreateAccessPointOutputTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
+    ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
     LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
+    DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
-    DeregisterEndPointsOutputTypeDef,
     RegisterEndPointsOutputTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
-    ListenerDescriptionTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogOutputTypeDef:
+def get_structure() -> AccessLogTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.py` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.pyi` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/__main__.py` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancing 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancing 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
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

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.py` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.pyi` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.py` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.pyi` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.py` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
         """
 
 
@@ -65,13 +65,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.pyi` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeLoadBalancersPaginator(Paginator):
@@ -61,13 +61,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.py` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,143 +2,112 @@
 Type annotations for elb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elb.type_defs import AccessLogOutputTypeDef
+    from mypy_boto3_elb.type_defs import AccessLogTypeDef
 
-    data: AccessLogOutputTypeDef = {...}
+    data: AccessLogTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
-    "AddAvailabilityZonesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "AdditionalAttributeOutputTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
-    "HealthCheckOutputTypeDef",
-    "ConnectionDrainingOutputTypeDef",
     "ConnectionDrainingTypeDef",
-    "ConnectionSettingsOutputTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
-    "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
-    "CrossZoneLoadBalancingOutputTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
-    "InstanceOutputTypeDef",
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
-    "ListenerOutputTypeDef",
     "SourceSecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
-    "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
-    "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
-    "TagOutputTypeDef",
+    "AddAvailabilityZonesOutputTypeDef",
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    "CreateAccessPointOutputTypeDef",
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    "RemoveAvailabilityZonesOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
+    "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
     "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
+    "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
-    "DeregisterEndPointsOutputTypeDef",
     "RegisterEndPointsOutputTypeDef",
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
-    "ListenerDescriptionTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "TagDescriptionTypeDef",
+    "DescribeTagsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
-    "DescribeTagsOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
-_RequiredAccessLogOutputTypeDef = TypedDict(
-    "_RequiredAccessLogOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalAccessLogOutputTypeDef = TypedDict(
-    "_OptionalAccessLogOutputTypeDef",
-    {
-        "S3BucketName": str,
-        "EmitInterval": int,
-        "S3BucketPrefix": str,
-    },
-    total=False,
-)
-
-
-class AccessLogOutputTypeDef(_RequiredAccessLogOutputTypeDef, _OptionalAccessLogOutputTypeDef):
-    pass
-
-
 _RequiredAccessLogTypeDef = TypedDict(
     "_RequiredAccessLogTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAccessLogTypeDef = TypedDict(
@@ -147,32 +116,33 @@
         "S3BucketName": str,
         "EmitInterval": int,
         "S3BucketPrefix": str,
     },
     total=False,
 )
 
-
 class AccessLogTypeDef(_RequiredAccessLogTypeDef, _OptionalAccessLogTypeDef):
     pass
 
-
 AddAvailabilityZonesInputRequestTypeDef = TypedDict(
     "AddAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-AddAvailabilityZonesOutputTypeDef = TypedDict(
-    "AddAvailabilityZonesOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
@@ -182,28 +152,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
-AdditionalAttributeOutputTypeDef = TypedDict(
-    "AdditionalAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AdditionalAttributeTypeDef = TypedDict(
     "AdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -222,38 +181,22 @@
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachLoadBalancerToSubnetsInputRequestTypeDef = TypedDict(
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackendServerDescriptionTypeDef = TypedDict(
     "BackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
     total=False,
@@ -266,74 +209,33 @@
         "Interval": int,
         "Timeout": int,
         "UnhealthyThreshold": int,
         "HealthyThreshold": int,
     },
 )
 
-HealthCheckOutputTypeDef = TypedDict(
-    "HealthCheckOutputTypeDef",
-    {
-        "Target": str,
-        "Interval": int,
-        "Timeout": int,
-        "UnhealthyThreshold": int,
-        "HealthyThreshold": int,
-    },
-)
-
-_RequiredConnectionDrainingOutputTypeDef = TypedDict(
-    "_RequiredConnectionDrainingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalConnectionDrainingOutputTypeDef = TypedDict(
-    "_OptionalConnectionDrainingOutputTypeDef",
-    {
-        "Timeout": int,
-    },
-    total=False,
-)
-
-
-class ConnectionDrainingOutputTypeDef(
-    _RequiredConnectionDrainingOutputTypeDef, _OptionalConnectionDrainingOutputTypeDef
-):
-    pass
-
-
 _RequiredConnectionDrainingTypeDef = TypedDict(
     "_RequiredConnectionDrainingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalConnectionDrainingTypeDef = TypedDict(
     "_OptionalConnectionDrainingTypeDef",
     {
         "Timeout": int,
     },
     total=False,
 )
 
-
 class ConnectionDrainingTypeDef(
     _RequiredConnectionDrainingTypeDef, _OptionalConnectionDrainingTypeDef
 ):
     pass
 
-
-ConnectionSettingsOutputTypeDef = TypedDict(
-    "ConnectionSettingsOutputTypeDef",
-    {
-        "IdleTimeout": int,
-    },
-)
-
 ConnectionSettingsTypeDef = TypedDict(
     "ConnectionSettingsTypeDef",
     {
         "IdleTimeout": int,
     },
 )
 
@@ -350,27 +252,17 @@
     {
         "InstanceProtocol": str,
         "SSLCertificateId": str,
     },
     total=False,
 )
 
-
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
-
-CreateAccessPointOutputTypeDef = TypedDict(
-    "CreateAccessPointOutputTypeDef",
-    {
-        "DNSName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAppCookieStickinessPolicyInputRequestTypeDef = TypedDict(
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "CookieName": str,
     },
@@ -387,38 +279,29 @@
     "_OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef",
     {
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
-
 class CreateLBCookieStickinessPolicyInputRequestTypeDef(
     _RequiredCreateLBCookieStickinessPolicyInputRequestTypeDef,
     _OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef,
 ):
     pass
 
-
 PolicyAttributeTypeDef = TypedDict(
     "PolicyAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
 )
 
-CrossZoneLoadBalancingOutputTypeDef = TypedDict(
-    "CrossZoneLoadBalancingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-
 CrossZoneLoadBalancingTypeDef = TypedDict(
     "CrossZoneLoadBalancingTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -449,49 +332,34 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-InstanceOutputTypeDef = TypedDict(
-    "InstanceOutputTypeDef",
-    {
-        "InstanceId": str,
-    },
-    total=False,
-)
-
-DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LoadBalancerNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccessPointsInputRequestTypeDef = TypedDict(
     "DescribeAccessPointsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
@@ -561,72 +429,32 @@
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LBCookieStickinessPolicyTypeDef = TypedDict(
     "LBCookieStickinessPolicyTypeDef",
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
-_RequiredListenerOutputTypeDef = TypedDict(
-    "_RequiredListenerOutputTypeDef",
-    {
-        "Protocol": str,
-        "LoadBalancerPort": int,
-        "InstancePort": int,
-    },
-)
-_OptionalListenerOutputTypeDef = TypedDict(
-    "_OptionalListenerOutputTypeDef",
-    {
-        "InstanceProtocol": str,
-        "SSLCertificateId": str,
-    },
-    total=False,
-)
-
-
-class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
-    pass
-
-
 SourceSecurityGroupTypeDef = TypedDict(
     "SourceSecurityGroupTypeDef",
     {
         "OwnerAlias": str,
         "GroupName": str,
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
 PolicyAttributeDescriptionTypeDef = TypedDict(
     "PolicyAttributeDescriptionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -648,41 +476,22 @@
     "RemoveAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-RemoveAvailabilityZonesOutputTypeDef = TypedDict(
-    "RemoveAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagKeyOnlyTypeDef = TypedDict(
     "TagKeyOnlyTypeDef",
     {
         "Key": str,
     },
     total=False,
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
 SetLoadBalancerListenerSSLCertificateInputRequestTypeDef = TypedDict(
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "SSLCertificateId": str,
     },
@@ -702,54 +511,92 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
+AddAvailabilityZonesOutputTypeDef = TypedDict(
+    "AddAvailabilityZonesOutputTypeDef",
     {
-        "Key": str,
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
+
+ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     {
-        "Value": str,
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
+CreateAccessPointOutputTypeDef = TypedDict(
+    "CreateAccessPointOutputTypeDef",
+    {
+        "DNSName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAvailabilityZonesOutputTypeDef = TypedDict(
+    "RemoveAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
+    {
+        "LoadBalancerName": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 ConfigureHealthCheckInputRequestTypeDef = TypedDict(
     "ConfigureHealthCheckInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "HealthCheck": HealthCheckTypeDef,
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
-        "HealthCheck": HealthCheckOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "HealthCheck": HealthCheckTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -764,29 +611,36 @@
         "SecurityGroups": Sequence[str],
         "Scheme": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateAccessPointInputRequestTypeDef(
     _RequiredCreateAccessPointInputRequestTypeDef, _OptionalCreateAccessPointInputRequestTypeDef
 ):
     pass
 
-
 CreateLoadBalancerListenerInputRequestTypeDef = TypedDict(
     "CreateLoadBalancerListenerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Listeners": Sequence[ListenerTypeDef],
     },
 )
 
+ListenerDescriptionTypeDef = TypedDict(
+    "ListenerDescriptionTypeDef",
+    {
+        "Listener": ListenerTypeDef,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 _RequiredCreateLoadBalancerPolicyInputRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "PolicyTypeName": str,
     },
@@ -795,30 +649,28 @@
     "_OptionalCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "PolicyAttributes": Sequence[PolicyAttributeTypeDef],
     },
     total=False,
 )
 
-
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
-
 LoadBalancerAttributesOutputTypeDef = TypedDict(
     "LoadBalancerAttributesOutputTypeDef",
     {
-        "CrossZoneLoadBalancing": CrossZoneLoadBalancingOutputTypeDef,
-        "AccessLog": AccessLogOutputTypeDef,
-        "ConnectionDraining": ConnectionDrainingOutputTypeDef,
-        "ConnectionSettings": ConnectionSettingsOutputTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeOutputTypeDef],
+        "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
+        "AccessLog": AccessLogTypeDef,
+        "ConnectionDraining": ConnectionDrainingTypeDef,
+        "ConnectionSettings": ConnectionSettingsTypeDef,
+        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
@@ -835,66 +687,81 @@
     "DeregisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
+DeregisterEndPointsOutputTypeDef = TypedDict(
+    "DeregisterEndPointsOutputTypeDef",
+    {
+        "Instances": List[InstanceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_OptionalDescribeEndPointStateInputRequestTypeDef",
     {
         "Instances": Sequence[InstanceTypeDef],
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputRequestTypeDef(
     _RequiredDescribeEndPointStateInputRequestTypeDef,
     _OptionalDescribeEndPointStateInputRequestTypeDef,
 ):
     pass
 
-
 RegisterEndPointsInputRequestTypeDef = TypedDict(
     "RegisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
-DeregisterEndPointsOutputTypeDef = TypedDict(
-    "DeregisterEndPointsOutputTypeDef",
+RegisterEndPointsOutputTypeDef = TypedDict(
+    "RegisterEndPointsOutputTypeDef",
     {
-        "Instances": List[InstanceOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Instances": List[InstanceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RegisterEndPointsOutputTypeDef = TypedDict(
-    "RegisterEndPointsOutputTypeDef",
+DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
-        "Instances": List[InstanceOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
@@ -905,22 +772,20 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
@@ -928,22 +793,20 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
@@ -951,49 +814,38 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
 ):
     pass
 
-
 DescribeEndPointStateOutputTypeDef = TypedDict(
     "DescribeEndPointStateOutputTypeDef",
     {
         "InstanceStates": List[InstanceStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeDef = TypedDict(
     "PoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
         "LBCookieStickinessPolicies": List[LBCookieStickinessPolicyTypeDef],
         "OtherPolicies": List[str],
     },
     total=False,
 )
 
-ListenerDescriptionTypeDef = TypedDict(
-    "ListenerDescriptionTypeDef",
-    {
-        "Listener": ListenerOutputTypeDef,
-        "PolicyNames": List[str],
-    },
-    total=False,
-)
-
 PolicyDescriptionTypeDef = TypedDict(
     "PolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "PolicyTypeName": str,
         "PolicyAttributeDescriptions": List[PolicyAttributeDescriptionTypeDef],
     },
@@ -1014,37 +866,36 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagKeyOnlyTypeDef],
     },
 )
 
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
     {
-        "LoadBalancerName": str,
-        "Tags": List[TagOutputTypeDef],
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -1061,49 +912,41 @@
         "CanonicalHostedZoneNameID": str,
         "ListenerDescriptions": List[ListenerDescriptionTypeDef],
         "Policies": PoliciesTypeDef,
         "BackendServerDescriptions": List[BackendServerDescriptionTypeDef],
         "AvailabilityZones": List[str],
         "Subnets": List[str],
         "VPCId": str,
-        "Instances": List[InstanceOutputTypeDef],
-        "HealthCheck": HealthCheckOutputTypeDef,
+        "Instances": List[InstanceTypeDef],
+        "HealthCheck": HealthCheckTypeDef,
         "SourceSecurityGroup": SourceSecurityGroupTypeDef,
         "SecurityGroups": List[str],
         "CreatedTime": datetime,
         "Scheme": str,
     },
     total=False,
 )
 
 DescribeLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     {
         "PolicyDescriptions": List[PolicyDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerPolicyTypesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
-    {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.pyi` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,140 +2,113 @@
 Type annotations for elb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elb.type_defs import AccessLogOutputTypeDef
+    from mypy_boto3_elb.type_defs import AccessLogTypeDef
 
-    data: AccessLogOutputTypeDef = {...}
+    data: AccessLogTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
-    "AddAvailabilityZonesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "AdditionalAttributeOutputTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
-    "HealthCheckOutputTypeDef",
-    "ConnectionDrainingOutputTypeDef",
     "ConnectionDrainingTypeDef",
-    "ConnectionSettingsOutputTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
-    "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
-    "CrossZoneLoadBalancingOutputTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
-    "InstanceOutputTypeDef",
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
-    "ListenerOutputTypeDef",
     "SourceSecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
-    "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
-    "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
-    "TagOutputTypeDef",
+    "AddAvailabilityZonesOutputTypeDef",
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    "CreateAccessPointOutputTypeDef",
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    "RemoveAvailabilityZonesOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
+    "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
     "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
+    "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
-    "DeregisterEndPointsOutputTypeDef",
     "RegisterEndPointsOutputTypeDef",
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
-    "ListenerDescriptionTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "TagDescriptionTypeDef",
+    "DescribeTagsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
-    "DescribeTagsOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
-_RequiredAccessLogOutputTypeDef = TypedDict(
-    "_RequiredAccessLogOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalAccessLogOutputTypeDef = TypedDict(
-    "_OptionalAccessLogOutputTypeDef",
-    {
-        "S3BucketName": str,
-        "EmitInterval": int,
-        "S3BucketPrefix": str,
-    },
-    total=False,
-)
-
-class AccessLogOutputTypeDef(_RequiredAccessLogOutputTypeDef, _OptionalAccessLogOutputTypeDef):
-    pass
-
 _RequiredAccessLogTypeDef = TypedDict(
     "_RequiredAccessLogTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAccessLogTypeDef = TypedDict(
@@ -144,30 +117,35 @@
         "S3BucketName": str,
         "EmitInterval": int,
         "S3BucketPrefix": str,
     },
     total=False,
 )
 
+
 class AccessLogTypeDef(_RequiredAccessLogTypeDef, _OptionalAccessLogTypeDef):
     pass
 
+
 AddAvailabilityZonesInputRequestTypeDef = TypedDict(
     "AddAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-AddAvailabilityZonesOutputTypeDef = TypedDict(
-    "AddAvailabilityZonesOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
@@ -177,25 +155,18 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-AdditionalAttributeOutputTypeDef = TypedDict(
-    "AdditionalAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
 
 AdditionalAttributeTypeDef = TypedDict(
     "AdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
@@ -215,38 +186,22 @@
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachLoadBalancerToSubnetsInputRequestTypeDef = TypedDict(
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackendServerDescriptionTypeDef = TypedDict(
     "BackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
     total=False,
@@ -259,69 +214,34 @@
         "Interval": int,
         "Timeout": int,
         "UnhealthyThreshold": int,
         "HealthyThreshold": int,
     },
 )
 
-HealthCheckOutputTypeDef = TypedDict(
-    "HealthCheckOutputTypeDef",
-    {
-        "Target": str,
-        "Interval": int,
-        "Timeout": int,
-        "UnhealthyThreshold": int,
-        "HealthyThreshold": int,
-    },
-)
-
-_RequiredConnectionDrainingOutputTypeDef = TypedDict(
-    "_RequiredConnectionDrainingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalConnectionDrainingOutputTypeDef = TypedDict(
-    "_OptionalConnectionDrainingOutputTypeDef",
-    {
-        "Timeout": int,
-    },
-    total=False,
-)
-
-class ConnectionDrainingOutputTypeDef(
-    _RequiredConnectionDrainingOutputTypeDef, _OptionalConnectionDrainingOutputTypeDef
-):
-    pass
-
 _RequiredConnectionDrainingTypeDef = TypedDict(
     "_RequiredConnectionDrainingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalConnectionDrainingTypeDef = TypedDict(
     "_OptionalConnectionDrainingTypeDef",
     {
         "Timeout": int,
     },
     total=False,
 )
 
+
 class ConnectionDrainingTypeDef(
     _RequiredConnectionDrainingTypeDef, _OptionalConnectionDrainingTypeDef
 ):
     pass
 
-ConnectionSettingsOutputTypeDef = TypedDict(
-    "ConnectionSettingsOutputTypeDef",
-    {
-        "IdleTimeout": int,
-    },
-)
 
 ConnectionSettingsTypeDef = TypedDict(
     "ConnectionSettingsTypeDef",
     {
         "IdleTimeout": int,
     },
 )
@@ -339,24 +259,18 @@
     {
         "InstanceProtocol": str,
         "SSLCertificateId": str,
     },
     total=False,
 )
 
+
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
-CreateAccessPointOutputTypeDef = TypedDict(
-    "CreateAccessPointOutputTypeDef",
-    {
-        "DNSName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateAppCookieStickinessPolicyInputRequestTypeDef = TypedDict(
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "CookieName": str,
@@ -374,36 +288,31 @@
     "_OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef",
     {
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
+
 class CreateLBCookieStickinessPolicyInputRequestTypeDef(
     _RequiredCreateLBCookieStickinessPolicyInputRequestTypeDef,
     _OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef,
 ):
     pass
 
+
 PolicyAttributeTypeDef = TypedDict(
     "PolicyAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
 )
 
-CrossZoneLoadBalancingOutputTypeDef = TypedDict(
-    "CrossZoneLoadBalancingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-
 CrossZoneLoadBalancingTypeDef = TypedDict(
     "CrossZoneLoadBalancingTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -434,49 +343,34 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-InstanceOutputTypeDef = TypedDict(
-    "InstanceOutputTypeDef",
-    {
-        "InstanceId": str,
-    },
-    total=False,
-)
-
-DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LoadBalancerNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccessPointsInputRequestTypeDef = TypedDict(
     "DescribeAccessPointsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
@@ -546,70 +440,32 @@
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LBCookieStickinessPolicyTypeDef = TypedDict(
     "LBCookieStickinessPolicyTypeDef",
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
-_RequiredListenerOutputTypeDef = TypedDict(
-    "_RequiredListenerOutputTypeDef",
-    {
-        "Protocol": str,
-        "LoadBalancerPort": int,
-        "InstancePort": int,
-    },
-)
-_OptionalListenerOutputTypeDef = TypedDict(
-    "_OptionalListenerOutputTypeDef",
-    {
-        "InstanceProtocol": str,
-        "SSLCertificateId": str,
-    },
-    total=False,
-)
-
-class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
-    pass
-
 SourceSecurityGroupTypeDef = TypedDict(
     "SourceSecurityGroupTypeDef",
     {
         "OwnerAlias": str,
         "GroupName": str,
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
 PolicyAttributeDescriptionTypeDef = TypedDict(
     "PolicyAttributeDescriptionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -631,41 +487,22 @@
     "RemoveAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-RemoveAvailabilityZonesOutputTypeDef = TypedDict(
-    "RemoveAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagKeyOnlyTypeDef = TypedDict(
     "TagKeyOnlyTypeDef",
     {
         "Key": str,
     },
     total=False,
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
 SetLoadBalancerListenerSSLCertificateInputRequestTypeDef = TypedDict(
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "SSLCertificateId": str,
     },
@@ -685,52 +522,92 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
+AddAvailabilityZonesOutputTypeDef = TypedDict(
+    "AddAvailabilityZonesOutputTypeDef",
     {
-        "Key": str,
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
+
+ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     {
-        "Value": str,
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
+AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAccessPointOutputTypeDef = TypedDict(
+    "CreateAccessPointOutputTypeDef",
+    {
+        "DNSName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAvailabilityZonesOutputTypeDef = TypedDict(
+    "RemoveAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
+    {
+        "LoadBalancerName": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 ConfigureHealthCheckInputRequestTypeDef = TypedDict(
     "ConfigureHealthCheckInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "HealthCheck": HealthCheckTypeDef,
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
-        "HealthCheck": HealthCheckOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "HealthCheck": HealthCheckTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -745,27 +622,38 @@
         "SecurityGroups": Sequence[str],
         "Scheme": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateAccessPointInputRequestTypeDef(
     _RequiredCreateAccessPointInputRequestTypeDef, _OptionalCreateAccessPointInputRequestTypeDef
 ):
     pass
 
+
 CreateLoadBalancerListenerInputRequestTypeDef = TypedDict(
     "CreateLoadBalancerListenerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Listeners": Sequence[ListenerTypeDef],
     },
 )
 
+ListenerDescriptionTypeDef = TypedDict(
+    "ListenerDescriptionTypeDef",
+    {
+        "Listener": ListenerTypeDef,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 _RequiredCreateLoadBalancerPolicyInputRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "PolicyTypeName": str,
     },
@@ -774,28 +662,30 @@
     "_OptionalCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "PolicyAttributes": Sequence[PolicyAttributeTypeDef],
     },
     total=False,
 )
 
+
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
+
 LoadBalancerAttributesOutputTypeDef = TypedDict(
     "LoadBalancerAttributesOutputTypeDef",
     {
-        "CrossZoneLoadBalancing": CrossZoneLoadBalancingOutputTypeDef,
-        "AccessLog": AccessLogOutputTypeDef,
-        "ConnectionDraining": ConnectionDrainingOutputTypeDef,
-        "ConnectionSettings": ConnectionSettingsOutputTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeOutputTypeDef],
+        "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
+        "AccessLog": AccessLogTypeDef,
+        "ConnectionDraining": ConnectionDrainingTypeDef,
+        "ConnectionSettings": ConnectionSettingsTypeDef,
+        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
@@ -812,64 +702,83 @@
     "DeregisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
+DeregisterEndPointsOutputTypeDef = TypedDict(
+    "DeregisterEndPointsOutputTypeDef",
+    {
+        "Instances": List[InstanceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_OptionalDescribeEndPointStateInputRequestTypeDef",
     {
         "Instances": Sequence[InstanceTypeDef],
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputRequestTypeDef(
     _RequiredDescribeEndPointStateInputRequestTypeDef,
     _OptionalDescribeEndPointStateInputRequestTypeDef,
 ):
     pass
 
+
 RegisterEndPointsInputRequestTypeDef = TypedDict(
     "RegisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
-DeregisterEndPointsOutputTypeDef = TypedDict(
-    "DeregisterEndPointsOutputTypeDef",
+RegisterEndPointsOutputTypeDef = TypedDict(
+    "RegisterEndPointsOutputTypeDef",
     {
-        "Instances": List[InstanceOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Instances": List[InstanceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RegisterEndPointsOutputTypeDef = TypedDict(
-    "RegisterEndPointsOutputTypeDef",
+DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     {
-        "Instances": List[InstanceOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoadBalancerNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
@@ -880,20 +789,22 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
@@ -901,20 +812,22 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
@@ -922,47 +835,40 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
 ):
     pass
 
+
 DescribeEndPointStateOutputTypeDef = TypedDict(
     "DescribeEndPointStateOutputTypeDef",
     {
         "InstanceStates": List[InstanceStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeDef = TypedDict(
     "PoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
         "LBCookieStickinessPolicies": List[LBCookieStickinessPolicyTypeDef],
         "OtherPolicies": List[str],
     },
     total=False,
 )
 
-ListenerDescriptionTypeDef = TypedDict(
-    "ListenerDescriptionTypeDef",
-    {
-        "Listener": ListenerOutputTypeDef,
-        "PolicyNames": List[str],
-    },
-    total=False,
-)
-
 PolicyDescriptionTypeDef = TypedDict(
     "PolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "PolicyTypeName": str,
         "PolicyAttributeDescriptions": List[PolicyAttributeDescriptionTypeDef],
     },
@@ -983,37 +889,36 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagKeyOnlyTypeDef],
     },
 )
 
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
     {
-        "LoadBalancerName": str,
-        "Tags": List[TagOutputTypeDef],
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -1030,49 +935,41 @@
         "CanonicalHostedZoneNameID": str,
         "ListenerDescriptions": List[ListenerDescriptionTypeDef],
         "Policies": PoliciesTypeDef,
         "BackendServerDescriptions": List[BackendServerDescriptionTypeDef],
         "AvailabilityZones": List[str],
         "Subnets": List[str],
         "VPCId": str,
-        "Instances": List[InstanceOutputTypeDef],
-        "HealthCheck": HealthCheckOutputTypeDef,
+        "Instances": List[InstanceTypeDef],
+        "HealthCheck": HealthCheckTypeDef,
         "SourceSecurityGroup": SourceSecurityGroupTypeDef,
         "SecurityGroups": List[str],
         "CreatedTime": datetime,
         "Scheme": str,
     },
     total=False,
 )
 
 DescribeLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     {
         "PolicyDescriptions": List[PolicyDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerPolicyTypesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
-    {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.py` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.pyi` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/PKG-INFO` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elb)](https://pepy.tech/project/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,108 +357,99 @@
 ### Typed dictionaries
 
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
-    AccessLogOutputTypeDef,
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    AdditionalAttributeOutputTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
-    HealthCheckOutputTypeDef,
-    ConnectionDrainingOutputTypeDef,
     ConnectionDrainingTypeDef,
-    ConnectionSettingsOutputTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
-    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
-    CrossZoneLoadBalancingOutputTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    InstanceOutputTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
-    ListenerOutputTypeDef,
     SourceSecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
-    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
-    TagOutputTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
+    CreateAccessPointOutputTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
+    ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
     LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
+    DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
-    DeregisterEndPointsOutputTypeDef,
     RegisterEndPointsOutputTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
-    ListenerDescriptionTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
-    DescribeTagsOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogOutputTypeDef:
+def get_structure() -> AccessLogTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/SOURCES.txt` & `mypy-boto3-elb-1.28.15/mypy_boto3_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.12/setup.py` & `mypy-boto3-elb-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elb",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticLoadBalancing 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ElasticLoadBalancing 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

