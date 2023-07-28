# Comparing `tmp/mypy-boto3-greengrassv2-1.28.12.tar.gz` & `tmp/mypy-boto3-greengrassv2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrassv2-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrassv2-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
```

## Comparing `mypy-boto3-greengrassv2-1.28.12.tar` & `mypy-boto3-greengrassv2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41680 2023-07-27 05:23:09.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41647 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:44.000000 mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.760499 mypy-boto3-greengrassv2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:23:08.000000 mypy-boto3-greengrassv2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.277172 mypy-boto3-greengrassv2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-07-28 20:42:53.265172 mypy-boto3-greengrassv2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.265172 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-28 20:27:06.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38534 2023-07-28 20:27:08.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38501 2023-07-28 20:27:07.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.265172 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-07-28 20:42:53.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:53.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:53.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:53.000000 mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.277172 mypy-boto3-greengrassv2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:27:05.000000 mypy-boto3-greengrassv2-1.28.15/setup.py
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/LICENSE` & `mypy-boto3-greengrassv2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/PKG-INFO` & `mypy-boto3-greengrassv2-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.28.12
-Summary: Type annotations for boto3.GreengrassV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GreengrassV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,118 +369,107 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
-    CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformOutputTypeDef,
     ComponentPlatformTypeDef,
-    SystemResourceLimitsOutputTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
-    CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
-    DeploymentComponentUpdatePolicyOutputTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
-    DeploymentConfigurationValidationPolicyOutputTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
-    IoTJobTimeoutConfigOutputTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetComponentVersionArtifactRequestRequestTypeDef,
-    GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
-    GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
-    IoTJobAbortCriteriaOutputTypeDef,
     IoTJobAbortCriteriaTypeDef,
-    IoTJobRateIncreaseCriteriaOutputTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
-    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
-    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     ListComponentVersionsRequestRequestTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
     ListCoreDevicesRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     ListEffectiveDeploymentsRequestRequestTypeDef,
-    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ListInstalledComponentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResolvedComponentVersionTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
+    CancelDeploymentResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetComponentResponseTypeDef,
+    GetComponentVersionArtifactResponseTypeDef,
+    GetCoreDeviceResponseTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
-    ComponentRunWithOutputTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
-    DeploymentPoliciesOutputTypeDef,
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
     IoTJobAbortConfigOutputTypeDef,
     IoTJobAbortConfigTypeDef,
-    IoTJobExponentialRolloutRateOutputTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
+    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
     ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
-    IoTJobExecutionsRolloutConfigOutputTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
     DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
     GetDeploymentResponseTypeDef,
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/README.md` & `mypy-boto3-greengrassv2-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,118 +337,107 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
-    CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformOutputTypeDef,
     ComponentPlatformTypeDef,
-    SystemResourceLimitsOutputTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
-    CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
-    DeploymentComponentUpdatePolicyOutputTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
-    DeploymentConfigurationValidationPolicyOutputTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
-    IoTJobTimeoutConfigOutputTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetComponentVersionArtifactRequestRequestTypeDef,
-    GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
-    GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
-    IoTJobAbortCriteriaOutputTypeDef,
     IoTJobAbortCriteriaTypeDef,
-    IoTJobRateIncreaseCriteriaOutputTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
-    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
-    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     ListComponentVersionsRequestRequestTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
     ListCoreDevicesRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     ListEffectiveDeploymentsRequestRequestTypeDef,
-    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ListInstalledComponentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResolvedComponentVersionTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
+    CancelDeploymentResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetComponentResponseTypeDef,
+    GetComponentVersionArtifactResponseTypeDef,
+    GetCoreDeviceResponseTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
-    ComponentRunWithOutputTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
-    DeploymentPoliciesOutputTypeDef,
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
     IoTJobAbortConfigOutputTypeDef,
     IoTJobAbortConfigTypeDef,
-    IoTJobExponentialRolloutRateOutputTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
+    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
     ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
-    IoTJobExecutionsRolloutConfigOutputTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
     DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
     GetDeploymentResponseTypeDef,
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.py` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__init__.pyi` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/__main__.py` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GreengrassV2 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.GreengrassV2 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
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

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.py` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/client.pyi` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.py` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/literals.pyi` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.py` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,30 +76,30 @@
 class ListClientDevicesAssociatedWithCoreDevicePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
         """
 
 
 class ListComponentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
         """
 
 
@@ -109,15 +109,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
         """
 
 
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
 
@@ -148,30 +148,30 @@
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
 
 class ListEffectiveDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEffectiveDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
         """
 
 
@@ -182,13 +182,13 @@
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/paginator.pyi` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,29 +73,29 @@
 class ListClientDevicesAssociatedWithCoreDevicePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
         """
 
 class ListComponentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
         """
 
 class ListComponentsPaginator(Paginator):
@@ -104,15 +104,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
         """
 
 class ListCoreDevicesPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
@@ -141,29 +141,29 @@
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
 class ListEffectiveDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEffectiveDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
         """
 
 class ListInstalledComponentsPaginator(Paginator):
@@ -173,13 +173,13 @@
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.py` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -43,123 +43,111 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
-    "CancelDeploymentResponseTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
     "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
     "ComponentPlatformOutputTypeDef",
     "ComponentPlatformTypeDef",
-    "SystemResourceLimitsOutputTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
-    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
-    "DeploymentComponentUpdatePolicyOutputTypeDef",
     "DeploymentComponentUpdatePolicyTypeDef",
-    "DeploymentConfigurationValidationPolicyOutputTypeDef",
     "DeploymentConfigurationValidationPolicyTypeDef",
-    "IoTJobTimeoutConfigOutputTypeDef",
     "IoTJobTimeoutConfigTypeDef",
     "DeploymentTypeDef",
     "DescribeComponentRequestRequestTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EffectiveDeploymentStatusDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetComponentRequestRequestTypeDef",
-    "GetComponentResponseTypeDef",
     "GetComponentVersionArtifactRequestRequestTypeDef",
-    "GetComponentVersionArtifactResponseTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetCoreDeviceRequestRequestTypeDef",
-    "GetCoreDeviceResponseTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
     "InstalledComponentTypeDef",
-    "IoTJobAbortCriteriaOutputTypeDef",
     "IoTJobAbortCriteriaTypeDef",
-    "IoTJobRateIncreaseCriteriaOutputTypeDef",
     "IoTJobRateIncreaseCriteriaTypeDef",
     "LambdaDeviceMountTypeDef",
     "LambdaVolumeMountTypeDef",
     "LambdaEventSourceTypeDef",
-    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
-    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentVersionsRequestRequestTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListCoreDevicesRequestRequestTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
-    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestRequestTypeDef",
-    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ListInstalledComponentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "ResolvedComponentVersionTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
+    "CancelDeploymentResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetComponentResponseTypeDef",
+    "GetComponentVersionArtifactResponseTypeDef",
+    "GetCoreDeviceResponseTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
-    "ComponentRunWithOutputTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
-    "DeploymentPoliciesOutputTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
     "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
-    "IoTJobExponentialRolloutRateOutputTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
+    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
     "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
-    "IoTJobExecutionsRolloutConfigOutputTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
     "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
     "GetDeploymentResponseTypeDef",
@@ -188,19 +176,22 @@
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "associatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociatedClientDeviceTypeDef = TypedDict(
     "AssociatedClientDeviceTypeDef",
     {
         "thingName": str,
@@ -229,22 +220,14 @@
 CancelDeploymentRequestRequestTypeDef = TypedDict(
     "CancelDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
-CancelDeploymentResponseTypeDef = TypedDict(
-    "CancelDeploymentResponseTypeDef",
-    {
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CloudComponentStatusTypeDef = TypedDict(
     "CloudComponentStatusTypeDef",
     {
         "componentState": CloudComponentStateType,
         "message": str,
         "errors": Dict[str, str],
         "vendorGuidance": VendorGuidanceType,
@@ -304,23 +287,14 @@
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
-SystemResourceLimitsOutputTypeDef = TypedDict(
-    "SystemResourceLimitsOutputTypeDef",
-    {
-        "memory": int,
-        "cpus": float,
-    },
-    total=False,
-)
-
 SystemResourceLimitsTypeDef = TypedDict(
     "SystemResourceLimitsTypeDef",
     {
         "memory": int,
         "cpus": float,
     },
     total=False,
@@ -332,25 +306,14 @@
         "componentName": str,
         "componentVersion": str,
         "arn": str,
     },
     total=False,
 )
 
-ConnectivityInfoOutputTypeDef = TypedDict(
-    "ConnectivityInfoOutputTypeDef",
-    {
-        "id": str,
-        "hostAddress": str,
-        "portNumber": int,
-        "metadata": str,
-    },
-    total=False,
-)
-
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "id": str,
         "hostAddress": str,
         "portNumber": int,
         "metadata": str,
@@ -364,24 +327,14 @@
         "coreDeviceThingName": str,
         "status": CoreDeviceStatusType,
         "lastStatusUpdateTimestamp": datetime,
     },
     total=False,
 )
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -395,56 +348,31 @@
 DeleteDeploymentRequestRequestTypeDef = TypedDict(
     "DeleteDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
-DeploymentComponentUpdatePolicyOutputTypeDef = TypedDict(
-    "DeploymentComponentUpdatePolicyOutputTypeDef",
-    {
-        "timeoutInSeconds": int,
-        "action": DeploymentComponentUpdatePolicyActionType,
-    },
-    total=False,
-)
-
 DeploymentComponentUpdatePolicyTypeDef = TypedDict(
     "DeploymentComponentUpdatePolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "action": DeploymentComponentUpdatePolicyActionType,
     },
     total=False,
 )
 
-DeploymentConfigurationValidationPolicyOutputTypeDef = TypedDict(
-    "DeploymentConfigurationValidationPolicyOutputTypeDef",
-    {
-        "timeoutInSeconds": int,
-    },
-    total=False,
-)
-
 DeploymentConfigurationValidationPolicyTypeDef = TypedDict(
     "DeploymentConfigurationValidationPolicyTypeDef",
     {
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
-IoTJobTimeoutConfigOutputTypeDef = TypedDict(
-    "IoTJobTimeoutConfigOutputTypeDef",
-    {
-        "inProgressTimeoutInMinutes": int,
-    },
-    total=False,
-)
-
 IoTJobTimeoutConfigTypeDef = TypedDict(
     "IoTJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
@@ -467,129 +395,71 @@
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "disassociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EffectiveDeploymentStatusDetailsTypeDef = TypedDict(
     "EffectiveDeploymentStatusDetailsTypeDef",
     {
         "errorStack": List[str],
         "errorTypes": List[str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetComponentRequestRequestTypeDef = TypedDict(
     "_RequiredGetComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetComponentRequestRequestTypeDef = TypedDict(
     "_OptionalGetComponentRequestRequestTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
     },
     total=False,
 )
 
-
 class GetComponentRequestRequestTypeDef(
     _RequiredGetComponentRequestRequestTypeDef, _OptionalGetComponentRequestRequestTypeDef
 ):
     pass
 
-
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
-    {
-        "recipeOutputFormat": RecipeOutputFormatType,
-        "recipe": bytes,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetComponentVersionArtifactRequestRequestTypeDef = TypedDict(
     "GetComponentVersionArtifactRequestRequestTypeDef",
     {
         "arn": str,
         "artifactName": str,
     },
 )
 
-GetComponentVersionArtifactResponseTypeDef = TypedDict(
-    "GetComponentVersionArtifactResponseTypeDef",
-    {
-        "preSignedUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConnectivityInfoRequestRequestTypeDef = TypedDict(
     "GetConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
 GetCoreDeviceRequestRequestTypeDef = TypedDict(
     "GetCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 
-GetCoreDeviceResponseTypeDef = TypedDict(
-    "GetCoreDeviceResponseTypeDef",
-    {
-        "coreDeviceThingName": str,
-        "coreVersion": str,
-        "platform": str,
-        "architecture": str,
-        "status": CoreDeviceStatusType,
-        "lastStatusUpdateTimestamp": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDeploymentRequestRequestTypeDef = TypedDict(
     "GetDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "associatedAt": str,
-        "roleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InstalledComponentTypeDef = TypedDict(
     "InstalledComponentTypeDef",
     {
         "componentName": str,
         "componentVersion": str,
         "lifecycleState": InstalledComponentLifecycleStateType,
         "lifecycleStateDetails": str,
@@ -598,43 +468,24 @@
         "lastReportedTimestamp": datetime,
         "lastInstallationSource": str,
         "lifecycleStatusCodes": List[str],
     },
     total=False,
 )
 
-IoTJobAbortCriteriaOutputTypeDef = TypedDict(
-    "IoTJobAbortCriteriaOutputTypeDef",
-    {
-        "failureType": IoTJobExecutionFailureTypeType,
-        "action": Literal["CANCEL"],
-        "thresholdPercentage": float,
-        "minNumberOfExecutedThings": int,
-    },
-)
-
 IoTJobAbortCriteriaTypeDef = TypedDict(
     "IoTJobAbortCriteriaTypeDef",
     {
         "failureType": IoTJobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
-IoTJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
-    "IoTJobRateIncreaseCriteriaOutputTypeDef",
-    {
-        "numberOfNotifiedThings": int,
-        "numberOfSucceededThings": int,
-    },
-    total=False,
-)
-
 IoTJobRateIncreaseCriteriaTypeDef = TypedDict(
     "IoTJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
@@ -651,21 +502,19 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
-
 class LambdaDeviceMountTypeDef(
     _RequiredLambdaDeviceMountTypeDef, _OptionalLambdaDeviceMountTypeDef
 ):
     pass
 
-
 _RequiredLambdaVolumeMountTypeDef = TypedDict(
     "_RequiredLambdaVolumeMountTypeDef",
     {
         "sourcePath": str,
         "destinationPath": str,
     },
 )
@@ -674,51 +523,37 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
-
 class LambdaVolumeMountTypeDef(
     _RequiredLambdaVolumeMountTypeDef, _OptionalLambdaVolumeMountTypeDef
 ):
     pass
 
-
 LambdaEventSourceTypeDef = TypedDict(
     "LambdaEventSourceTypeDef",
     {
         "topic": str,
         "type": LambdaEventSourceTypeType,
     },
 )
 
-_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
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
 
-
-class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
-    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
@@ -726,44 +561,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
-    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListComponentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListComponentVersionsRequestRequestTypeDef = TypedDict(
@@ -771,107 +582,53 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListComponentVersionsRequestRequestTypeDef(
     _RequiredListComponentVersionsRequestRequestTypeDef,
     _OptionalListComponentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsRequestListComponentsPaginateTypeDef",
-    {
-        "scope": ComponentVisibilityScopeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComponentsRequestRequestTypeDef = TypedDict(
     "ListComponentsRequestRequestTypeDef",
     {
         "scope": ComponentVisibilityScopeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
-    {
-        "thingGroupArn": str,
-        "status": CoreDeviceStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCoreDevicesRequestRequestTypeDef = TypedDict(
     "ListCoreDevicesRequestRequestTypeDef",
     {
         "thingGroupArn": str,
         "status": CoreDeviceStatusType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "targetArn": str,
-        "historyFilter": DeploymentHistoryFilterType,
-        "parentTargetArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentsRequestRequestTypeDef = TypedDict(
     "ListDeploymentsRequestRequestTypeDef",
     {
         "targetArn": str,
         "historyFilter": DeploymentHistoryFilterType,
         "parentTargetArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
-    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListEffectiveDeploymentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
@@ -879,45 +636,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEffectiveDeploymentsRequestRequestTypeDef(
     _RequiredListEffectiveDeploymentsRequestRequestTypeDef,
     _OptionalListEffectiveDeploymentsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "topologyFilter": InstalledComponentTopologyFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
-    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstalledComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListInstalledComponentsRequestRequestTypeDef = TypedDict(
@@ -926,71 +658,40 @@
         "maxResults": int,
         "nextToken": str,
         "topologyFilter": InstalledComponentTopologyFilterType,
     },
     total=False,
 )
 
-
 class ListInstalledComponentsRequestRequestTypeDef(
     _RequiredListInstalledComponentsRequestRequestTypeDef,
     _OptionalListInstalledComponentsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 ResolvedComponentVersionTypeDef = TypedDict(
     "ResolvedComponentVersionTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "recipe": bytes,
         "vendorGuidance": VendorGuidanceType,
         "message": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -999,59 +700,147 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "version": str,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
-
 class BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef(
     _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
     _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    {
+        "associatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef = TypedDict(
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelDeploymentResponseTypeDef = TypedDict(
+    "CancelDeploymentResponseTypeDef",
+    {
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "disassociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
+    {
+        "recipeOutputFormat": RecipeOutputFormatType,
+        "recipe": bytes,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentVersionArtifactResponseTypeDef = TypedDict(
+    "GetComponentVersionArtifactResponseTypeDef",
+    {
+        "preSignedUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCoreDeviceResponseTypeDef = TypedDict(
+    "GetCoreDeviceResponseTypeDef",
+    {
+        "coreDeviceThingName": str,
+        "coreVersion": str,
+        "platform": str,
+        "architecture": str,
+        "status": CoreDeviceStatusType,
+        "lastStatusUpdateTimestamp": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "associatedAt": str,
+        "roleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "version": str,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef = TypedDict(
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     {
         "associatedClientDevices": List[AssociatedClientDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
@@ -1061,39 +850,37 @@
     "_OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
-
 class BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef(
     _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     _OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef = TypedDict(
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateComponentVersionResponseTypeDef = TypedDict(
     "CreateComponentVersionResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "status": CloudComponentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentLatestVersionTypeDef = TypedDict(
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
@@ -1114,37 +901,27 @@
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
         "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
 )
 
-ComponentRunWithOutputTypeDef = TypedDict(
-    "ComponentRunWithOutputTypeDef",
-    {
-        "posixUser": str,
-        "systemResourceLimits": SystemResourceLimitsOutputTypeDef,
-        "windowsUser": str,
-    },
-    total=False,
-)
-
 ComponentRunWithTypeDef = TypedDict(
     "ComponentRunWithTypeDef",
     {
         "posixUser": str,
         "systemResourceLimits": SystemResourceLimitsTypeDef,
         "windowsUser": str,
     },
@@ -1152,24 +929,24 @@
 )
 
 ListComponentVersionsResponseTypeDef = TypedDict(
     "ListComponentVersionsResponseTypeDef",
     {
         "componentVersions": List[ComponentVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "connectivityInfo": List[ConnectivityInfoOutputTypeDef],
+        "connectivityInfo": List[ConnectivityInfoTypeDef],
         "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
@@ -1178,26 +955,16 @@
 )
 
 ListCoreDevicesResponseTypeDef = TypedDict(
     "ListCoreDevicesResponseTypeDef",
     {
         "coreDevices": List[CoreDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeploymentPoliciesOutputTypeDef = TypedDict(
-    "DeploymentPoliciesOutputTypeDef",
-    {
-        "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
-        "componentUpdatePolicy": DeploymentComponentUpdatePolicyOutputTypeDef,
-        "configurationValidationPolicy": DeploymentConfigurationValidationPolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DeploymentPoliciesTypeDef = TypedDict(
     "DeploymentPoliciesTypeDef",
     {
         "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
         "componentUpdatePolicy": DeploymentComponentUpdatePolicyTypeDef,
@@ -1207,15 +974,15 @@
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEffectiveDeploymentTypeDef = TypedDict(
     "_RequiredEffectiveDeploymentTypeDef",
     {
         "deploymentId": str,
@@ -1234,53 +1001,42 @@
         "description": str,
         "reason": str,
         "statusDetails": EffectiveDeploymentStatusDetailsTypeDef,
     },
     total=False,
 )
 
-
 class EffectiveDeploymentTypeDef(
     _RequiredEffectiveDeploymentTypeDef, _OptionalEffectiveDeploymentTypeDef
 ):
     pass
 
-
 ListInstalledComponentsResponseTypeDef = TypedDict(
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IoTJobAbortConfigOutputTypeDef = TypedDict(
     "IoTJobAbortConfigOutputTypeDef",
     {
-        "criteriaList": List[IoTJobAbortCriteriaOutputTypeDef],
+        "criteriaList": List[IoTJobAbortCriteriaTypeDef],
     },
 )
 
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 
-IoTJobExponentialRolloutRateOutputTypeDef = TypedDict(
-    "IoTJobExponentialRolloutRateOutputTypeDef",
-    {
-        "baseRatePerMinute": int,
-        "incrementFactor": float,
-        "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaOutputTypeDef,
-    },
-)
-
 IoTJobExponentialRolloutRateTypeDef = TypedDict(
     "IoTJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaTypeDef,
     },
@@ -1293,19 +1049,130 @@
         "mountROSysfs": bool,
         "volumes": Sequence[LambdaVolumeMountTypeDef],
         "devices": Sequence[LambdaDeviceMountTypeDef],
     },
     total=False,
 )
 
+_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
+    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+):
+    pass
+
+_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
+    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+):
+    pass
+
+ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    {
+        "scope": ComponentVisibilityScopeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
+    {
+        "thingGroupArn": str,
+        "status": CoreDeviceStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "targetArn": str,
+        "historyFilter": DeploymentHistoryFilterType,
+        "parentTargetArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
+    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "topologyFilter": InstalledComponentTopologyFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
+    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+):
+    pass
+
 ResolveComponentCandidatesResponseTypeDef = TypedDict(
     "ResolveComponentCandidatesResponseTypeDef",
     {
         "resolvedComponentVersions": List[ResolvedComponentVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "arn": str,
@@ -1316,15 +1183,15 @@
 )
 
 ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
     "ComponentDeploymentSpecificationOutputTypeDef",
     {
         "componentVersion": str,
         "configurationUpdate": ComponentConfigurationUpdateOutputTypeDef,
-        "runWith": ComponentRunWithOutputTypeDef,
+        "runWith": ComponentRunWithTypeDef,
     },
     total=False,
 )
 
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
@@ -1336,27 +1203,18 @@
 )
 
 ListEffectiveDeploymentsResponseTypeDef = TypedDict(
     "ListEffectiveDeploymentsResponseTypeDef",
     {
         "effectiveDeployments": List[EffectiveDeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IoTJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
-    "IoTJobExecutionsRolloutConfigOutputTypeDef",
-    {
-        "exponentialRate": IoTJobExponentialRolloutRateOutputTypeDef,
-        "maximumPerMinute": int,
-    },
-    total=False,
-)
-
 IoTJobExecutionsRolloutConfigTypeDef = TypedDict(
     "IoTJobExecutionsRolloutConfigTypeDef",
     {
         "exponentialRate": IoTJobExponentialRolloutRateTypeDef,
         "maximumPerMinute": int,
     },
     total=False,
@@ -1372,24 +1230,24 @@
 )
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationOutputTypeDef",
     {
-        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigOutputTypeDef,
+        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigOutputTypeDef,
-        "timeoutConfig": IoTJobTimeoutConfigOutputTypeDef,
+        "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
     total=False,
 )
 
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
@@ -1425,21 +1283,21 @@
         "revisionId": str,
         "deploymentId": str,
         "deploymentName": str,
         "deploymentStatus": DeploymentStatusType,
         "iotJobId": str,
         "iotJobArn": str,
         "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
-        "deploymentPolicies": DeploymentPoliciesOutputTypeDef,
+        "deploymentPolicies": DeploymentPoliciesTypeDef,
         "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
         "creationTimestamp": datetime,
         "isLatestForTarget": bool,
         "parentTargetArn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "targetArn": str,
@@ -1455,21 +1313,19 @@
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
 _OptionalLambdaFunctionRecipeSourceTypeDef = TypedDict(
@@ -1480,21 +1336,19 @@
         "componentPlatforms": Sequence[ComponentPlatformTypeDef],
         "componentDependencies": Mapping[str, ComponentDependencyRequirementTypeDef],
         "componentLambdaParameters": LambdaExecutionParametersTypeDef,
     },
     total=False,
 )
 
-
 class LambdaFunctionRecipeSourceTypeDef(
     _RequiredLambdaFunctionRecipeSourceTypeDef, _OptionalLambdaFunctionRecipeSourceTypeDef
 ):
     pass
 
-
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
         "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2/type_defs.pyi` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,122 +43,112 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
-    "CancelDeploymentResponseTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
     "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
     "ComponentPlatformOutputTypeDef",
     "ComponentPlatformTypeDef",
-    "SystemResourceLimitsOutputTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
-    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
-    "DeploymentComponentUpdatePolicyOutputTypeDef",
     "DeploymentComponentUpdatePolicyTypeDef",
-    "DeploymentConfigurationValidationPolicyOutputTypeDef",
     "DeploymentConfigurationValidationPolicyTypeDef",
-    "IoTJobTimeoutConfigOutputTypeDef",
     "IoTJobTimeoutConfigTypeDef",
     "DeploymentTypeDef",
     "DescribeComponentRequestRequestTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EffectiveDeploymentStatusDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetComponentRequestRequestTypeDef",
-    "GetComponentResponseTypeDef",
     "GetComponentVersionArtifactRequestRequestTypeDef",
-    "GetComponentVersionArtifactResponseTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetCoreDeviceRequestRequestTypeDef",
-    "GetCoreDeviceResponseTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
     "InstalledComponentTypeDef",
-    "IoTJobAbortCriteriaOutputTypeDef",
     "IoTJobAbortCriteriaTypeDef",
-    "IoTJobRateIncreaseCriteriaOutputTypeDef",
     "IoTJobRateIncreaseCriteriaTypeDef",
     "LambdaDeviceMountTypeDef",
     "LambdaVolumeMountTypeDef",
     "LambdaEventSourceTypeDef",
-    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
-    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentVersionsRequestRequestTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListCoreDevicesRequestRequestTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
-    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestRequestTypeDef",
-    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ListInstalledComponentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "ResolvedComponentVersionTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
+    "CancelDeploymentResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetComponentResponseTypeDef",
+    "GetComponentVersionArtifactResponseTypeDef",
+    "GetCoreDeviceResponseTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
-    "ComponentRunWithOutputTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
-    "DeploymentPoliciesOutputTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
     "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
-    "IoTJobExponentialRolloutRateOutputTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
+    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
     "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
-    "IoTJobExecutionsRolloutConfigOutputTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
     "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
     "GetDeploymentResponseTypeDef",
@@ -187,19 +177,22 @@
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "associatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociatedClientDeviceTypeDef = TypedDict(
     "AssociatedClientDeviceTypeDef",
     {
         "thingName": str,
@@ -228,22 +221,14 @@
 CancelDeploymentRequestRequestTypeDef = TypedDict(
     "CancelDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
-CancelDeploymentResponseTypeDef = TypedDict(
-    "CancelDeploymentResponseTypeDef",
-    {
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CloudComponentStatusTypeDef = TypedDict(
     "CloudComponentStatusTypeDef",
     {
         "componentState": CloudComponentStateType,
         "message": str,
         "errors": Dict[str, str],
         "vendorGuidance": VendorGuidanceType,
@@ -303,23 +288,14 @@
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
-SystemResourceLimitsOutputTypeDef = TypedDict(
-    "SystemResourceLimitsOutputTypeDef",
-    {
-        "memory": int,
-        "cpus": float,
-    },
-    total=False,
-)
-
 SystemResourceLimitsTypeDef = TypedDict(
     "SystemResourceLimitsTypeDef",
     {
         "memory": int,
         "cpus": float,
     },
     total=False,
@@ -331,25 +307,14 @@
         "componentName": str,
         "componentVersion": str,
         "arn": str,
     },
     total=False,
 )
 
-ConnectivityInfoOutputTypeDef = TypedDict(
-    "ConnectivityInfoOutputTypeDef",
-    {
-        "id": str,
-        "hostAddress": str,
-        "portNumber": int,
-        "metadata": str,
-    },
-    total=False,
-)
-
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "id": str,
         "hostAddress": str,
         "portNumber": int,
         "metadata": str,
@@ -363,24 +328,14 @@
         "coreDeviceThingName": str,
         "status": CoreDeviceStatusType,
         "lastStatusUpdateTimestamp": datetime,
     },
     total=False,
 )
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -394,56 +349,31 @@
 DeleteDeploymentRequestRequestTypeDef = TypedDict(
     "DeleteDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
-DeploymentComponentUpdatePolicyOutputTypeDef = TypedDict(
-    "DeploymentComponentUpdatePolicyOutputTypeDef",
-    {
-        "timeoutInSeconds": int,
-        "action": DeploymentComponentUpdatePolicyActionType,
-    },
-    total=False,
-)
-
 DeploymentComponentUpdatePolicyTypeDef = TypedDict(
     "DeploymentComponentUpdatePolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "action": DeploymentComponentUpdatePolicyActionType,
     },
     total=False,
 )
 
-DeploymentConfigurationValidationPolicyOutputTypeDef = TypedDict(
-    "DeploymentConfigurationValidationPolicyOutputTypeDef",
-    {
-        "timeoutInSeconds": int,
-    },
-    total=False,
-)
-
 DeploymentConfigurationValidationPolicyTypeDef = TypedDict(
     "DeploymentConfigurationValidationPolicyTypeDef",
     {
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
-IoTJobTimeoutConfigOutputTypeDef = TypedDict(
-    "IoTJobTimeoutConfigOutputTypeDef",
-    {
-        "inProgressTimeoutInMinutes": int,
-    },
-    total=False,
-)
-
 IoTJobTimeoutConfigTypeDef = TypedDict(
     "IoTJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
@@ -466,127 +396,73 @@
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "disassociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EffectiveDeploymentStatusDetailsTypeDef = TypedDict(
     "EffectiveDeploymentStatusDetailsTypeDef",
     {
         "errorStack": List[str],
         "errorTypes": List[str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetComponentRequestRequestTypeDef = TypedDict(
     "_RequiredGetComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetComponentRequestRequestTypeDef = TypedDict(
     "_OptionalGetComponentRequestRequestTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
     },
     total=False,
 )
 
+
 class GetComponentRequestRequestTypeDef(
     _RequiredGetComponentRequestRequestTypeDef, _OptionalGetComponentRequestRequestTypeDef
 ):
     pass
 
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
-    {
-        "recipeOutputFormat": RecipeOutputFormatType,
-        "recipe": bytes,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetComponentVersionArtifactRequestRequestTypeDef = TypedDict(
     "GetComponentVersionArtifactRequestRequestTypeDef",
     {
         "arn": str,
         "artifactName": str,
     },
 )
 
-GetComponentVersionArtifactResponseTypeDef = TypedDict(
-    "GetComponentVersionArtifactResponseTypeDef",
-    {
-        "preSignedUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConnectivityInfoRequestRequestTypeDef = TypedDict(
     "GetConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
 GetCoreDeviceRequestRequestTypeDef = TypedDict(
     "GetCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 
-GetCoreDeviceResponseTypeDef = TypedDict(
-    "GetCoreDeviceResponseTypeDef",
-    {
-        "coreDeviceThingName": str,
-        "coreVersion": str,
-        "platform": str,
-        "architecture": str,
-        "status": CoreDeviceStatusType,
-        "lastStatusUpdateTimestamp": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDeploymentRequestRequestTypeDef = TypedDict(
     "GetDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "associatedAt": str,
-        "roleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InstalledComponentTypeDef = TypedDict(
     "InstalledComponentTypeDef",
     {
         "componentName": str,
         "componentVersion": str,
         "lifecycleState": InstalledComponentLifecycleStateType,
         "lifecycleStateDetails": str,
@@ -595,43 +471,24 @@
         "lastReportedTimestamp": datetime,
         "lastInstallationSource": str,
         "lifecycleStatusCodes": List[str],
     },
     total=False,
 )
 
-IoTJobAbortCriteriaOutputTypeDef = TypedDict(
-    "IoTJobAbortCriteriaOutputTypeDef",
-    {
-        "failureType": IoTJobExecutionFailureTypeType,
-        "action": Literal["CANCEL"],
-        "thresholdPercentage": float,
-        "minNumberOfExecutedThings": int,
-    },
-)
-
 IoTJobAbortCriteriaTypeDef = TypedDict(
     "IoTJobAbortCriteriaTypeDef",
     {
         "failureType": IoTJobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
-IoTJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
-    "IoTJobRateIncreaseCriteriaOutputTypeDef",
-    {
-        "numberOfNotifiedThings": int,
-        "numberOfSucceededThings": int,
-    },
-    total=False,
-)
-
 IoTJobRateIncreaseCriteriaTypeDef = TypedDict(
     "IoTJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
@@ -648,19 +505,21 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
+
 class LambdaDeviceMountTypeDef(
     _RequiredLambdaDeviceMountTypeDef, _OptionalLambdaDeviceMountTypeDef
 ):
     pass
 
+
 _RequiredLambdaVolumeMountTypeDef = TypedDict(
     "_RequiredLambdaVolumeMountTypeDef",
     {
         "sourcePath": str,
         "destinationPath": str,
     },
 )
@@ -669,47 +528,39 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
+
 class LambdaVolumeMountTypeDef(
     _RequiredLambdaVolumeMountTypeDef, _OptionalLambdaVolumeMountTypeDef
 ):
     pass
 
+
 LambdaEventSourceTypeDef = TypedDict(
     "LambdaEventSourceTypeDef",
     {
         "topic": str,
         "type": LambdaEventSourceTypeType,
     },
 )
 
-_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
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
 
-class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
-    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-):
-    pass
-
 _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
@@ -717,39 +568,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
-    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListComponentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
@@ -758,103 +591,55 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListComponentVersionsRequestRequestTypeDef(
     _RequiredListComponentVersionsRequestRequestTypeDef,
     _OptionalListComponentVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsRequestListComponentsPaginateTypeDef",
-    {
-        "scope": ComponentVisibilityScopeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListComponentsRequestRequestTypeDef = TypedDict(
     "ListComponentsRequestRequestTypeDef",
     {
         "scope": ComponentVisibilityScopeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
-    {
-        "thingGroupArn": str,
-        "status": CoreDeviceStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCoreDevicesRequestRequestTypeDef = TypedDict(
     "ListCoreDevicesRequestRequestTypeDef",
     {
         "thingGroupArn": str,
         "status": CoreDeviceStatusType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "targetArn": str,
-        "historyFilter": DeploymentHistoryFilterType,
-        "parentTargetArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentsRequestRequestTypeDef = TypedDict(
     "ListDeploymentsRequestRequestTypeDef",
     {
         "targetArn": str,
         "historyFilter": DeploymentHistoryFilterType,
         "parentTargetArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
-    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListEffectiveDeploymentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
@@ -862,40 +647,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEffectiveDeploymentsRequestRequestTypeDef(
     _RequiredListEffectiveDeploymentsRequestRequestTypeDef,
     _OptionalListEffectiveDeploymentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "topologyFilter": InstalledComponentTopologyFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
-    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-):
-    pass
 
 _RequiredListInstalledComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
@@ -905,69 +671,42 @@
         "maxResults": int,
         "nextToken": str,
         "topologyFilter": InstalledComponentTopologyFilterType,
     },
     total=False,
 )
 
+
 class ListInstalledComponentsRequestRequestTypeDef(
     _RequiredListInstalledComponentsRequestRequestTypeDef,
     _OptionalListInstalledComponentsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 ResolvedComponentVersionTypeDef = TypedDict(
     "ResolvedComponentVersionTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "recipe": bytes,
         "vendorGuidance": VendorGuidanceType,
         "message": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -976,57 +715,149 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "version": str,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
+
 class BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef(
     _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
     _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    {
+        "associatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef = TypedDict(
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelDeploymentResponseTypeDef = TypedDict(
+    "CancelDeploymentResponseTypeDef",
+    {
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "disassociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
+    {
+        "recipeOutputFormat": RecipeOutputFormatType,
+        "recipe": bytes,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentVersionArtifactResponseTypeDef = TypedDict(
+    "GetComponentVersionArtifactResponseTypeDef",
+    {
+        "preSignedUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCoreDeviceResponseTypeDef = TypedDict(
+    "GetCoreDeviceResponseTypeDef",
+    {
+        "coreDeviceThingName": str,
+        "coreVersion": str,
+        "platform": str,
+        "architecture": str,
+        "status": CoreDeviceStatusType,
+        "lastStatusUpdateTimestamp": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "associatedAt": str,
+        "roleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "version": str,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef = TypedDict(
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     {
         "associatedClientDevices": List[AssociatedClientDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
@@ -1036,37 +867,39 @@
     "_OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
+
 class BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef(
     _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     _OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef = TypedDict(
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateComponentVersionResponseTypeDef = TypedDict(
     "CreateComponentVersionResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "status": CloudComponentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentLatestVersionTypeDef = TypedDict(
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
@@ -1087,37 +920,27 @@
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
         "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
 )
 
-ComponentRunWithOutputTypeDef = TypedDict(
-    "ComponentRunWithOutputTypeDef",
-    {
-        "posixUser": str,
-        "systemResourceLimits": SystemResourceLimitsOutputTypeDef,
-        "windowsUser": str,
-    },
-    total=False,
-)
-
 ComponentRunWithTypeDef = TypedDict(
     "ComponentRunWithTypeDef",
     {
         "posixUser": str,
         "systemResourceLimits": SystemResourceLimitsTypeDef,
         "windowsUser": str,
     },
@@ -1125,24 +948,24 @@
 )
 
 ListComponentVersionsResponseTypeDef = TypedDict(
     "ListComponentVersionsResponseTypeDef",
     {
         "componentVersions": List[ComponentVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "connectivityInfo": List[ConnectivityInfoOutputTypeDef],
+        "connectivityInfo": List[ConnectivityInfoTypeDef],
         "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
@@ -1151,26 +974,16 @@
 )
 
 ListCoreDevicesResponseTypeDef = TypedDict(
     "ListCoreDevicesResponseTypeDef",
     {
         "coreDevices": List[CoreDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeploymentPoliciesOutputTypeDef = TypedDict(
-    "DeploymentPoliciesOutputTypeDef",
-    {
-        "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
-        "componentUpdatePolicy": DeploymentComponentUpdatePolicyOutputTypeDef,
-        "configurationValidationPolicy": DeploymentConfigurationValidationPolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DeploymentPoliciesTypeDef = TypedDict(
     "DeploymentPoliciesTypeDef",
     {
         "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
         "componentUpdatePolicy": DeploymentComponentUpdatePolicyTypeDef,
@@ -1180,15 +993,15 @@
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEffectiveDeploymentTypeDef = TypedDict(
     "_RequiredEffectiveDeploymentTypeDef",
     {
         "deploymentId": str,
@@ -1207,51 +1020,44 @@
         "description": str,
         "reason": str,
         "statusDetails": EffectiveDeploymentStatusDetailsTypeDef,
     },
     total=False,
 )
 
+
 class EffectiveDeploymentTypeDef(
     _RequiredEffectiveDeploymentTypeDef, _OptionalEffectiveDeploymentTypeDef
 ):
     pass
 
+
 ListInstalledComponentsResponseTypeDef = TypedDict(
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IoTJobAbortConfigOutputTypeDef = TypedDict(
     "IoTJobAbortConfigOutputTypeDef",
     {
-        "criteriaList": List[IoTJobAbortCriteriaOutputTypeDef],
+        "criteriaList": List[IoTJobAbortCriteriaTypeDef],
     },
 )
 
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 
-IoTJobExponentialRolloutRateOutputTypeDef = TypedDict(
-    "IoTJobExponentialRolloutRateOutputTypeDef",
-    {
-        "baseRatePerMinute": int,
-        "incrementFactor": float,
-        "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaOutputTypeDef,
-    },
-)
-
 IoTJobExponentialRolloutRateTypeDef = TypedDict(
     "IoTJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": IoTJobRateIncreaseCriteriaTypeDef,
     },
@@ -1264,19 +1070,138 @@
         "mountROSysfs": bool,
         "volumes": Sequence[LambdaVolumeMountTypeDef],
         "devices": Sequence[LambdaDeviceMountTypeDef],
     },
     total=False,
 )
 
+_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
+    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
+    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    {
+        "scope": ComponentVisibilityScopeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
+    {
+        "thingGroupArn": str,
+        "status": CoreDeviceStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "targetArn": str,
+        "historyFilter": DeploymentHistoryFilterType,
+        "parentTargetArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
+    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "topologyFilter": InstalledComponentTopologyFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
+    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+):
+    pass
+
+
 ResolveComponentCandidatesResponseTypeDef = TypedDict(
     "ResolveComponentCandidatesResponseTypeDef",
     {
         "resolvedComponentVersions": List[ResolvedComponentVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "arn": str,
@@ -1287,15 +1212,15 @@
 )
 
 ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
     "ComponentDeploymentSpecificationOutputTypeDef",
     {
         "componentVersion": str,
         "configurationUpdate": ComponentConfigurationUpdateOutputTypeDef,
-        "runWith": ComponentRunWithOutputTypeDef,
+        "runWith": ComponentRunWithTypeDef,
     },
     total=False,
 )
 
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
@@ -1307,27 +1232,18 @@
 )
 
 ListEffectiveDeploymentsResponseTypeDef = TypedDict(
     "ListEffectiveDeploymentsResponseTypeDef",
     {
         "effectiveDeployments": List[EffectiveDeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IoTJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
-    "IoTJobExecutionsRolloutConfigOutputTypeDef",
-    {
-        "exponentialRate": IoTJobExponentialRolloutRateOutputTypeDef,
-        "maximumPerMinute": int,
-    },
-    total=False,
-)
-
 IoTJobExecutionsRolloutConfigTypeDef = TypedDict(
     "IoTJobExecutionsRolloutConfigTypeDef",
     {
         "exponentialRate": IoTJobExponentialRolloutRateTypeDef,
         "maximumPerMinute": int,
     },
     total=False,
@@ -1343,24 +1259,24 @@
 )
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationOutputTypeDef",
     {
-        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigOutputTypeDef,
+        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigOutputTypeDef,
-        "timeoutConfig": IoTJobTimeoutConfigOutputTypeDef,
+        "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
     total=False,
 )
 
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
@@ -1396,21 +1312,21 @@
         "revisionId": str,
         "deploymentId": str,
         "deploymentName": str,
         "deploymentStatus": DeploymentStatusType,
         "iotJobId": str,
         "iotJobArn": str,
         "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
-        "deploymentPolicies": DeploymentPoliciesOutputTypeDef,
+        "deploymentPolicies": DeploymentPoliciesTypeDef,
         "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
         "creationTimestamp": datetime,
         "isLatestForTarget": bool,
         "parentTargetArn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "targetArn": str,
@@ -1426,19 +1342,21 @@
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
 _OptionalLambdaFunctionRecipeSourceTypeDef = TypedDict(
@@ -1449,19 +1367,21 @@
         "componentPlatforms": Sequence[ComponentPlatformTypeDef],
         "componentDependencies": Mapping[str, ComponentDependencyRequirementTypeDef],
         "componentLambdaParameters": LambdaExecutionParametersTypeDef,
     },
     total=False,
 )
 
+
 class LambdaFunctionRecipeSourceTypeDef(
     _RequiredLambdaFunctionRecipeSourceTypeDef, _OptionalLambdaFunctionRecipeSourceTypeDef
 ):
     pass
 
+
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
         "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/PKG-INFO` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.28.12
-Summary: Type annotations for boto3.GreengrassV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GreengrassV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,118 +369,107 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
-    CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformOutputTypeDef,
     ComponentPlatformTypeDef,
-    SystemResourceLimitsOutputTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
-    CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
-    DeploymentComponentUpdatePolicyOutputTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
-    DeploymentConfigurationValidationPolicyOutputTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
-    IoTJobTimeoutConfigOutputTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetComponentVersionArtifactRequestRequestTypeDef,
-    GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
-    GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
-    IoTJobAbortCriteriaOutputTypeDef,
     IoTJobAbortCriteriaTypeDef,
-    IoTJobRateIncreaseCriteriaOutputTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
-    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
-    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     ListComponentVersionsRequestRequestTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
     ListCoreDevicesRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     ListEffectiveDeploymentsRequestRequestTypeDef,
-    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ListInstalledComponentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResolvedComponentVersionTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
+    CancelDeploymentResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetComponentResponseTypeDef,
+    GetComponentVersionArtifactResponseTypeDef,
+    GetCoreDeviceResponseTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
-    ComponentRunWithOutputTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
-    DeploymentPoliciesOutputTypeDef,
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
     IoTJobAbortConfigOutputTypeDef,
     IoTJobAbortConfigTypeDef,
-    IoTJobExponentialRolloutRateOutputTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
+    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
     ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
-    IoTJobExecutionsRolloutConfigOutputTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
     DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
     GetDeploymentResponseTypeDef,
```

### Comparing `mypy-boto3-greengrassv2-1.28.12/mypy_boto3_greengrassv2.egg-info/SOURCES.txt` & `mypy-boto3-greengrassv2-1.28.15/mypy_boto3_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.12/setup.py` & `mypy-boto3-greengrassv2-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrassv2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GreengrassV2 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.GreengrassV2 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

