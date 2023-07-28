# Comparing `tmp/mypy-boto3-greengrass-1.28.12.tar.gz` & `tmp/mypy-boto3-greengrass-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrass-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrass-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
```

## Comparing `mypy-boto3-greengrass-1.28.12.tar` & `mypy-boto3-greengrass-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.672500 mypy-boto3-greengrass-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-27 05:34:44.668500 mypy-boto3-greengrass-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27434 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.656499 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68595 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    99009 2023-07-27 05:23:07.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98880 2023-07-27 05:23:06.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.668500 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.672500 mypy-boto3-greengrass-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.121170 mypy-boto3-greengrass-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28275 2023-07-28 20:42:53.113170 mypy-boto3-greengrass-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.105169 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68595 2023-07-28 20:27:01.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-28 20:27:02.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93312 2023-07-28 20:27:04.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93191 2023-07-28 20:27:03.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.109169 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28275 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:52.000000 mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.121170 mypy-boto3-greengrass-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:26:59.000000 mypy-boto3-greengrass-1.28.15/setup.py
```

### Comparing `mypy-boto3-greengrass-1.28.12/LICENSE` & `mypy-boto3-greengrass-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/PKG-INFO` & `mypy-boto3-greengrass-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.28.12
-Summary: Type annotations for boto3.Greengrass 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,255 +423,238 @@
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
-    AssociateRoleToGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     ConnectorOutputTypeDef,
     ConnectorTypeDef,
-    CoreOutputTypeDef,
     CoreTypeDef,
-    CreateConnectorDefinitionResponseTypeDef,
-    CreateConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionResponseTypeDef,
-    CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateDeviceDefinitionResponseTypeDef,
     DeviceTypeDef,
-    CreateDeviceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionResponseTypeDef,
-    CreateFunctionDefinitionVersionResponseTypeDef,
     CreateGroupCertificateAuthorityRequestRequestTypeDef,
-    CreateGroupCertificateAuthorityResponseTypeDef,
     GroupVersionTypeDef,
-    CreateGroupResponseTypeDef,
     CreateGroupVersionRequestRequestTypeDef,
-    CreateGroupVersionResponseTypeDef,
-    CreateLoggerDefinitionResponseTypeDef,
     LoggerTypeDef,
-    CreateLoggerDefinitionVersionResponseTypeDef,
-    CreateResourceDefinitionResponseTypeDef,
-    CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobRequestRequestTypeDef,
-    CreateSoftwareUpdateJobResponseTypeDef,
-    CreateSubscriptionDefinitionResponseTypeDef,
     SubscriptionTypeDef,
-    CreateSubscriptionDefinitionVersionResponseTypeDef,
     DefinitionInformationTypeDef,
     DeleteConnectorDefinitionRequestRequestTypeDef,
     DeleteCoreDefinitionRequestRequestTypeDef,
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DeviceOutputTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
-    DisassociateRoleFromGroupResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ResourceAccessPolicyOutputTypeDef,
     ResourceAccessPolicyTypeDef,
-    FunctionRunAsConfigOutputTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
-    GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
-    GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionRequestRequestTypeDef,
-    GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionRequestRequestTypeDef,
     GetDeploymentStatusRequestRequestTypeDef,
     GetDeviceDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionResponseTypeDef,
     GetDeviceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionRequestRequestTypeDef,
-    GetFunctionDefinitionResponseTypeDef,
     GetFunctionDefinitionVersionRequestRequestTypeDef,
     GetGroupCertificateAuthorityRequestRequestTypeDef,
-    GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
-    GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
-    GroupVersionOutputTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
-    GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
-    GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
-    GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
-    GroupOwnerSettingOutputTypeDef,
     GroupOwnerSettingTypeDef,
-    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
-    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
-    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
     VersionInformationTypeDef,
-    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
     ListConnectorDefinitionsRequestRequestTypeDef,
-    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     ListCoreDefinitionVersionsRequestRequestTypeDef,
-    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
     ListCoreDefinitionsRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     ListDeviceDefinitionVersionsRequestRequestTypeDef,
-    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
     ListDeviceDefinitionsRequestRequestTypeDef,
-    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     ListFunctionDefinitionVersionsRequestRequestTypeDef,
-    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
     ListFunctionDefinitionsRequestRequestTypeDef,
     ListGroupCertificateAuthoritiesRequestRequestTypeDef,
-    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     ListGroupVersionsRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     ListLoggerDefinitionVersionsRequestRequestTypeDef,
-    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
     ListLoggerDefinitionsRequestRequestTypeDef,
-    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     ListResourceDefinitionVersionsRequestRequestTypeDef,
-    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
     ListResourceDefinitionsRequestRequestTypeDef,
-    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
-    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LoggerOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
-    ResetDeploymentsResponseTypeDef,
     SecretsManagerSecretResourceDataOutputTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
-    ResourceDownloadOwnerSettingOutputTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
-    ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
-    StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
-    SubscriptionOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
     UpdateFunctionDefinitionRequestRequestTypeDef,
     UpdateGroupCertificateConfigurationRequestRequestTypeDef,
-    UpdateGroupCertificateConfigurationResponseTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateLoggerDefinitionRequestRequestTypeDef,
     UpdateResourceDefinitionRequestRequestTypeDef,
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
+    AssociateRoleToGroupResponseTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
+    CreateConnectorDefinitionResponseTypeDef,
+    CreateConnectorDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionResponseTypeDef,
+    CreateCoreDefinitionVersionResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateDeviceDefinitionResponseTypeDef,
+    CreateDeviceDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionResponseTypeDef,
+    CreateFunctionDefinitionVersionResponseTypeDef,
+    CreateGroupCertificateAuthorityResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateGroupVersionResponseTypeDef,
+    CreateLoggerDefinitionResponseTypeDef,
+    CreateLoggerDefinitionVersionResponseTypeDef,
+    CreateResourceDefinitionResponseTypeDef,
+    CreateResourceDefinitionVersionResponseTypeDef,
+    CreateSoftwareUpdateJobResponseTypeDef,
+    CreateSubscriptionDefinitionResponseTypeDef,
+    CreateSubscriptionDefinitionVersionResponseTypeDef,
+    DisassociateRoleFromGroupResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssociatedRoleResponseTypeDef,
+    GetConnectorDefinitionResponseTypeDef,
+    GetCoreDefinitionResponseTypeDef,
+    GetDeviceDefinitionResponseTypeDef,
+    GetFunctionDefinitionResponseTypeDef,
+    GetGroupCertificateAuthorityResponseTypeDef,
+    GetGroupCertificateConfigurationResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetLoggerDefinitionResponseTypeDef,
+    GetResourceDefinitionResponseTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
+    GetSubscriptionDefinitionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResetDeploymentsResponseTypeDef,
+    StartBulkDeploymentResponseTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
+    UpdateGroupCertificateConfigurationResponseTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
     CreateConnectorDefinitionVersionRequestRequestTypeDef,
     CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
+    GetGroupVersionResponseTypeDef,
     CreateLoggerDefinitionVersionRequestRequestTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
     LoggerDefinitionVersionTypeDef,
     CreateSubscriptionDefinitionVersionRequestRequestTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     ListConnectorDefinitionsResponseTypeDef,
     ListCoreDefinitionsResponseTypeDef,
     ListDeviceDefinitionsResponseTypeDef,
     ListFunctionDefinitionsResponseTypeDef,
     ListLoggerDefinitionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
-    DeviceDefinitionVersionOutputTypeDef,
-    FunctionDefaultExecutionConfigOutputTypeDef,
-    FunctionExecutionConfigOutputTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
-    GetGroupVersionResponseTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
-    LocalDeviceResourceDataOutputTypeDef,
-    LocalVolumeResourceDataOutputTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
+    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
+    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
+    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
+    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
+    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
+    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
+    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
-    LoggerDefinitionVersionOutputTypeDef,
-    S3MachineLearningModelResourceDataOutputTypeDef,
-    SageMakerMachineLearningModelResourceDataOutputTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
-    SubscriptionDefinitionVersionOutputTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     CreateConnectorDefinitionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionRequestRequestTypeDef,
+    GetDeviceDefinitionVersionResponseTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
+    GetLoggerDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
+    GetSubscriptionDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionVersionResponseTypeDef,
-    FunctionDefaultConfigOutputTypeDef,
-    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionDefaultConfigTypeDef,
+    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
-    GetLoggerDefinitionVersionResponseTypeDef,
     ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
-    GetSubscriptionDefinitionVersionResponseTypeDef,
     FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     FunctionOutputTypeDef,
     FunctionTypeDef,
     ResourceDefinitionVersionOutputTypeDef,
```

### Comparing `mypy-boto3-greengrass-1.28.12/README.md` & `mypy-boto3-greengrass-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,255 +391,238 @@
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
-    AssociateRoleToGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     ConnectorOutputTypeDef,
     ConnectorTypeDef,
-    CoreOutputTypeDef,
     CoreTypeDef,
-    CreateConnectorDefinitionResponseTypeDef,
-    CreateConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionResponseTypeDef,
-    CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateDeviceDefinitionResponseTypeDef,
     DeviceTypeDef,
-    CreateDeviceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionResponseTypeDef,
-    CreateFunctionDefinitionVersionResponseTypeDef,
     CreateGroupCertificateAuthorityRequestRequestTypeDef,
-    CreateGroupCertificateAuthorityResponseTypeDef,
     GroupVersionTypeDef,
-    CreateGroupResponseTypeDef,
     CreateGroupVersionRequestRequestTypeDef,
-    CreateGroupVersionResponseTypeDef,
-    CreateLoggerDefinitionResponseTypeDef,
     LoggerTypeDef,
-    CreateLoggerDefinitionVersionResponseTypeDef,
-    CreateResourceDefinitionResponseTypeDef,
-    CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobRequestRequestTypeDef,
-    CreateSoftwareUpdateJobResponseTypeDef,
-    CreateSubscriptionDefinitionResponseTypeDef,
     SubscriptionTypeDef,
-    CreateSubscriptionDefinitionVersionResponseTypeDef,
     DefinitionInformationTypeDef,
     DeleteConnectorDefinitionRequestRequestTypeDef,
     DeleteCoreDefinitionRequestRequestTypeDef,
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DeviceOutputTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
-    DisassociateRoleFromGroupResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ResourceAccessPolicyOutputTypeDef,
     ResourceAccessPolicyTypeDef,
-    FunctionRunAsConfigOutputTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
-    GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
-    GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionRequestRequestTypeDef,
-    GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionRequestRequestTypeDef,
     GetDeploymentStatusRequestRequestTypeDef,
     GetDeviceDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionResponseTypeDef,
     GetDeviceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionRequestRequestTypeDef,
-    GetFunctionDefinitionResponseTypeDef,
     GetFunctionDefinitionVersionRequestRequestTypeDef,
     GetGroupCertificateAuthorityRequestRequestTypeDef,
-    GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
-    GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
-    GroupVersionOutputTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
-    GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
-    GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
-    GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
-    GroupOwnerSettingOutputTypeDef,
     GroupOwnerSettingTypeDef,
-    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
-    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
-    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
     VersionInformationTypeDef,
-    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
     ListConnectorDefinitionsRequestRequestTypeDef,
-    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     ListCoreDefinitionVersionsRequestRequestTypeDef,
-    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
     ListCoreDefinitionsRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     ListDeviceDefinitionVersionsRequestRequestTypeDef,
-    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
     ListDeviceDefinitionsRequestRequestTypeDef,
-    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     ListFunctionDefinitionVersionsRequestRequestTypeDef,
-    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
     ListFunctionDefinitionsRequestRequestTypeDef,
     ListGroupCertificateAuthoritiesRequestRequestTypeDef,
-    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     ListGroupVersionsRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     ListLoggerDefinitionVersionsRequestRequestTypeDef,
-    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
     ListLoggerDefinitionsRequestRequestTypeDef,
-    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     ListResourceDefinitionVersionsRequestRequestTypeDef,
-    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
     ListResourceDefinitionsRequestRequestTypeDef,
-    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
-    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LoggerOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
-    ResetDeploymentsResponseTypeDef,
     SecretsManagerSecretResourceDataOutputTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
-    ResourceDownloadOwnerSettingOutputTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
-    ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
-    StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
-    SubscriptionOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
     UpdateFunctionDefinitionRequestRequestTypeDef,
     UpdateGroupCertificateConfigurationRequestRequestTypeDef,
-    UpdateGroupCertificateConfigurationResponseTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateLoggerDefinitionRequestRequestTypeDef,
     UpdateResourceDefinitionRequestRequestTypeDef,
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
+    AssociateRoleToGroupResponseTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
+    CreateConnectorDefinitionResponseTypeDef,
+    CreateConnectorDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionResponseTypeDef,
+    CreateCoreDefinitionVersionResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateDeviceDefinitionResponseTypeDef,
+    CreateDeviceDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionResponseTypeDef,
+    CreateFunctionDefinitionVersionResponseTypeDef,
+    CreateGroupCertificateAuthorityResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateGroupVersionResponseTypeDef,
+    CreateLoggerDefinitionResponseTypeDef,
+    CreateLoggerDefinitionVersionResponseTypeDef,
+    CreateResourceDefinitionResponseTypeDef,
+    CreateResourceDefinitionVersionResponseTypeDef,
+    CreateSoftwareUpdateJobResponseTypeDef,
+    CreateSubscriptionDefinitionResponseTypeDef,
+    CreateSubscriptionDefinitionVersionResponseTypeDef,
+    DisassociateRoleFromGroupResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssociatedRoleResponseTypeDef,
+    GetConnectorDefinitionResponseTypeDef,
+    GetCoreDefinitionResponseTypeDef,
+    GetDeviceDefinitionResponseTypeDef,
+    GetFunctionDefinitionResponseTypeDef,
+    GetGroupCertificateAuthorityResponseTypeDef,
+    GetGroupCertificateConfigurationResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetLoggerDefinitionResponseTypeDef,
+    GetResourceDefinitionResponseTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
+    GetSubscriptionDefinitionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResetDeploymentsResponseTypeDef,
+    StartBulkDeploymentResponseTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
+    UpdateGroupCertificateConfigurationResponseTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
     CreateConnectorDefinitionVersionRequestRequestTypeDef,
     CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
+    GetGroupVersionResponseTypeDef,
     CreateLoggerDefinitionVersionRequestRequestTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
     LoggerDefinitionVersionTypeDef,
     CreateSubscriptionDefinitionVersionRequestRequestTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     ListConnectorDefinitionsResponseTypeDef,
     ListCoreDefinitionsResponseTypeDef,
     ListDeviceDefinitionsResponseTypeDef,
     ListFunctionDefinitionsResponseTypeDef,
     ListLoggerDefinitionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
-    DeviceDefinitionVersionOutputTypeDef,
-    FunctionDefaultExecutionConfigOutputTypeDef,
-    FunctionExecutionConfigOutputTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
-    GetGroupVersionResponseTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
-    LocalDeviceResourceDataOutputTypeDef,
-    LocalVolumeResourceDataOutputTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
+    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
+    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
+    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
+    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
+    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
+    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
+    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
-    LoggerDefinitionVersionOutputTypeDef,
-    S3MachineLearningModelResourceDataOutputTypeDef,
-    SageMakerMachineLearningModelResourceDataOutputTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
-    SubscriptionDefinitionVersionOutputTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     CreateConnectorDefinitionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionRequestRequestTypeDef,
+    GetDeviceDefinitionVersionResponseTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
+    GetLoggerDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
+    GetSubscriptionDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionVersionResponseTypeDef,
-    FunctionDefaultConfigOutputTypeDef,
-    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionDefaultConfigTypeDef,
+    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
-    GetLoggerDefinitionVersionResponseTypeDef,
     ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
-    GetSubscriptionDefinitionVersionResponseTypeDef,
     FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     FunctionOutputTypeDef,
     FunctionTypeDef,
     ResourceDefinitionVersionOutputTypeDef,
```

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.py` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.pyi` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__main__.py` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Greengrass 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Greengrass 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.py` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.pyi` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.py` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.pyi` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.py` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,283 +118,283 @@
 class ListBulkDeploymentDetailedReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
     """
 
     def paginate(
-        self, *, BulkDeploymentId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BulkDeploymentId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkDeploymentDetailedReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
         """
 
 
 class ListBulkDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
         """
 
 
 class ListConnectorDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ConnectorDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ConnectorDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
         """
 
 
 class ListConnectorDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
         """
 
 
 class ListCoreDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, CoreDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CoreDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoreDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
         """
 
 
 class ListCoreDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoreDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
         """
 
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
         """
 
 
 class ListDeviceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, DeviceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeviceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
         """
 
 
 class ListDeviceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
         """
 
 
 class ListFunctionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, FunctionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
         """
 
 
 class ListFunctionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
         """
 
 
 class ListGroupVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
         """
 
 
 class ListLoggerDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, LoggerDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LoggerDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLoggerDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
         """
 
 
 class ListLoggerDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLoggerDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
         """
 
 
 class ListResourceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ResourceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
         """
 
 
 class ListResourceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
         """
 
 
 class ListSubscriptionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, SubscriptionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SubscriptionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
         """
 
 
 class ListSubscriptionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
         """
```

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.pyi` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -115,265 +115,265 @@
 class ListBulkDeploymentDetailedReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
     """
 
     def paginate(
-        self, *, BulkDeploymentId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BulkDeploymentId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkDeploymentDetailedReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
         """
 
 class ListBulkDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBulkDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
         """
 
 class ListConnectorDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ConnectorDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ConnectorDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
         """
 
 class ListConnectorDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConnectorDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
         """
 
 class ListCoreDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, CoreDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CoreDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoreDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
         """
 
 class ListCoreDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoreDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
         """
 
 class ListDeviceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, DeviceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeviceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
         """
 
 class ListDeviceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
         """
 
 class ListFunctionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, FunctionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
         """
 
 class ListFunctionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
         """
 
 class ListGroupVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
         """
 
 class ListLoggerDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, LoggerDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LoggerDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLoggerDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
         """
 
 class ListLoggerDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLoggerDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
         """
 
 class ListResourceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ResourceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
         """
 
 class ListResourceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
         """
 
 class ListSubscriptionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, SubscriptionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SubscriptionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
         """
 
 class ListSubscriptionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
         """
```

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.py` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -32,258 +32,240 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateRoleToGroupRequestRequestTypeDef",
-    "AssociateRoleToGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
-    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "ConnectorOutputTypeDef",
     "ConnectorTypeDef",
-    "CoreOutputTypeDef",
     "CoreTypeDef",
-    "CreateConnectorDefinitionResponseTypeDef",
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    "CreateCoreDefinitionResponseTypeDef",
-    "CreateCoreDefinitionVersionResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateDeviceDefinitionResponseTypeDef",
     "DeviceTypeDef",
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    "CreateFunctionDefinitionResponseTypeDef",
-    "CreateFunctionDefinitionVersionResponseTypeDef",
     "CreateGroupCertificateAuthorityRequestRequestTypeDef",
-    "CreateGroupCertificateAuthorityResponseTypeDef",
     "GroupVersionTypeDef",
-    "CreateGroupResponseTypeDef",
     "CreateGroupVersionRequestRequestTypeDef",
-    "CreateGroupVersionResponseTypeDef",
-    "CreateLoggerDefinitionResponseTypeDef",
     "LoggerTypeDef",
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    "CreateResourceDefinitionResponseTypeDef",
-    "CreateResourceDefinitionVersionResponseTypeDef",
     "CreateSoftwareUpdateJobRequestRequestTypeDef",
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    "CreateSubscriptionDefinitionResponseTypeDef",
     "SubscriptionTypeDef",
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
     "DefinitionInformationTypeDef",
     "DeleteConnectorDefinitionRequestRequestTypeDef",
     "DeleteCoreDefinitionRequestRequestTypeDef",
     "DeleteDeviceDefinitionRequestRequestTypeDef",
     "DeleteFunctionDefinitionRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteLoggerDefinitionRequestRequestTypeDef",
     "DeleteResourceDefinitionRequestRequestTypeDef",
     "DeleteSubscriptionDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "DeviceOutputTypeDef",
     "DisassociateRoleFromGroupRequestRequestTypeDef",
-    "DisassociateRoleFromGroupResponseTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ResourceAccessPolicyOutputTypeDef",
     "ResourceAccessPolicyTypeDef",
-    "FunctionRunAsConfigOutputTypeDef",
     "FunctionRunAsConfigTypeDef",
     "GetAssociatedRoleRequestRequestTypeDef",
-    "GetAssociatedRoleResponseTypeDef",
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetConnectorDefinitionRequestRequestTypeDef",
-    "GetConnectorDefinitionResponseTypeDef",
     "GetConnectorDefinitionVersionRequestRequestTypeDef",
     "GetCoreDefinitionRequestRequestTypeDef",
-    "GetCoreDefinitionResponseTypeDef",
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     "GetDeploymentStatusRequestRequestTypeDef",
     "GetDeviceDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionResponseTypeDef",
     "GetDeviceDefinitionVersionRequestRequestTypeDef",
     "GetFunctionDefinitionRequestRequestTypeDef",
-    "GetFunctionDefinitionResponseTypeDef",
     "GetFunctionDefinitionVersionRequestRequestTypeDef",
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
-    "GetGroupCertificateAuthorityResponseTypeDef",
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
-    "GetGroupCertificateConfigurationResponseTypeDef",
     "GetGroupRequestRequestTypeDef",
-    "GetGroupResponseTypeDef",
     "GetGroupVersionRequestRequestTypeDef",
-    "GroupVersionOutputTypeDef",
     "GetLoggerDefinitionRequestRequestTypeDef",
-    "GetLoggerDefinitionResponseTypeDef",
     "GetLoggerDefinitionVersionRequestRequestTypeDef",
     "GetResourceDefinitionRequestRequestTypeDef",
-    "GetResourceDefinitionResponseTypeDef",
     "GetResourceDefinitionVersionRequestRequestTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
     "GetSubscriptionDefinitionRequestRequestTypeDef",
-    "GetSubscriptionDefinitionResponseTypeDef",
     "GetSubscriptionDefinitionVersionRequestRequestTypeDef",
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     "GroupCertificateAuthorityPropertiesTypeDef",
     "GroupInformationTypeDef",
-    "GroupOwnerSettingOutputTypeDef",
     "GroupOwnerSettingTypeDef",
-    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBulkDeploymentDetailedReportsRequestRequestTypeDef",
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     "ListBulkDeploymentsRequestRequestTypeDef",
-    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsRequestRequestTypeDef",
     "VersionInformationTypeDef",
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionsRequestRequestTypeDef",
-    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     "ListCoreDefinitionVersionsRequestRequestTypeDef",
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     "ListCoreDefinitionsRequestRequestTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
-    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     "ListDeviceDefinitionVersionsRequestRequestTypeDef",
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
     "ListDeviceDefinitionsRequestRequestTypeDef",
-    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
     "ListFunctionDefinitionVersionsRequestRequestTypeDef",
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
     "ListFunctionDefinitionsRequestRequestTypeDef",
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
-    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
     "ListGroupVersionsRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
     "ListLoggerDefinitionVersionsRequestRequestTypeDef",
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
     "ListLoggerDefinitionsRequestRequestTypeDef",
-    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
     "ListResourceDefinitionVersionsRequestRequestTypeDef",
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
     "ListResourceDefinitionsRequestRequestTypeDef",
-    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LoggerOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
-    "ResetDeploymentsResponseTypeDef",
     "SecretsManagerSecretResourceDataOutputTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
-    "ResourceDownloadOwnerSettingOutputTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
-    "ResponseMetadataTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
-    "StartBulkDeploymentResponseTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
-    "SubscriptionOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
     "UpdateConnectorDefinitionRequestRequestTypeDef",
     "UpdateCoreDefinitionRequestRequestTypeDef",
     "UpdateDeviceDefinitionRequestRequestTypeDef",
     "UpdateFunctionDefinitionRequestRequestTypeDef",
     "UpdateGroupCertificateConfigurationRequestRequestTypeDef",
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateLoggerDefinitionRequestRequestTypeDef",
     "UpdateResourceDefinitionRequestRequestTypeDef",
     "UpdateSubscriptionDefinitionRequestRequestTypeDef",
+    "AssociateRoleToGroupResponseTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    "CreateConnectorDefinitionResponseTypeDef",
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    "CreateCoreDefinitionResponseTypeDef",
+    "CreateCoreDefinitionVersionResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateDeviceDefinitionResponseTypeDef",
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    "CreateFunctionDefinitionResponseTypeDef",
+    "CreateFunctionDefinitionVersionResponseTypeDef",
+    "CreateGroupCertificateAuthorityResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateGroupVersionResponseTypeDef",
+    "CreateLoggerDefinitionResponseTypeDef",
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    "CreateResourceDefinitionResponseTypeDef",
+    "CreateResourceDefinitionVersionResponseTypeDef",
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    "CreateSubscriptionDefinitionResponseTypeDef",
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
+    "DisassociateRoleFromGroupResponseTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAssociatedRoleResponseTypeDef",
+    "GetConnectorDefinitionResponseTypeDef",
+    "GetCoreDefinitionResponseTypeDef",
+    "GetDeviceDefinitionResponseTypeDef",
+    "GetFunctionDefinitionResponseTypeDef",
+    "GetGroupCertificateAuthorityResponseTypeDef",
+    "GetGroupCertificateConfigurationResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetLoggerDefinitionResponseTypeDef",
+    "GetResourceDefinitionResponseTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
+    "GetSubscriptionDefinitionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResetDeploymentsResponseTypeDef",
+    "StartBulkDeploymentResponseTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
     "CreateConnectorDefinitionVersionRequestRequestTypeDef",
     "CoreDefinitionVersionOutputTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
+    "DeviceDefinitionVersionOutputTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "GetGroupVersionResponseTypeDef",
     "CreateLoggerDefinitionVersionRequestRequestTypeDef",
+    "LoggerDefinitionVersionOutputTypeDef",
     "LoggerDefinitionVersionTypeDef",
     "CreateSubscriptionDefinitionVersionRequestRequestTypeDef",
+    "SubscriptionDefinitionVersionOutputTypeDef",
     "SubscriptionDefinitionVersionTypeDef",
     "ListConnectorDefinitionsResponseTypeDef",
     "ListCoreDefinitionsResponseTypeDef",
     "ListDeviceDefinitionsResponseTypeDef",
     "ListFunctionDefinitionsResponseTypeDef",
     "ListLoggerDefinitionsResponseTypeDef",
     "ListResourceDefinitionsResponseTypeDef",
     "ListSubscriptionDefinitionsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
-    "DeviceDefinitionVersionOutputTypeDef",
-    "FunctionDefaultExecutionConfigOutputTypeDef",
-    "FunctionExecutionConfigOutputTypeDef",
     "FunctionDefaultExecutionConfigTypeDef",
     "FunctionExecutionConfigTypeDef",
-    "GetGroupVersionResponseTypeDef",
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     "ListGroupsResponseTypeDef",
-    "LocalDeviceResourceDataOutputTypeDef",
-    "LocalVolumeResourceDataOutputTypeDef",
     "LocalDeviceResourceDataTypeDef",
     "LocalVolumeResourceDataTypeDef",
+    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
+    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
+    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
+    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
+    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
+    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
+    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsResponseTypeDef",
     "ListCoreDefinitionVersionsResponseTypeDef",
     "ListDeviceDefinitionVersionsResponseTypeDef",
     "ListFunctionDefinitionVersionsResponseTypeDef",
     "ListGroupVersionsResponseTypeDef",
     "ListLoggerDefinitionVersionsResponseTypeDef",
     "ListResourceDefinitionVersionsResponseTypeDef",
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
-    "LoggerDefinitionVersionOutputTypeDef",
-    "S3MachineLearningModelResourceDataOutputTypeDef",
-    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
-    "SubscriptionDefinitionVersionOutputTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     "GetConnectorDefinitionVersionResponseTypeDef",
     "CreateConnectorDefinitionRequestRequestTypeDef",
     "GetCoreDefinitionVersionResponseTypeDef",
     "CreateCoreDefinitionRequestRequestTypeDef",
+    "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
+    "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionVersionResponseTypeDef",
-    "FunctionDefaultConfigOutputTypeDef",
-    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionDefaultConfigTypeDef",
+    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
-    "GetLoggerDefinitionVersionResponseTypeDef",
     "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
     "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "FunctionOutputTypeDef",
     "FunctionTypeDef",
     "ResourceDefinitionVersionOutputTypeDef",
@@ -302,37 +284,32 @@
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
     },
 )
 
-AssociateRoleToGroupResponseTypeDef = TypedDict(
-    "AssociateRoleToGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AssociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "RoleArn": str,
     },
 )
 
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BulkDeploymentMetricsTypeDef = TypedDict(
     "BulkDeploymentMetricsTypeDef",
     {
         "InvalidInputRecords": int,
         "RecordsProcessed": int,
         "RetryAttempts": int,
     },
@@ -354,25 +331,14 @@
         "BulkDeploymentArn": str,
         "BulkDeploymentId": str,
         "CreatedAt": str,
     },
     total=False,
 )
 
-ConnectivityInfoOutputTypeDef = TypedDict(
-    "ConnectivityInfoOutputTypeDef",
-    {
-        "HostAddress": str,
-        "Id": str,
-        "Metadata": str,
-        "PortNumber": int,
-    },
-    total=False,
-)
-
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "HostAddress": str,
         "Id": str,
         "Metadata": str,
         "PortNumber": int,
@@ -391,19 +357,17 @@
     "_OptionalConnectorOutputTypeDef",
     {
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
-
 class ConnectorOutputTypeDef(_RequiredConnectorOutputTypeDef, _OptionalConnectorOutputTypeDef):
     pass
 
-
 _RequiredConnectorTypeDef = TypedDict(
     "_RequiredConnectorTypeDef",
     {
         "ConnectorArn": str,
         "Id": str,
     },
 )
@@ -411,40 +375,17 @@
     "_OptionalConnectorTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ConnectorTypeDef(_RequiredConnectorTypeDef, _OptionalConnectorTypeDef):
     pass
 
-
-_RequiredCoreOutputTypeDef = TypedDict(
-    "_RequiredCoreOutputTypeDef",
-    {
-        "CertificateArn": str,
-        "Id": str,
-        "ThingArn": str,
-    },
-)
-_OptionalCoreOutputTypeDef = TypedDict(
-    "_OptionalCoreOutputTypeDef",
-    {
-        "SyncShadow": bool,
-    },
-    total=False,
-)
-
-
-class CoreOutputTypeDef(_RequiredCoreOutputTypeDef, _OptionalCoreOutputTypeDef):
-    pass
-
-
 _RequiredCoreTypeDef = TypedDict(
     "_RequiredCoreTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -453,69 +394,17 @@
     "_OptionalCoreTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
-
 class CoreTypeDef(_RequiredCoreTypeDef, _OptionalCoreTypeDef):
     pass
 
-
-CreateConnectorDefinitionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCoreDefinitionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "DeploymentType": DeploymentTypeType,
         "GroupId": str,
     },
 )
@@ -525,44 +414,19 @@
         "AmznClientToken": str,
         "DeploymentId": str,
         "GroupVersionId": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDeviceDefinitionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -571,113 +435,51 @@
     "_OptionalDeviceTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
-
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
-
-CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFunctionDefinitionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "AmznClientToken": str,
     },
     total=False,
 )
 
-
 class CreateGroupCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
-CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "CreateGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupVersionTypeDef = TypedDict(
     "GroupVersionTypeDef",
     {
         "ConnectorDefinitionVersionArn": str,
         "CoreDefinitionVersionArn": str,
         "DeviceDefinitionVersionArn": str,
         "FunctionDefinitionVersionArn": str,
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateGroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupVersionRequestRequestTypeDef = TypedDict(
@@ -691,47 +493,20 @@
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
-
 class CreateGroupVersionRequestRequestTypeDef(
     _RequiredCreateGroupVersionRequestRequestTypeDef,
     _OptionalCreateGroupVersionRequestRequestTypeDef,
 ):
     pass
 
-
-CreateGroupVersionResponseTypeDef = TypedDict(
-    "CreateGroupVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLoggerDefinitionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredLoggerTypeDef = TypedDict(
     "_RequiredLoggerTypeDef",
     {
         "Component": LoggerComponentType,
         "Id": str,
         "Level": LoggerLevelType,
         "Type": LoggerTypeType,
@@ -741,55 +516,17 @@
     "_OptionalLoggerTypeDef",
     {
         "Space": int,
     },
     total=False,
 )
 
-
 class LoggerTypeDef(_RequiredLoggerTypeDef, _OptionalLoggerTypeDef):
     pass
 
-
-CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateResourceDefinitionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSoftwareUpdateJobRequestRequestTypeDef",
     {
         "S3UrlSignerRole": str,
         "SoftwareToUpdate": SoftwareToUpdateType,
         "UpdateTargets": Sequence[str],
         "UpdateTargetsArchitecture": UpdateTargetsArchitectureType,
@@ -801,67 +538,30 @@
     {
         "AmznClientToken": str,
         "UpdateAgentLogLevel": UpdateAgentLogLevelType,
     },
     total=False,
 )
 
-
 class CreateSoftwareUpdateJobRequestRequestTypeDef(
     _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef,
     _OptionalCreateSoftwareUpdateJobRequestRequestTypeDef,
 ):
     pass
 
-
-CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    {
-        "IotJobArn": str,
-        "IotJobId": str,
-        "PlatformSoftwareVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Id": str,
         "Source": str,
         "Subject": str,
         "Target": str,
     },
 )
 
-CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DefinitionInformationTypeDef = TypedDict(
     "DefinitionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "LastUpdatedTimestamp": str,
@@ -937,116 +637,40 @@
         "DeploymentId": str,
         "DeploymentType": DeploymentTypeType,
         "GroupArn": str,
     },
     total=False,
 )
 
-_RequiredDeviceOutputTypeDef = TypedDict(
-    "_RequiredDeviceOutputTypeDef",
-    {
-        "CertificateArn": str,
-        "Id": str,
-        "ThingArn": str,
-    },
-)
-_OptionalDeviceOutputTypeDef = TypedDict(
-    "_OptionalDeviceOutputTypeDef",
-    {
-        "SyncShadow": bool,
-    },
-    total=False,
-)
-
-
-class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
-    pass
-
-
 DisassociateRoleFromGroupRequestRequestTypeDef = TypedDict(
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-DisassociateRoleFromGroupResponseTypeDef = TypedDict(
-    "DisassociateRoleFromGroupResponseTypeDef",
-    {
-        "DisassociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "DisassociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredResourceAccessPolicyOutputTypeDef = TypedDict(
-    "_RequiredResourceAccessPolicyOutputTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalResourceAccessPolicyOutputTypeDef = TypedDict(
-    "_OptionalResourceAccessPolicyOutputTypeDef",
-    {
-        "Permission": PermissionType,
-    },
-    total=False,
-)
-
-
-class ResourceAccessPolicyOutputTypeDef(
-    _RequiredResourceAccessPolicyOutputTypeDef, _OptionalResourceAccessPolicyOutputTypeDef
-):
-    pass
-
-
 _RequiredResourceAccessPolicyTypeDef = TypedDict(
     "_RequiredResourceAccessPolicyTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalResourceAccessPolicyTypeDef = TypedDict(
     "_OptionalResourceAccessPolicyTypeDef",
     {
         "Permission": PermissionType,
     },
     total=False,
 )
 
-
 class ResourceAccessPolicyTypeDef(
     _RequiredResourceAccessPolicyTypeDef, _OptionalResourceAccessPolicyTypeDef
 ):
     pass
 
-
-FunctionRunAsConfigOutputTypeDef = TypedDict(
-    "FunctionRunAsConfigOutputTypeDef",
-    {
-        "Gid": int,
-        "Uid": int,
-    },
-    total=False,
-)
-
 FunctionRunAsConfigTypeDef = TypedDict(
     "FunctionRunAsConfigTypeDef",
     {
         "Gid": int,
         "Uid": int,
     },
     total=False,
@@ -1055,23 +679,14 @@
 GetAssociatedRoleRequestRequestTypeDef = TypedDict(
     "GetAssociatedRoleRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-GetAssociatedRoleResponseTypeDef = TypedDict(
-    "GetAssociatedRoleResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBulkDeploymentStatusRequestRequestTypeDef = TypedDict(
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -1085,29 +700,14 @@
 GetConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "GetConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 
-GetConnectorDefinitionResponseTypeDef = TypedDict(
-    "GetConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
         "ConnectorDefinitionVersionId": str,
     },
 )
@@ -1115,44 +715,27 @@
     "_OptionalGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalGetConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetCoreDefinitionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 
-GetCoreDefinitionResponseTypeDef = TypedDict(
-    "GetCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCoreDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
         "CoreDefinitionVersionId": str,
     },
 )
@@ -1168,29 +751,14 @@
 GetDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "GetDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 
-GetDeviceDefinitionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
         "DeviceDefinitionVersionId": str,
     },
 )
@@ -1198,44 +766,27 @@
     "_OptionalGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalGetDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "GetFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 
-GetFunctionDefinitionResponseTypeDef = TypedDict(
-    "GetFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
         "FunctionDefinitionVersionId": str,
     },
 )
@@ -1243,123 +794,57 @@
     "_OptionalGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetFunctionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityId": str,
         "GroupId": str,
     },
 )
 
-GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "GetGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "GroupCertificateAuthorityId": str,
-        "PemEncodedCertificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "GetGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupVersionRequestRequestTypeDef = TypedDict(
     "GetGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
         "GroupVersionId": str,
     },
 )
 
-GroupVersionOutputTypeDef = TypedDict(
-    "GroupVersionOutputTypeDef",
-    {
-        "ConnectorDefinitionVersionArn": str,
-        "CoreDefinitionVersionArn": str,
-        "DeviceDefinitionVersionArn": str,
-        "FunctionDefinitionVersionArn": str,
-        "LoggerDefinitionVersionArn": str,
-        "ResourceDefinitionVersionArn": str,
-        "SubscriptionDefinitionVersionArn": str,
-    },
-    total=False,
-)
-
 GetLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "GetLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 
-GetLoggerDefinitionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
         "LoggerDefinitionVersionId": str,
     },
 )
@@ -1367,83 +852,42 @@
     "_OptionalGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalGetLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourceDefinitionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 
-GetResourceDefinitionResponseTypeDef = TypedDict(
-    "GetResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionVersionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
         "ResourceDefinitionVersionId": str,
     },
 )
 
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 
-GetSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
         "SubscriptionDefinitionVersionId": str,
     },
 )
@@ -1451,22 +895,20 @@
     "_OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 
@@ -1489,54 +931,33 @@
         "LatestVersion": str,
         "LatestVersionArn": str,
         "Name": str,
     },
     total=False,
 )
 
-GroupOwnerSettingOutputTypeDef = TypedDict(
-    "GroupOwnerSettingOutputTypeDef",
-    {
-        "AutoAddGroupOwner": bool,
-        "GroupOwner": str,
-    },
-    total=False,
-)
-
 GroupOwnerSettingTypeDef = TypedDict(
     "GroupOwnerSettingTypeDef",
     {
         "AutoAddGroupOwner": bool,
         "GroupOwner": str,
     },
     total=False,
 )
 
-_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    {
-        "BulkDeploymentId": str,
-    },
-)
-_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
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
-class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
-    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
@@ -1544,61 +965,29 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListBulkDeploymentDetailedReportsRequestRequestTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef,
 ):
     pass
 
-
-ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBulkDeploymentsRequestRequestTypeDef = TypedDict(
     "ListBulkDeploymentsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
-    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConnectorDefinitionVersionsRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1606,72 +995,40 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListConnectorDefinitionVersionsRequestRequestTypeDef(
     _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef,
     _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 VersionInformationTypeDef = TypedDict(
     "VersionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "Version": str,
     },
     total=False,
 )
 
-ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConnectorDefinitionsRequestRequestTypeDef = TypedDict(
     "ListConnectorDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "CoreDefinitionId": str,
-    },
-)
-_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
-    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCoreDefinitionVersionsRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1679,61 +1036,29 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListCoreDefinitionVersionsRequestRequestTypeDef(
     _RequiredListCoreDefinitionVersionsRequestRequestTypeDef,
     _OptionalListCoreDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCoreDefinitionsRequestRequestTypeDef = TypedDict(
     "ListCoreDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1741,43 +1066,19 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "DeviceDefinitionId": str,
-    },
-)
-_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
-    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1785,61 +1086,29 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDeviceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeviceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
-    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionDefinitionVersionsRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1847,30 +1116,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFunctionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFunctionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1879,36 +1138,14 @@
 ListGroupCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
-    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupVersionsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListGroupVersionsRequestRequestTypeDef = TypedDict(
@@ -1916,60 +1153,28 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGroupVersionsRequestRequestTypeDef(
     _RequiredListGroupVersionsRequestRequestTypeDef, _OptionalListGroupVersionsRequestRequestTypeDef
 ):
     pass
 
-
-ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "LoggerDefinitionId": str,
-    },
-)
-_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
-    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLoggerDefinitionVersionsRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1977,61 +1182,29 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListLoggerDefinitionVersionsRequestRequestTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLoggerDefinitionsRequestRequestTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
-    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceDefinitionVersionsRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -2039,61 +1212,29 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResourceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListResourceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListResourceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListResourceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "SubscriptionDefinitionId": str,
-    },
-)
-_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
-    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -2101,30 +1242,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSubscriptionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscriptionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -2133,54 +1264,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
-_RequiredLoggerOutputTypeDef = TypedDict(
-    "_RequiredLoggerOutputTypeDef",
-    {
-        "Component": LoggerComponentType,
-        "Id": str,
-        "Level": LoggerLevelType,
-        "Type": LoggerTypeType,
-    },
-)
-_OptionalLoggerOutputTypeDef = TypedDict(
-    "_OptionalLoggerOutputTypeDef",
-    {
-        "Space": int,
-    },
-    total=False,
-)
-
-
-class LoggerOutputTypeDef(_RequiredLoggerOutputTypeDef, _OptionalLoggerOutputTypeDef):
-    pass
-
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
 _RequiredResetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredResetDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalResetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -2188,30 +1279,19 @@
     {
         "AmznClientToken": str,
         "Force": bool,
     },
     total=False,
 )
 
-
 class ResetDeploymentsRequestRequestTypeDef(
     _RequiredResetDeploymentsRequestRequestTypeDef, _OptionalResetDeploymentsRequestRequestTypeDef
 ):
     pass
 
-
-ResetDeploymentsResponseTypeDef = TypedDict(
-    "ResetDeploymentsResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SecretsManagerSecretResourceDataOutputTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataOutputTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": List[str],
     },
     total=False,
@@ -2222,62 +1302,41 @@
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
     total=False,
 )
 
-ResourceDownloadOwnerSettingOutputTypeDef = TypedDict(
-    "ResourceDownloadOwnerSettingOutputTypeDef",
-    {
-        "GroupOwner": str,
-        "GroupPermission": PermissionType,
-    },
-)
-
 ResourceDownloadOwnerSettingTypeDef = TypedDict(
     "ResourceDownloadOwnerSettingTypeDef",
     {
         "GroupOwner": str,
         "GroupPermission": PermissionType,
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
 _RequiredTelemetryConfigurationTypeDef = TypedDict(
     "_RequiredTelemetryConfigurationTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 _OptionalTelemetryConfigurationTypeDef = TypedDict(
     "_OptionalTelemetryConfigurationTypeDef",
     {
         "ConfigurationSyncStatus": ConfigurationSyncStatusType,
     },
     total=False,
 )
 
-
 class TelemetryConfigurationTypeDef(
     _RequiredTelemetryConfigurationTypeDef, _OptionalTelemetryConfigurationTypeDef
 ):
     pass
 
-
 _RequiredStartBulkDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDeploymentRequestRequestTypeDef",
     {
         "ExecutionRoleArn": str,
         "InputFileUri": str,
     },
 )
@@ -2286,69 +1345,46 @@
     {
         "AmznClientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartBulkDeploymentRequestRequestTypeDef(
     _RequiredStartBulkDeploymentRequestRequestTypeDef,
     _OptionalStartBulkDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
-StartBulkDeploymentResponseTypeDef = TypedDict(
-    "StartBulkDeploymentResponseTypeDef",
-    {
-        "BulkDeploymentArn": str,
-        "BulkDeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
-SubscriptionOutputTypeDef = TypedDict(
-    "SubscriptionOutputTypeDef",
-    {
-        "Id": str,
-        "Source": str,
-        "Subject": str,
-        "Target": str,
-    },
-)
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 TelemetryConfigurationUpdateTypeDef = TypedDict(
     "TelemetryConfigurationUpdateTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 
@@ -2356,229 +1392,661 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "Message": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateConnectorDefinitionRequestRequestTypeDef(
     _RequiredUpdateConnectorDefinitionRequestRequestTypeDef,
     _OptionalUpdateConnectorDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateCoreDefinitionRequestRequestTypeDef(
     _RequiredUpdateCoreDefinitionRequestRequestTypeDef,
     _OptionalUpdateCoreDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateDeviceDefinitionRequestRequestTypeDef(
     _RequiredUpdateDeviceDefinitionRequestRequestTypeDef,
     _OptionalUpdateDeviceDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateFunctionDefinitionRequestRequestTypeDef(
     _RequiredUpdateFunctionDefinitionRequestRequestTypeDef,
     _OptionalUpdateFunctionDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "CertificateExpiryInMilliseconds": str,
     },
     total=False,
 )
 
-
 class UpdateGroupCertificateConfigurationRequestRequestTypeDef(
     _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef,
     _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateLoggerDefinitionRequestRequestTypeDef(
     _RequiredUpdateLoggerDefinitionRequestRequestTypeDef,
     _OptionalUpdateLoggerDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateResourceDefinitionRequestRequestTypeDef(
     _RequiredUpdateResourceDefinitionRequestRequestTypeDef,
     _OptionalUpdateResourceDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateSubscriptionDefinitionRequestRequestTypeDef(
     _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef,
     _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef,
 ):
     pass
 
+AssociateRoleToGroupResponseTypeDef = TypedDict(
+    "AssociateRoleToGroupResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorDefinitionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCoreDefinitionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceDefinitionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFunctionDefinitionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "CreateGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupVersionResponseTypeDef = TypedDict(
+    "CreateGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLoggerDefinitionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourceDefinitionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    {
+        "IotJobArn": str,
+        "IotJobId": str,
+        "PlatformSoftwareVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateRoleFromGroupResponseTypeDef = TypedDict(
+    "DisassociateRoleFromGroupResponseTypeDef",
+    {
+        "DisassociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "DisassociatedAt": str,
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
+GetAssociatedRoleResponseTypeDef = TypedDict(
+    "GetAssociatedRoleResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectorDefinitionResponseTypeDef = TypedDict(
+    "GetConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCoreDefinitionResponseTypeDef = TypedDict(
+    "GetCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceDefinitionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionDefinitionResponseTypeDef = TypedDict(
+    "GetFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "GetGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "GroupCertificateAuthorityId": str,
+        "PemEncodedCertificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "GetGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLoggerDefinitionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourceDefinitionResponseTypeDef = TypedDict(
+    "GetResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
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
+ResetDeploymentsResponseTypeDef = TypedDict(
+    "ResetDeploymentsResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartBulkDeploymentResponseTypeDef = TypedDict(
+    "StartBulkDeploymentResponseTypeDef",
+    {
+        "BulkDeploymentArn": str,
+        "BulkDeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "Message": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 BulkDeploymentResultTypeDef = TypedDict(
     "BulkDeploymentResultTypeDef",
     {
         "CreatedAt": str,
         "DeploymentArn": str,
         "DeploymentId": str,
@@ -2596,45 +2064,45 @@
     {
         "BulkDeploymentMetrics": BulkDeploymentMetricsTypeDef,
         "BulkDeploymentStatus": BulkDeploymentStatusType,
         "CreatedAt": str,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentStatusResponseTypeDef = TypedDict(
     "GetDeploymentStatusResponseTypeDef",
     {
         "DeploymentStatus": str,
         "DeploymentType": DeploymentTypeType,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "UpdatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBulkDeploymentsResponseTypeDef = TypedDict(
     "ListBulkDeploymentsResponseTypeDef",
     {
         "BulkDeployments": List[BulkDeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "ConnectivityInfo": List[ConnectivityInfoOutputTypeDef],
+        "ConnectivityInfo": List[ConnectivityInfoTypeDef],
         "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ThingName": str,
@@ -2644,22 +2112,20 @@
     "_OptionalUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ConnectivityInfo": Sequence[ConnectivityInfoTypeDef],
     },
     total=False,
 )
 
-
 class UpdateConnectivityInfoRequestRequestTypeDef(
     _RequiredUpdateConnectivityInfoRequestRequestTypeDef,
     _OptionalUpdateConnectivityInfoRequestRequestTypeDef,
 ):
     pass
 
-
 ConnectorDefinitionVersionOutputTypeDef = TypedDict(
     "ConnectorDefinitionVersionOutputTypeDef",
     {
         "Connectors": List[ConnectorOutputTypeDef],
     },
     total=False,
 )
@@ -2683,26 +2149,24 @@
     {
         "AmznClientToken": str,
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
-
 class CreateConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 CoreDefinitionVersionOutputTypeDef = TypedDict(
     "CoreDefinitionVersionOutputTypeDef",
     {
-        "Cores": List[CoreOutputTypeDef],
+        "Cores": List[CoreTypeDef],
     },
     total=False,
 )
 
 CoreDefinitionVersionTypeDef = TypedDict(
     "CoreDefinitionVersionTypeDef",
     {
@@ -2722,22 +2186,20 @@
     {
         "AmznClientToken": str,
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
 
-
 class CreateCoreDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateCoreDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateCoreDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -2745,21 +2207,27 @@
     {
         "AmznClientToken": str,
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+DeviceDefinitionVersionOutputTypeDef = TypedDict(
+    "DeviceDefinitionVersionOutputTypeDef",
+    {
+        "Devices": List[DeviceTypeDef],
+    },
+    total=False,
+)
 
 DeviceDefinitionVersionTypeDef = TypedDict(
     "DeviceDefinitionVersionTypeDef",
     {
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
@@ -2777,20 +2245,30 @@
         "AmznClientToken": str,
         "InitialVersion": GroupVersionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+GetGroupVersionResponseTypeDef = TypedDict(
+    "GetGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": GroupVersionTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
@@ -2799,21 +2277,27 @@
     {
         "AmznClientToken": str,
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
 )
 
-
 class CreateLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+LoggerDefinitionVersionOutputTypeDef = TypedDict(
+    "LoggerDefinitionVersionOutputTypeDef",
+    {
+        "Loggers": List[LoggerTypeDef],
+    },
+    total=False,
+)
 
 LoggerDefinitionVersionTypeDef = TypedDict(
     "LoggerDefinitionVersionTypeDef",
     {
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
@@ -2830,311 +2314,504 @@
     {
         "AmznClientToken": str,
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
 )
 
-
 class CreateSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
+    "SubscriptionDefinitionVersionOutputTypeDef",
+    {
+        "Subscriptions": List[SubscriptionTypeDef],
+    },
+    total=False,
+)
 
 SubscriptionDefinitionVersionTypeDef = TypedDict(
     "SubscriptionDefinitionVersionTypeDef",
     {
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
 )
 
 ListConnectorDefinitionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoreDefinitionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceDefinitionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionDefinitionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggerDefinitionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceDefinitionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionDefinitionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeviceDefinitionVersionOutputTypeDef = TypedDict(
-    "DeviceDefinitionVersionOutputTypeDef",
+FunctionDefaultExecutionConfigTypeDef = TypedDict(
+    "FunctionDefaultExecutionConfigTypeDef",
     {
-        "Devices": List[DeviceOutputTypeDef],
+        "IsolationMode": FunctionIsolationModeType,
+        "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
 )
 
-FunctionDefaultExecutionConfigOutputTypeDef = TypedDict(
-    "FunctionDefaultExecutionConfigOutputTypeDef",
+FunctionExecutionConfigTypeDef = TypedDict(
+    "FunctionExecutionConfigTypeDef",
     {
         "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigOutputTypeDef,
+        "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
 )
 
-FunctionExecutionConfigOutputTypeDef = TypedDict(
-    "FunctionExecutionConfigOutputTypeDef",
+ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
+    "ListGroupCertificateAuthoritiesResponseTypeDef",
     {
-        "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigOutputTypeDef,
+        "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
+    {
+        "Groups": List[GroupInformationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LocalDeviceResourceDataTypeDef = TypedDict(
+    "LocalDeviceResourceDataTypeDef",
+    {
+        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
+        "SourcePath": str,
     },
     total=False,
 )
 
-FunctionDefaultExecutionConfigTypeDef = TypedDict(
-    "FunctionDefaultExecutionConfigTypeDef",
+LocalVolumeResourceDataTypeDef = TypedDict(
+    "LocalVolumeResourceDataTypeDef",
     {
-        "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigTypeDef,
+        "DestinationPath": str,
+        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
+        "SourcePath": str,
     },
     total=False,
 )
 
-FunctionExecutionConfigTypeDef = TypedDict(
-    "FunctionExecutionConfigTypeDef",
+_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     {
-        "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigTypeDef,
+        "BulkDeploymentId": str,
+    },
+)
+_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GetGroupVersionResponseTypeDef = TypedDict(
-    "GetGroupVersionResponseTypeDef",
+class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
+    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+):
+    pass
+
+ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": GroupVersionOutputTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
-    "ListGroupCertificateAuthoritiesResponseTypeDef",
+_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     {
-        "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConnectorDefinitionId": str,
     },
 )
+_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
+class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
+    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     {
-        "Groups": List[GroupInformationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-LocalDeviceResourceDataOutputTypeDef = TypedDict(
-    "LocalDeviceResourceDataOutputTypeDef",
+_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     {
-        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
-        "SourcePath": str,
+        "CoreDefinitionId": str,
+    },
+)
+_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LocalVolumeResourceDataOutputTypeDef = TypedDict(
-    "LocalVolumeResourceDataOutputTypeDef",
+class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
+    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     {
-        "DestinationPath": str,
-        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
-        "SourcePath": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LocalDeviceResourceDataTypeDef = TypedDict(
-    "LocalDeviceResourceDataTypeDef",
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
-        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
-        "SourcePath": str,
+        "GroupId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LocalVolumeResourceDataTypeDef = TypedDict(
-    "LocalVolumeResourceDataTypeDef",
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     {
-        "DestinationPath": str,
-        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
-        "SourcePath": str,
+        "DeviceDefinitionId": str,
+    },
+)
+_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
+    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
+    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
+    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+):
+    pass
+
+ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "LoggerDefinitionId": str,
+    },
+)
+_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
+    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
+    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "SubscriptionDefinitionId": str,
+    },
+)
+_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
+    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListConnectorDefinitionVersionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoreDefinitionVersionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupVersionsResponseTypeDef = TypedDict(
     "ListGroupVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggerDefinitionVersionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LoggerDefinitionVersionOutputTypeDef = TypedDict(
-    "LoggerDefinitionVersionOutputTypeDef",
-    {
-        "Loggers": List[LoggerOutputTypeDef],
-    },
-    total=False,
-)
-
-S3MachineLearningModelResourceDataOutputTypeDef = TypedDict(
-    "S3MachineLearningModelResourceDataOutputTypeDef",
-    {
-        "DestinationPath": str,
-        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
-        "S3Uri": str,
-    },
-    total=False,
-)
-
-SageMakerMachineLearningModelResourceDataOutputTypeDef = TypedDict(
-    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
-    {
-        "DestinationPath": str,
-        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
-        "SageMakerJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 S3MachineLearningModelResourceDataTypeDef = TypedDict(
     "S3MachineLearningModelResourceDataTypeDef",
     {
         "DestinationPath": str,
         "OwnerSetting": ResourceDownloadOwnerSettingTypeDef,
@@ -3157,63 +2834,53 @@
     "RuntimeConfigurationTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationTypeDef,
     },
     total=False,
 )
 
-SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
-    "SubscriptionDefinitionVersionOutputTypeDef",
-    {
-        "Subscriptions": List[SubscriptionOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationUpdateTypeDef,
     },
     total=False,
 )
 
-
 class UpdateThingRuntimeConfigurationRequestRequestTypeDef(
     _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef,
     _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 ListBulkDeploymentDetailedReportsResponseTypeDef = TypedDict(
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
     "GetConnectorDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ConnectorDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -3229,98 +2896,115 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": CoreDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": DeviceDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateDeviceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": DeviceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateLoggerDefinitionRequestRequestTypeDef",
+GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionVersionResponseTypeDef",
     {
-        "AmznClientToken": str,
-        "InitialVersion": LoggerDefinitionVersionTypeDef,
-        "Name": str,
-        "tags": Mapping[str, str],
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": LoggerDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionRequestRequestTypeDef",
+CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateLoggerDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": SubscriptionDefinitionVersionTypeDef,
+        "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionVersionResponseTypeDef",
+GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": DeviceDefinitionVersionOutputTypeDef,
+        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionDefaultConfigOutputTypeDef = TypedDict(
-    "FunctionDefaultConfigOutputTypeDef",
+CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionRequestRequestTypeDef",
     {
-        "Execution": FunctionDefaultExecutionConfigOutputTypeDef,
+        "AmznClientToken": str,
+        "InitialVersion": SubscriptionDefinitionVersionTypeDef,
+        "Name": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
-    "FunctionConfigurationEnvironmentOutputTypeDef",
+FunctionDefaultConfigTypeDef = TypedDict(
+    "FunctionDefaultConfigTypeDef",
     {
-        "AccessSysfs": bool,
-        "Execution": FunctionExecutionConfigOutputTypeDef,
-        "ResourceAccessPolicies": List[ResourceAccessPolicyOutputTypeDef],
-        "Variables": Dict[str, str],
+        "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
 
-FunctionDefaultConfigTypeDef = TypedDict(
-    "FunctionDefaultConfigTypeDef",
+FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
+    "FunctionConfigurationEnvironmentOutputTypeDef",
     {
-        "Execution": FunctionDefaultExecutionConfigTypeDef,
+        "AccessSysfs": bool,
+        "Execution": FunctionExecutionConfigTypeDef,
+        "ResourceAccessPolicies": List[ResourceAccessPolicyTypeDef],
+        "Variables": Dict[str, str],
     },
     total=False,
 )
 
 FunctionConfigurationEnvironmentTypeDef = TypedDict(
     "FunctionConfigurationEnvironmentTypeDef",
     {
@@ -3328,34 +3012,22 @@
         "Execution": FunctionExecutionConfigTypeDef,
         "ResourceAccessPolicies": Sequence[ResourceAccessPolicyTypeDef],
         "Variables": Mapping[str, str],
     },
     total=False,
 )
 
-GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": LoggerDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceDataContainerOutputTypeDef = TypedDict(
     "ResourceDataContainerOutputTypeDef",
     {
-        "LocalDeviceResourceData": LocalDeviceResourceDataOutputTypeDef,
-        "LocalVolumeResourceData": LocalVolumeResourceDataOutputTypeDef,
-        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataOutputTypeDef,
+        "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
+        "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
+        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
         "SageMakerMachineLearningModelResourceData": (
-            SageMakerMachineLearningModelResourceDataOutputTypeDef
+            SageMakerMachineLearningModelResourceDataTypeDef
         ),
         "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataOutputTypeDef,
     },
     total=False,
 )
 
 ResourceDataContainerTypeDef = TypedDict(
@@ -3372,28 +3044,15 @@
     total=False,
 )
 
 GetThingRuntimeConfigurationResponseTypeDef = TypedDict(
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "NextToken": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FunctionConfigurationOutputTypeDef = TypedDict(
     "FunctionConfigurationOutputTypeDef",
     {
         "EncodingType": EncodingTypeType,
@@ -3452,19 +3111,17 @@
     {
         "FunctionArn": str,
         "FunctionConfiguration": FunctionConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class FunctionOutputTypeDef(_RequiredFunctionOutputTypeDef, _OptionalFunctionOutputTypeDef):
     pass
 
-
 _RequiredFunctionTypeDef = TypedDict(
     "_RequiredFunctionTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalFunctionTypeDef = TypedDict(
@@ -3472,19 +3129,17 @@
     {
         "FunctionArn": str,
         "FunctionConfiguration": FunctionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class FunctionTypeDef(_RequiredFunctionTypeDef, _OptionalFunctionTypeDef):
     pass
 
-
 ResourceDefinitionVersionOutputTypeDef = TypedDict(
     "ResourceDefinitionVersionOutputTypeDef",
     {
         "Resources": List[ResourceOutputTypeDef],
     },
     total=False,
 )
@@ -3500,34 +3155,32 @@
     {
         "AmznClientToken": str,
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
-
 class CreateResourceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceDefinitionVersionTypeDef = TypedDict(
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
 FunctionDefinitionVersionOutputTypeDef = TypedDict(
     "FunctionDefinitionVersionOutputTypeDef",
     {
-        "DefaultConfig": FunctionDefaultConfigOutputTypeDef,
+        "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": List[FunctionOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
@@ -3541,22 +3194,20 @@
         "AmznClientToken": str,
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
-
 class CreateFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 FunctionDefinitionVersionTypeDef = TypedDict(
     "FunctionDefinitionVersionTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
@@ -3566,15 +3217,15 @@
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ResourceDefinitionVersionOutputTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateResourceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -3590,15 +3241,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": FunctionDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateFunctionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
```

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.pyi` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,257 +32,241 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateRoleToGroupRequestRequestTypeDef",
-    "AssociateRoleToGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
-    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "ConnectorOutputTypeDef",
     "ConnectorTypeDef",
-    "CoreOutputTypeDef",
     "CoreTypeDef",
-    "CreateConnectorDefinitionResponseTypeDef",
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    "CreateCoreDefinitionResponseTypeDef",
-    "CreateCoreDefinitionVersionResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateDeviceDefinitionResponseTypeDef",
     "DeviceTypeDef",
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    "CreateFunctionDefinitionResponseTypeDef",
-    "CreateFunctionDefinitionVersionResponseTypeDef",
     "CreateGroupCertificateAuthorityRequestRequestTypeDef",
-    "CreateGroupCertificateAuthorityResponseTypeDef",
     "GroupVersionTypeDef",
-    "CreateGroupResponseTypeDef",
     "CreateGroupVersionRequestRequestTypeDef",
-    "CreateGroupVersionResponseTypeDef",
-    "CreateLoggerDefinitionResponseTypeDef",
     "LoggerTypeDef",
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    "CreateResourceDefinitionResponseTypeDef",
-    "CreateResourceDefinitionVersionResponseTypeDef",
     "CreateSoftwareUpdateJobRequestRequestTypeDef",
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    "CreateSubscriptionDefinitionResponseTypeDef",
     "SubscriptionTypeDef",
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
     "DefinitionInformationTypeDef",
     "DeleteConnectorDefinitionRequestRequestTypeDef",
     "DeleteCoreDefinitionRequestRequestTypeDef",
     "DeleteDeviceDefinitionRequestRequestTypeDef",
     "DeleteFunctionDefinitionRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteLoggerDefinitionRequestRequestTypeDef",
     "DeleteResourceDefinitionRequestRequestTypeDef",
     "DeleteSubscriptionDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "DeviceOutputTypeDef",
     "DisassociateRoleFromGroupRequestRequestTypeDef",
-    "DisassociateRoleFromGroupResponseTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ResourceAccessPolicyOutputTypeDef",
     "ResourceAccessPolicyTypeDef",
-    "FunctionRunAsConfigOutputTypeDef",
     "FunctionRunAsConfigTypeDef",
     "GetAssociatedRoleRequestRequestTypeDef",
-    "GetAssociatedRoleResponseTypeDef",
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetConnectorDefinitionRequestRequestTypeDef",
-    "GetConnectorDefinitionResponseTypeDef",
     "GetConnectorDefinitionVersionRequestRequestTypeDef",
     "GetCoreDefinitionRequestRequestTypeDef",
-    "GetCoreDefinitionResponseTypeDef",
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     "GetDeploymentStatusRequestRequestTypeDef",
     "GetDeviceDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionResponseTypeDef",
     "GetDeviceDefinitionVersionRequestRequestTypeDef",
     "GetFunctionDefinitionRequestRequestTypeDef",
-    "GetFunctionDefinitionResponseTypeDef",
     "GetFunctionDefinitionVersionRequestRequestTypeDef",
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
-    "GetGroupCertificateAuthorityResponseTypeDef",
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
-    "GetGroupCertificateConfigurationResponseTypeDef",
     "GetGroupRequestRequestTypeDef",
-    "GetGroupResponseTypeDef",
     "GetGroupVersionRequestRequestTypeDef",
-    "GroupVersionOutputTypeDef",
     "GetLoggerDefinitionRequestRequestTypeDef",
-    "GetLoggerDefinitionResponseTypeDef",
     "GetLoggerDefinitionVersionRequestRequestTypeDef",
     "GetResourceDefinitionRequestRequestTypeDef",
-    "GetResourceDefinitionResponseTypeDef",
     "GetResourceDefinitionVersionRequestRequestTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
     "GetSubscriptionDefinitionRequestRequestTypeDef",
-    "GetSubscriptionDefinitionResponseTypeDef",
     "GetSubscriptionDefinitionVersionRequestRequestTypeDef",
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     "GroupCertificateAuthorityPropertiesTypeDef",
     "GroupInformationTypeDef",
-    "GroupOwnerSettingOutputTypeDef",
     "GroupOwnerSettingTypeDef",
-    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBulkDeploymentDetailedReportsRequestRequestTypeDef",
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     "ListBulkDeploymentsRequestRequestTypeDef",
-    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsRequestRequestTypeDef",
     "VersionInformationTypeDef",
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionsRequestRequestTypeDef",
-    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     "ListCoreDefinitionVersionsRequestRequestTypeDef",
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     "ListCoreDefinitionsRequestRequestTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
-    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     "ListDeviceDefinitionVersionsRequestRequestTypeDef",
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
     "ListDeviceDefinitionsRequestRequestTypeDef",
-    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
     "ListFunctionDefinitionVersionsRequestRequestTypeDef",
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
     "ListFunctionDefinitionsRequestRequestTypeDef",
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
-    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
     "ListGroupVersionsRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
     "ListLoggerDefinitionVersionsRequestRequestTypeDef",
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
     "ListLoggerDefinitionsRequestRequestTypeDef",
-    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
     "ListResourceDefinitionVersionsRequestRequestTypeDef",
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
     "ListResourceDefinitionsRequestRequestTypeDef",
-    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LoggerOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
-    "ResetDeploymentsResponseTypeDef",
     "SecretsManagerSecretResourceDataOutputTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
-    "ResourceDownloadOwnerSettingOutputTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
-    "ResponseMetadataTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
-    "StartBulkDeploymentResponseTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
-    "SubscriptionOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
     "UpdateConnectorDefinitionRequestRequestTypeDef",
     "UpdateCoreDefinitionRequestRequestTypeDef",
     "UpdateDeviceDefinitionRequestRequestTypeDef",
     "UpdateFunctionDefinitionRequestRequestTypeDef",
     "UpdateGroupCertificateConfigurationRequestRequestTypeDef",
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateLoggerDefinitionRequestRequestTypeDef",
     "UpdateResourceDefinitionRequestRequestTypeDef",
     "UpdateSubscriptionDefinitionRequestRequestTypeDef",
+    "AssociateRoleToGroupResponseTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    "CreateConnectorDefinitionResponseTypeDef",
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    "CreateCoreDefinitionResponseTypeDef",
+    "CreateCoreDefinitionVersionResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateDeviceDefinitionResponseTypeDef",
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    "CreateFunctionDefinitionResponseTypeDef",
+    "CreateFunctionDefinitionVersionResponseTypeDef",
+    "CreateGroupCertificateAuthorityResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateGroupVersionResponseTypeDef",
+    "CreateLoggerDefinitionResponseTypeDef",
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    "CreateResourceDefinitionResponseTypeDef",
+    "CreateResourceDefinitionVersionResponseTypeDef",
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    "CreateSubscriptionDefinitionResponseTypeDef",
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
+    "DisassociateRoleFromGroupResponseTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAssociatedRoleResponseTypeDef",
+    "GetConnectorDefinitionResponseTypeDef",
+    "GetCoreDefinitionResponseTypeDef",
+    "GetDeviceDefinitionResponseTypeDef",
+    "GetFunctionDefinitionResponseTypeDef",
+    "GetGroupCertificateAuthorityResponseTypeDef",
+    "GetGroupCertificateConfigurationResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetLoggerDefinitionResponseTypeDef",
+    "GetResourceDefinitionResponseTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
+    "GetSubscriptionDefinitionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResetDeploymentsResponseTypeDef",
+    "StartBulkDeploymentResponseTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
     "CreateConnectorDefinitionVersionRequestRequestTypeDef",
     "CoreDefinitionVersionOutputTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
+    "DeviceDefinitionVersionOutputTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "GetGroupVersionResponseTypeDef",
     "CreateLoggerDefinitionVersionRequestRequestTypeDef",
+    "LoggerDefinitionVersionOutputTypeDef",
     "LoggerDefinitionVersionTypeDef",
     "CreateSubscriptionDefinitionVersionRequestRequestTypeDef",
+    "SubscriptionDefinitionVersionOutputTypeDef",
     "SubscriptionDefinitionVersionTypeDef",
     "ListConnectorDefinitionsResponseTypeDef",
     "ListCoreDefinitionsResponseTypeDef",
     "ListDeviceDefinitionsResponseTypeDef",
     "ListFunctionDefinitionsResponseTypeDef",
     "ListLoggerDefinitionsResponseTypeDef",
     "ListResourceDefinitionsResponseTypeDef",
     "ListSubscriptionDefinitionsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
-    "DeviceDefinitionVersionOutputTypeDef",
-    "FunctionDefaultExecutionConfigOutputTypeDef",
-    "FunctionExecutionConfigOutputTypeDef",
     "FunctionDefaultExecutionConfigTypeDef",
     "FunctionExecutionConfigTypeDef",
-    "GetGroupVersionResponseTypeDef",
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     "ListGroupsResponseTypeDef",
-    "LocalDeviceResourceDataOutputTypeDef",
-    "LocalVolumeResourceDataOutputTypeDef",
     "LocalDeviceResourceDataTypeDef",
     "LocalVolumeResourceDataTypeDef",
+    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
+    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
+    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
+    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
+    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
+    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
+    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsResponseTypeDef",
     "ListCoreDefinitionVersionsResponseTypeDef",
     "ListDeviceDefinitionVersionsResponseTypeDef",
     "ListFunctionDefinitionVersionsResponseTypeDef",
     "ListGroupVersionsResponseTypeDef",
     "ListLoggerDefinitionVersionsResponseTypeDef",
     "ListResourceDefinitionVersionsResponseTypeDef",
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
-    "LoggerDefinitionVersionOutputTypeDef",
-    "S3MachineLearningModelResourceDataOutputTypeDef",
-    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
-    "SubscriptionDefinitionVersionOutputTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     "GetConnectorDefinitionVersionResponseTypeDef",
     "CreateConnectorDefinitionRequestRequestTypeDef",
     "GetCoreDefinitionVersionResponseTypeDef",
     "CreateCoreDefinitionRequestRequestTypeDef",
+    "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
+    "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionVersionResponseTypeDef",
-    "FunctionDefaultConfigOutputTypeDef",
-    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionDefaultConfigTypeDef",
+    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
-    "GetLoggerDefinitionVersionResponseTypeDef",
     "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
     "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "FunctionOutputTypeDef",
     "FunctionTypeDef",
     "ResourceDefinitionVersionOutputTypeDef",
@@ -301,37 +285,32 @@
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
     },
 )
 
-AssociateRoleToGroupResponseTypeDef = TypedDict(
-    "AssociateRoleToGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AssociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "RoleArn": str,
     },
 )
 
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BulkDeploymentMetricsTypeDef = TypedDict(
     "BulkDeploymentMetricsTypeDef",
     {
         "InvalidInputRecords": int,
         "RecordsProcessed": int,
         "RetryAttempts": int,
     },
@@ -353,25 +332,14 @@
         "BulkDeploymentArn": str,
         "BulkDeploymentId": str,
         "CreatedAt": str,
     },
     total=False,
 )
 
-ConnectivityInfoOutputTypeDef = TypedDict(
-    "ConnectivityInfoOutputTypeDef",
-    {
-        "HostAddress": str,
-        "Id": str,
-        "Metadata": str,
-        "PortNumber": int,
-    },
-    total=False,
-)
-
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "HostAddress": str,
         "Id": str,
         "Metadata": str,
         "PortNumber": int,
@@ -390,17 +358,19 @@
     "_OptionalConnectorOutputTypeDef",
     {
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
+
 class ConnectorOutputTypeDef(_RequiredConnectorOutputTypeDef, _OptionalConnectorOutputTypeDef):
     pass
 
+
 _RequiredConnectorTypeDef = TypedDict(
     "_RequiredConnectorTypeDef",
     {
         "ConnectorArn": str,
         "Id": str,
     },
 )
@@ -408,35 +378,18 @@
     "_OptionalConnectorTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ConnectorTypeDef(_RequiredConnectorTypeDef, _OptionalConnectorTypeDef):
     pass
 
-_RequiredCoreOutputTypeDef = TypedDict(
-    "_RequiredCoreOutputTypeDef",
-    {
-        "CertificateArn": str,
-        "Id": str,
-        "ThingArn": str,
-    },
-)
-_OptionalCoreOutputTypeDef = TypedDict(
-    "_OptionalCoreOutputTypeDef",
-    {
-        "SyncShadow": bool,
-    },
-    total=False,
-)
-
-class CoreOutputTypeDef(_RequiredCoreOutputTypeDef, _OptionalCoreOutputTypeDef):
-    pass
 
 _RequiredCoreTypeDef = TypedDict(
     "_RequiredCoreTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
@@ -446,66 +399,18 @@
     "_OptionalCoreTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
+
 class CoreTypeDef(_RequiredCoreTypeDef, _OptionalCoreTypeDef):
     pass
 
-CreateConnectorDefinitionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCoreDefinitionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "DeploymentType": DeploymentTypeType,
         "GroupId": str,
     },
@@ -516,41 +421,20 @@
         "AmznClientToken": str,
         "DeploymentId": str,
         "GroupVersionId": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDeviceDefinitionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
@@ -560,52 +444,18 @@
     "_OptionalDeviceTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
+
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
-CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFunctionDefinitionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
@@ -613,27 +463,21 @@
     "_OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "AmznClientToken": str,
     },
     total=False,
 )
 
+
 class CreateGroupCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "CreateGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GroupVersionTypeDef = TypedDict(
     "GroupVersionTypeDef",
     {
         "ConnectorDefinitionVersionArn": str,
         "CoreDefinitionVersionArn": str,
         "DeviceDefinitionVersionArn": str,
@@ -641,28 +485,14 @@
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateGroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupVersionRequestRequestTypeDef = TypedDict(
@@ -676,44 +506,21 @@
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
+
 class CreateGroupVersionRequestRequestTypeDef(
     _RequiredCreateGroupVersionRequestRequestTypeDef,
     _OptionalCreateGroupVersionRequestRequestTypeDef,
 ):
     pass
 
-CreateGroupVersionResponseTypeDef = TypedDict(
-    "CreateGroupVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLoggerDefinitionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredLoggerTypeDef = TypedDict(
     "_RequiredLoggerTypeDef",
     {
         "Component": LoggerComponentType,
         "Id": str,
         "Level": LoggerLevelType,
@@ -724,52 +531,18 @@
     "_OptionalLoggerTypeDef",
     {
         "Space": int,
     },
     total=False,
 )
 
+
 class LoggerTypeDef(_RequiredLoggerTypeDef, _OptionalLoggerTypeDef):
     pass
 
-CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateResourceDefinitionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSoftwareUpdateJobRequestRequestTypeDef",
     {
         "S3UrlSignerRole": str,
         "SoftwareToUpdate": SoftwareToUpdateType,
         "UpdateTargets": Sequence[str],
@@ -782,65 +555,32 @@
     {
         "AmznClientToken": str,
         "UpdateAgentLogLevel": UpdateAgentLogLevelType,
     },
     total=False,
 )
 
+
 class CreateSoftwareUpdateJobRequestRequestTypeDef(
     _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef,
     _OptionalCreateSoftwareUpdateJobRequestRequestTypeDef,
 ):
     pass
 
-CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    {
-        "IotJobArn": str,
-        "IotJobId": str,
-        "PlatformSoftwareVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Id": str,
         "Source": str,
         "Subject": str,
         "Target": str,
     },
 )
 
-CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DefinitionInformationTypeDef = TypedDict(
     "DefinitionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "LastUpdatedTimestamp": str,
@@ -916,109 +656,41 @@
         "DeploymentId": str,
         "DeploymentType": DeploymentTypeType,
         "GroupArn": str,
     },
     total=False,
 )
 
-_RequiredDeviceOutputTypeDef = TypedDict(
-    "_RequiredDeviceOutputTypeDef",
-    {
-        "CertificateArn": str,
-        "Id": str,
-        "ThingArn": str,
-    },
-)
-_OptionalDeviceOutputTypeDef = TypedDict(
-    "_OptionalDeviceOutputTypeDef",
-    {
-        "SyncShadow": bool,
-    },
-    total=False,
-)
-
-class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
-    pass
-
 DisassociateRoleFromGroupRequestRequestTypeDef = TypedDict(
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-DisassociateRoleFromGroupResponseTypeDef = TypedDict(
-    "DisassociateRoleFromGroupResponseTypeDef",
-    {
-        "DisassociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "DisassociatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredResourceAccessPolicyOutputTypeDef = TypedDict(
-    "_RequiredResourceAccessPolicyOutputTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalResourceAccessPolicyOutputTypeDef = TypedDict(
-    "_OptionalResourceAccessPolicyOutputTypeDef",
-    {
-        "Permission": PermissionType,
-    },
-    total=False,
-)
-
-class ResourceAccessPolicyOutputTypeDef(
-    _RequiredResourceAccessPolicyOutputTypeDef, _OptionalResourceAccessPolicyOutputTypeDef
-):
-    pass
-
 _RequiredResourceAccessPolicyTypeDef = TypedDict(
     "_RequiredResourceAccessPolicyTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalResourceAccessPolicyTypeDef = TypedDict(
     "_OptionalResourceAccessPolicyTypeDef",
     {
         "Permission": PermissionType,
     },
     total=False,
 )
 
+
 class ResourceAccessPolicyTypeDef(
     _RequiredResourceAccessPolicyTypeDef, _OptionalResourceAccessPolicyTypeDef
 ):
     pass
 
-FunctionRunAsConfigOutputTypeDef = TypedDict(
-    "FunctionRunAsConfigOutputTypeDef",
-    {
-        "Gid": int,
-        "Uid": int,
-    },
-    total=False,
-)
 
 FunctionRunAsConfigTypeDef = TypedDict(
     "FunctionRunAsConfigTypeDef",
     {
         "Gid": int,
         "Uid": int,
     },
@@ -1028,23 +700,14 @@
 GetAssociatedRoleRequestRequestTypeDef = TypedDict(
     "GetAssociatedRoleRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-GetAssociatedRoleResponseTypeDef = TypedDict(
-    "GetAssociatedRoleResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBulkDeploymentStatusRequestRequestTypeDef = TypedDict(
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -1058,29 +721,14 @@
 GetConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "GetConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 
-GetConnectorDefinitionResponseTypeDef = TypedDict(
-    "GetConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
         "ConnectorDefinitionVersionId": str,
     },
 )
@@ -1088,42 +736,29 @@
     "_OptionalGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalGetConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetCoreDefinitionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 
-GetCoreDefinitionResponseTypeDef = TypedDict(
-    "GetCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCoreDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
         "CoreDefinitionVersionId": str,
     },
 )
@@ -1139,29 +774,14 @@
 GetDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "GetDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 
-GetDeviceDefinitionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
         "DeviceDefinitionVersionId": str,
     },
 )
@@ -1169,42 +789,29 @@
     "_OptionalGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalGetDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "GetFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 
-GetFunctionDefinitionResponseTypeDef = TypedDict(
-    "GetFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
         "FunctionDefinitionVersionId": str,
     },
 )
@@ -1212,121 +819,59 @@
     "_OptionalGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetFunctionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityId": str,
         "GroupId": str,
     },
 )
 
-GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "GetGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "GroupCertificateAuthorityId": str,
-        "PemEncodedCertificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "GetGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupVersionRequestRequestTypeDef = TypedDict(
     "GetGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
         "GroupVersionId": str,
     },
 )
 
-GroupVersionOutputTypeDef = TypedDict(
-    "GroupVersionOutputTypeDef",
-    {
-        "ConnectorDefinitionVersionArn": str,
-        "CoreDefinitionVersionArn": str,
-        "DeviceDefinitionVersionArn": str,
-        "FunctionDefinitionVersionArn": str,
-        "LoggerDefinitionVersionArn": str,
-        "ResourceDefinitionVersionArn": str,
-        "SubscriptionDefinitionVersionArn": str,
-    },
-    total=False,
-)
-
 GetLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "GetLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 
-GetLoggerDefinitionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
         "LoggerDefinitionVersionId": str,
     },
 )
@@ -1334,81 +879,44 @@
     "_OptionalGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalGetLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourceDefinitionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 
-GetResourceDefinitionResponseTypeDef = TypedDict(
-    "GetResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionVersionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
         "ResourceDefinitionVersionId": str,
     },
 )
 
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 
-GetSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
         "SubscriptionDefinitionVersionId": str,
     },
 )
@@ -1416,20 +924,22 @@
     "_OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 
@@ -1452,52 +962,33 @@
         "LatestVersion": str,
         "LatestVersionArn": str,
         "Name": str,
     },
     total=False,
 )
 
-GroupOwnerSettingOutputTypeDef = TypedDict(
-    "GroupOwnerSettingOutputTypeDef",
-    {
-        "AutoAddGroupOwner": bool,
-        "GroupOwner": str,
-    },
-    total=False,
-)
-
 GroupOwnerSettingTypeDef = TypedDict(
     "GroupOwnerSettingTypeDef",
     {
         "AutoAddGroupOwner": bool,
         "GroupOwner": str,
     },
     total=False,
 )
 
-_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    {
-        "BulkDeploymentId": str,
-    },
-)
-_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
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
 
-class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
-    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-):
-    pass
-
 _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
@@ -1505,57 +996,31 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListBulkDeploymentDetailedReportsRequestRequestTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef,
 ):
     pass
 
-ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListBulkDeploymentsRequestRequestTypeDef = TypedDict(
     "ListBulkDeploymentsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
-    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConnectorDefinitionVersionsRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1563,68 +1028,42 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListConnectorDefinitionVersionsRequestRequestTypeDef(
     _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef,
     _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 VersionInformationTypeDef = TypedDict(
     "VersionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "Version": str,
     },
     total=False,
 )
 
-ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConnectorDefinitionsRequestRequestTypeDef = TypedDict(
     "ListConnectorDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "CoreDefinitionId": str,
-    },
-)
-_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
-    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCoreDefinitionVersionsRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1632,57 +1071,31 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListCoreDefinitionVersionsRequestRequestTypeDef(
     _RequiredListCoreDefinitionVersionsRequestRequestTypeDef,
     _OptionalListCoreDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListCoreDefinitionsRequestRequestTypeDef = TypedDict(
     "ListCoreDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1690,38 +1103,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "DeviceDefinitionId": str,
-    },
-)
-_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
-    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
@@ -1730,57 +1125,31 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDeviceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDeviceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
-    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionDefinitionVersionsRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1788,27 +1157,21 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFunctionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListFunctionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
@@ -1818,34 +1181,14 @@
 ListGroupCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
-_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
-    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupVersionsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListGroupVersionsRequestRequestTypeDef = TypedDict(
@@ -1853,56 +1196,30 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGroupVersionsRequestRequestTypeDef(
     _RequiredListGroupVersionsRequestRequestTypeDef, _OptionalListGroupVersionsRequestRequestTypeDef
 ):
     pass
 
-ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "LoggerDefinitionId": str,
-    },
-)
-_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
-    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLoggerDefinitionVersionsRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1910,57 +1227,31 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListLoggerDefinitionVersionsRequestRequestTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListLoggerDefinitionsRequestRequestTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
-    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceDefinitionVersionsRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1968,57 +1259,31 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResourceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListResourceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListResourceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListResourceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListResourceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "SubscriptionDefinitionId": str,
-    },
-)
-_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
-    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -2026,27 +1291,21 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSubscriptionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListSubscriptionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
@@ -2056,52 +1315,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
-_RequiredLoggerOutputTypeDef = TypedDict(
-    "_RequiredLoggerOutputTypeDef",
-    {
-        "Component": LoggerComponentType,
-        "Id": str,
-        "Level": LoggerLevelType,
-        "Type": LoggerTypeType,
-    },
-)
-_OptionalLoggerOutputTypeDef = TypedDict(
-    "_OptionalLoggerOutputTypeDef",
-    {
-        "Space": int,
-    },
-    total=False,
-)
-
-class LoggerOutputTypeDef(_RequiredLoggerOutputTypeDef, _OptionalLoggerOutputTypeDef):
-    pass
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
 _RequiredResetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredResetDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalResetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -2109,27 +1330,20 @@
     {
         "AmznClientToken": str,
         "Force": bool,
     },
     total=False,
 )
 
+
 class ResetDeploymentsRequestRequestTypeDef(
     _RequiredResetDeploymentsRequestRequestTypeDef, _OptionalResetDeploymentsRequestRequestTypeDef
 ):
     pass
 
-ResetDeploymentsResponseTypeDef = TypedDict(
-    "ResetDeploymentsResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SecretsManagerSecretResourceDataOutputTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataOutputTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": List[str],
     },
@@ -2141,60 +1355,43 @@
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
     total=False,
 )
 
-ResourceDownloadOwnerSettingOutputTypeDef = TypedDict(
-    "ResourceDownloadOwnerSettingOutputTypeDef",
-    {
-        "GroupOwner": str,
-        "GroupPermission": PermissionType,
-    },
-)
-
 ResourceDownloadOwnerSettingTypeDef = TypedDict(
     "ResourceDownloadOwnerSettingTypeDef",
     {
         "GroupOwner": str,
         "GroupPermission": PermissionType,
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
 _RequiredTelemetryConfigurationTypeDef = TypedDict(
     "_RequiredTelemetryConfigurationTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 _OptionalTelemetryConfigurationTypeDef = TypedDict(
     "_OptionalTelemetryConfigurationTypeDef",
     {
         "ConfigurationSyncStatus": ConfigurationSyncStatusType,
     },
     total=False,
 )
 
+
 class TelemetryConfigurationTypeDef(
     _RequiredTelemetryConfigurationTypeDef, _OptionalTelemetryConfigurationTypeDef
 ):
     pass
 
+
 _RequiredStartBulkDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDeploymentRequestRequestTypeDef",
     {
         "ExecutionRoleArn": str,
         "InputFileUri": str,
     },
 )
@@ -2203,65 +1400,50 @@
     {
         "AmznClientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartBulkDeploymentRequestRequestTypeDef(
     _RequiredStartBulkDeploymentRequestRequestTypeDef,
     _OptionalStartBulkDeploymentRequestRequestTypeDef,
 ):
     pass
 
-StartBulkDeploymentResponseTypeDef = TypedDict(
-    "StartBulkDeploymentResponseTypeDef",
-    {
-        "BulkDeploymentArn": str,
-        "BulkDeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
-SubscriptionOutputTypeDef = TypedDict(
-    "SubscriptionOutputTypeDef",
-    {
-        "Id": str,
-        "Source": str,
-        "Subject": str,
-        "Target": str,
-    },
-)
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 TelemetryConfigurationUpdateTypeDef = TypedDict(
     "TelemetryConfigurationUpdateTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 
@@ -2269,132 +1451,123 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "Message": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateConnectorDefinitionRequestRequestTypeDef(
     _RequiredUpdateConnectorDefinitionRequestRequestTypeDef,
     _OptionalUpdateConnectorDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateCoreDefinitionRequestRequestTypeDef(
     _RequiredUpdateCoreDefinitionRequestRequestTypeDef,
     _OptionalUpdateCoreDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateDeviceDefinitionRequestRequestTypeDef(
     _RequiredUpdateDeviceDefinitionRequestRequestTypeDef,
     _OptionalUpdateDeviceDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateFunctionDefinitionRequestRequestTypeDef(
     _RequiredUpdateFunctionDefinitionRequestRequestTypeDef,
     _OptionalUpdateFunctionDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "CertificateExpiryInMilliseconds": str,
     },
     total=False,
 )
 
+
 class UpdateGroupCertificateConfigurationRequestRequestTypeDef(
     _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef,
     _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
@@ -2402,79 +1575,556 @@
     "_OptionalUpdateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateLoggerDefinitionRequestRequestTypeDef(
     _RequiredUpdateLoggerDefinitionRequestRequestTypeDef,
     _OptionalUpdateLoggerDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateResourceDefinitionRequestRequestTypeDef(
     _RequiredUpdateResourceDefinitionRequestRequestTypeDef,
     _OptionalUpdateResourceDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateSubscriptionDefinitionRequestRequestTypeDef(
     _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef,
     _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
+AssociateRoleToGroupResponseTypeDef = TypedDict(
+    "AssociateRoleToGroupResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorDefinitionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCoreDefinitionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceDefinitionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFunctionDefinitionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "CreateGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupVersionResponseTypeDef = TypedDict(
+    "CreateGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLoggerDefinitionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourceDefinitionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    {
+        "IotJobArn": str,
+        "IotJobId": str,
+        "PlatformSoftwareVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateRoleFromGroupResponseTypeDef = TypedDict(
+    "DisassociateRoleFromGroupResponseTypeDef",
+    {
+        "DisassociatedAt": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "DisassociatedAt": str,
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
+GetAssociatedRoleResponseTypeDef = TypedDict(
+    "GetAssociatedRoleResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectorDefinitionResponseTypeDef = TypedDict(
+    "GetConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCoreDefinitionResponseTypeDef = TypedDict(
+    "GetCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceDefinitionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionDefinitionResponseTypeDef = TypedDict(
+    "GetFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "GetGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "GroupCertificateAuthorityId": str,
+        "PemEncodedCertificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "GetGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLoggerDefinitionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourceDefinitionResponseTypeDef = TypedDict(
+    "GetResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
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
+ResetDeploymentsResponseTypeDef = TypedDict(
+    "ResetDeploymentsResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartBulkDeploymentResponseTypeDef = TypedDict(
+    "StartBulkDeploymentResponseTypeDef",
+    {
+        "BulkDeploymentArn": str,
+        "BulkDeploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "Message": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BulkDeploymentResultTypeDef = TypedDict(
     "BulkDeploymentResultTypeDef",
     {
         "CreatedAt": str,
         "DeploymentArn": str,
         "DeploymentId": str,
         "DeploymentStatus": str,
@@ -2491,45 +2141,45 @@
     {
         "BulkDeploymentMetrics": BulkDeploymentMetricsTypeDef,
         "BulkDeploymentStatus": BulkDeploymentStatusType,
         "CreatedAt": str,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentStatusResponseTypeDef = TypedDict(
     "GetDeploymentStatusResponseTypeDef",
     {
         "DeploymentStatus": str,
         "DeploymentType": DeploymentTypeType,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "UpdatedAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBulkDeploymentsResponseTypeDef = TypedDict(
     "ListBulkDeploymentsResponseTypeDef",
     {
         "BulkDeployments": List[BulkDeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "ConnectivityInfo": List[ConnectivityInfoOutputTypeDef],
+        "ConnectivityInfo": List[ConnectivityInfoTypeDef],
         "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ThingName": str,
@@ -2539,20 +2189,22 @@
     "_OptionalUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ConnectivityInfo": Sequence[ConnectivityInfoTypeDef],
     },
     total=False,
 )
 
+
 class UpdateConnectivityInfoRequestRequestTypeDef(
     _RequiredUpdateConnectivityInfoRequestRequestTypeDef,
     _OptionalUpdateConnectivityInfoRequestRequestTypeDef,
 ):
     pass
 
+
 ConnectorDefinitionVersionOutputTypeDef = TypedDict(
     "ConnectorDefinitionVersionOutputTypeDef",
     {
         "Connectors": List[ConnectorOutputTypeDef],
     },
     total=False,
 )
@@ -2576,24 +2228,26 @@
     {
         "AmznClientToken": str,
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
+
 class CreateConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 CoreDefinitionVersionOutputTypeDef = TypedDict(
     "CoreDefinitionVersionOutputTypeDef",
     {
-        "Cores": List[CoreOutputTypeDef],
+        "Cores": List[CoreTypeDef],
     },
     total=False,
 )
 
 CoreDefinitionVersionTypeDef = TypedDict(
     "CoreDefinitionVersionTypeDef",
     {
@@ -2613,20 +2267,22 @@
     {
         "AmznClientToken": str,
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
 
+
 class CreateCoreDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateCoreDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateCoreDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -2634,20 +2290,30 @@
     {
         "AmznClientToken": str,
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
+DeviceDefinitionVersionOutputTypeDef = TypedDict(
+    "DeviceDefinitionVersionOutputTypeDef",
+    {
+        "Devices": List[DeviceTypeDef],
+    },
+    total=False,
+)
+
 DeviceDefinitionVersionTypeDef = TypedDict(
     "DeviceDefinitionVersionTypeDef",
     {
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
 )
@@ -2664,19 +2330,33 @@
         "AmznClientToken": str,
         "InitialVersion": GroupVersionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+
+GetGroupVersionResponseTypeDef = TypedDict(
+    "GetGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": GroupVersionTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -2684,20 +2364,30 @@
     {
         "AmznClientToken": str,
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
 )
 
+
 class CreateLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
+LoggerDefinitionVersionOutputTypeDef = TypedDict(
+    "LoggerDefinitionVersionOutputTypeDef",
+    {
+        "Loggers": List[LoggerTypeDef],
+    },
+    total=False,
+)
+
 LoggerDefinitionVersionTypeDef = TypedDict(
     "LoggerDefinitionVersionTypeDef",
     {
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
 )
@@ -2713,309 +2403,526 @@
     {
         "AmznClientToken": str,
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
 )
 
+
 class CreateSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
+SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
+    "SubscriptionDefinitionVersionOutputTypeDef",
+    {
+        "Subscriptions": List[SubscriptionTypeDef],
+    },
+    total=False,
+)
+
 SubscriptionDefinitionVersionTypeDef = TypedDict(
     "SubscriptionDefinitionVersionTypeDef",
     {
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
 )
 
 ListConnectorDefinitionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoreDefinitionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceDefinitionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionDefinitionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggerDefinitionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceDefinitionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionDefinitionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeviceDefinitionVersionOutputTypeDef = TypedDict(
-    "DeviceDefinitionVersionOutputTypeDef",
+FunctionDefaultExecutionConfigTypeDef = TypedDict(
+    "FunctionDefaultExecutionConfigTypeDef",
     {
-        "Devices": List[DeviceOutputTypeDef],
+        "IsolationMode": FunctionIsolationModeType,
+        "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
 )
 
-FunctionDefaultExecutionConfigOutputTypeDef = TypedDict(
-    "FunctionDefaultExecutionConfigOutputTypeDef",
+FunctionExecutionConfigTypeDef = TypedDict(
+    "FunctionExecutionConfigTypeDef",
     {
         "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigOutputTypeDef,
+        "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
 )
 
-FunctionExecutionConfigOutputTypeDef = TypedDict(
-    "FunctionExecutionConfigOutputTypeDef",
+ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
+    "ListGroupCertificateAuthoritiesResponseTypeDef",
     {
-        "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigOutputTypeDef,
+        "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
+    {
+        "Groups": List[GroupInformationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LocalDeviceResourceDataTypeDef = TypedDict(
+    "LocalDeviceResourceDataTypeDef",
+    {
+        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
+        "SourcePath": str,
     },
     total=False,
 )
 
-FunctionDefaultExecutionConfigTypeDef = TypedDict(
-    "FunctionDefaultExecutionConfigTypeDef",
+LocalVolumeResourceDataTypeDef = TypedDict(
+    "LocalVolumeResourceDataTypeDef",
     {
-        "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigTypeDef,
+        "DestinationPath": str,
+        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
+        "SourcePath": str,
     },
     total=False,
 )
 
-FunctionExecutionConfigTypeDef = TypedDict(
-    "FunctionExecutionConfigTypeDef",
+_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     {
-        "IsolationMode": FunctionIsolationModeType,
-        "RunAs": FunctionRunAsConfigTypeDef,
+        "BulkDeploymentId": str,
+    },
+)
+_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GetGroupVersionResponseTypeDef = TypedDict(
-    "GetGroupVersionResponseTypeDef",
+
+class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
+    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+):
+    pass
+
+
+ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": GroupVersionOutputTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
-    "ListGroupCertificateAuthoritiesResponseTypeDef",
+_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     {
-        "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConnectorDefinitionId": str,
+    },
+)
+_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
+
+class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
+    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     {
-        "Groups": List[GroupInformationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-LocalDeviceResourceDataOutputTypeDef = TypedDict(
-    "LocalDeviceResourceDataOutputTypeDef",
+_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     {
-        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
-        "SourcePath": str,
+        "CoreDefinitionId": str,
+    },
+)
+_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LocalVolumeResourceDataOutputTypeDef = TypedDict(
-    "LocalVolumeResourceDataOutputTypeDef",
+
+class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
+    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     {
-        "DestinationPath": str,
-        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
-        "SourcePath": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LocalDeviceResourceDataTypeDef = TypedDict(
-    "LocalDeviceResourceDataTypeDef",
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
-        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
-        "SourcePath": str,
+        "GroupId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LocalVolumeResourceDataTypeDef = TypedDict(
-    "LocalVolumeResourceDataTypeDef",
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     {
-        "DestinationPath": str,
-        "GroupOwnerSetting": GroupOwnerSettingTypeDef,
-        "SourcePath": str,
+        "DeviceDefinitionId": str,
+    },
+)
+_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
+    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
+    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
+    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "LoggerDefinitionId": str,
+    },
+)
+_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
+    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
+    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "SubscriptionDefinitionId": str,
+    },
+)
+_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
+    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListConnectorDefinitionVersionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoreDefinitionVersionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupVersionsResponseTypeDef = TypedDict(
     "ListGroupVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggerDefinitionVersionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LoggerDefinitionVersionOutputTypeDef = TypedDict(
-    "LoggerDefinitionVersionOutputTypeDef",
-    {
-        "Loggers": List[LoggerOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
-)
-
-S3MachineLearningModelResourceDataOutputTypeDef = TypedDict(
-    "S3MachineLearningModelResourceDataOutputTypeDef",
-    {
-        "DestinationPath": str,
-        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
-        "S3Uri": str,
-    },
-    total=False,
-)
-
-SageMakerMachineLearningModelResourceDataOutputTypeDef = TypedDict(
-    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
-    {
-        "DestinationPath": str,
-        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
-        "SageMakerJobArn": str,
-    },
-    total=False,
 )
 
 S3MachineLearningModelResourceDataTypeDef = TypedDict(
     "S3MachineLearningModelResourceDataTypeDef",
     {
         "DestinationPath": str,
         "OwnerSetting": ResourceDownloadOwnerSettingTypeDef,
@@ -3038,61 +2945,55 @@
     "RuntimeConfigurationTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationTypeDef,
     },
     total=False,
 )
 
-SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
-    "SubscriptionDefinitionVersionOutputTypeDef",
-    {
-        "Subscriptions": List[SubscriptionOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationUpdateTypeDef,
     },
     total=False,
 )
 
+
 class UpdateThingRuntimeConfigurationRequestRequestTypeDef(
     _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef,
     _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 ListBulkDeploymentDetailedReportsResponseTypeDef = TypedDict(
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
     "GetConnectorDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ConnectorDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -3108,98 +3009,115 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": CoreDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": DeviceDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateDeviceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": DeviceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateLoggerDefinitionRequestRequestTypeDef",
+GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionVersionResponseTypeDef",
     {
-        "AmznClientToken": str,
-        "InitialVersion": LoggerDefinitionVersionTypeDef,
-        "Name": str,
-        "tags": Mapping[str, str],
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": LoggerDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionRequestRequestTypeDef",
+CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateLoggerDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": SubscriptionDefinitionVersionTypeDef,
+        "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionVersionResponseTypeDef",
+GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": DeviceDefinitionVersionOutputTypeDef,
+        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionDefaultConfigOutputTypeDef = TypedDict(
-    "FunctionDefaultConfigOutputTypeDef",
+CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionRequestRequestTypeDef",
     {
-        "Execution": FunctionDefaultExecutionConfigOutputTypeDef,
+        "AmznClientToken": str,
+        "InitialVersion": SubscriptionDefinitionVersionTypeDef,
+        "Name": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
-    "FunctionConfigurationEnvironmentOutputTypeDef",
+FunctionDefaultConfigTypeDef = TypedDict(
+    "FunctionDefaultConfigTypeDef",
     {
-        "AccessSysfs": bool,
-        "Execution": FunctionExecutionConfigOutputTypeDef,
-        "ResourceAccessPolicies": List[ResourceAccessPolicyOutputTypeDef],
-        "Variables": Dict[str, str],
+        "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
 
-FunctionDefaultConfigTypeDef = TypedDict(
-    "FunctionDefaultConfigTypeDef",
+FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
+    "FunctionConfigurationEnvironmentOutputTypeDef",
     {
-        "Execution": FunctionDefaultExecutionConfigTypeDef,
+        "AccessSysfs": bool,
+        "Execution": FunctionExecutionConfigTypeDef,
+        "ResourceAccessPolicies": List[ResourceAccessPolicyTypeDef],
+        "Variables": Dict[str, str],
     },
     total=False,
 )
 
 FunctionConfigurationEnvironmentTypeDef = TypedDict(
     "FunctionConfigurationEnvironmentTypeDef",
     {
@@ -3207,34 +3125,22 @@
         "Execution": FunctionExecutionConfigTypeDef,
         "ResourceAccessPolicies": Sequence[ResourceAccessPolicyTypeDef],
         "Variables": Mapping[str, str],
     },
     total=False,
 )
 
-GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": LoggerDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceDataContainerOutputTypeDef = TypedDict(
     "ResourceDataContainerOutputTypeDef",
     {
-        "LocalDeviceResourceData": LocalDeviceResourceDataOutputTypeDef,
-        "LocalVolumeResourceData": LocalVolumeResourceDataOutputTypeDef,
-        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataOutputTypeDef,
+        "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
+        "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
+        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
         "SageMakerMachineLearningModelResourceData": (
-            SageMakerMachineLearningModelResourceDataOutputTypeDef
+            SageMakerMachineLearningModelResourceDataTypeDef
         ),
         "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataOutputTypeDef,
     },
     total=False,
 )
 
 ResourceDataContainerTypeDef = TypedDict(
@@ -3251,28 +3157,15 @@
     total=False,
 )
 
 GetThingRuntimeConfigurationResponseTypeDef = TypedDict(
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "NextToken": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FunctionConfigurationOutputTypeDef = TypedDict(
     "FunctionConfigurationOutputTypeDef",
     {
         "EncodingType": EncodingTypeType,
@@ -3331,17 +3224,19 @@
     {
         "FunctionArn": str,
         "FunctionConfiguration": FunctionConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class FunctionOutputTypeDef(_RequiredFunctionOutputTypeDef, _OptionalFunctionOutputTypeDef):
     pass
 
+
 _RequiredFunctionTypeDef = TypedDict(
     "_RequiredFunctionTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalFunctionTypeDef = TypedDict(
@@ -3349,17 +3244,19 @@
     {
         "FunctionArn": str,
         "FunctionConfiguration": FunctionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class FunctionTypeDef(_RequiredFunctionTypeDef, _OptionalFunctionTypeDef):
     pass
 
+
 ResourceDefinitionVersionOutputTypeDef = TypedDict(
     "ResourceDefinitionVersionOutputTypeDef",
     {
         "Resources": List[ResourceOutputTypeDef],
     },
     total=False,
 )
@@ -3375,32 +3272,34 @@
     {
         "AmznClientToken": str,
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
+
 class CreateResourceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceDefinitionVersionTypeDef = TypedDict(
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
 FunctionDefinitionVersionOutputTypeDef = TypedDict(
     "FunctionDefinitionVersionOutputTypeDef",
     {
-        "DefaultConfig": FunctionDefaultConfigOutputTypeDef,
+        "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": List[FunctionOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
@@ -3414,20 +3313,22 @@
         "AmznClientToken": str,
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
+
 class CreateFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 FunctionDefinitionVersionTypeDef = TypedDict(
     "FunctionDefinitionVersionTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
@@ -3437,15 +3338,15 @@
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ResourceDefinitionVersionOutputTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateResourceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -3461,15 +3362,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": FunctionDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateFunctionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
```

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/PKG-INFO` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.28.12
-Summary: Type annotations for boto3.Greengrass 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,255 +423,238 @@
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
-    AssociateRoleToGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     ConnectorOutputTypeDef,
     ConnectorTypeDef,
-    CoreOutputTypeDef,
     CoreTypeDef,
-    CreateConnectorDefinitionResponseTypeDef,
-    CreateConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionResponseTypeDef,
-    CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateDeviceDefinitionResponseTypeDef,
     DeviceTypeDef,
-    CreateDeviceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionResponseTypeDef,
-    CreateFunctionDefinitionVersionResponseTypeDef,
     CreateGroupCertificateAuthorityRequestRequestTypeDef,
-    CreateGroupCertificateAuthorityResponseTypeDef,
     GroupVersionTypeDef,
-    CreateGroupResponseTypeDef,
     CreateGroupVersionRequestRequestTypeDef,
-    CreateGroupVersionResponseTypeDef,
-    CreateLoggerDefinitionResponseTypeDef,
     LoggerTypeDef,
-    CreateLoggerDefinitionVersionResponseTypeDef,
-    CreateResourceDefinitionResponseTypeDef,
-    CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobRequestRequestTypeDef,
-    CreateSoftwareUpdateJobResponseTypeDef,
-    CreateSubscriptionDefinitionResponseTypeDef,
     SubscriptionTypeDef,
-    CreateSubscriptionDefinitionVersionResponseTypeDef,
     DefinitionInformationTypeDef,
     DeleteConnectorDefinitionRequestRequestTypeDef,
     DeleteCoreDefinitionRequestRequestTypeDef,
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DeviceOutputTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
-    DisassociateRoleFromGroupResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ResourceAccessPolicyOutputTypeDef,
     ResourceAccessPolicyTypeDef,
-    FunctionRunAsConfigOutputTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
-    GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
-    GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionRequestRequestTypeDef,
-    GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionRequestRequestTypeDef,
     GetDeploymentStatusRequestRequestTypeDef,
     GetDeviceDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionResponseTypeDef,
     GetDeviceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionRequestRequestTypeDef,
-    GetFunctionDefinitionResponseTypeDef,
     GetFunctionDefinitionVersionRequestRequestTypeDef,
     GetGroupCertificateAuthorityRequestRequestTypeDef,
-    GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
-    GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
-    GroupVersionOutputTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
-    GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
-    GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
-    GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
-    GroupOwnerSettingOutputTypeDef,
     GroupOwnerSettingTypeDef,
-    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
-    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
-    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
     VersionInformationTypeDef,
-    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
     ListConnectorDefinitionsRequestRequestTypeDef,
-    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     ListCoreDefinitionVersionsRequestRequestTypeDef,
-    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
     ListCoreDefinitionsRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     ListDeviceDefinitionVersionsRequestRequestTypeDef,
-    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
     ListDeviceDefinitionsRequestRequestTypeDef,
-    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     ListFunctionDefinitionVersionsRequestRequestTypeDef,
-    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
     ListFunctionDefinitionsRequestRequestTypeDef,
     ListGroupCertificateAuthoritiesRequestRequestTypeDef,
-    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     ListGroupVersionsRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     ListLoggerDefinitionVersionsRequestRequestTypeDef,
-    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
     ListLoggerDefinitionsRequestRequestTypeDef,
-    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     ListResourceDefinitionVersionsRequestRequestTypeDef,
-    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
     ListResourceDefinitionsRequestRequestTypeDef,
-    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
-    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LoggerOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
-    ResetDeploymentsResponseTypeDef,
     SecretsManagerSecretResourceDataOutputTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
-    ResourceDownloadOwnerSettingOutputTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
-    ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
-    StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
-    SubscriptionOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
     UpdateFunctionDefinitionRequestRequestTypeDef,
     UpdateGroupCertificateConfigurationRequestRequestTypeDef,
-    UpdateGroupCertificateConfigurationResponseTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateLoggerDefinitionRequestRequestTypeDef,
     UpdateResourceDefinitionRequestRequestTypeDef,
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
+    AssociateRoleToGroupResponseTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
+    CreateConnectorDefinitionResponseTypeDef,
+    CreateConnectorDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionResponseTypeDef,
+    CreateCoreDefinitionVersionResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateDeviceDefinitionResponseTypeDef,
+    CreateDeviceDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionResponseTypeDef,
+    CreateFunctionDefinitionVersionResponseTypeDef,
+    CreateGroupCertificateAuthorityResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateGroupVersionResponseTypeDef,
+    CreateLoggerDefinitionResponseTypeDef,
+    CreateLoggerDefinitionVersionResponseTypeDef,
+    CreateResourceDefinitionResponseTypeDef,
+    CreateResourceDefinitionVersionResponseTypeDef,
+    CreateSoftwareUpdateJobResponseTypeDef,
+    CreateSubscriptionDefinitionResponseTypeDef,
+    CreateSubscriptionDefinitionVersionResponseTypeDef,
+    DisassociateRoleFromGroupResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssociatedRoleResponseTypeDef,
+    GetConnectorDefinitionResponseTypeDef,
+    GetCoreDefinitionResponseTypeDef,
+    GetDeviceDefinitionResponseTypeDef,
+    GetFunctionDefinitionResponseTypeDef,
+    GetGroupCertificateAuthorityResponseTypeDef,
+    GetGroupCertificateConfigurationResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetLoggerDefinitionResponseTypeDef,
+    GetResourceDefinitionResponseTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
+    GetSubscriptionDefinitionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResetDeploymentsResponseTypeDef,
+    StartBulkDeploymentResponseTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
+    UpdateGroupCertificateConfigurationResponseTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
     CreateConnectorDefinitionVersionRequestRequestTypeDef,
     CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
+    GetGroupVersionResponseTypeDef,
     CreateLoggerDefinitionVersionRequestRequestTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
     LoggerDefinitionVersionTypeDef,
     CreateSubscriptionDefinitionVersionRequestRequestTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     ListConnectorDefinitionsResponseTypeDef,
     ListCoreDefinitionsResponseTypeDef,
     ListDeviceDefinitionsResponseTypeDef,
     ListFunctionDefinitionsResponseTypeDef,
     ListLoggerDefinitionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
-    DeviceDefinitionVersionOutputTypeDef,
-    FunctionDefaultExecutionConfigOutputTypeDef,
-    FunctionExecutionConfigOutputTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
-    GetGroupVersionResponseTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
-    LocalDeviceResourceDataOutputTypeDef,
-    LocalVolumeResourceDataOutputTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
+    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
+    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
+    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
+    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
+    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
+    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
+    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
-    LoggerDefinitionVersionOutputTypeDef,
-    S3MachineLearningModelResourceDataOutputTypeDef,
-    SageMakerMachineLearningModelResourceDataOutputTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
-    SubscriptionDefinitionVersionOutputTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     CreateConnectorDefinitionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionRequestRequestTypeDef,
+    GetDeviceDefinitionVersionResponseTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
+    GetLoggerDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
+    GetSubscriptionDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionVersionResponseTypeDef,
-    FunctionDefaultConfigOutputTypeDef,
-    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionDefaultConfigTypeDef,
+    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
-    GetLoggerDefinitionVersionResponseTypeDef,
     ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
-    GetSubscriptionDefinitionVersionResponseTypeDef,
     FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     FunctionOutputTypeDef,
     FunctionTypeDef,
     ResourceDefinitionVersionOutputTypeDef,
```

### Comparing `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/SOURCES.txt` & `mypy-boto3-greengrass-1.28.15/mypy_boto3_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.12/setup.py` & `mypy-boto3-greengrass-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrass",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Greengrass 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

