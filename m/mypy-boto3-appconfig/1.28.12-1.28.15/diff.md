# Comparing `tmp/mypy-boto3-appconfig-1.28.12.tar.gz` & `tmp/mypy-boto3-appconfig-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appconfig-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
+gzip compressed data, was "mypy-boto3-appconfig-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-appconfig-1.28.12.tar` & `mypy-boto3-appconfig-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.340584 mypy-boto3-appconfig-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-27 05:34:16.332584 mypy-boto3-appconfig-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32185 2023-07-27 05:17:17.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32138 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.340584 mypy-boto3-appconfig-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.240654 mypy-boto3-appconfig-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-28 20:42:16.240654 mypy-boto3-appconfig-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.232654 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28973 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28924 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-07-28 20:19:14.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31041 2023-07-28 20:19:13.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.240654 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-28 20:42:15.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 20:42:16.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:15.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:15.000000 mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.240654 mypy-boto3-appconfig-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:19:12.000000 mypy-boto3-appconfig-1.28.15/setup.py
```

### Comparing `mypy-boto3-appconfig-1.28.12/LICENSE` & `mypy-boto3-appconfig-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.12/PKG-INFO` & `mypy-boto3-appconfig-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.28.12
-Summary: Type annotations for boto3.AppConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppConfig 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,92 +304,88 @@
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
-    ValidatorOutputTypeDef,
-    ConfigurationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
     ValidatorTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
-    MonitorOutputTypeDef,
     ExtensionAssociationSummaryTypeDef,
-    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
-    ParameterOutputTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
-    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagsTypeDef,
-    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
+    ApplicationResponseTypeDef,
+    ConfigurationTypeDef,
+    DeploymentStrategyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExtensionAssociationTypeDef,
+    HostedConfigurationVersionTypeDef,
+    ResourceTagsTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    EnvironmentResponseTypeDef,
+    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
+    ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
-    EnvironmentResponseMetadataTypeDef,
-    EnvironmentTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionsTypeDef,
-    ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
 def get_structure() -> ActionInvocationTypeDef:
```

### Comparing `mypy-boto3-appconfig-1.28.12/README.md` & `mypy-boto3-appconfig-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,92 +272,88 @@
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
-    ValidatorOutputTypeDef,
-    ConfigurationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
     ValidatorTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
-    MonitorOutputTypeDef,
     ExtensionAssociationSummaryTypeDef,
-    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
-    ParameterOutputTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
-    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagsTypeDef,
-    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
+    ApplicationResponseTypeDef,
+    ConfigurationTypeDef,
+    DeploymentStrategyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExtensionAssociationTypeDef,
+    HostedConfigurationVersionTypeDef,
+    ResourceTagsTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    EnvironmentResponseTypeDef,
+    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
+    ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
-    EnvironmentResponseMetadataTypeDef,
-    EnvironmentTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionsTypeDef,
-    ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
 def get_structure() -> ActionInvocationTypeDef:
```

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__main__.py` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppConfig 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppConfig 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
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

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.py` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import ActionPointType, GrowthTypeType, ReplicateToType
 from .type_defs import (
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ApplicationResponseTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     ConfigurationTypeDef,
     DeploymentStrategiesTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
+    DeploymentStrategyResponseTypeDef,
     DeploymentsTypeDef,
     DeploymentTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentResponseMetadataTypeDef,
+    EnvironmentResponseTypeDef,
     EnvironmentsTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionAssociationTypeDef,
     ExtensionsTypeDef,
     ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     HostedConfigurationVersionTypeDef,
@@ -97,15 +97,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#close)
         """
 
     def create_application(
         self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#create_application)
         """
 
@@ -136,15 +136,15 @@
         DeploymentDurationInMinutes: int,
         GrowthFactor: float,
         Description: str = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthType: GrowthTypeType = ...,
         ReplicateTo: ReplicateToType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Creates a deployment strategy that defines important criteria for rolling out
         your configuration to the designated targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_deployment_strategy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#create_deployment_strategy)
         """
@@ -153,15 +153,15 @@
         self,
         *,
         ApplicationId: str,
         Name: str,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Creates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#create_environment)
         """
 
@@ -297,15 +297,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#generate_presigned_url)
         """
 
-    def get_application(self, *, ApplicationId: str) -> ApplicationResponseMetadataTypeDef:
+    def get_application(self, *, ApplicationId: str) -> ApplicationResponseTypeDef:
         """
         Retrieves information about an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_application)
         """
 
@@ -343,25 +343,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_deployment)
         """
 
     def get_deployment_strategy(
         self, *, DeploymentStrategyId: str
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Retrieves information about a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment_strategy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_deployment_strategy)
         """
 
     def get_environment(
         self, *, ApplicationId: str, EnvironmentId: str
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Retrieves information about an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_environment)
         """
 
@@ -544,15 +544,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#untag_resource)
         """
 
     def update_application(
         self, *, ApplicationId: str, Name: str = ..., Description: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#update_application)
         """
 
@@ -578,15 +578,15 @@
         *,
         DeploymentStrategyId: str,
         Description: str = ...,
         DeploymentDurationInMinutes: int = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthFactor: float = ...,
         GrowthType: GrowthTypeType = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Updates a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_deployment_strategy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#update_deployment_strategy)
         """
 
@@ -594,15 +594,15 @@
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
         Name: str = ...,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#update_environment)
         """
```

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.pyi` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import ActionPointType, GrowthTypeType, ReplicateToType
 from .type_defs import (
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ApplicationResponseTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     ConfigurationTypeDef,
     DeploymentStrategiesTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
+    DeploymentStrategyResponseTypeDef,
     DeploymentsTypeDef,
     DeploymentTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentResponseMetadataTypeDef,
+    EnvironmentResponseTypeDef,
     EnvironmentsTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionAssociationTypeDef,
     ExtensionsTypeDef,
     ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     HostedConfigurationVersionTypeDef,
@@ -91,15 +91,15 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#close)
         """
     def create_application(
         self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#create_application)
         """
     def create_configuration_profile(
@@ -128,15 +128,15 @@
         DeploymentDurationInMinutes: int,
         GrowthFactor: float,
         Description: str = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthType: GrowthTypeType = ...,
         ReplicateTo: ReplicateToType = ...,
         Tags: Mapping[str, str] = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Creates a deployment strategy that defines important criteria for rolling out
         your configuration to the designated targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_deployment_strategy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#create_deployment_strategy)
         """
@@ -144,15 +144,15 @@
         self,
         *,
         ApplicationId: str,
         Name: str,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...,
         Tags: Mapping[str, str] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Creates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.create_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#create_environment)
         """
     def create_extension(
@@ -276,15 +276,15 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#generate_presigned_url)
         """
-    def get_application(self, *, ApplicationId: str) -> ApplicationResponseMetadataTypeDef:
+    def get_application(self, *, ApplicationId: str) -> ApplicationResponseTypeDef:
         """
         Retrieves information about an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_application)
         """
     def get_configuration(
@@ -318,24 +318,24 @@
         Retrieves information about a configuration deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_deployment)
         """
     def get_deployment_strategy(
         self, *, DeploymentStrategyId: str
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Retrieves information about a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_deployment_strategy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_deployment_strategy)
         """
     def get_environment(
         self, *, ApplicationId: str, EnvironmentId: str
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Retrieves information about an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#get_environment)
         """
     def get_extension(
@@ -501,15 +501,15 @@
         Deletes a tag key and value from an AppConfig resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#untag_resource)
         """
     def update_application(
         self, *, ApplicationId: str, Name: str = ..., Description: str = ...
-    ) -> ApplicationResponseMetadataTypeDef:
+    ) -> ApplicationResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#update_application)
         """
     def update_configuration_profile(
@@ -533,30 +533,30 @@
         *,
         DeploymentStrategyId: str,
         Description: str = ...,
         DeploymentDurationInMinutes: int = ...,
         FinalBakeTimeInMinutes: int = ...,
         GrowthFactor: float = ...,
         GrowthType: GrowthTypeType = ...
-    ) -> DeploymentStrategyResponseMetadataTypeDef:
+    ) -> DeploymentStrategyResponseTypeDef:
         """
         Updates a deployment strategy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_deployment_strategy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#update_deployment_strategy)
         """
     def update_environment(
         self,
         *,
         ApplicationId: str,
         EnvironmentId: str,
         Name: str = ...,
         Description: str = ...,
         Monitors: Sequence[MonitorTypeDef] = ...
-    ) -> EnvironmentResponseMetadataTypeDef:
+    ) -> EnvironmentResponseTypeDef:
         """
         Updates an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#update_environment)
         """
     def update_extension(
```

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.py` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.pyi` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.py` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,92 +32,88 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActionInvocationTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
-    "ApplicationResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
     "ConfigurationProfileSummaryTypeDef",
-    "ValidatorOutputTypeDef",
-    "ConfigurationTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
     "ValidatorTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
     "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
-    "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "MonitorOutputTypeDef",
     "ExtensionAssociationSummaryTypeDef",
-    "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
-    "ParameterOutputTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
     "GetExtensionRequestRequestTypeDef",
     "GetHostedConfigurationVersionRequestRequestTypeDef",
     "HostedConfigurationVersionSummaryTypeDef",
-    "HostedConfigurationVersionTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListConfigurationProfilesRequestRequestTypeDef",
     "ListDeploymentStrategiesRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListExtensionAssociationsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListHostedConfigurationVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResourceTagsTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateDeploymentStrategyRequestRequestTypeDef",
     "UpdateExtensionAssociationRequestRequestTypeDef",
     "ValidateConfigurationRequestRequestTypeDef",
     "DeploymentEventTypeDef",
+    "ApplicationResponseTypeDef",
+    "ConfigurationTypeDef",
+    "DeploymentStrategyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExtensionAssociationTypeDef",
+    "HostedConfigurationVersionTypeDef",
+    "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "EnvironmentResponseTypeDef",
+    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateExtensionRequestRequestTypeDef",
+    "ExtensionTypeDef",
     "UpdateExtensionRequestRequestTypeDef",
     "DeploymentStrategiesTypeDef",
     "DeploymentsTypeDef",
-    "EnvironmentResponseMetadataTypeDef",
-    "EnvironmentTypeDef",
     "ExtensionAssociationsTypeDef",
     "ExtensionsTypeDef",
-    "ExtensionTypeDef",
     "HostedConfigurationVersionsTypeDef",
     "DeploymentTypeDef",
     "EnvironmentsTypeDef",
 )
 
 ActionInvocationTypeDef = TypedDict(
     "ActionInvocationTypeDef",
@@ -129,43 +125,33 @@
         "ErrorMessage": str,
         "ErrorCode": str,
         "InvocationId": str,
     },
     total=False,
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Uri": str,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "Name": str,
         "Description": str,
         "Uri": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Id": str,
@@ -195,32 +181,22 @@
         "LocationUri": str,
         "ValidatorTypes": List[ValidatorTypeType],
         "Type": str,
     },
     total=False,
 )
 
-ValidatorOutputTypeDef = TypedDict(
-    "ValidatorOutputTypeDef",
+ValidatorTypeDef = TypedDict(
+    "ValidatorTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Content": StreamingBody,
-        "ConfigurationVersion": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
@@ -235,22 +211,14 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-ValidatorTypeDef = TypedDict(
-    "ValidatorTypeDef",
-    {
-        "Type": ValidatorTypeType,
-        "Content": str,
-    },
-)
-
 _RequiredCreateDeploymentStrategyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentStrategyRequestRequestTypeDef",
     {
         "Name": str,
         "DeploymentDurationInMinutes": int,
         "GrowthFactor": float,
     },
@@ -433,29 +401,14 @@
         "GrowthFactor": float,
         "FinalBakeTimeInMinutes": int,
         "ReplicateTo": ReplicateToType,
     },
     total=False,
 )
 
-DeploymentStrategyResponseMetadataTypeDef = TypedDict(
-    "DeploymentStrategyResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "DeploymentDurationInMinutes": int,
-        "GrowthType": GrowthTypeType,
-        "GrowthFactor": float,
-        "FinalBakeTimeInMinutes": int,
-        "ReplicateTo": ReplicateToType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentSummaryTypeDef = TypedDict(
     "DeploymentSummaryTypeDef",
     {
         "DeploymentNumber": int,
         "ConfigurationName": str,
         "ConfigurationVersion": str,
         "DeploymentDurationInMinutes": int,
@@ -466,84 +419,36 @@
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
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
-_RequiredMonitorOutputTypeDef = TypedDict(
-    "_RequiredMonitorOutputTypeDef",
-    {
-        "AlarmArn": str,
-    },
-)
-_OptionalMonitorOutputTypeDef = TypedDict(
-    "_OptionalMonitorOutputTypeDef",
-    {
-        "AlarmRoleArn": str,
-    },
-    total=False,
-)
-
-
-class MonitorOutputTypeDef(_RequiredMonitorOutputTypeDef, _OptionalMonitorOutputTypeDef):
-    pass
-
-
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
-ExtensionAssociationTypeDef = TypedDict(
-    "ExtensionAssociationTypeDef",
-    {
-        "Id": str,
-        "ExtensionArn": str,
-        "ResourceArn": str,
-        "Arn": str,
-        "Parameters": Dict[str, str],
-        "ExtensionVersionNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionSummaryTypeDef = TypedDict(
     "ExtensionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
-    {
-        "Description": str,
-        "Required": bool,
-    },
-    total=False,
-)
-
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -649,28 +554,14 @@
         "Description": str,
         "ContentType": str,
         "VersionLabel": str,
     },
     total=False,
 )
 
-HostedConfigurationVersionTypeDef = TypedDict(
-    "HostedConfigurationVersionTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "VersionNumber": int,
-        "Description": str,
-        "Content": StreamingBody,
-        "ContentType": str,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -804,33 +695,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ResourceTagsTypeDef = TypedDict(
-    "ResourceTagsTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredStartDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDeploymentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
         "DeploymentStrategyId": str,
         "ConfigurationProfileId": str,
@@ -966,44 +838,121 @@
         "Description": str,
         "ActionInvocations": List[ActionInvocationTypeDef],
         "OccurredAt": datetime,
     },
     total=False,
 )
 
+ApplicationResponseTypeDef = TypedDict(
+    "ApplicationResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Content": StreamingBody,
+        "ConfigurationVersion": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeploymentStrategyResponseTypeDef = TypedDict(
+    "DeploymentStrategyResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "DeploymentDurationInMinutes": int,
+        "GrowthType": GrowthTypeType,
+        "GrowthFactor": float,
+        "FinalBakeTimeInMinutes": int,
+        "ReplicateTo": ReplicateToType,
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
+ExtensionAssociationTypeDef = TypedDict(
+    "ExtensionAssociationTypeDef",
+    {
+        "Id": str,
+        "ExtensionArn": str,
+        "ResourceArn": str,
+        "Arn": str,
+        "Parameters": Dict[str, str],
+        "ExtensionVersionNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HostedConfigurationVersionTypeDef = TypedDict(
+    "HostedConfigurationVersionTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "VersionNumber": int,
+        "Description": str,
+        "Content": StreamingBody,
+        "ContentType": str,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResourceTagsTypeDef = TypedDict(
+    "ResourceTagsTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplicationsTypeDef = TypedDict(
     "ApplicationsTypeDef",
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationProfileTypeDef = TypedDict(
     "ConfigurationProfileTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
-        "Validators": List[ValidatorOutputTypeDef],
+        "Validators": List[ValidatorTypeDef],
         "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -1077,14 +1026,40 @@
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
+EnvironmentResponseTypeDef = TypedDict(
+    "EnvironmentResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
     },
 )
@@ -1126,14 +1101,28 @@
 
 class CreateExtensionRequestRequestTypeDef(
     _RequiredCreateExtensionRequestRequestTypeDef, _OptionalCreateExtensionRequestRequestTypeDef
 ):
     pass
 
 
+ExtensionTypeDef = TypedDict(
+    "ExtensionTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "VersionNumber": int,
+        "Arn": str,
+        "Description": str,
+        "Actions": Dict[ActionPointType, List[ActionTypeDef]],
+        "Parameters": Dict[str, ParameterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
     },
 )
 _OptionalUpdateExtensionRequestRequestTypeDef = TypedDict(
@@ -1155,91 +1144,51 @@
 
 
 DeploymentStrategiesTypeDef = TypedDict(
     "DeploymentStrategiesTypeDef",
     {
         "Items": List[DeploymentStrategyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnvironmentResponseMetadataTypeDef = TypedDict(
-    "EnvironmentResponseMetadataTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorOutputTypeDef],
-    },
-    total=False,
-)
-
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtensionsTypeDef = TypedDict(
     "ExtensionsTypeDef",
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExtensionTypeDef = TypedDict(
-    "ExtensionTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "VersionNumber": int,
-        "Arn": str,
-        "Description": str,
-        "Actions": Dict[ActionPointType, List[ActionOutputTypeDef]],
-        "Parameters": Dict[str, ParameterOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "ApplicationId": str,
@@ -1259,19 +1208,19 @@
         "EventLog": List[DeploymentEventTypeDef],
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
         "AppliedExtensions": List[AppliedExtensionTypeDef],
         "KmsKeyArn": str,
         "KmsKeyIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentsTypeDef = TypedDict(
     "EnvironmentsTypeDef",
     {
         "Items": List[EnvironmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.pyi` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -31,92 +31,88 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionInvocationTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
-    "ApplicationResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
     "ConfigurationProfileSummaryTypeDef",
-    "ValidatorOutputTypeDef",
-    "ConfigurationTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
     "ValidatorTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
     "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
-    "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "MonitorOutputTypeDef",
     "ExtensionAssociationSummaryTypeDef",
-    "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
-    "ParameterOutputTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
     "GetExtensionRequestRequestTypeDef",
     "GetHostedConfigurationVersionRequestRequestTypeDef",
     "HostedConfigurationVersionSummaryTypeDef",
-    "HostedConfigurationVersionTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListConfigurationProfilesRequestRequestTypeDef",
     "ListDeploymentStrategiesRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListExtensionAssociationsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListHostedConfigurationVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResourceTagsTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateDeploymentStrategyRequestRequestTypeDef",
     "UpdateExtensionAssociationRequestRequestTypeDef",
     "ValidateConfigurationRequestRequestTypeDef",
     "DeploymentEventTypeDef",
+    "ApplicationResponseTypeDef",
+    "ConfigurationTypeDef",
+    "DeploymentStrategyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExtensionAssociationTypeDef",
+    "HostedConfigurationVersionTypeDef",
+    "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "EnvironmentResponseTypeDef",
+    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateExtensionRequestRequestTypeDef",
+    "ExtensionTypeDef",
     "UpdateExtensionRequestRequestTypeDef",
     "DeploymentStrategiesTypeDef",
     "DeploymentsTypeDef",
-    "EnvironmentResponseMetadataTypeDef",
-    "EnvironmentTypeDef",
     "ExtensionAssociationsTypeDef",
     "ExtensionsTypeDef",
-    "ExtensionTypeDef",
     "HostedConfigurationVersionsTypeDef",
     "DeploymentTypeDef",
     "EnvironmentsTypeDef",
 )
 
 ActionInvocationTypeDef = TypedDict(
     "ActionInvocationTypeDef",
@@ -128,43 +124,33 @@
         "ErrorMessage": str,
         "ErrorCode": str,
         "InvocationId": str,
     },
     total=False,
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Uri": str,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "Name": str,
         "Description": str,
         "Uri": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Id": str,
@@ -194,32 +180,22 @@
         "LocationUri": str,
         "ValidatorTypes": List[ValidatorTypeType],
         "Type": str,
     },
     total=False,
 )
 
-ValidatorOutputTypeDef = TypedDict(
-    "ValidatorOutputTypeDef",
+ValidatorTypeDef = TypedDict(
+    "ValidatorTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Content": StreamingBody,
-        "ConfigurationVersion": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
@@ -232,22 +208,14 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-ValidatorTypeDef = TypedDict(
-    "ValidatorTypeDef",
-    {
-        "Type": ValidatorTypeType,
-        "Content": str,
-    },
-)
-
 _RequiredCreateDeploymentStrategyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentStrategyRequestRequestTypeDef",
     {
         "Name": str,
         "DeploymentDurationInMinutes": int,
         "GrowthFactor": float,
     },
@@ -420,29 +388,14 @@
         "GrowthFactor": float,
         "FinalBakeTimeInMinutes": int,
         "ReplicateTo": ReplicateToType,
     },
     total=False,
 )
 
-DeploymentStrategyResponseMetadataTypeDef = TypedDict(
-    "DeploymentStrategyResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "DeploymentDurationInMinutes": int,
-        "GrowthType": GrowthTypeType,
-        "GrowthFactor": float,
-        "FinalBakeTimeInMinutes": int,
-        "ReplicateTo": ReplicateToType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentSummaryTypeDef = TypedDict(
     "DeploymentSummaryTypeDef",
     {
         "DeploymentNumber": int,
         "ConfigurationName": str,
         "ConfigurationVersion": str,
         "DeploymentDurationInMinutes": int,
@@ -453,82 +406,36 @@
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
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
-_RequiredMonitorOutputTypeDef = TypedDict(
-    "_RequiredMonitorOutputTypeDef",
-    {
-        "AlarmArn": str,
-    },
-)
-_OptionalMonitorOutputTypeDef = TypedDict(
-    "_OptionalMonitorOutputTypeDef",
-    {
-        "AlarmRoleArn": str,
-    },
-    total=False,
-)
-
-class MonitorOutputTypeDef(_RequiredMonitorOutputTypeDef, _OptionalMonitorOutputTypeDef):
-    pass
-
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
-ExtensionAssociationTypeDef = TypedDict(
-    "ExtensionAssociationTypeDef",
-    {
-        "Id": str,
-        "ExtensionArn": str,
-        "ResourceArn": str,
-        "Arn": str,
-        "Parameters": Dict[str, str],
-        "ExtensionVersionNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionSummaryTypeDef = TypedDict(
     "ExtensionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
-    {
-        "Description": str,
-        "Required": bool,
-    },
-    total=False,
-)
-
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -630,28 +537,14 @@
         "Description": str,
         "ContentType": str,
         "VersionLabel": str,
     },
     total=False,
 )
 
-HostedConfigurationVersionTypeDef = TypedDict(
-    "HostedConfigurationVersionTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "VersionNumber": int,
-        "Description": str,
-        "Content": StreamingBody,
-        "ContentType": str,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -777,33 +670,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ResourceTagsTypeDef = TypedDict(
-    "ResourceTagsTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredStartDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDeploymentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
         "DeploymentStrategyId": str,
         "ConfigurationProfileId": str,
@@ -931,44 +805,121 @@
         "Description": str,
         "ActionInvocations": List[ActionInvocationTypeDef],
         "OccurredAt": datetime,
     },
     total=False,
 )
 
+ApplicationResponseTypeDef = TypedDict(
+    "ApplicationResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Content": StreamingBody,
+        "ConfigurationVersion": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeploymentStrategyResponseTypeDef = TypedDict(
+    "DeploymentStrategyResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "DeploymentDurationInMinutes": int,
+        "GrowthType": GrowthTypeType,
+        "GrowthFactor": float,
+        "FinalBakeTimeInMinutes": int,
+        "ReplicateTo": ReplicateToType,
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
+ExtensionAssociationTypeDef = TypedDict(
+    "ExtensionAssociationTypeDef",
+    {
+        "Id": str,
+        "ExtensionArn": str,
+        "ResourceArn": str,
+        "Arn": str,
+        "Parameters": Dict[str, str],
+        "ExtensionVersionNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HostedConfigurationVersionTypeDef = TypedDict(
+    "HostedConfigurationVersionTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "VersionNumber": int,
+        "Description": str,
+        "Content": StreamingBody,
+        "ContentType": str,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResourceTagsTypeDef = TypedDict(
+    "ResourceTagsTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplicationsTypeDef = TypedDict(
     "ApplicationsTypeDef",
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationProfileTypeDef = TypedDict(
     "ConfigurationProfileTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
-        "Validators": List[ValidatorOutputTypeDef],
+        "Validators": List[ValidatorTypeDef],
         "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -1036,14 +987,40 @@
 )
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+EnvironmentResponseTypeDef = TypedDict(
+    "EnvironmentResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
     },
 )
@@ -1081,14 +1058,28 @@
 )
 
 class CreateExtensionRequestRequestTypeDef(
     _RequiredCreateExtensionRequestRequestTypeDef, _OptionalCreateExtensionRequestRequestTypeDef
 ):
     pass
 
+ExtensionTypeDef = TypedDict(
+    "ExtensionTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "VersionNumber": int,
+        "Arn": str,
+        "Description": str,
+        "Actions": Dict[ActionPointType, List[ActionTypeDef]],
+        "Parameters": Dict[str, ParameterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
     },
 )
 _OptionalUpdateExtensionRequestRequestTypeDef = TypedDict(
@@ -1108,91 +1099,51 @@
     pass
 
 DeploymentStrategiesTypeDef = TypedDict(
     "DeploymentStrategiesTypeDef",
     {
         "Items": List[DeploymentStrategyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnvironmentResponseMetadataTypeDef = TypedDict(
-    "EnvironmentResponseMetadataTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorOutputTypeDef],
-    },
-    total=False,
-)
-
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtensionsTypeDef = TypedDict(
     "ExtensionsTypeDef",
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExtensionTypeDef = TypedDict(
-    "ExtensionTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "VersionNumber": int,
-        "Arn": str,
-        "Description": str,
-        "Actions": Dict[ActionPointType, List[ActionOutputTypeDef]],
-        "Parameters": Dict[str, ParameterOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "ApplicationId": str,
@@ -1212,19 +1163,19 @@
         "EventLog": List[DeploymentEventTypeDef],
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
         "AppliedExtensions": List[AppliedExtensionTypeDef],
         "KmsKeyArn": str,
         "KmsKeyIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentsTypeDef = TypedDict(
     "EnvironmentsTypeDef",
     {
         "Items": List[EnvironmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/PKG-INFO` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.28.12
-Summary: Type annotations for boto3.AppConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppConfig 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,92 +304,88 @@
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
-    ActionOutputTypeDef,
     ActionTypeDef,
-    ApplicationResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
-    ValidatorOutputTypeDef,
-    ConfigurationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
     ValidatorTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
-    MonitorOutputTypeDef,
     ExtensionAssociationSummaryTypeDef,
-    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
-    ParameterOutputTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
-    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResourceTagsTypeDef,
-    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
+    ApplicationResponseTypeDef,
+    ConfigurationTypeDef,
+    DeploymentStrategyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExtensionAssociationTypeDef,
+    HostedConfigurationVersionTypeDef,
+    ResourceTagsTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    EnvironmentResponseTypeDef,
+    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
+    ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
-    EnvironmentResponseMetadataTypeDef,
-    EnvironmentTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionsTypeDef,
-    ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
 def get_structure() -> ActionInvocationTypeDef:
```

### Comparing `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/SOURCES.txt` & `mypy-boto3-appconfig-1.28.15/mypy_boto3_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.12/setup.py` & `mypy-boto3-appconfig-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appconfig",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppConfig 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AppConfig 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

