# Comparing `tmp/mypy-boto3-apprunner-1.28.12.tar.gz` & `tmp/mypy-boto3-apprunner-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apprunner-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-apprunner-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-apprunner-1.28.12.tar` & `mypy-boto3-apprunner-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.516577 mypy-boto3-apprunner-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-07-27 05:34:18.504577 mypy-boto3-apprunner-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.504577 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41889 2023-07-27 05:17:33.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41844 2023-07-27 05:17:33.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.504577 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.516577 mypy-boto3-apprunner-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.172694 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-28 20:19:34.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38636 2023-07-28 20:19:35.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-07-28 20:19:35.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:18.000000 mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.180694 mypy-boto3-apprunner-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:19:33.000000 mypy-boto3-apprunner-1.28.15/setup.py
```

### Comparing `mypy-boto3-apprunner-1.28.12/LICENSE` & `mypy-boto3-apprunner-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.12/PKG-INFO` & `mypy-boto3-apprunner-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.28.12
-Summary: Type annotations for boto3.AppRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,23 +314,22 @@
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
-    AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
     CodeConfigurationValuesOutputTypeDef,
     CodeConfigurationValuesTypeDef,
-    SourceCodeVersionOutputTypeDef,
     SourceCodeVersionTypeDef,
     ConnectionSummaryTypeDef,
     ConnectionTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HealthCheckConfigurationTypeDef,
@@ -347,90 +346,79 @@
     DescribeAutoScalingConfigurationRequestRequestTypeDef,
     DescribeCustomDomainsRequestRequestTypeDef,
     DescribeObservabilityConfigurationRequestRequestTypeDef,
     DescribeServiceRequestRequestTypeDef,
     DescribeVpcConnectorRequestRequestTypeDef,
     DescribeVpcIngressConnectionRequestRequestTypeDef,
     DisassociateCustomDomainRequestRequestTypeDef,
-    EgressConfigurationOutputTypeDef,
     EgressConfigurationTypeDef,
-    EncryptionConfigurationOutputTypeDef,
-    HealthCheckConfigurationOutputTypeDef,
     ImageConfigurationOutputTypeDef,
     ImageConfigurationTypeDef,
-    IngressConfigurationOutputTypeDef,
     IngressConfigurationTypeDef,
-    IngressVpcConfigurationOutputTypeDef,
-    InstanceConfigurationOutputTypeDef,
     ListAutoScalingConfigurationsRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListObservabilityConfigurationsRequestRequestTypeDef,
     ObservabilityConfigurationSummaryTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
-    TraceConfigurationOutputTypeDef,
     PauseServiceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
-    ServiceObservabilityConfigurationOutputTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartDeploymentResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    StartDeploymentResponseTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
     CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
     CreateConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     CreateAutoScalingConfigurationRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateVpcConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateObservabilityConfigurationRequestRequestTypeDef,
+    ObservabilityConfigurationTypeDef,
     CreateVpcConnectorResponseTypeDef,
     DeleteVpcConnectorResponseTypeDef,
     DescribeVpcConnectorResponseTypeDef,
     ListVpcConnectorsResponseTypeDef,
     CreateVpcIngressConnectionRequestRequestTypeDef,
     UpdateVpcIngressConnectionRequestRequestTypeDef,
+    VpcIngressConnectionTypeDef,
     ImageRepositoryOutputTypeDef,
     ImageRepositoryTypeDef,
-    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
-    VpcIngressConnectionTypeDef,
     ListObservabilityConfigurationsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVpcIngressConnectionsRequestRequestTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
-    ObservabilityConfigurationTypeDef,
     AssociateCustomDomainResponseTypeDef,
     DescribeCustomDomainsResponseTypeDef,
     DisassociateCustomDomainResponseTypeDef,
     CodeRepositoryOutputTypeDef,
     CodeRepositoryTypeDef,
+    CreateObservabilityConfigurationResponseTypeDef,
+    DeleteObservabilityConfigurationResponseTypeDef,
+    DescribeObservabilityConfigurationResponseTypeDef,
     CreateVpcIngressConnectionResponseTypeDef,
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
-    CreateObservabilityConfigurationResponseTypeDef,
-    DeleteObservabilityConfigurationResponseTypeDef,
-    DescribeObservabilityConfigurationResponseTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
```

### Comparing `mypy-boto3-apprunner-1.28.12/README.md` & `mypy-boto3-apprunner-1.28.15/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,23 +282,22 @@
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
-    AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
     CodeConfigurationValuesOutputTypeDef,
     CodeConfigurationValuesTypeDef,
-    SourceCodeVersionOutputTypeDef,
     SourceCodeVersionTypeDef,
     ConnectionSummaryTypeDef,
     ConnectionTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HealthCheckConfigurationTypeDef,
@@ -315,90 +314,79 @@
     DescribeAutoScalingConfigurationRequestRequestTypeDef,
     DescribeCustomDomainsRequestRequestTypeDef,
     DescribeObservabilityConfigurationRequestRequestTypeDef,
     DescribeServiceRequestRequestTypeDef,
     DescribeVpcConnectorRequestRequestTypeDef,
     DescribeVpcIngressConnectionRequestRequestTypeDef,
     DisassociateCustomDomainRequestRequestTypeDef,
-    EgressConfigurationOutputTypeDef,
     EgressConfigurationTypeDef,
-    EncryptionConfigurationOutputTypeDef,
-    HealthCheckConfigurationOutputTypeDef,
     ImageConfigurationOutputTypeDef,
     ImageConfigurationTypeDef,
-    IngressConfigurationOutputTypeDef,
     IngressConfigurationTypeDef,
-    IngressVpcConfigurationOutputTypeDef,
-    InstanceConfigurationOutputTypeDef,
     ListAutoScalingConfigurationsRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListObservabilityConfigurationsRequestRequestTypeDef,
     ObservabilityConfigurationSummaryTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
-    TraceConfigurationOutputTypeDef,
     PauseServiceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
-    ServiceObservabilityConfigurationOutputTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartDeploymentResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    StartDeploymentResponseTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
     CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
     CreateConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     CreateAutoScalingConfigurationRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateVpcConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateObservabilityConfigurationRequestRequestTypeDef,
+    ObservabilityConfigurationTypeDef,
     CreateVpcConnectorResponseTypeDef,
     DeleteVpcConnectorResponseTypeDef,
     DescribeVpcConnectorResponseTypeDef,
     ListVpcConnectorsResponseTypeDef,
     CreateVpcIngressConnectionRequestRequestTypeDef,
     UpdateVpcIngressConnectionRequestRequestTypeDef,
+    VpcIngressConnectionTypeDef,
     ImageRepositoryOutputTypeDef,
     ImageRepositoryTypeDef,
-    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
-    VpcIngressConnectionTypeDef,
     ListObservabilityConfigurationsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVpcIngressConnectionsRequestRequestTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
-    ObservabilityConfigurationTypeDef,
     AssociateCustomDomainResponseTypeDef,
     DescribeCustomDomainsResponseTypeDef,
     DisassociateCustomDomainResponseTypeDef,
     CodeRepositoryOutputTypeDef,
     CodeRepositoryTypeDef,
+    CreateObservabilityConfigurationResponseTypeDef,
+    DeleteObservabilityConfigurationResponseTypeDef,
+    DescribeObservabilityConfigurationResponseTypeDef,
     CreateVpcIngressConnectionResponseTypeDef,
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
-    CreateObservabilityConfigurationResponseTypeDef,
-    DeleteObservabilityConfigurationResponseTypeDef,
-    DescribeObservabilityConfigurationResponseTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
```

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__main__.py` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRunner 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppRunner 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
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

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.py` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.pyi` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.py` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.pyi` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.py` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,22 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcDNSTargetTypeDef",
-    "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
     "CertificateValidationRecordTypeDef",
     "CodeConfigurationValuesOutputTypeDef",
     "CodeConfigurationValuesTypeDef",
-    "SourceCodeVersionOutputTypeDef",
     "SourceCodeVersionTypeDef",
     "ConnectionSummaryTypeDef",
     "ConnectionTypeDef",
     "TagTypeDef",
     "TraceConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
     "HealthCheckConfigurationTypeDef",
@@ -74,90 +73,79 @@
     "DescribeAutoScalingConfigurationRequestRequestTypeDef",
     "DescribeCustomDomainsRequestRequestTypeDef",
     "DescribeObservabilityConfigurationRequestRequestTypeDef",
     "DescribeServiceRequestRequestTypeDef",
     "DescribeVpcConnectorRequestRequestTypeDef",
     "DescribeVpcIngressConnectionRequestRequestTypeDef",
     "DisassociateCustomDomainRequestRequestTypeDef",
-    "EgressConfigurationOutputTypeDef",
     "EgressConfigurationTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
-    "HealthCheckConfigurationOutputTypeDef",
     "ImageConfigurationOutputTypeDef",
     "ImageConfigurationTypeDef",
-    "IngressConfigurationOutputTypeDef",
     "IngressConfigurationTypeDef",
-    "IngressVpcConfigurationOutputTypeDef",
-    "InstanceConfigurationOutputTypeDef",
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListObservabilityConfigurationsRequestRequestTypeDef",
     "ObservabilityConfigurationSummaryTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListVpcConnectorsRequestRequestTypeDef",
     "ListVpcIngressConnectionsFilterTypeDef",
     "VpcIngressConnectionSummaryTypeDef",
-    "TraceConfigurationOutputTypeDef",
     "PauseServiceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeServiceRequestRequestTypeDef",
-    "ServiceObservabilityConfigurationOutputTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "StartDeploymentResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "StartDeploymentResponseTypeDef",
     "ListAutoScalingConfigurationsResponseTypeDef",
     "CreateAutoScalingConfigurationResponseTypeDef",
     "DeleteAutoScalingConfigurationResponseTypeDef",
     "DescribeAutoScalingConfigurationResponseTypeDef",
     "CustomDomainTypeDef",
     "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateConnectionResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "CreateAutoScalingConfigurationRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateVpcConnectorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateObservabilityConfigurationRequestRequestTypeDef",
+    "ObservabilityConfigurationTypeDef",
     "CreateVpcConnectorResponseTypeDef",
     "DeleteVpcConnectorResponseTypeDef",
     "DescribeVpcConnectorResponseTypeDef",
     "ListVpcConnectorsResponseTypeDef",
     "CreateVpcIngressConnectionRequestRequestTypeDef",
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
+    "VpcIngressConnectionTypeDef",
     "ImageRepositoryOutputTypeDef",
     "ImageRepositoryTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
-    "VpcIngressConnectionTypeDef",
     "ListObservabilityConfigurationsResponseTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     "ListVpcIngressConnectionsResponseTypeDef",
-    "ObservabilityConfigurationTypeDef",
     "AssociateCustomDomainResponseTypeDef",
     "DescribeCustomDomainsResponseTypeDef",
     "DisassociateCustomDomainResponseTypeDef",
     "CodeRepositoryOutputTypeDef",
     "CodeRepositoryTypeDef",
+    "CreateObservabilityConfigurationResponseTypeDef",
+    "DeleteObservabilityConfigurationResponseTypeDef",
+    "DescribeObservabilityConfigurationResponseTypeDef",
     "CreateVpcIngressConnectionResponseTypeDef",
     "DeleteVpcIngressConnectionResponseTypeDef",
     "DescribeVpcIngressConnectionResponseTypeDef",
     "UpdateVpcIngressConnectionResponseTypeDef",
-    "CreateObservabilityConfigurationResponseTypeDef",
-    "DeleteObservabilityConfigurationResponseTypeDef",
-    "DescribeObservabilityConfigurationResponseTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "ServiceTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
@@ -186,33 +174,35 @@
 class AssociateCustomDomainRequestRequestTypeDef(
     _RequiredAssociateCustomDomainRequestRequestTypeDef,
     _OptionalAssociateCustomDomainRequestRequestTypeDef,
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
 VpcDNSTargetTypeDef = TypedDict(
     "VpcDNSTargetTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "VpcId": str,
         "DomainName": str,
     },
     total=False,
 )
 
-AuthenticationConfigurationOutputTypeDef = TypedDict(
-    "AuthenticationConfigurationOutputTypeDef",
-    {
-        "ConnectionArn": str,
-        "AccessRoleArn": str,
-    },
-    total=False,
-)
-
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "ConnectionArn": str,
         "AccessRoleArn": str,
     },
     total=False,
@@ -302,22 +292,14 @@
 
 class CodeConfigurationValuesTypeDef(
     _RequiredCodeConfigurationValuesTypeDef, _OptionalCodeConfigurationValuesTypeDef
 ):
     pass
 
 
-SourceCodeVersionOutputTypeDef = TypedDict(
-    "SourceCodeVersionOutputTypeDef",
-    {
-        "Type": Literal["BRANCH"],
-        "Value": str,
-    },
-)
-
 SourceCodeVersionTypeDef = TypedDict(
     "SourceCodeVersionTypeDef",
     {
         "Type": Literal["BRANCH"],
         "Value": str,
     },
 )
@@ -542,52 +524,23 @@
     "DisassociateCustomDomainRequestRequestTypeDef",
     {
         "ServiceArn": str,
         "DomainName": str,
     },
 )
 
-EgressConfigurationOutputTypeDef = TypedDict(
-    "EgressConfigurationOutputTypeDef",
-    {
-        "EgressType": EgressTypeType,
-        "VpcConnectorArn": str,
-    },
-    total=False,
-)
-
 EgressConfigurationTypeDef = TypedDict(
     "EgressConfigurationTypeDef",
     {
         "EgressType": EgressTypeType,
         "VpcConnectorArn": str,
     },
     total=False,
 )
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKey": str,
-    },
-)
-
-HealthCheckConfigurationOutputTypeDef = TypedDict(
-    "HealthCheckConfigurationOutputTypeDef",
-    {
-        "Protocol": HealthCheckProtocolType,
-        "Path": str,
-        "Interval": int,
-        "Timeout": int,
-        "HealthyThreshold": int,
-        "UnhealthyThreshold": int,
-    },
-    total=False,
-)
-
 ImageConfigurationOutputTypeDef = TypedDict(
     "ImageConfigurationOutputTypeDef",
     {
         "RuntimeEnvironmentVariables": Dict[str, str],
         "StartCommand": str,
         "Port": str,
         "RuntimeEnvironmentSecrets": Dict[str, str],
@@ -602,49 +555,22 @@
         "StartCommand": str,
         "Port": str,
         "RuntimeEnvironmentSecrets": Mapping[str, str],
     },
     total=False,
 )
 
-IngressConfigurationOutputTypeDef = TypedDict(
-    "IngressConfigurationOutputTypeDef",
-    {
-        "IsPubliclyAccessible": bool,
-    },
-    total=False,
-)
-
 IngressConfigurationTypeDef = TypedDict(
     "IngressConfigurationTypeDef",
     {
         "IsPubliclyAccessible": bool,
     },
     total=False,
 )
 
-IngressVpcConfigurationOutputTypeDef = TypedDict(
-    "IngressVpcConfigurationOutputTypeDef",
-    {
-        "VpcId": str,
-        "VpcEndpointId": str,
-    },
-    total=False,
-)
-
-InstanceConfigurationOutputTypeDef = TypedDict(
-    "InstanceConfigurationOutputTypeDef",
-    {
-        "Cpu": str,
-        "Memory": str,
-        "InstanceRoleArn": str,
-    },
-    total=False,
-)
-
 ListAutoScalingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
         "LatestOnly": bool,
         "MaxResults": int,
         "NextToken": str,
@@ -745,23 +671,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ListVpcConnectorsRequestRequestTypeDef = TypedDict(
     "ListVpcConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -781,121 +698,81 @@
     {
         "VpcIngressConnectionArn": str,
         "ServiceArn": str,
     },
     total=False,
 )
 
-TraceConfigurationOutputTypeDef = TypedDict(
-    "TraceConfigurationOutputTypeDef",
-    {
-        "Vendor": Literal["AWSXRAY"],
-    },
-)
-
 PauseServiceRequestRequestTypeDef = TypedDict(
     "PauseServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
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
 ResumeServiceRequestRequestTypeDef = TypedDict(
     "ResumeServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
-_RequiredServiceObservabilityConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceObservabilityConfigurationOutputTypeDef",
-    {
-        "ObservabilityEnabled": bool,
-    },
-)
-_OptionalServiceObservabilityConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceObservabilityConfigurationOutputTypeDef",
-    {
-        "ObservabilityConfigurationArn": str,
-    },
-    total=False,
-)
-
-
-class ServiceObservabilityConfigurationOutputTypeDef(
-    _RequiredServiceObservabilityConfigurationOutputTypeDef,
-    _OptionalServiceObservabilityConfigurationOutputTypeDef,
-):
-    pass
-
-
 StartDeploymentRequestRequestTypeDef = TypedDict(
     "StartDeploymentRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
-StartDeploymentResponseTypeDef = TypedDict(
-    "StartDeploymentResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+StartDeploymentResponseTypeDef = TypedDict(
+    "StartDeploymentResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAutoScalingConfigurationsResponseTypeDef = TypedDict(
     "ListAutoScalingConfigurationsResponseTypeDef",
     {
         "AutoScalingConfigurationSummaryList": List[AutoScalingConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAutoScalingConfigurationResponseTypeDef = TypedDict(
     "CreateAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DeleteAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DescribeAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCustomDomainTypeDef = TypedDict(
     "_RequiredCustomDomainTypeDef",
     {
         "DomainName": str,
@@ -959,31 +836,31 @@
 
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "ConnectionSummaryList": List[ConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConnectionResponseTypeDef = TypedDict(
     "CreateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAutoScalingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingConfigurationRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
@@ -1050,14 +927,22 @@
 class CreateVpcConnectorRequestRequestTypeDef(
     _RequiredCreateVpcConnectorRequestRequestTypeDef,
     _OptionalCreateVpcConnectorRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1081,44 +966,59 @@
 class CreateObservabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateObservabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateObservabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+ObservabilityConfigurationTypeDef = TypedDict(
+    "ObservabilityConfigurationTypeDef",
+    {
+        "ObservabilityConfigurationArn": str,
+        "ObservabilityConfigurationName": str,
+        "TraceConfiguration": TraceConfigurationTypeDef,
+        "ObservabilityConfigurationRevision": int,
+        "Latest": bool,
+        "Status": ObservabilityConfigurationStatusType,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 CreateVpcConnectorResponseTypeDef = TypedDict(
     "CreateVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVpcConnectorResponseTypeDef = TypedDict(
     "DeleteVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVpcConnectorResponseTypeDef = TypedDict(
     "DescribeVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcConnectorsResponseTypeDef = TypedDict(
     "ListVpcConnectorsResponseTypeDef",
     {
         "VpcConnectors": List[VpcConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateVpcIngressConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcIngressConnectionRequestRequestTypeDef",
     {
         "ServiceArn": str,
@@ -1146,14 +1046,30 @@
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
     },
 )
 
+VpcIngressConnectionTypeDef = TypedDict(
+    "VpcIngressConnectionTypeDef",
+    {
+        "VpcIngressConnectionArn": str,
+        "VpcIngressConnectionName": str,
+        "ServiceArn": str,
+        "Status": VpcIngressConnectionStatusType,
+        "AccountId": str,
+        "DomainName": str,
+        "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 _RequiredImageRepositoryOutputTypeDef = TypedDict(
     "_RequiredImageRepositoryOutputTypeDef",
     {
         "ImageIdentifier": str,
         "ImageRepositoryType": ImageRepositoryTypeType,
     },
 )
@@ -1188,80 +1104,47 @@
 )
 
 
 class ImageRepositoryTypeDef(_RequiredImageRepositoryTypeDef, _OptionalImageRepositoryTypeDef):
     pass
 
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "EgressConfiguration": EgressConfigurationOutputTypeDef,
-        "IngressConfiguration": IngressConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "EgressConfiguration": EgressConfigurationTypeDef,
         "IngressConfiguration": IngressConfigurationTypeDef,
     },
     total=False,
 )
 
-VpcIngressConnectionTypeDef = TypedDict(
-    "VpcIngressConnectionTypeDef",
-    {
-        "VpcIngressConnectionArn": str,
-        "VpcIngressConnectionName": str,
-        "ServiceArn": str,
-        "Status": VpcIngressConnectionStatusType,
-        "AccountId": str,
-        "DomainName": str,
-        "IngressVpcConfiguration": IngressVpcConfigurationOutputTypeDef,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
-    },
-    total=False,
-)
-
 ListObservabilityConfigurationsResponseTypeDef = TypedDict(
     "ListObservabilityConfigurationsResponseTypeDef",
     {
         "ObservabilityConfigurationSummaryList": List[ObservabilityConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "OperationSummaryList": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcIngressConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     {
         "Filter": ListVpcIngressConnectionsFilterTypeDef,
@@ -1272,72 +1155,57 @@
 )
 
 ListVpcIngressConnectionsResponseTypeDef = TypedDict(
     "ListVpcIngressConnectionsResponseTypeDef",
     {
         "VpcIngressConnectionSummaryList": List[VpcIngressConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ObservabilityConfigurationTypeDef = TypedDict(
-    "ObservabilityConfigurationTypeDef",
-    {
-        "ObservabilityConfigurationArn": str,
-        "ObservabilityConfigurationName": str,
-        "TraceConfiguration": TraceConfigurationOutputTypeDef,
-        "ObservabilityConfigurationRevision": int,
-        "Latest": bool,
-        "Status": ObservabilityConfigurationStatusType,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
-    },
-    total=False,
-)
-
 AssociateCustomDomainResponseTypeDef = TypedDict(
     "AssociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomDomainsResponseTypeDef = TypedDict(
     "DescribeCustomDomainsResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomains": List[CustomDomainTypeDef],
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateCustomDomainResponseTypeDef = TypedDict(
     "DisassociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCodeRepositoryOutputTypeDef = TypedDict(
     "_RequiredCodeRepositoryOutputTypeDef",
     {
         "RepositoryUrl": str,
-        "SourceCodeVersion": SourceCodeVersionOutputTypeDef,
+        "SourceCodeVersion": SourceCodeVersionTypeDef,
     },
 )
 _OptionalCodeRepositoryOutputTypeDef = TypedDict(
     "_OptionalCodeRepositoryOutputTypeDef",
     {
         "CodeConfiguration": CodeConfigurationOutputTypeDef,
     },
@@ -1367,77 +1235,77 @@
 )
 
 
 class CodeRepositoryTypeDef(_RequiredCodeRepositoryTypeDef, _OptionalCodeRepositoryTypeDef):
     pass
 
 
-CreateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "CreateVpcIngressConnectionResponseTypeDef",
+CreateObservabilityConfigurationResponseTypeDef = TypedDict(
+    "CreateObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcIngressConnectionResponseTypeDef",
+DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DeleteObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcIngressConnectionResponseTypeDef",
+DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DescribeObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "UpdateVpcIngressConnectionResponseTypeDef",
+CreateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "CreateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateObservabilityConfigurationResponseTypeDef = TypedDict(
-    "CreateObservabilityConfigurationResponseTypeDef",
+DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DeleteObservabilityConfigurationResponseTypeDef",
+DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DescribeObservabilityConfigurationResponseTypeDef",
+UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "UpdateVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "CodeRepository": CodeRepositoryOutputTypeDef,
         "ImageRepository": ImageRepositoryOutputTypeDef,
         "AutoDeploymentsEnabled": bool,
-        "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
+        "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
     },
     total=False,
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
@@ -1455,27 +1323,27 @@
         "ServiceName": str,
         "ServiceId": str,
         "ServiceArn": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": ServiceStatusType,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "InstanceConfiguration": InstanceConfigurationOutputTypeDef,
+        "InstanceConfiguration": InstanceConfigurationTypeDef,
         "AutoScalingConfigurationSummary": AutoScalingConfigurationSummaryTypeDef,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "NetworkConfiguration": NetworkConfigurationTypeDef,
     },
 )
 _OptionalServiceTypeDef = TypedDict(
     "_OptionalServiceTypeDef",
     {
         "ServiceUrl": str,
         "DeletedAt": datetime,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "HealthCheckConfiguration": HealthCheckConfigurationOutputTypeDef,
-        "ObservabilityConfiguration": ServiceObservabilityConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
+        "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
     pass
@@ -1536,54 +1404,54 @@
 
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceResponseTypeDef = TypedDict(
     "DescribeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PauseServiceResponseTypeDef = TypedDict(
     "PauseServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResumeServiceResponseTypeDef = TypedDict(
     "ResumeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.pyi` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -40,23 +40,22 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcDNSTargetTypeDef",
-    "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
     "CertificateValidationRecordTypeDef",
     "CodeConfigurationValuesOutputTypeDef",
     "CodeConfigurationValuesTypeDef",
-    "SourceCodeVersionOutputTypeDef",
     "SourceCodeVersionTypeDef",
     "ConnectionSummaryTypeDef",
     "ConnectionTypeDef",
     "TagTypeDef",
     "TraceConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
     "HealthCheckConfigurationTypeDef",
@@ -73,90 +72,79 @@
     "DescribeAutoScalingConfigurationRequestRequestTypeDef",
     "DescribeCustomDomainsRequestRequestTypeDef",
     "DescribeObservabilityConfigurationRequestRequestTypeDef",
     "DescribeServiceRequestRequestTypeDef",
     "DescribeVpcConnectorRequestRequestTypeDef",
     "DescribeVpcIngressConnectionRequestRequestTypeDef",
     "DisassociateCustomDomainRequestRequestTypeDef",
-    "EgressConfigurationOutputTypeDef",
     "EgressConfigurationTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
-    "HealthCheckConfigurationOutputTypeDef",
     "ImageConfigurationOutputTypeDef",
     "ImageConfigurationTypeDef",
-    "IngressConfigurationOutputTypeDef",
     "IngressConfigurationTypeDef",
-    "IngressVpcConfigurationOutputTypeDef",
-    "InstanceConfigurationOutputTypeDef",
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListObservabilityConfigurationsRequestRequestTypeDef",
     "ObservabilityConfigurationSummaryTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListVpcConnectorsRequestRequestTypeDef",
     "ListVpcIngressConnectionsFilterTypeDef",
     "VpcIngressConnectionSummaryTypeDef",
-    "TraceConfigurationOutputTypeDef",
     "PauseServiceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeServiceRequestRequestTypeDef",
-    "ServiceObservabilityConfigurationOutputTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "StartDeploymentResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "StartDeploymentResponseTypeDef",
     "ListAutoScalingConfigurationsResponseTypeDef",
     "CreateAutoScalingConfigurationResponseTypeDef",
     "DeleteAutoScalingConfigurationResponseTypeDef",
     "DescribeAutoScalingConfigurationResponseTypeDef",
     "CustomDomainTypeDef",
     "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateConnectionResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "CreateAutoScalingConfigurationRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateVpcConnectorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateObservabilityConfigurationRequestRequestTypeDef",
+    "ObservabilityConfigurationTypeDef",
     "CreateVpcConnectorResponseTypeDef",
     "DeleteVpcConnectorResponseTypeDef",
     "DescribeVpcConnectorResponseTypeDef",
     "ListVpcConnectorsResponseTypeDef",
     "CreateVpcIngressConnectionRequestRequestTypeDef",
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
+    "VpcIngressConnectionTypeDef",
     "ImageRepositoryOutputTypeDef",
     "ImageRepositoryTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
-    "VpcIngressConnectionTypeDef",
     "ListObservabilityConfigurationsResponseTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     "ListVpcIngressConnectionsResponseTypeDef",
-    "ObservabilityConfigurationTypeDef",
     "AssociateCustomDomainResponseTypeDef",
     "DescribeCustomDomainsResponseTypeDef",
     "DisassociateCustomDomainResponseTypeDef",
     "CodeRepositoryOutputTypeDef",
     "CodeRepositoryTypeDef",
+    "CreateObservabilityConfigurationResponseTypeDef",
+    "DeleteObservabilityConfigurationResponseTypeDef",
+    "DescribeObservabilityConfigurationResponseTypeDef",
     "CreateVpcIngressConnectionResponseTypeDef",
     "DeleteVpcIngressConnectionResponseTypeDef",
     "DescribeVpcIngressConnectionResponseTypeDef",
     "UpdateVpcIngressConnectionResponseTypeDef",
-    "CreateObservabilityConfigurationResponseTypeDef",
-    "DeleteObservabilityConfigurationResponseTypeDef",
-    "DescribeObservabilityConfigurationResponseTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "ServiceTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
@@ -183,33 +171,35 @@
 
 class AssociateCustomDomainRequestRequestTypeDef(
     _RequiredAssociateCustomDomainRequestRequestTypeDef,
     _OptionalAssociateCustomDomainRequestRequestTypeDef,
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
 VpcDNSTargetTypeDef = TypedDict(
     "VpcDNSTargetTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "VpcId": str,
         "DomainName": str,
     },
     total=False,
 )
 
-AuthenticationConfigurationOutputTypeDef = TypedDict(
-    "AuthenticationConfigurationOutputTypeDef",
-    {
-        "ConnectionArn": str,
-        "AccessRoleArn": str,
-    },
-    total=False,
-)
-
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "ConnectionArn": str,
         "AccessRoleArn": str,
     },
     total=False,
@@ -295,22 +285,14 @@
 )
 
 class CodeConfigurationValuesTypeDef(
     _RequiredCodeConfigurationValuesTypeDef, _OptionalCodeConfigurationValuesTypeDef
 ):
     pass
 
-SourceCodeVersionOutputTypeDef = TypedDict(
-    "SourceCodeVersionOutputTypeDef",
-    {
-        "Type": Literal["BRANCH"],
-        "Value": str,
-    },
-)
-
 SourceCodeVersionTypeDef = TypedDict(
     "SourceCodeVersionTypeDef",
     {
         "Type": Literal["BRANCH"],
         "Value": str,
     },
 )
@@ -531,52 +513,23 @@
     "DisassociateCustomDomainRequestRequestTypeDef",
     {
         "ServiceArn": str,
         "DomainName": str,
     },
 )
 
-EgressConfigurationOutputTypeDef = TypedDict(
-    "EgressConfigurationOutputTypeDef",
-    {
-        "EgressType": EgressTypeType,
-        "VpcConnectorArn": str,
-    },
-    total=False,
-)
-
 EgressConfigurationTypeDef = TypedDict(
     "EgressConfigurationTypeDef",
     {
         "EgressType": EgressTypeType,
         "VpcConnectorArn": str,
     },
     total=False,
 )
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKey": str,
-    },
-)
-
-HealthCheckConfigurationOutputTypeDef = TypedDict(
-    "HealthCheckConfigurationOutputTypeDef",
-    {
-        "Protocol": HealthCheckProtocolType,
-        "Path": str,
-        "Interval": int,
-        "Timeout": int,
-        "HealthyThreshold": int,
-        "UnhealthyThreshold": int,
-    },
-    total=False,
-)
-
 ImageConfigurationOutputTypeDef = TypedDict(
     "ImageConfigurationOutputTypeDef",
     {
         "RuntimeEnvironmentVariables": Dict[str, str],
         "StartCommand": str,
         "Port": str,
         "RuntimeEnvironmentSecrets": Dict[str, str],
@@ -591,49 +544,22 @@
         "StartCommand": str,
         "Port": str,
         "RuntimeEnvironmentSecrets": Mapping[str, str],
     },
     total=False,
 )
 
-IngressConfigurationOutputTypeDef = TypedDict(
-    "IngressConfigurationOutputTypeDef",
-    {
-        "IsPubliclyAccessible": bool,
-    },
-    total=False,
-)
-
 IngressConfigurationTypeDef = TypedDict(
     "IngressConfigurationTypeDef",
     {
         "IsPubliclyAccessible": bool,
     },
     total=False,
 )
 
-IngressVpcConfigurationOutputTypeDef = TypedDict(
-    "IngressVpcConfigurationOutputTypeDef",
-    {
-        "VpcId": str,
-        "VpcEndpointId": str,
-    },
-    total=False,
-)
-
-InstanceConfigurationOutputTypeDef = TypedDict(
-    "InstanceConfigurationOutputTypeDef",
-    {
-        "Cpu": str,
-        "Memory": str,
-        "InstanceRoleArn": str,
-    },
-    total=False,
-)
-
 ListAutoScalingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
         "LatestOnly": bool,
         "MaxResults": int,
         "NextToken": str,
@@ -732,23 +658,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 ListVpcConnectorsRequestRequestTypeDef = TypedDict(
     "ListVpcConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -768,119 +685,81 @@
     {
         "VpcIngressConnectionArn": str,
         "ServiceArn": str,
     },
     total=False,
 )
 
-TraceConfigurationOutputTypeDef = TypedDict(
-    "TraceConfigurationOutputTypeDef",
-    {
-        "Vendor": Literal["AWSXRAY"],
-    },
-)
-
 PauseServiceRequestRequestTypeDef = TypedDict(
     "PauseServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
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
 ResumeServiceRequestRequestTypeDef = TypedDict(
     "ResumeServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
-_RequiredServiceObservabilityConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceObservabilityConfigurationOutputTypeDef",
-    {
-        "ObservabilityEnabled": bool,
-    },
-)
-_OptionalServiceObservabilityConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceObservabilityConfigurationOutputTypeDef",
-    {
-        "ObservabilityConfigurationArn": str,
-    },
-    total=False,
-)
-
-class ServiceObservabilityConfigurationOutputTypeDef(
-    _RequiredServiceObservabilityConfigurationOutputTypeDef,
-    _OptionalServiceObservabilityConfigurationOutputTypeDef,
-):
-    pass
-
 StartDeploymentRequestRequestTypeDef = TypedDict(
     "StartDeploymentRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
-StartDeploymentResponseTypeDef = TypedDict(
-    "StartDeploymentResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+StartDeploymentResponseTypeDef = TypedDict(
+    "StartDeploymentResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAutoScalingConfigurationsResponseTypeDef = TypedDict(
     "ListAutoScalingConfigurationsResponseTypeDef",
     {
         "AutoScalingConfigurationSummaryList": List[AutoScalingConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAutoScalingConfigurationResponseTypeDef = TypedDict(
     "CreateAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DeleteAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DescribeAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCustomDomainTypeDef = TypedDict(
     "_RequiredCustomDomainTypeDef",
     {
         "DomainName": str,
@@ -938,31 +817,31 @@
     pass
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "ConnectionSummaryList": List[ConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConnectionResponseTypeDef = TypedDict(
     "CreateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAutoScalingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingConfigurationRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
@@ -1023,14 +902,22 @@
 
 class CreateVpcConnectorRequestRequestTypeDef(
     _RequiredCreateVpcConnectorRequestRequestTypeDef,
     _OptionalCreateVpcConnectorRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1052,44 +939,59 @@
 
 class CreateObservabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateObservabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateObservabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+ObservabilityConfigurationTypeDef = TypedDict(
+    "ObservabilityConfigurationTypeDef",
+    {
+        "ObservabilityConfigurationArn": str,
+        "ObservabilityConfigurationName": str,
+        "TraceConfiguration": TraceConfigurationTypeDef,
+        "ObservabilityConfigurationRevision": int,
+        "Latest": bool,
+        "Status": ObservabilityConfigurationStatusType,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 CreateVpcConnectorResponseTypeDef = TypedDict(
     "CreateVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVpcConnectorResponseTypeDef = TypedDict(
     "DeleteVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVpcConnectorResponseTypeDef = TypedDict(
     "DescribeVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcConnectorsResponseTypeDef = TypedDict(
     "ListVpcConnectorsResponseTypeDef",
     {
         "VpcConnectors": List[VpcConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateVpcIngressConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcIngressConnectionRequestRequestTypeDef",
     {
         "ServiceArn": str,
@@ -1115,14 +1017,30 @@
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
     },
 )
 
+VpcIngressConnectionTypeDef = TypedDict(
+    "VpcIngressConnectionTypeDef",
+    {
+        "VpcIngressConnectionArn": str,
+        "VpcIngressConnectionName": str,
+        "ServiceArn": str,
+        "Status": VpcIngressConnectionStatusType,
+        "AccountId": str,
+        "DomainName": str,
+        "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 _RequiredImageRepositoryOutputTypeDef = TypedDict(
     "_RequiredImageRepositoryOutputTypeDef",
     {
         "ImageIdentifier": str,
         "ImageRepositoryType": ImageRepositoryTypeType,
     },
 )
@@ -1153,80 +1071,47 @@
     },
     total=False,
 )
 
 class ImageRepositoryTypeDef(_RequiredImageRepositoryTypeDef, _OptionalImageRepositoryTypeDef):
     pass
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "EgressConfiguration": EgressConfigurationOutputTypeDef,
-        "IngressConfiguration": IngressConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "EgressConfiguration": EgressConfigurationTypeDef,
         "IngressConfiguration": IngressConfigurationTypeDef,
     },
     total=False,
 )
 
-VpcIngressConnectionTypeDef = TypedDict(
-    "VpcIngressConnectionTypeDef",
-    {
-        "VpcIngressConnectionArn": str,
-        "VpcIngressConnectionName": str,
-        "ServiceArn": str,
-        "Status": VpcIngressConnectionStatusType,
-        "AccountId": str,
-        "DomainName": str,
-        "IngressVpcConfiguration": IngressVpcConfigurationOutputTypeDef,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
-    },
-    total=False,
-)
-
 ListObservabilityConfigurationsResponseTypeDef = TypedDict(
     "ListObservabilityConfigurationsResponseTypeDef",
     {
         "ObservabilityConfigurationSummaryList": List[ObservabilityConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "OperationSummaryList": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcIngressConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     {
         "Filter": ListVpcIngressConnectionsFilterTypeDef,
@@ -1237,72 +1122,57 @@
 )
 
 ListVpcIngressConnectionsResponseTypeDef = TypedDict(
     "ListVpcIngressConnectionsResponseTypeDef",
     {
         "VpcIngressConnectionSummaryList": List[VpcIngressConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ObservabilityConfigurationTypeDef = TypedDict(
-    "ObservabilityConfigurationTypeDef",
-    {
-        "ObservabilityConfigurationArn": str,
-        "ObservabilityConfigurationName": str,
-        "TraceConfiguration": TraceConfigurationOutputTypeDef,
-        "ObservabilityConfigurationRevision": int,
-        "Latest": bool,
-        "Status": ObservabilityConfigurationStatusType,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 AssociateCustomDomainResponseTypeDef = TypedDict(
     "AssociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomDomainsResponseTypeDef = TypedDict(
     "DescribeCustomDomainsResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomains": List[CustomDomainTypeDef],
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateCustomDomainResponseTypeDef = TypedDict(
     "DisassociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCodeRepositoryOutputTypeDef = TypedDict(
     "_RequiredCodeRepositoryOutputTypeDef",
     {
         "RepositoryUrl": str,
-        "SourceCodeVersion": SourceCodeVersionOutputTypeDef,
+        "SourceCodeVersion": SourceCodeVersionTypeDef,
     },
 )
 _OptionalCodeRepositoryOutputTypeDef = TypedDict(
     "_OptionalCodeRepositoryOutputTypeDef",
     {
         "CodeConfiguration": CodeConfigurationOutputTypeDef,
     },
@@ -1328,77 +1198,77 @@
     },
     total=False,
 )
 
 class CodeRepositoryTypeDef(_RequiredCodeRepositoryTypeDef, _OptionalCodeRepositoryTypeDef):
     pass
 
-CreateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "CreateVpcIngressConnectionResponseTypeDef",
+CreateObservabilityConfigurationResponseTypeDef = TypedDict(
+    "CreateObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcIngressConnectionResponseTypeDef",
+DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DeleteObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcIngressConnectionResponseTypeDef",
+DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DescribeObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "UpdateVpcIngressConnectionResponseTypeDef",
+CreateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "CreateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateObservabilityConfigurationResponseTypeDef = TypedDict(
-    "CreateObservabilityConfigurationResponseTypeDef",
+DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DeleteObservabilityConfigurationResponseTypeDef",
+DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DescribeObservabilityConfigurationResponseTypeDef",
+UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "UpdateVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "CodeRepository": CodeRepositoryOutputTypeDef,
         "ImageRepository": ImageRepositoryOutputTypeDef,
         "AutoDeploymentsEnabled": bool,
-        "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
+        "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
     },
     total=False,
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
@@ -1416,27 +1286,27 @@
         "ServiceName": str,
         "ServiceId": str,
         "ServiceArn": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": ServiceStatusType,
         "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "InstanceConfiguration": InstanceConfigurationOutputTypeDef,
+        "InstanceConfiguration": InstanceConfigurationTypeDef,
         "AutoScalingConfigurationSummary": AutoScalingConfigurationSummaryTypeDef,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "NetworkConfiguration": NetworkConfigurationTypeDef,
     },
 )
 _OptionalServiceTypeDef = TypedDict(
     "_OptionalServiceTypeDef",
     {
         "ServiceUrl": str,
         "DeletedAt": datetime,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "HealthCheckConfiguration": HealthCheckConfigurationOutputTypeDef,
-        "ObservabilityConfiguration": ServiceObservabilityConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
+        "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
 class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
     pass
 
@@ -1491,54 +1361,54 @@
     pass
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceResponseTypeDef = TypedDict(
     "DescribeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PauseServiceResponseTypeDef = TypedDict(
     "PauseServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResumeServiceResponseTypeDef = TypedDict(
     "ResumeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/PKG-INFO` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.28.12
-Summary: Type annotations for boto3.AppRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,23 +314,22 @@
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
-    AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
     CodeConfigurationValuesOutputTypeDef,
     CodeConfigurationValuesTypeDef,
-    SourceCodeVersionOutputTypeDef,
     SourceCodeVersionTypeDef,
     ConnectionSummaryTypeDef,
     ConnectionTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HealthCheckConfigurationTypeDef,
@@ -347,90 +346,79 @@
     DescribeAutoScalingConfigurationRequestRequestTypeDef,
     DescribeCustomDomainsRequestRequestTypeDef,
     DescribeObservabilityConfigurationRequestRequestTypeDef,
     DescribeServiceRequestRequestTypeDef,
     DescribeVpcConnectorRequestRequestTypeDef,
     DescribeVpcIngressConnectionRequestRequestTypeDef,
     DisassociateCustomDomainRequestRequestTypeDef,
-    EgressConfigurationOutputTypeDef,
     EgressConfigurationTypeDef,
-    EncryptionConfigurationOutputTypeDef,
-    HealthCheckConfigurationOutputTypeDef,
     ImageConfigurationOutputTypeDef,
     ImageConfigurationTypeDef,
-    IngressConfigurationOutputTypeDef,
     IngressConfigurationTypeDef,
-    IngressVpcConfigurationOutputTypeDef,
-    InstanceConfigurationOutputTypeDef,
     ListAutoScalingConfigurationsRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListObservabilityConfigurationsRequestRequestTypeDef,
     ObservabilityConfigurationSummaryTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
-    TraceConfigurationOutputTypeDef,
     PauseServiceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
-    ServiceObservabilityConfigurationOutputTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    StartDeploymentResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    StartDeploymentResponseTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
     CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
     CreateConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     CreateAutoScalingConfigurationRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateVpcConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateObservabilityConfigurationRequestRequestTypeDef,
+    ObservabilityConfigurationTypeDef,
     CreateVpcConnectorResponseTypeDef,
     DeleteVpcConnectorResponseTypeDef,
     DescribeVpcConnectorResponseTypeDef,
     ListVpcConnectorsResponseTypeDef,
     CreateVpcIngressConnectionRequestRequestTypeDef,
     UpdateVpcIngressConnectionRequestRequestTypeDef,
+    VpcIngressConnectionTypeDef,
     ImageRepositoryOutputTypeDef,
     ImageRepositoryTypeDef,
-    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
-    VpcIngressConnectionTypeDef,
     ListObservabilityConfigurationsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVpcIngressConnectionsRequestRequestTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
-    ObservabilityConfigurationTypeDef,
     AssociateCustomDomainResponseTypeDef,
     DescribeCustomDomainsResponseTypeDef,
     DisassociateCustomDomainResponseTypeDef,
     CodeRepositoryOutputTypeDef,
     CodeRepositoryTypeDef,
+    CreateObservabilityConfigurationResponseTypeDef,
+    DeleteObservabilityConfigurationResponseTypeDef,
+    DescribeObservabilityConfigurationResponseTypeDef,
     CreateVpcIngressConnectionResponseTypeDef,
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
-    CreateObservabilityConfigurationResponseTypeDef,
-    DeleteObservabilityConfigurationResponseTypeDef,
-    DescribeObservabilityConfigurationResponseTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
```

### Comparing `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/SOURCES.txt` & `mypy-boto3-apprunner-1.28.15/mypy_boto3_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.12/setup.py` & `mypy-boto3-apprunner-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apprunner",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppRunner 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

