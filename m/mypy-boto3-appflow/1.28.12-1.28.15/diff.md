# Comparing `tmp/mypy-boto3-appflow-1.28.12.tar.gz` & `tmp/mypy-boto3-appflow-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appflow-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-appflow-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-appflow-1.28.12.tar` & `mypy-boto3-appflow-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.356577 mypy-boto3-appflow-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-07-27 05:34:18.348577 mypy-boto3-appflow-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.344577 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   101626 2023-07-27 05:17:22.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   101472 2023-07-27 05:17:21.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.348577 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.356577 mypy-boto3-appflow-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.240654 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-07-28 20:19:18.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-28 20:19:18.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-07-28 20:19:19.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-28 20:19:18.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85991 2023-07-28 20:19:21.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85859 2023-07-28 20:19:20.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:16.000000 mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.244654 mypy-boto3-appflow-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:19:17.000000 mypy-boto3-appflow-1.28.15/setup.py
```

### Comparing `mypy-boto3-appflow-1.28.12/LICENSE` & `mypy-boto3-appflow-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.12/PKG-INFO` & `mypy-boto3-appflow-1.28.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.12
-Summary: Type annotations for boto3.Appflow 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,209 +339,164 @@
 ### Typed dictionaries
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
-    AggregationConfigOutputTypeDef,
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
-    AmplitudeSourcePropertiesOutputTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
-    CancelFlowExecutionsResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectorRuntimeSettingTypeDef,
-    DataTransferApiOutputTypeDef,
+    DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
     SlackMetadataTypeDef,
     SnowflakeMetadataTypeDef,
     ZendeskMetadataTypeDef,
     ConnectorOAuthRequestTypeDef,
-    ConnectorOperatorOutputTypeDef,
     ConnectorOperatorTypeDef,
     DatadogConnectorProfileCredentialsTypeDef,
     DynatraceConnectorProfileCredentialsTypeDef,
     InforNexusConnectorProfileCredentialsTypeDef,
     RedshiftConnectorProfileCredentialsTypeDef,
     ServiceNowConnectorProfileCredentialsTypeDef,
     SingularConnectorProfileCredentialsTypeDef,
     SnowflakeConnectorProfileCredentialsTypeDef,
     TrendmicroConnectorProfileCredentialsTypeDef,
     VeevaConnectorProfileCredentialsTypeDef,
-    DatadogConnectorProfilePropertiesOutputTypeDef,
-    DynatraceConnectorProfilePropertiesOutputTypeDef,
-    InforNexusConnectorProfilePropertiesOutputTypeDef,
-    MarketoConnectorProfilePropertiesOutputTypeDef,
-    PardotConnectorProfilePropertiesOutputTypeDef,
-    RedshiftConnectorProfilePropertiesOutputTypeDef,
-    SalesforceConnectorProfilePropertiesOutputTypeDef,
-    ServiceNowConnectorProfilePropertiesOutputTypeDef,
-    SlackConnectorProfilePropertiesOutputTypeDef,
-    SnowflakeConnectorProfilePropertiesOutputTypeDef,
-    VeevaConnectorProfilePropertiesOutputTypeDef,
-    ZendeskConnectorProfilePropertiesOutputTypeDef,
     DatadogConnectorProfilePropertiesTypeDef,
     DynatraceConnectorProfilePropertiesTypeDef,
     InforNexusConnectorProfilePropertiesTypeDef,
     MarketoConnectorProfilePropertiesTypeDef,
     PardotConnectorProfilePropertiesTypeDef,
     RedshiftConnectorProfilePropertiesTypeDef,
     SalesforceConnectorProfilePropertiesTypeDef,
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
-    LambdaConnectorProvisioningConfigOutputTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
-    ErrorHandlingConfigOutputTypeDef,
     ErrorHandlingConfigTypeDef,
     OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
-    DataTransferApiTypeDef,
-    CustomerProfilesDestinationPropertiesOutputTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
-    DatadogSourcePropertiesOutputTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     DescribeConnectorsRequestRequestTypeDef,
     DescribeFlowExecutionRecordsRequestRequestTypeDef,
     DescribeFlowRequestRequestTypeDef,
     ExecutionDetailsTypeDef,
-    DynatraceSourcePropertiesOutputTypeDef,
     DynatraceSourcePropertiesTypeDef,
     ErrorInfoTypeDef,
     RangeTypeDef,
-    GlueDataCatalogConfigOutputTypeDef,
     GlueDataCatalogConfigTypeDef,
-    GoogleAnalyticsSourcePropertiesOutputTypeDef,
     GoogleAnalyticsSourcePropertiesTypeDef,
-    IncrementalPullConfigOutputTypeDef,
     IncrementalPullConfigTypeDef,
-    InforNexusSourcePropertiesOutputTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MarketoSourcePropertiesOutputTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
     OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
-    PardotSourcePropertiesOutputTypeDef,
     PardotSourcePropertiesTypeDef,
     PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
-    RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3InputFormatConfigOutputTypeDef,
     S3InputFormatConfigTypeDef,
-    SuccessResponseHandlingConfigOutputTypeDef,
     SuccessResponseHandlingConfigTypeDef,
-    SAPODataSourcePropertiesOutputTypeDef,
     SAPODataSourcePropertiesTypeDef,
-    SalesforceSourcePropertiesOutputTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesOutputTypeDef,
     ScheduledTriggerPropertiesTypeDef,
-    ServiceNowSourcePropertiesOutputTypeDef,
     ServiceNowSourcePropertiesTypeDef,
-    SingularSourcePropertiesOutputTypeDef,
     SingularSourcePropertiesTypeDef,
-    SlackSourcePropertiesOutputTypeDef,
     SlackSourcePropertiesTypeDef,
-    TrendmicroSourcePropertiesOutputTypeDef,
-    VeevaSourcePropertiesOutputTypeDef,
-    ZendeskSourcePropertiesOutputTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CustomAuthConfigTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterConnectorResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
-    CustomAuthConfigTypeDef,
     CustomConnectorSourcePropertiesOutputTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
     TaskOutputTypeDef,
     TaskTypeDef,
-    ConnectorProvisioningConfigOutputTypeDef,
     ConnectorProvisioningConfigTypeDef,
     CustomConnectorDestinationPropertiesOutputTypeDef,
-    EventBridgeDestinationPropertiesOutputTypeDef,
-    HoneycodeDestinationPropertiesOutputTypeDef,
-    MarketoDestinationPropertiesOutputTypeDef,
-    RedshiftDestinationPropertiesOutputTypeDef,
-    SalesforceDestinationPropertiesOutputTypeDef,
-    SnowflakeDestinationPropertiesOutputTypeDef,
-    ZendeskDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     ZendeskDestinationPropertiesTypeDef,
     CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
-    MetadataCatalogConfigOutputTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
     SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
     S3OutputFormatConfigOutputTypeDef,
     UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
-    S3SourcePropertiesOutputTypeDef,
     S3SourcePropertiesTypeDef,
     SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
     TriggerPropertiesOutputTypeDef,
     TriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
@@ -581,15 +536,15 @@
     UpdateConnectorProfileRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
     CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigOutputTypeDef:
+def get_structure() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.12/README.md` & `mypy-boto3-appflow-1.28.15/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,209 +307,164 @@
 ### Typed dictionaries
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
-    AggregationConfigOutputTypeDef,
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
-    AmplitudeSourcePropertiesOutputTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
-    CancelFlowExecutionsResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectorRuntimeSettingTypeDef,
-    DataTransferApiOutputTypeDef,
+    DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
     SlackMetadataTypeDef,
     SnowflakeMetadataTypeDef,
     ZendeskMetadataTypeDef,
     ConnectorOAuthRequestTypeDef,
-    ConnectorOperatorOutputTypeDef,
     ConnectorOperatorTypeDef,
     DatadogConnectorProfileCredentialsTypeDef,
     DynatraceConnectorProfileCredentialsTypeDef,
     InforNexusConnectorProfileCredentialsTypeDef,
     RedshiftConnectorProfileCredentialsTypeDef,
     ServiceNowConnectorProfileCredentialsTypeDef,
     SingularConnectorProfileCredentialsTypeDef,
     SnowflakeConnectorProfileCredentialsTypeDef,
     TrendmicroConnectorProfileCredentialsTypeDef,
     VeevaConnectorProfileCredentialsTypeDef,
-    DatadogConnectorProfilePropertiesOutputTypeDef,
-    DynatraceConnectorProfilePropertiesOutputTypeDef,
-    InforNexusConnectorProfilePropertiesOutputTypeDef,
-    MarketoConnectorProfilePropertiesOutputTypeDef,
-    PardotConnectorProfilePropertiesOutputTypeDef,
-    RedshiftConnectorProfilePropertiesOutputTypeDef,
-    SalesforceConnectorProfilePropertiesOutputTypeDef,
-    ServiceNowConnectorProfilePropertiesOutputTypeDef,
-    SlackConnectorProfilePropertiesOutputTypeDef,
-    SnowflakeConnectorProfilePropertiesOutputTypeDef,
-    VeevaConnectorProfilePropertiesOutputTypeDef,
-    ZendeskConnectorProfilePropertiesOutputTypeDef,
     DatadogConnectorProfilePropertiesTypeDef,
     DynatraceConnectorProfilePropertiesTypeDef,
     InforNexusConnectorProfilePropertiesTypeDef,
     MarketoConnectorProfilePropertiesTypeDef,
     PardotConnectorProfilePropertiesTypeDef,
     RedshiftConnectorProfilePropertiesTypeDef,
     SalesforceConnectorProfilePropertiesTypeDef,
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
-    LambdaConnectorProvisioningConfigOutputTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
-    ErrorHandlingConfigOutputTypeDef,
     ErrorHandlingConfigTypeDef,
     OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
-    DataTransferApiTypeDef,
-    CustomerProfilesDestinationPropertiesOutputTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
-    DatadogSourcePropertiesOutputTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     DescribeConnectorsRequestRequestTypeDef,
     DescribeFlowExecutionRecordsRequestRequestTypeDef,
     DescribeFlowRequestRequestTypeDef,
     ExecutionDetailsTypeDef,
-    DynatraceSourcePropertiesOutputTypeDef,
     DynatraceSourcePropertiesTypeDef,
     ErrorInfoTypeDef,
     RangeTypeDef,
-    GlueDataCatalogConfigOutputTypeDef,
     GlueDataCatalogConfigTypeDef,
-    GoogleAnalyticsSourcePropertiesOutputTypeDef,
     GoogleAnalyticsSourcePropertiesTypeDef,
-    IncrementalPullConfigOutputTypeDef,
     IncrementalPullConfigTypeDef,
-    InforNexusSourcePropertiesOutputTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MarketoSourcePropertiesOutputTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
     OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
-    PardotSourcePropertiesOutputTypeDef,
     PardotSourcePropertiesTypeDef,
     PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
-    RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3InputFormatConfigOutputTypeDef,
     S3InputFormatConfigTypeDef,
-    SuccessResponseHandlingConfigOutputTypeDef,
     SuccessResponseHandlingConfigTypeDef,
-    SAPODataSourcePropertiesOutputTypeDef,
     SAPODataSourcePropertiesTypeDef,
-    SalesforceSourcePropertiesOutputTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesOutputTypeDef,
     ScheduledTriggerPropertiesTypeDef,
-    ServiceNowSourcePropertiesOutputTypeDef,
     ServiceNowSourcePropertiesTypeDef,
-    SingularSourcePropertiesOutputTypeDef,
     SingularSourcePropertiesTypeDef,
-    SlackSourcePropertiesOutputTypeDef,
     SlackSourcePropertiesTypeDef,
-    TrendmicroSourcePropertiesOutputTypeDef,
-    VeevaSourcePropertiesOutputTypeDef,
-    ZendeskSourcePropertiesOutputTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CustomAuthConfigTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterConnectorResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
-    CustomAuthConfigTypeDef,
     CustomConnectorSourcePropertiesOutputTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
     TaskOutputTypeDef,
     TaskTypeDef,
-    ConnectorProvisioningConfigOutputTypeDef,
     ConnectorProvisioningConfigTypeDef,
     CustomConnectorDestinationPropertiesOutputTypeDef,
-    EventBridgeDestinationPropertiesOutputTypeDef,
-    HoneycodeDestinationPropertiesOutputTypeDef,
-    MarketoDestinationPropertiesOutputTypeDef,
-    RedshiftDestinationPropertiesOutputTypeDef,
-    SalesforceDestinationPropertiesOutputTypeDef,
-    SnowflakeDestinationPropertiesOutputTypeDef,
-    ZendeskDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     ZendeskDestinationPropertiesTypeDef,
     CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
-    MetadataCatalogConfigOutputTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
     SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
     S3OutputFormatConfigOutputTypeDef,
     UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
-    S3SourcePropertiesOutputTypeDef,
     S3SourcePropertiesTypeDef,
     SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
     TriggerPropertiesOutputTypeDef,
     TriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
@@ -549,15 +504,15 @@
     UpdateConnectorProfileRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
     CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigOutputTypeDef:
+def get_structure() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__main__.py` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Appflow 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Appflow 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.py` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.pyi` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.py` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.pyi` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.py` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appflow service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appflow.type_defs import AggregationConfigOutputTypeDef
+    from mypy_boto3_appflow.type_defs import AggregationConfigTypeDef
 
-    data: AggregationConfigOutputTypeDef = {...}
+    data: AggregationConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -66,209 +66,164 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AggregationConfigOutputTypeDef",
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
-    "AmplitudeSourcePropertiesOutputTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
     "CancelFlowExecutionsRequestRequestTypeDef",
-    "CancelFlowExecutionsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectorRuntimeSettingTypeDef",
-    "DataTransferApiOutputTypeDef",
+    "DataTransferApiTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
     "HoneycodeMetadataTypeDef",
     "SalesforceMetadataTypeDef",
     "SlackMetadataTypeDef",
     "SnowflakeMetadataTypeDef",
     "ZendeskMetadataTypeDef",
     "ConnectorOAuthRequestTypeDef",
-    "ConnectorOperatorOutputTypeDef",
     "ConnectorOperatorTypeDef",
     "DatadogConnectorProfileCredentialsTypeDef",
     "DynatraceConnectorProfileCredentialsTypeDef",
     "InforNexusConnectorProfileCredentialsTypeDef",
     "RedshiftConnectorProfileCredentialsTypeDef",
     "ServiceNowConnectorProfileCredentialsTypeDef",
     "SingularConnectorProfileCredentialsTypeDef",
     "SnowflakeConnectorProfileCredentialsTypeDef",
     "TrendmicroConnectorProfileCredentialsTypeDef",
     "VeevaConnectorProfileCredentialsTypeDef",
-    "DatadogConnectorProfilePropertiesOutputTypeDef",
-    "DynatraceConnectorProfilePropertiesOutputTypeDef",
-    "InforNexusConnectorProfilePropertiesOutputTypeDef",
-    "MarketoConnectorProfilePropertiesOutputTypeDef",
-    "PardotConnectorProfilePropertiesOutputTypeDef",
-    "RedshiftConnectorProfilePropertiesOutputTypeDef",
-    "SalesforceConnectorProfilePropertiesOutputTypeDef",
-    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
-    "SlackConnectorProfilePropertiesOutputTypeDef",
-    "SnowflakeConnectorProfilePropertiesOutputTypeDef",
-    "VeevaConnectorProfilePropertiesOutputTypeDef",
-    "ZendeskConnectorProfilePropertiesOutputTypeDef",
     "DatadogConnectorProfilePropertiesTypeDef",
     "DynatraceConnectorProfilePropertiesTypeDef",
     "InforNexusConnectorProfilePropertiesTypeDef",
     "MarketoConnectorProfilePropertiesTypeDef",
     "PardotConnectorProfilePropertiesTypeDef",
     "RedshiftConnectorProfilePropertiesTypeDef",
     "SalesforceConnectorProfilePropertiesTypeDef",
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
-    "LambdaConnectorProvisioningConfigOutputTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
-    "CreateConnectorProfileResponseTypeDef",
-    "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
-    "ErrorHandlingConfigOutputTypeDef",
     "ErrorHandlingConfigTypeDef",
     "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
-    "DataTransferApiTypeDef",
-    "CustomerProfilesDestinationPropertiesOutputTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
-    "DatadogSourcePropertiesOutputTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "DescribeConnectorsRequestRequestTypeDef",
     "DescribeFlowExecutionRecordsRequestRequestTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "ExecutionDetailsTypeDef",
-    "DynatraceSourcePropertiesOutputTypeDef",
     "DynatraceSourcePropertiesTypeDef",
     "ErrorInfoTypeDef",
     "RangeTypeDef",
-    "GlueDataCatalogConfigOutputTypeDef",
     "GlueDataCatalogConfigTypeDef",
-    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
     "GoogleAnalyticsSourcePropertiesTypeDef",
-    "IncrementalPullConfigOutputTypeDef",
     "IncrementalPullConfigTypeDef",
-    "InforNexusSourcePropertiesOutputTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MarketoSourcePropertiesOutputTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
     "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
-    "PardotSourcePropertiesOutputTypeDef",
     "PardotSourcePropertiesTypeDef",
     "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
-    "RegisterConnectorResponseTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3InputFormatConfigOutputTypeDef",
     "S3InputFormatConfigTypeDef",
-    "SuccessResponseHandlingConfigOutputTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
-    "SAPODataSourcePropertiesOutputTypeDef",
     "SAPODataSourcePropertiesTypeDef",
-    "SalesforceSourcePropertiesOutputTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesOutputTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
-    "ServiceNowSourcePropertiesOutputTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
-    "SingularSourcePropertiesOutputTypeDef",
     "SingularSourcePropertiesTypeDef",
-    "SlackSourcePropertiesOutputTypeDef",
     "SlackSourcePropertiesTypeDef",
-    "TrendmicroSourcePropertiesOutputTypeDef",
-    "VeevaSourcePropertiesOutputTypeDef",
-    "ZendeskSourcePropertiesOutputTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
-    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
-    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CustomAuthConfigTypeDef",
+    "CancelFlowExecutionsResponseTypeDef",
+    "CreateConnectorProfileResponseTypeDef",
+    "CreateFlowResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterConnectorResponseTypeDef",
+    "StartFlowResponseTypeDef",
+    "StopFlowResponseTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
-    "CustomAuthConfigTypeDef",
     "CustomConnectorSourcePropertiesOutputTypeDef",
+    "CustomConnectorSourcePropertiesTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
     "TaskOutputTypeDef",
     "TaskTypeDef",
-    "ConnectorProvisioningConfigOutputTypeDef",
     "ConnectorProvisioningConfigTypeDef",
     "CustomConnectorDestinationPropertiesOutputTypeDef",
-    "EventBridgeDestinationPropertiesOutputTypeDef",
-    "HoneycodeDestinationPropertiesOutputTypeDef",
-    "MarketoDestinationPropertiesOutputTypeDef",
-    "RedshiftDestinationPropertiesOutputTypeDef",
-    "SalesforceDestinationPropertiesOutputTypeDef",
-    "SnowflakeDestinationPropertiesOutputTypeDef",
-    "ZendeskDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
+    "SalesforceDestinationPropertiesOutputTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
+    "ZendeskDestinationPropertiesOutputTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
     "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
-    "CustomConnectorSourcePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
-    "MetadataCatalogConfigOutputTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
     "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
     "S3OutputFormatConfigOutputTypeDef",
     "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
-    "S3SourcePropertiesOutputTypeDef",
     "S3SourcePropertiesTypeDef",
     "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
     "TriggerPropertiesOutputTypeDef",
     "TriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
@@ -307,23 +262,14 @@
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
     "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
-AggregationConfigOutputTypeDef = TypedDict(
-    "AggregationConfigOutputTypeDef",
-    {
-        "aggregationType": AggregationTypeType,
-        "targetFileSize": int,
-    },
-    total=False,
-)
-
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "targetFileSize": int,
     },
     total=False,
@@ -333,21 +279,14 @@
     "AmplitudeConnectorProfileCredentialsTypeDef",
     {
         "apiKey": str,
         "secretKey": str,
     },
 )
 
-AmplitudeSourcePropertiesOutputTypeDef = TypedDict(
-    "AmplitudeSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 AmplitudeSourcePropertiesTypeDef = TypedDict(
     "AmplitudeSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -411,19 +350,22 @@
 class CancelFlowExecutionsRequestRequestTypeDef(
     _RequiredCancelFlowExecutionsRequestRequestTypeDef,
     _OptionalCancelFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
 
-CancelFlowExecutionsResponseTypeDef = TypedDict(
-    "CancelFlowExecutionsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "invalidExecutions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectorRuntimeSettingTypeDef = TypedDict(
     "ConnectorRuntimeSettingTypeDef",
     {
         "key": str,
@@ -433,16 +375,16 @@
         "description": str,
         "scope": str,
         "connectorSuppliedValueOptions": List[str],
     },
     total=False,
 )
 
-DataTransferApiOutputTypeDef = TypedDict(
-    "DataTransferApiOutputTypeDef",
+DataTransferApiTypeDef = TypedDict(
+    "DataTransferApiTypeDef",
     {
         "Name": str,
         "Type": DataTransferApiTypeType,
     },
     total=False,
 )
 
@@ -563,38 +505,14 @@
     {
         "authCode": str,
         "redirectUri": str,
     },
     total=False,
 )
 
-ConnectorOperatorOutputTypeDef = TypedDict(
-    "ConnectorOperatorOutputTypeDef",
-    {
-        "Amplitude": Literal["BETWEEN"],
-        "Datadog": DatadogConnectorOperatorType,
-        "Dynatrace": DynatraceConnectorOperatorType,
-        "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
-        "InforNexus": InforNexusConnectorOperatorType,
-        "Marketo": MarketoConnectorOperatorType,
-        "S3": S3ConnectorOperatorType,
-        "Salesforce": SalesforceConnectorOperatorType,
-        "ServiceNow": ServiceNowConnectorOperatorType,
-        "Singular": SingularConnectorOperatorType,
-        "Slack": SlackConnectorOperatorType,
-        "Trendmicro": TrendmicroConnectorOperatorType,
-        "Veeva": VeevaConnectorOperatorType,
-        "Zendesk": ZendeskConnectorOperatorType,
-        "SAPOData": SAPODataConnectorOperatorType,
-        "CustomConnector": OperatorType,
-        "Pardot": PardotConnectorOperatorType,
-    },
-    total=False,
-)
-
 ConnectorOperatorTypeDef = TypedDict(
     "ConnectorOperatorTypeDef",
     {
         "Amplitude": Literal["BETWEEN"],
         "Datadog": DatadogConnectorOperatorType,
         "Dynatrace": DynatraceConnectorOperatorType,
         "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
@@ -683,146 +601,14 @@
     "VeevaConnectorProfileCredentialsTypeDef",
     {
         "username": str,
         "password": str,
     },
 )
 
-DatadogConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "DatadogConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-DynatraceConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "DynatraceConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-InforNexusConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "InforNexusConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-MarketoConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "MarketoConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-PardotConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "PardotConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-        "isSandboxEnvironment": bool,
-        "businessUnitId": str,
-    },
-    total=False,
-)
-
-_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-        "roleArn": str,
-    },
-)
-_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef",
-    {
-        "databaseUrl": str,
-        "bucketPrefix": str,
-        "dataApiRoleArn": str,
-        "isRedshiftServerless": bool,
-        "clusterIdentifier": str,
-        "workgroupName": str,
-        "databaseName": str,
-    },
-    total=False,
-)
-
-
-class RedshiftConnectorProfilePropertiesOutputTypeDef(
-    _RequiredRedshiftConnectorProfilePropertiesOutputTypeDef,
-    _OptionalRedshiftConnectorProfilePropertiesOutputTypeDef,
-):
-    pass
-
-
-SalesforceConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "SalesforceConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-        "isSandboxEnvironment": bool,
-        "usePrivateLinkForMetadataAndAuthorization": bool,
-    },
-    total=False,
-)
-
-ServiceNowConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-SlackConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "SlackConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef",
-    {
-        "warehouse": str,
-        "stage": str,
-        "bucketName": str,
-    },
-)
-_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "privateLinkServiceName": str,
-        "accountName": str,
-        "region": str,
-    },
-    total=False,
-)
-
-
-class SnowflakeConnectorProfilePropertiesOutputTypeDef(
-    _RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef,
-    _OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef,
-):
-    pass
-
-
-VeevaConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "VeevaConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-ZendeskConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "ZendeskConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
 DatadogConnectorProfilePropertiesTypeDef = TypedDict(
     "DatadogConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -957,45 +743,21 @@
         "status": PrivateConnectionProvisioningStatusType,
         "failureMessage": str,
         "failureCause": PrivateConnectionProvisioningFailureCauseType,
     },
     total=False,
 )
 
-LambdaConnectorProvisioningConfigOutputTypeDef = TypedDict(
-    "LambdaConnectorProvisioningConfigOutputTypeDef",
-    {
-        "lambdaArn": str,
-    },
-)
-
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
-CreateConnectorProfileResponseTypeDef = TypedDict(
-    "CreateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlowResponseTypeDef = TypedDict(
-    "CreateFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCustomAuthCredentialsTypeDef = TypedDict(
     "_RequiredCustomAuthCredentialsTypeDef",
     {
         "customAuthenticationType": str,
     },
 )
 _OptionalCustomAuthCredentialsTypeDef = TypedDict(
@@ -1009,24 +771,14 @@
 
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
 
-ErrorHandlingConfigOutputTypeDef = TypedDict(
-    "ErrorHandlingConfigOutputTypeDef",
-    {
-        "failOnFirstDestinationError": bool,
-        "bucketPrefix": str,
-        "bucketName": str,
-    },
-    total=False,
-)
-
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
@@ -1071,45 +823,14 @@
 )
 
 
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
 
-DataTransferApiTypeDef = TypedDict(
-    "DataTransferApiTypeDef",
-    {
-        "Name": str,
-        "Type": DataTransferApiTypeType,
-    },
-    total=False,
-)
-
-_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef",
-    {
-        "domainName": str,
-    },
-)
-_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef",
-    {
-        "objectTypeName": str,
-    },
-    total=False,
-)
-
-
-class CustomerProfilesDestinationPropertiesOutputTypeDef(
-    _RequiredCustomerProfilesDestinationPropertiesOutputTypeDef,
-    _OptionalCustomerProfilesDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
@@ -1124,21 +845,14 @@
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
 
-DatadogSourcePropertiesOutputTypeDef = TypedDict(
-    "DatadogSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1288,21 +1002,14 @@
         "mostRecentExecutionMessage": str,
         "mostRecentExecutionTime": datetime,
         "mostRecentExecutionStatus": ExecutionStatusType,
     },
     total=False,
 )
 
-DynatraceSourcePropertiesOutputTypeDef = TypedDict(
-    "DynatraceSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 DynatraceSourcePropertiesTypeDef = TypedDict(
     "DynatraceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1320,69 +1027,38 @@
     {
         "maximum": float,
         "minimum": float,
     },
     total=False,
 )
 
-GlueDataCatalogConfigOutputTypeDef = TypedDict(
-    "GlueDataCatalogConfigOutputTypeDef",
-    {
-        "roleArn": str,
-        "databaseName": str,
-        "tablePrefix": str,
-    },
-)
-
 GlueDataCatalogConfigTypeDef = TypedDict(
     "GlueDataCatalogConfigTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tablePrefix": str,
     },
 )
 
-GoogleAnalyticsSourcePropertiesOutputTypeDef = TypedDict(
-    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 GoogleAnalyticsSourcePropertiesTypeDef = TypedDict(
     "GoogleAnalyticsSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-IncrementalPullConfigOutputTypeDef = TypedDict(
-    "IncrementalPullConfigOutputTypeDef",
-    {
-        "datetimeTypeFieldName": str,
-    },
-    total=False,
-)
-
 IncrementalPullConfigTypeDef = TypedDict(
     "IncrementalPullConfigTypeDef",
     {
         "datetimeTypeFieldName": str,
     },
     total=False,
 )
 
-InforNexusSourcePropertiesOutputTypeDef = TypedDict(
-    "InforNexusSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 InforNexusSourcePropertiesTypeDef = TypedDict(
     "InforNexusSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1420,29 +1096,14 @@
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
-MarketoSourcePropertiesOutputTypeDef = TypedDict(
-    "MarketoSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1484,21 +1145,14 @@
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
 )
 
-PardotSourcePropertiesOutputTypeDef = TypedDict(
-    "PardotSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1518,119 +1172,51 @@
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
     total=False,
 )
 
-RegisterConnectorResponseTypeDef = TypedDict(
-    "RegisterConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResetConnectorMetadataCacheRequestRequestTypeDef = TypedDict(
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorEntityName": str,
         "entitiesPath": str,
         "apiVersion": str,
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
-S3InputFormatConfigOutputTypeDef = TypedDict(
-    "S3InputFormatConfigOutputTypeDef",
-    {
-        "s3InputFileType": S3InputFileTypeType,
-    },
-    total=False,
-)
-
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
 
-SuccessResponseHandlingConfigOutputTypeDef = TypedDict(
-    "SuccessResponseHandlingConfigOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "bucketName": str,
-    },
-    total=False,
-)
-
 SuccessResponseHandlingConfigTypeDef = TypedDict(
     "SuccessResponseHandlingConfigTypeDef",
     {
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
-SAPODataSourcePropertiesOutputTypeDef = TypedDict(
-    "SAPODataSourcePropertiesOutputTypeDef",
-    {
-        "objectPath": str,
-    },
-    total=False,
-)
-
 SAPODataSourcePropertiesTypeDef = TypedDict(
     "SAPODataSourcePropertiesTypeDef",
     {
         "objectPath": str,
     },
     total=False,
 )
 
-_RequiredSalesforceSourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredSalesforceSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalSalesforceSourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalSalesforceSourcePropertiesOutputTypeDef",
-    {
-        "enableDynamicFieldUpdate": bool,
-        "includeDeletedRecords": bool,
-        "dataTransferApi": SalesforceDataTransferApiType,
-    },
-    total=False,
-)
-
-
-class SalesforceSourcePropertiesOutputTypeDef(
-    _RequiredSalesforceSourcePropertiesOutputTypeDef,
-    _OptionalSalesforceSourcePropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredSalesforceSourcePropertiesTypeDef = TypedDict(
     "_RequiredSalesforceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceSourcePropertiesTypeDef = TypedDict(
@@ -1701,94 +1287,35 @@
 
 class ScheduledTriggerPropertiesTypeDef(
     _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
 ):
     pass
 
 
-ServiceNowSourcePropertiesOutputTypeDef = TypedDict(
-    "ServiceNowSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-SingularSourcePropertiesOutputTypeDef = TypedDict(
-    "SingularSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 SingularSourcePropertiesTypeDef = TypedDict(
     "SingularSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-SlackSourcePropertiesOutputTypeDef = TypedDict(
-    "SlackSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 SlackSourcePropertiesTypeDef = TypedDict(
     "SlackSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-TrendmicroSourcePropertiesOutputTypeDef = TypedDict(
-    "TrendmicroSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
-_RequiredVeevaSourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredVeevaSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalVeevaSourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalVeevaSourcePropertiesOutputTypeDef",
-    {
-        "documentType": str,
-        "includeSourceFiles": bool,
-        "includeRenditions": bool,
-        "includeAllVersions": bool,
-    },
-    total=False,
-)
-
-
-class VeevaSourcePropertiesOutputTypeDef(
-    _RequiredVeevaSourcePropertiesOutputTypeDef, _OptionalVeevaSourcePropertiesOutputTypeDef
-):
-    pass
-
-
-ZendeskSourcePropertiesOutputTypeDef = TypedDict(
-    "ZendeskSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 TrendmicroSourcePropertiesTypeDef = TypedDict(
     "TrendmicroSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1840,40 +1367,21 @@
 
 class StartFlowRequestRequestTypeDef(
     _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
 ):
     pass
 
 
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "executionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1904,85 +1412,167 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CustomAuthConfigTypeDef = TypedDict(
+    "CustomAuthConfigTypeDef",
+    {
+        "customAuthenticationType": str,
+        "authParameters": List[AuthParameterTypeDef],
+    },
+    total=False,
+)
+
+CancelFlowExecutionsResponseTypeDef = TypedDict(
+    "CancelFlowExecutionsResponseTypeDef",
+    {
+        "invalidExecutions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorProfileResponseTypeDef = TypedDict(
+    "CreateConnectorProfileResponseTypeDef",
+    {
+        "connectorProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFlowResponseTypeDef = TypedDict(
+    "CreateFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
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
+RegisterConnectorResponseTypeDef = TypedDict(
+    "RegisterConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "executionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateConnectorProfileResponseTypeDef = TypedDict(
     "UpdateConnectorProfileResponseTypeDef",
     {
         "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectorRegistrationResponseTypeDef = TypedDict(
     "UpdateConnectorRegistrationResponseTypeDef",
     {
         "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomAuthConfigTypeDef = TypedDict(
-    "CustomAuthConfigTypeDef",
-    {
-        "customAuthenticationType": str,
-        "authParameters": List[AuthParameterTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
     "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
     "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
     {
         "customProperties": Dict[str, str],
-        "dataTransferApi": DataTransferApiOutputTypeDef,
+        "dataTransferApi": DataTransferApiTypeDef,
     },
     total=False,
 )
 
 
 class CustomConnectorSourcePropertiesOutputTypeDef(
     _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
     _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
 ):
     pass
 
 
+_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+    {
+        "customProperties": Mapping[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
+    },
+    total=False,
+)
+
+
+class CustomConnectorSourcePropertiesTypeDef(
+    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+):
+    pass
+
+
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorEntitiesResponseTypeDef = TypedDict(
     "ListConnectorEntitiesResponseTypeDef",
     {
         "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorMetadataTypeDef = TypedDict(
     "ConnectorMetadataTypeDef",
     {
         "Amplitude": Dict[str, Any],
@@ -2182,15 +1772,15 @@
         "sourceFields": List[str],
         "taskType": TaskTypeType,
     },
 )
 _OptionalTaskOutputTypeDef = TypedDict(
     "_OptionalTaskOutputTypeDef",
     {
-        "connectorOperator": ConnectorOperatorOutputTypeDef,
+        "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Dict[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
 
@@ -2216,22 +1806,14 @@
 )
 
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
 
-ConnectorProvisioningConfigOutputTypeDef = TypedDict(
-    "ConnectorProvisioningConfigOutputTypeDef",
-    {
-        "lambda": LambdaConnectorProvisioningConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
@@ -2241,15 +1823,15 @@
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
     "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
     {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": List[str],
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
@@ -2257,177 +1839,14 @@
 class CustomConnectorDestinationPropertiesOutputTypeDef(
     _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
     _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
 ):
     pass
 
 
-_RequiredEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EventBridgeDestinationPropertiesOutputTypeDef(
-    _RequiredEventBridgeDestinationPropertiesOutputTypeDef,
-    _OptionalEventBridgeDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
-_RequiredHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredHoneycodeDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalHoneycodeDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class HoneycodeDestinationPropertiesOutputTypeDef(
-    _RequiredHoneycodeDestinationPropertiesOutputTypeDef,
-    _OptionalHoneycodeDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
-_RequiredMarketoDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredMarketoDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalMarketoDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalMarketoDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class MarketoDestinationPropertiesOutputTypeDef(
-    _RequiredMarketoDestinationPropertiesOutputTypeDef,
-    _OptionalMarketoDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
-_RequiredRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredRedshiftDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-        "intermediateBucketName": str,
-    },
-)
-_OptionalRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalRedshiftDestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class RedshiftDestinationPropertiesOutputTypeDef(
-    _RequiredRedshiftDestinationPropertiesOutputTypeDef,
-    _OptionalRedshiftDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
-_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-        "dataTransferApi": SalesforceDataTransferApiType,
-    },
-    total=False,
-)
-
-
-class SalesforceDestinationPropertiesOutputTypeDef(
-    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
-    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
-_RequiredSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSnowflakeDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-        "intermediateBucketName": str,
-    },
-)
-_OptionalSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSnowflakeDestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SnowflakeDestinationPropertiesOutputTypeDef(
-    _RequiredSnowflakeDestinationPropertiesOutputTypeDef,
-    _OptionalSnowflakeDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
-_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-    },
-    total=False,
-)
-
-
-class ZendeskDestinationPropertiesOutputTypeDef(
-    _RequiredZendeskDestinationPropertiesOutputTypeDef,
-    _OptionalZendeskDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -2532,14 +1951,39 @@
 
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
 
+_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+
+class SalesforceDestinationPropertiesOutputTypeDef(
+    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
+    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -2579,14 +2023,38 @@
 
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
 
+_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+
+class ZendeskDestinationPropertiesOutputTypeDef(
+    _RequiredZendeskDestinationPropertiesOutputTypeDef,
+    _OptionalZendeskDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -2620,36 +2088,14 @@
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesTypeDef",
-    {
-        "customProperties": Mapping[str, str],
-        "dataTransferApi": DataTransferApiTypeDef,
-    },
-    total=False,
-)
-
-
-class CustomConnectorSourcePropertiesTypeDef(
-    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
-):
-    pass
-
-
 FlowDefinitionTypeDef = TypedDict(
     "FlowDefinitionTypeDef",
     {
         "flowArn": str,
         "description": str,
         "flowName": str,
         "flowStatus": FlowStatusType,
@@ -2699,22 +2145,14 @@
 )
 
 
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
 
-MetadataCatalogConfigOutputTypeDef = TypedDict(
-    "MetadataCatalogConfigOutputTypeDef",
-    {
-        "glueDataCatalog": GlueDataCatalogConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
 )
@@ -2799,15 +2237,15 @@
 
 
 S3OutputFormatConfigOutputTypeDef = TypedDict(
     "S3OutputFormatConfigOutputTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigOutputTypeDef,
-        "aggregationConfig": AggregationConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
     },
     total=False,
 )
 
 _RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
     "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
@@ -2815,15 +2253,15 @@
         "prefixConfig": PrefixConfigOutputTypeDef,
     },
 )
 _OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
     "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
     {
         "fileType": FileTypeType,
-        "aggregationConfig": AggregationConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
 
 class UpsolverS3OutputFormatConfigOutputTypeDef(
     _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
@@ -2861,36 +2299,14 @@
 
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
 
-_RequiredS3SourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredS3SourcePropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3SourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalS3SourcePropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "s3InputFormatConfig": S3InputFormatConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class S3SourcePropertiesOutputTypeDef(
-    _RequiredS3SourcePropertiesOutputTypeDef, _OptionalS3SourcePropertiesOutputTypeDef
-):
-    pass
-
-
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -2914,17 +2330,17 @@
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
     "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
     {
-        "successResponseHandlingConfig": SuccessResponseHandlingConfigOutputTypeDef,
+        "successResponseHandlingConfig": SuccessResponseHandlingConfigTypeDef,
         "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
 
 class SAPODataDestinationPropertiesOutputTypeDef(
@@ -3045,15 +2461,15 @@
 
 
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SupportedFieldTypeDetailsTypeDef = TypedDict(
     "SupportedFieldTypeDetailsTypeDef",
     {
         "v1": FieldTypeDetailsTypeDef,
@@ -3088,32 +2504,32 @@
     total=False,
 )
 
 ConnectorProfilePropertiesOutputTypeDef = TypedDict(
     "ConnectorProfilePropertiesOutputTypeDef",
     {
         "Amplitude": Dict[str, Any],
-        "Datadog": DatadogConnectorProfilePropertiesOutputTypeDef,
-        "Dynatrace": DynatraceConnectorProfilePropertiesOutputTypeDef,
+        "Datadog": DatadogConnectorProfilePropertiesTypeDef,
+        "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Dict[str, Any],
         "Honeycode": Dict[str, Any],
-        "InforNexus": InforNexusConnectorProfilePropertiesOutputTypeDef,
-        "Marketo": MarketoConnectorProfilePropertiesOutputTypeDef,
-        "Redshift": RedshiftConnectorProfilePropertiesOutputTypeDef,
-        "Salesforce": SalesforceConnectorProfilePropertiesOutputTypeDef,
-        "ServiceNow": ServiceNowConnectorProfilePropertiesOutputTypeDef,
+        "InforNexus": InforNexusConnectorProfilePropertiesTypeDef,
+        "Marketo": MarketoConnectorProfilePropertiesTypeDef,
+        "Redshift": RedshiftConnectorProfilePropertiesTypeDef,
+        "Salesforce": SalesforceConnectorProfilePropertiesTypeDef,
+        "ServiceNow": ServiceNowConnectorProfilePropertiesTypeDef,
         "Singular": Dict[str, Any],
-        "Slack": SlackConnectorProfilePropertiesOutputTypeDef,
-        "Snowflake": SnowflakeConnectorProfilePropertiesOutputTypeDef,
+        "Slack": SlackConnectorProfilePropertiesTypeDef,
+        "Snowflake": SnowflakeConnectorProfilePropertiesTypeDef,
         "Trendmicro": Dict[str, Any],
-        "Veeva": VeevaConnectorProfilePropertiesOutputTypeDef,
-        "Zendesk": ZendeskConnectorProfilePropertiesOutputTypeDef,
+        "Veeva": VeevaConnectorProfilePropertiesTypeDef,
+        "Zendesk": ZendeskConnectorProfilePropertiesTypeDef,
         "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
-        "Pardot": PardotConnectorProfilePropertiesOutputTypeDef,
+        "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
@@ -3228,31 +2644,31 @@
 ):
     pass
 
 
 SourceConnectorPropertiesOutputTypeDef = TypedDict(
     "SourceConnectorPropertiesOutputTypeDef",
     {
-        "Amplitude": AmplitudeSourcePropertiesOutputTypeDef,
-        "Datadog": DatadogSourcePropertiesOutputTypeDef,
-        "Dynatrace": DynatraceSourcePropertiesOutputTypeDef,
-        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesOutputTypeDef,
-        "InforNexus": InforNexusSourcePropertiesOutputTypeDef,
-        "Marketo": MarketoSourcePropertiesOutputTypeDef,
-        "S3": S3SourcePropertiesOutputTypeDef,
-        "Salesforce": SalesforceSourcePropertiesOutputTypeDef,
-        "ServiceNow": ServiceNowSourcePropertiesOutputTypeDef,
-        "Singular": SingularSourcePropertiesOutputTypeDef,
-        "Slack": SlackSourcePropertiesOutputTypeDef,
-        "Trendmicro": TrendmicroSourcePropertiesOutputTypeDef,
-        "Veeva": VeevaSourcePropertiesOutputTypeDef,
-        "Zendesk": ZendeskSourcePropertiesOutputTypeDef,
-        "SAPOData": SAPODataSourcePropertiesOutputTypeDef,
+        "Amplitude": AmplitudeSourcePropertiesTypeDef,
+        "Datadog": DatadogSourcePropertiesTypeDef,
+        "Dynatrace": DynatraceSourcePropertiesTypeDef,
+        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
+        "InforNexus": InforNexusSourcePropertiesTypeDef,
+        "Marketo": MarketoSourcePropertiesTypeDef,
+        "S3": S3SourcePropertiesTypeDef,
+        "Salesforce": SalesforceSourcePropertiesTypeDef,
+        "ServiceNow": ServiceNowSourcePropertiesTypeDef,
+        "Singular": SingularSourcePropertiesTypeDef,
+        "Slack": SlackSourcePropertiesTypeDef,
+        "Trendmicro": TrendmicroSourcePropertiesTypeDef,
+        "Veeva": VeevaSourcePropertiesTypeDef,
+        "Zendesk": ZendeskSourcePropertiesTypeDef,
+        "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
-        "Pardot": PardotSourcePropertiesOutputTypeDef,
+        "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
@@ -3374,15 +2790,15 @@
 
 
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorConfigurationTypeDef = TypedDict(
     "ConnectorConfigurationTypeDef",
     {
         "canUseAsSource": bool,
@@ -3403,20 +2819,20 @@
         "connectorModes": List[str],
         "authenticationConfig": AuthenticationConfigTypeDef,
         "connectorRuntimeSettings": List[ConnectorRuntimeSettingTypeDef],
         "supportedApiVersions": List[str],
         "supportedOperators": List[OperatorsType],
         "supportedWriteOperations": List[WriteOperationTypeType],
         "connectorProvisioningType": Literal["LAMBDA"],
-        "connectorProvisioningConfig": ConnectorProvisioningConfigOutputTypeDef,
+        "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "logoURL": str,
         "registeredAt": datetime,
         "registeredBy": str,
         "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
-        "supportedDataTransferApis": List[DataTransferApiOutputTypeDef],
+        "supportedDataTransferApis": List[DataTransferApiTypeDef],
     },
     total=False,
 )
 
 ConnectorProfileTypeDef = TypedDict(
     "ConnectorProfileTypeDef",
     {
@@ -3433,25 +2849,25 @@
     },
     total=False,
 )
 
 DestinationConnectorPropertiesOutputTypeDef = TypedDict(
     "DestinationConnectorPropertiesOutputTypeDef",
     {
-        "Redshift": RedshiftDestinationPropertiesOutputTypeDef,
+        "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesOutputTypeDef,
         "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
-        "Snowflake": SnowflakeDestinationPropertiesOutputTypeDef,
-        "EventBridge": EventBridgeDestinationPropertiesOutputTypeDef,
+        "Snowflake": SnowflakeDestinationPropertiesTypeDef,
+        "EventBridge": EventBridgeDestinationPropertiesTypeDef,
         "LookoutMetrics": Dict[str, Any],
         "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
-        "Honeycode": HoneycodeDestinationPropertiesOutputTypeDef,
-        "CustomerProfiles": CustomerProfilesDestinationPropertiesOutputTypeDef,
+        "Honeycode": HoneycodeDestinationPropertiesTypeDef,
+        "CustomerProfiles": CustomerProfilesDestinationPropertiesTypeDef,
         "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
-        "Marketo": MarketoDestinationPropertiesOutputTypeDef,
+        "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
         "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
     },
     total=False,
 )
 
 DestinationConnectorPropertiesTypeDef = TypedDict(
@@ -3482,15 +2898,15 @@
     },
 )
 _OptionalSourceFlowConfigOutputTypeDef = TypedDict(
     "_OptionalSourceFlowConfigOutputTypeDef",
     {
         "apiVersion": str,
         "connectorProfileName": str,
-        "incrementalPullConfig": IncrementalPullConfigOutputTypeDef,
+        "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
 
 class SourceFlowConfigOutputTypeDef(
     _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
@@ -3541,42 +2957,42 @@
     pass
 
 
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "connectorConfiguration": ConnectorConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorsResponseTypeDef = TypedDict(
     "DescribeConnectorsResponseTypeDef",
     {
         "connectorConfigurations": Dict[ConnectorTypeType, ConnectorConfigurationTypeDef],
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorProfilesResponseTypeDef = TypedDict(
     "DescribeConnectorProfilesResponseTypeDef",
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigOutputTypeDef",
     {
         "connectorType": ConnectorTypeType,
@@ -3688,18 +3104,18 @@
         "triggerConfig": TriggerConfigOutputTypeDef,
         "tasks": List[TaskOutputTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigOutputTypeDef,
+        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
         "schemaVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
```

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.pyi` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appflow service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appflow.type_defs import AggregationConfigOutputTypeDef
+    from mypy_boto3_appflow.type_defs import AggregationConfigTypeDef
 
-    data: AggregationConfigOutputTypeDef = {...}
+    data: AggregationConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -65,209 +65,164 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AggregationConfigOutputTypeDef",
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
-    "AmplitudeSourcePropertiesOutputTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
     "CancelFlowExecutionsRequestRequestTypeDef",
-    "CancelFlowExecutionsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectorRuntimeSettingTypeDef",
-    "DataTransferApiOutputTypeDef",
+    "DataTransferApiTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
     "HoneycodeMetadataTypeDef",
     "SalesforceMetadataTypeDef",
     "SlackMetadataTypeDef",
     "SnowflakeMetadataTypeDef",
     "ZendeskMetadataTypeDef",
     "ConnectorOAuthRequestTypeDef",
-    "ConnectorOperatorOutputTypeDef",
     "ConnectorOperatorTypeDef",
     "DatadogConnectorProfileCredentialsTypeDef",
     "DynatraceConnectorProfileCredentialsTypeDef",
     "InforNexusConnectorProfileCredentialsTypeDef",
     "RedshiftConnectorProfileCredentialsTypeDef",
     "ServiceNowConnectorProfileCredentialsTypeDef",
     "SingularConnectorProfileCredentialsTypeDef",
     "SnowflakeConnectorProfileCredentialsTypeDef",
     "TrendmicroConnectorProfileCredentialsTypeDef",
     "VeevaConnectorProfileCredentialsTypeDef",
-    "DatadogConnectorProfilePropertiesOutputTypeDef",
-    "DynatraceConnectorProfilePropertiesOutputTypeDef",
-    "InforNexusConnectorProfilePropertiesOutputTypeDef",
-    "MarketoConnectorProfilePropertiesOutputTypeDef",
-    "PardotConnectorProfilePropertiesOutputTypeDef",
-    "RedshiftConnectorProfilePropertiesOutputTypeDef",
-    "SalesforceConnectorProfilePropertiesOutputTypeDef",
-    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
-    "SlackConnectorProfilePropertiesOutputTypeDef",
-    "SnowflakeConnectorProfilePropertiesOutputTypeDef",
-    "VeevaConnectorProfilePropertiesOutputTypeDef",
-    "ZendeskConnectorProfilePropertiesOutputTypeDef",
     "DatadogConnectorProfilePropertiesTypeDef",
     "DynatraceConnectorProfilePropertiesTypeDef",
     "InforNexusConnectorProfilePropertiesTypeDef",
     "MarketoConnectorProfilePropertiesTypeDef",
     "PardotConnectorProfilePropertiesTypeDef",
     "RedshiftConnectorProfilePropertiesTypeDef",
     "SalesforceConnectorProfilePropertiesTypeDef",
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
-    "LambdaConnectorProvisioningConfigOutputTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
-    "CreateConnectorProfileResponseTypeDef",
-    "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
-    "ErrorHandlingConfigOutputTypeDef",
     "ErrorHandlingConfigTypeDef",
     "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
-    "DataTransferApiTypeDef",
-    "CustomerProfilesDestinationPropertiesOutputTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
-    "DatadogSourcePropertiesOutputTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "DescribeConnectorsRequestRequestTypeDef",
     "DescribeFlowExecutionRecordsRequestRequestTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "ExecutionDetailsTypeDef",
-    "DynatraceSourcePropertiesOutputTypeDef",
     "DynatraceSourcePropertiesTypeDef",
     "ErrorInfoTypeDef",
     "RangeTypeDef",
-    "GlueDataCatalogConfigOutputTypeDef",
     "GlueDataCatalogConfigTypeDef",
-    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
     "GoogleAnalyticsSourcePropertiesTypeDef",
-    "IncrementalPullConfigOutputTypeDef",
     "IncrementalPullConfigTypeDef",
-    "InforNexusSourcePropertiesOutputTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MarketoSourcePropertiesOutputTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
     "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
-    "PardotSourcePropertiesOutputTypeDef",
     "PardotSourcePropertiesTypeDef",
     "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
-    "RegisterConnectorResponseTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "S3InputFormatConfigOutputTypeDef",
     "S3InputFormatConfigTypeDef",
-    "SuccessResponseHandlingConfigOutputTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
-    "SAPODataSourcePropertiesOutputTypeDef",
     "SAPODataSourcePropertiesTypeDef",
-    "SalesforceSourcePropertiesOutputTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesOutputTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
-    "ServiceNowSourcePropertiesOutputTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
-    "SingularSourcePropertiesOutputTypeDef",
     "SingularSourcePropertiesTypeDef",
-    "SlackSourcePropertiesOutputTypeDef",
     "SlackSourcePropertiesTypeDef",
-    "TrendmicroSourcePropertiesOutputTypeDef",
-    "VeevaSourcePropertiesOutputTypeDef",
-    "ZendeskSourcePropertiesOutputTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
-    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
-    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CustomAuthConfigTypeDef",
+    "CancelFlowExecutionsResponseTypeDef",
+    "CreateConnectorProfileResponseTypeDef",
+    "CreateFlowResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterConnectorResponseTypeDef",
+    "StartFlowResponseTypeDef",
+    "StopFlowResponseTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
-    "CustomAuthConfigTypeDef",
     "CustomConnectorSourcePropertiesOutputTypeDef",
+    "CustomConnectorSourcePropertiesTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
     "TaskOutputTypeDef",
     "TaskTypeDef",
-    "ConnectorProvisioningConfigOutputTypeDef",
     "ConnectorProvisioningConfigTypeDef",
     "CustomConnectorDestinationPropertiesOutputTypeDef",
-    "EventBridgeDestinationPropertiesOutputTypeDef",
-    "HoneycodeDestinationPropertiesOutputTypeDef",
-    "MarketoDestinationPropertiesOutputTypeDef",
-    "RedshiftDestinationPropertiesOutputTypeDef",
-    "SalesforceDestinationPropertiesOutputTypeDef",
-    "SnowflakeDestinationPropertiesOutputTypeDef",
-    "ZendeskDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
+    "SalesforceDestinationPropertiesOutputTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
+    "ZendeskDestinationPropertiesOutputTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
     "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
-    "CustomConnectorSourcePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
-    "MetadataCatalogConfigOutputTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
     "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
     "S3OutputFormatConfigOutputTypeDef",
     "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
-    "S3SourcePropertiesOutputTypeDef",
     "S3SourcePropertiesTypeDef",
     "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
     "TriggerPropertiesOutputTypeDef",
     "TriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
@@ -306,23 +261,14 @@
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
     "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
-AggregationConfigOutputTypeDef = TypedDict(
-    "AggregationConfigOutputTypeDef",
-    {
-        "aggregationType": AggregationTypeType,
-        "targetFileSize": int,
-    },
-    total=False,
-)
-
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "targetFileSize": int,
     },
     total=False,
@@ -332,21 +278,14 @@
     "AmplitudeConnectorProfileCredentialsTypeDef",
     {
         "apiKey": str,
         "secretKey": str,
     },
 )
 
-AmplitudeSourcePropertiesOutputTypeDef = TypedDict(
-    "AmplitudeSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 AmplitudeSourcePropertiesTypeDef = TypedDict(
     "AmplitudeSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -406,19 +345,22 @@
 
 class CancelFlowExecutionsRequestRequestTypeDef(
     _RequiredCancelFlowExecutionsRequestRequestTypeDef,
     _OptionalCancelFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-CancelFlowExecutionsResponseTypeDef = TypedDict(
-    "CancelFlowExecutionsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "invalidExecutions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectorRuntimeSettingTypeDef = TypedDict(
     "ConnectorRuntimeSettingTypeDef",
     {
         "key": str,
@@ -428,16 +370,16 @@
         "description": str,
         "scope": str,
         "connectorSuppliedValueOptions": List[str],
     },
     total=False,
 )
 
-DataTransferApiOutputTypeDef = TypedDict(
-    "DataTransferApiOutputTypeDef",
+DataTransferApiTypeDef = TypedDict(
+    "DataTransferApiTypeDef",
     {
         "Name": str,
         "Type": DataTransferApiTypeType,
     },
     total=False,
 )
 
@@ -556,38 +498,14 @@
     {
         "authCode": str,
         "redirectUri": str,
     },
     total=False,
 )
 
-ConnectorOperatorOutputTypeDef = TypedDict(
-    "ConnectorOperatorOutputTypeDef",
-    {
-        "Amplitude": Literal["BETWEEN"],
-        "Datadog": DatadogConnectorOperatorType,
-        "Dynatrace": DynatraceConnectorOperatorType,
-        "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
-        "InforNexus": InforNexusConnectorOperatorType,
-        "Marketo": MarketoConnectorOperatorType,
-        "S3": S3ConnectorOperatorType,
-        "Salesforce": SalesforceConnectorOperatorType,
-        "ServiceNow": ServiceNowConnectorOperatorType,
-        "Singular": SingularConnectorOperatorType,
-        "Slack": SlackConnectorOperatorType,
-        "Trendmicro": TrendmicroConnectorOperatorType,
-        "Veeva": VeevaConnectorOperatorType,
-        "Zendesk": ZendeskConnectorOperatorType,
-        "SAPOData": SAPODataConnectorOperatorType,
-        "CustomConnector": OperatorType,
-        "Pardot": PardotConnectorOperatorType,
-    },
-    total=False,
-)
-
 ConnectorOperatorTypeDef = TypedDict(
     "ConnectorOperatorTypeDef",
     {
         "Amplitude": Literal["BETWEEN"],
         "Datadog": DatadogConnectorOperatorType,
         "Dynatrace": DynatraceConnectorOperatorType,
         "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
@@ -676,142 +594,14 @@
     "VeevaConnectorProfileCredentialsTypeDef",
     {
         "username": str,
         "password": str,
     },
 )
 
-DatadogConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "DatadogConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-DynatraceConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "DynatraceConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-InforNexusConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "InforNexusConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-MarketoConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "MarketoConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-PardotConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "PardotConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-        "isSandboxEnvironment": bool,
-        "businessUnitId": str,
-    },
-    total=False,
-)
-
-_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-        "roleArn": str,
-    },
-)
-_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef",
-    {
-        "databaseUrl": str,
-        "bucketPrefix": str,
-        "dataApiRoleArn": str,
-        "isRedshiftServerless": bool,
-        "clusterIdentifier": str,
-        "workgroupName": str,
-        "databaseName": str,
-    },
-    total=False,
-)
-
-class RedshiftConnectorProfilePropertiesOutputTypeDef(
-    _RequiredRedshiftConnectorProfilePropertiesOutputTypeDef,
-    _OptionalRedshiftConnectorProfilePropertiesOutputTypeDef,
-):
-    pass
-
-SalesforceConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "SalesforceConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-        "isSandboxEnvironment": bool,
-        "usePrivateLinkForMetadataAndAuthorization": bool,
-    },
-    total=False,
-)
-
-ServiceNowConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-SlackConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "SlackConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef",
-    {
-        "warehouse": str,
-        "stage": str,
-        "bucketName": str,
-    },
-)
-_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "privateLinkServiceName": str,
-        "accountName": str,
-        "region": str,
-    },
-    total=False,
-)
-
-class SnowflakeConnectorProfilePropertiesOutputTypeDef(
-    _RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef,
-    _OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef,
-):
-    pass
-
-VeevaConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "VeevaConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
-ZendeskConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "ZendeskConnectorProfilePropertiesOutputTypeDef",
-    {
-        "instanceUrl": str,
-    },
-)
-
 DatadogConnectorProfilePropertiesTypeDef = TypedDict(
     "DatadogConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -942,45 +732,21 @@
         "status": PrivateConnectionProvisioningStatusType,
         "failureMessage": str,
         "failureCause": PrivateConnectionProvisioningFailureCauseType,
     },
     total=False,
 )
 
-LambdaConnectorProvisioningConfigOutputTypeDef = TypedDict(
-    "LambdaConnectorProvisioningConfigOutputTypeDef",
-    {
-        "lambdaArn": str,
-    },
-)
-
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
-CreateConnectorProfileResponseTypeDef = TypedDict(
-    "CreateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlowResponseTypeDef = TypedDict(
-    "CreateFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCustomAuthCredentialsTypeDef = TypedDict(
     "_RequiredCustomAuthCredentialsTypeDef",
     {
         "customAuthenticationType": str,
     },
 )
 _OptionalCustomAuthCredentialsTypeDef = TypedDict(
@@ -992,24 +758,14 @@
 )
 
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
-ErrorHandlingConfigOutputTypeDef = TypedDict(
-    "ErrorHandlingConfigOutputTypeDef",
-    {
-        "failOnFirstDestinationError": bool,
-        "bucketPrefix": str,
-        "bucketName": str,
-    },
-    total=False,
-)
-
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
@@ -1050,43 +806,14 @@
     },
     total=False,
 )
 
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
-DataTransferApiTypeDef = TypedDict(
-    "DataTransferApiTypeDef",
-    {
-        "Name": str,
-        "Type": DataTransferApiTypeType,
-    },
-    total=False,
-)
-
-_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef",
-    {
-        "domainName": str,
-    },
-)
-_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef",
-    {
-        "objectTypeName": str,
-    },
-    total=False,
-)
-
-class CustomerProfilesDestinationPropertiesOutputTypeDef(
-    _RequiredCustomerProfilesDestinationPropertiesOutputTypeDef,
-    _OptionalCustomerProfilesDestinationPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
@@ -1099,21 +826,14 @@
 
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
-DatadogSourcePropertiesOutputTypeDef = TypedDict(
-    "DatadogSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1253,21 +973,14 @@
         "mostRecentExecutionMessage": str,
         "mostRecentExecutionTime": datetime,
         "mostRecentExecutionStatus": ExecutionStatusType,
     },
     total=False,
 )
 
-DynatraceSourcePropertiesOutputTypeDef = TypedDict(
-    "DynatraceSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 DynatraceSourcePropertiesTypeDef = TypedDict(
     "DynatraceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1285,69 +998,38 @@
     {
         "maximum": float,
         "minimum": float,
     },
     total=False,
 )
 
-GlueDataCatalogConfigOutputTypeDef = TypedDict(
-    "GlueDataCatalogConfigOutputTypeDef",
-    {
-        "roleArn": str,
-        "databaseName": str,
-        "tablePrefix": str,
-    },
-)
-
 GlueDataCatalogConfigTypeDef = TypedDict(
     "GlueDataCatalogConfigTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tablePrefix": str,
     },
 )
 
-GoogleAnalyticsSourcePropertiesOutputTypeDef = TypedDict(
-    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 GoogleAnalyticsSourcePropertiesTypeDef = TypedDict(
     "GoogleAnalyticsSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-IncrementalPullConfigOutputTypeDef = TypedDict(
-    "IncrementalPullConfigOutputTypeDef",
-    {
-        "datetimeTypeFieldName": str,
-    },
-    total=False,
-)
-
 IncrementalPullConfigTypeDef = TypedDict(
     "IncrementalPullConfigTypeDef",
     {
         "datetimeTypeFieldName": str,
     },
     total=False,
 )
 
-InforNexusSourcePropertiesOutputTypeDef = TypedDict(
-    "InforNexusSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 InforNexusSourcePropertiesTypeDef = TypedDict(
     "InforNexusSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1385,29 +1067,14 @@
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
-MarketoSourcePropertiesOutputTypeDef = TypedDict(
-    "MarketoSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1449,21 +1116,14 @@
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
 )
 
-PardotSourcePropertiesOutputTypeDef = TypedDict(
-    "PardotSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1483,117 +1143,51 @@
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
     total=False,
 )
 
-RegisterConnectorResponseTypeDef = TypedDict(
-    "RegisterConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResetConnectorMetadataCacheRequestRequestTypeDef = TypedDict(
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorEntityName": str,
         "entitiesPath": str,
         "apiVersion": str,
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
-S3InputFormatConfigOutputTypeDef = TypedDict(
-    "S3InputFormatConfigOutputTypeDef",
-    {
-        "s3InputFileType": S3InputFileTypeType,
-    },
-    total=False,
-)
-
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
 
-SuccessResponseHandlingConfigOutputTypeDef = TypedDict(
-    "SuccessResponseHandlingConfigOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "bucketName": str,
-    },
-    total=False,
-)
-
 SuccessResponseHandlingConfigTypeDef = TypedDict(
     "SuccessResponseHandlingConfigTypeDef",
     {
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
-SAPODataSourcePropertiesOutputTypeDef = TypedDict(
-    "SAPODataSourcePropertiesOutputTypeDef",
-    {
-        "objectPath": str,
-    },
-    total=False,
-)
-
 SAPODataSourcePropertiesTypeDef = TypedDict(
     "SAPODataSourcePropertiesTypeDef",
     {
         "objectPath": str,
     },
     total=False,
 )
 
-_RequiredSalesforceSourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredSalesforceSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalSalesforceSourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalSalesforceSourcePropertiesOutputTypeDef",
-    {
-        "enableDynamicFieldUpdate": bool,
-        "includeDeletedRecords": bool,
-        "dataTransferApi": SalesforceDataTransferApiType,
-    },
-    total=False,
-)
-
-class SalesforceSourcePropertiesOutputTypeDef(
-    _RequiredSalesforceSourcePropertiesOutputTypeDef,
-    _OptionalSalesforceSourcePropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredSalesforceSourcePropertiesTypeDef = TypedDict(
     "_RequiredSalesforceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceSourcePropertiesTypeDef = TypedDict(
@@ -1658,92 +1252,35 @@
 )
 
 class ScheduledTriggerPropertiesTypeDef(
     _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
 ):
     pass
 
-ServiceNowSourcePropertiesOutputTypeDef = TypedDict(
-    "ServiceNowSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-SingularSourcePropertiesOutputTypeDef = TypedDict(
-    "SingularSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 SingularSourcePropertiesTypeDef = TypedDict(
     "SingularSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-SlackSourcePropertiesOutputTypeDef = TypedDict(
-    "SlackSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 SlackSourcePropertiesTypeDef = TypedDict(
     "SlackSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-TrendmicroSourcePropertiesOutputTypeDef = TypedDict(
-    "TrendmicroSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
-_RequiredVeevaSourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredVeevaSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalVeevaSourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalVeevaSourcePropertiesOutputTypeDef",
-    {
-        "documentType": str,
-        "includeSourceFiles": bool,
-        "includeRenditions": bool,
-        "includeAllVersions": bool,
-    },
-    total=False,
-)
-
-class VeevaSourcePropertiesOutputTypeDef(
-    _RequiredVeevaSourcePropertiesOutputTypeDef, _OptionalVeevaSourcePropertiesOutputTypeDef
-):
-    pass
-
-ZendeskSourcePropertiesOutputTypeDef = TypedDict(
-    "ZendeskSourcePropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-
 TrendmicroSourcePropertiesTypeDef = TypedDict(
     "TrendmicroSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1791,40 +1328,21 @@
 )
 
 class StartFlowRequestRequestTypeDef(
     _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
 ):
     pass
 
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "executionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1853,83 +1371,163 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CustomAuthConfigTypeDef = TypedDict(
+    "CustomAuthConfigTypeDef",
+    {
+        "customAuthenticationType": str,
+        "authParameters": List[AuthParameterTypeDef],
+    },
+    total=False,
+)
+
+CancelFlowExecutionsResponseTypeDef = TypedDict(
+    "CancelFlowExecutionsResponseTypeDef",
+    {
+        "invalidExecutions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorProfileResponseTypeDef = TypedDict(
+    "CreateConnectorProfileResponseTypeDef",
+    {
+        "connectorProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFlowResponseTypeDef = TypedDict(
+    "CreateFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
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
+RegisterConnectorResponseTypeDef = TypedDict(
+    "RegisterConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "executionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateConnectorProfileResponseTypeDef = TypedDict(
     "UpdateConnectorProfileResponseTypeDef",
     {
         "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectorRegistrationResponseTypeDef = TypedDict(
     "UpdateConnectorRegistrationResponseTypeDef",
     {
         "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CustomAuthConfigTypeDef = TypedDict(
-    "CustomAuthConfigTypeDef",
-    {
-        "customAuthenticationType": str,
-        "authParameters": List[AuthParameterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
     "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
     "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
     {
         "customProperties": Dict[str, str],
-        "dataTransferApi": DataTransferApiOutputTypeDef,
+        "dataTransferApi": DataTransferApiTypeDef,
     },
     total=False,
 )
 
 class CustomConnectorSourcePropertiesOutputTypeDef(
     _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
     _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
 ):
     pass
 
+_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+    {
+        "customProperties": Mapping[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
+    },
+    total=False,
+)
+
+class CustomConnectorSourcePropertiesTypeDef(
+    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+):
+    pass
+
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorEntitiesResponseTypeDef = TypedDict(
     "ListConnectorEntitiesResponseTypeDef",
     {
         "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorMetadataTypeDef = TypedDict(
     "ConnectorMetadataTypeDef",
     {
         "Amplitude": Dict[str, Any],
@@ -2119,15 +1717,15 @@
         "sourceFields": List[str],
         "taskType": TaskTypeType,
     },
 )
 _OptionalTaskOutputTypeDef = TypedDict(
     "_OptionalTaskOutputTypeDef",
     {
-        "connectorOperator": ConnectorOperatorOutputTypeDef,
+        "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Dict[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
 class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
@@ -2149,22 +1747,14 @@
     },
     total=False,
 )
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
-ConnectorProvisioningConfigOutputTypeDef = TypedDict(
-    "ConnectorProvisioningConfigOutputTypeDef",
-    {
-        "lambda": LambdaConnectorProvisioningConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
@@ -2174,177 +1764,28 @@
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
     "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
     {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": List[str],
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
 class CustomConnectorDestinationPropertiesOutputTypeDef(
     _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
     _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
 ):
     pass
 
-_RequiredEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class EventBridgeDestinationPropertiesOutputTypeDef(
-    _RequiredEventBridgeDestinationPropertiesOutputTypeDef,
-    _OptionalEventBridgeDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-_RequiredHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredHoneycodeDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalHoneycodeDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class HoneycodeDestinationPropertiesOutputTypeDef(
-    _RequiredHoneycodeDestinationPropertiesOutputTypeDef,
-    _OptionalHoneycodeDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-_RequiredMarketoDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredMarketoDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalMarketoDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalMarketoDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class MarketoDestinationPropertiesOutputTypeDef(
-    _RequiredMarketoDestinationPropertiesOutputTypeDef,
-    _OptionalMarketoDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-_RequiredRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredRedshiftDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-        "intermediateBucketName": str,
-    },
-)
-_OptionalRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalRedshiftDestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class RedshiftDestinationPropertiesOutputTypeDef(
-    _RequiredRedshiftDestinationPropertiesOutputTypeDef,
-    _OptionalRedshiftDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-        "dataTransferApi": SalesforceDataTransferApiType,
-    },
-    total=False,
-)
-
-class SalesforceDestinationPropertiesOutputTypeDef(
-    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
-    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-_RequiredSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSnowflakeDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-        "intermediateBucketName": str,
-    },
-)
-_OptionalSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSnowflakeDestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class SnowflakeDestinationPropertiesOutputTypeDef(
-    _RequiredSnowflakeDestinationPropertiesOutputTypeDef,
-    _OptionalSnowflakeDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-    },
-    total=False,
-)
-
-class ZendeskDestinationPropertiesOutputTypeDef(
-    _RequiredZendeskDestinationPropertiesOutputTypeDef,
-    _OptionalZendeskDestinationPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -2439,14 +1880,37 @@
 )
 
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
+_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+class SalesforceDestinationPropertiesOutputTypeDef(
+    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
+    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -2482,14 +1946,36 @@
 )
 
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
+_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+class ZendeskDestinationPropertiesOutputTypeDef(
+    _RequiredZendeskDestinationPropertiesOutputTypeDef,
+    _OptionalZendeskDestinationPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -2521,34 +2007,14 @@
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesTypeDef",
-    {
-        "customProperties": Mapping[str, str],
-        "dataTransferApi": DataTransferApiTypeDef,
-    },
-    total=False,
-)
-
-class CustomConnectorSourcePropertiesTypeDef(
-    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
-):
-    pass
-
 FlowDefinitionTypeDef = TypedDict(
     "FlowDefinitionTypeDef",
     {
         "flowArn": str,
         "description": str,
         "flowName": str,
         "flowStatus": FlowStatusType,
@@ -2596,22 +2062,14 @@
     },
     total=False,
 )
 
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
-MetadataCatalogConfigOutputTypeDef = TypedDict(
-    "MetadataCatalogConfigOutputTypeDef",
-    {
-        "glueDataCatalog": GlueDataCatalogConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
 )
@@ -2692,15 +2150,15 @@
     pass
 
 S3OutputFormatConfigOutputTypeDef = TypedDict(
     "S3OutputFormatConfigOutputTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigOutputTypeDef,
-        "aggregationConfig": AggregationConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
     },
     total=False,
 )
 
 _RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
     "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
@@ -2708,15 +2166,15 @@
         "prefixConfig": PrefixConfigOutputTypeDef,
     },
 )
 _OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
     "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
     {
         "fileType": FileTypeType,
-        "aggregationConfig": AggregationConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
 class UpsolverS3OutputFormatConfigOutputTypeDef(
     _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
     _OptionalUpsolverS3OutputFormatConfigOutputTypeDef,
@@ -2750,34 +2208,14 @@
 )
 
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
-_RequiredS3SourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredS3SourcePropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3SourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalS3SourcePropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "s3InputFormatConfig": S3InputFormatConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class S3SourcePropertiesOutputTypeDef(
-    _RequiredS3SourcePropertiesOutputTypeDef, _OptionalS3SourcePropertiesOutputTypeDef
-):
-    pass
-
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -2799,17 +2237,17 @@
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
     "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
     {
-        "successResponseHandlingConfig": SuccessResponseHandlingConfigOutputTypeDef,
+        "successResponseHandlingConfig": SuccessResponseHandlingConfigTypeDef,
         "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
 class SAPODataDestinationPropertiesOutputTypeDef(
     _RequiredSAPODataDestinationPropertiesOutputTypeDef,
@@ -2922,15 +2360,15 @@
     pass
 
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SupportedFieldTypeDetailsTypeDef = TypedDict(
     "SupportedFieldTypeDetailsTypeDef",
     {
         "v1": FieldTypeDetailsTypeDef,
@@ -2965,32 +2403,32 @@
     total=False,
 )
 
 ConnectorProfilePropertiesOutputTypeDef = TypedDict(
     "ConnectorProfilePropertiesOutputTypeDef",
     {
         "Amplitude": Dict[str, Any],
-        "Datadog": DatadogConnectorProfilePropertiesOutputTypeDef,
-        "Dynatrace": DynatraceConnectorProfilePropertiesOutputTypeDef,
+        "Datadog": DatadogConnectorProfilePropertiesTypeDef,
+        "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Dict[str, Any],
         "Honeycode": Dict[str, Any],
-        "InforNexus": InforNexusConnectorProfilePropertiesOutputTypeDef,
-        "Marketo": MarketoConnectorProfilePropertiesOutputTypeDef,
-        "Redshift": RedshiftConnectorProfilePropertiesOutputTypeDef,
-        "Salesforce": SalesforceConnectorProfilePropertiesOutputTypeDef,
-        "ServiceNow": ServiceNowConnectorProfilePropertiesOutputTypeDef,
+        "InforNexus": InforNexusConnectorProfilePropertiesTypeDef,
+        "Marketo": MarketoConnectorProfilePropertiesTypeDef,
+        "Redshift": RedshiftConnectorProfilePropertiesTypeDef,
+        "Salesforce": SalesforceConnectorProfilePropertiesTypeDef,
+        "ServiceNow": ServiceNowConnectorProfilePropertiesTypeDef,
         "Singular": Dict[str, Any],
-        "Slack": SlackConnectorProfilePropertiesOutputTypeDef,
-        "Snowflake": SnowflakeConnectorProfilePropertiesOutputTypeDef,
+        "Slack": SlackConnectorProfilePropertiesTypeDef,
+        "Snowflake": SnowflakeConnectorProfilePropertiesTypeDef,
         "Trendmicro": Dict[str, Any],
-        "Veeva": VeevaConnectorProfilePropertiesOutputTypeDef,
-        "Zendesk": ZendeskConnectorProfilePropertiesOutputTypeDef,
+        "Veeva": VeevaConnectorProfilePropertiesTypeDef,
+        "Zendesk": ZendeskConnectorProfilePropertiesTypeDef,
         "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
-        "Pardot": PardotConnectorProfilePropertiesOutputTypeDef,
+        "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
@@ -3097,31 +2535,31 @@
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
 SourceConnectorPropertiesOutputTypeDef = TypedDict(
     "SourceConnectorPropertiesOutputTypeDef",
     {
-        "Amplitude": AmplitudeSourcePropertiesOutputTypeDef,
-        "Datadog": DatadogSourcePropertiesOutputTypeDef,
-        "Dynatrace": DynatraceSourcePropertiesOutputTypeDef,
-        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesOutputTypeDef,
-        "InforNexus": InforNexusSourcePropertiesOutputTypeDef,
-        "Marketo": MarketoSourcePropertiesOutputTypeDef,
-        "S3": S3SourcePropertiesOutputTypeDef,
-        "Salesforce": SalesforceSourcePropertiesOutputTypeDef,
-        "ServiceNow": ServiceNowSourcePropertiesOutputTypeDef,
-        "Singular": SingularSourcePropertiesOutputTypeDef,
-        "Slack": SlackSourcePropertiesOutputTypeDef,
-        "Trendmicro": TrendmicroSourcePropertiesOutputTypeDef,
-        "Veeva": VeevaSourcePropertiesOutputTypeDef,
-        "Zendesk": ZendeskSourcePropertiesOutputTypeDef,
-        "SAPOData": SAPODataSourcePropertiesOutputTypeDef,
+        "Amplitude": AmplitudeSourcePropertiesTypeDef,
+        "Datadog": DatadogSourcePropertiesTypeDef,
+        "Dynatrace": DynatraceSourcePropertiesTypeDef,
+        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
+        "InforNexus": InforNexusSourcePropertiesTypeDef,
+        "Marketo": MarketoSourcePropertiesTypeDef,
+        "S3": S3SourcePropertiesTypeDef,
+        "Salesforce": SalesforceSourcePropertiesTypeDef,
+        "ServiceNow": ServiceNowSourcePropertiesTypeDef,
+        "Singular": SingularSourcePropertiesTypeDef,
+        "Slack": SlackSourcePropertiesTypeDef,
+        "Trendmicro": TrendmicroSourcePropertiesTypeDef,
+        "Veeva": VeevaSourcePropertiesTypeDef,
+        "Zendesk": ZendeskSourcePropertiesTypeDef,
+        "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
-        "Pardot": PardotSourcePropertiesOutputTypeDef,
+        "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
@@ -3237,15 +2675,15 @@
     pass
 
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorConfigurationTypeDef = TypedDict(
     "ConnectorConfigurationTypeDef",
     {
         "canUseAsSource": bool,
@@ -3266,20 +2704,20 @@
         "connectorModes": List[str],
         "authenticationConfig": AuthenticationConfigTypeDef,
         "connectorRuntimeSettings": List[ConnectorRuntimeSettingTypeDef],
         "supportedApiVersions": List[str],
         "supportedOperators": List[OperatorsType],
         "supportedWriteOperations": List[WriteOperationTypeType],
         "connectorProvisioningType": Literal["LAMBDA"],
-        "connectorProvisioningConfig": ConnectorProvisioningConfigOutputTypeDef,
+        "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "logoURL": str,
         "registeredAt": datetime,
         "registeredBy": str,
         "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
-        "supportedDataTransferApis": List[DataTransferApiOutputTypeDef],
+        "supportedDataTransferApis": List[DataTransferApiTypeDef],
     },
     total=False,
 )
 
 ConnectorProfileTypeDef = TypedDict(
     "ConnectorProfileTypeDef",
     {
@@ -3296,25 +2734,25 @@
     },
     total=False,
 )
 
 DestinationConnectorPropertiesOutputTypeDef = TypedDict(
     "DestinationConnectorPropertiesOutputTypeDef",
     {
-        "Redshift": RedshiftDestinationPropertiesOutputTypeDef,
+        "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesOutputTypeDef,
         "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
-        "Snowflake": SnowflakeDestinationPropertiesOutputTypeDef,
-        "EventBridge": EventBridgeDestinationPropertiesOutputTypeDef,
+        "Snowflake": SnowflakeDestinationPropertiesTypeDef,
+        "EventBridge": EventBridgeDestinationPropertiesTypeDef,
         "LookoutMetrics": Dict[str, Any],
         "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
-        "Honeycode": HoneycodeDestinationPropertiesOutputTypeDef,
-        "CustomerProfiles": CustomerProfilesDestinationPropertiesOutputTypeDef,
+        "Honeycode": HoneycodeDestinationPropertiesTypeDef,
+        "CustomerProfiles": CustomerProfilesDestinationPropertiesTypeDef,
         "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
-        "Marketo": MarketoDestinationPropertiesOutputTypeDef,
+        "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
         "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
     },
     total=False,
 )
 
 DestinationConnectorPropertiesTypeDef = TypedDict(
@@ -3345,15 +2783,15 @@
     },
 )
 _OptionalSourceFlowConfigOutputTypeDef = TypedDict(
     "_OptionalSourceFlowConfigOutputTypeDef",
     {
         "apiVersion": str,
         "connectorProfileName": str,
-        "incrementalPullConfig": IncrementalPullConfigOutputTypeDef,
+        "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
 class SourceFlowConfigOutputTypeDef(
     _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
 ):
@@ -3398,42 +2836,42 @@
 ):
     pass
 
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "connectorConfiguration": ConnectorConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorsResponseTypeDef = TypedDict(
     "DescribeConnectorsResponseTypeDef",
     {
         "connectorConfigurations": Dict[ConnectorTypeType, ConnectorConfigurationTypeDef],
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorProfilesResponseTypeDef = TypedDict(
     "DescribeConnectorProfilesResponseTypeDef",
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigOutputTypeDef",
     {
         "connectorType": ConnectorTypeType,
@@ -3537,18 +2975,18 @@
         "triggerConfig": TriggerConfigOutputTypeDef,
         "tasks": List[TaskOutputTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigOutputTypeDef,
+        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
         "schemaVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
```

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/PKG-INFO` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.12
-Summary: Type annotations for boto3.Appflow 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,209 +339,164 @@
 ### Typed dictionaries
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
-    AggregationConfigOutputTypeDef,
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
-    AmplitudeSourcePropertiesOutputTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
-    CancelFlowExecutionsResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectorRuntimeSettingTypeDef,
-    DataTransferApiOutputTypeDef,
+    DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
     SlackMetadataTypeDef,
     SnowflakeMetadataTypeDef,
     ZendeskMetadataTypeDef,
     ConnectorOAuthRequestTypeDef,
-    ConnectorOperatorOutputTypeDef,
     ConnectorOperatorTypeDef,
     DatadogConnectorProfileCredentialsTypeDef,
     DynatraceConnectorProfileCredentialsTypeDef,
     InforNexusConnectorProfileCredentialsTypeDef,
     RedshiftConnectorProfileCredentialsTypeDef,
     ServiceNowConnectorProfileCredentialsTypeDef,
     SingularConnectorProfileCredentialsTypeDef,
     SnowflakeConnectorProfileCredentialsTypeDef,
     TrendmicroConnectorProfileCredentialsTypeDef,
     VeevaConnectorProfileCredentialsTypeDef,
-    DatadogConnectorProfilePropertiesOutputTypeDef,
-    DynatraceConnectorProfilePropertiesOutputTypeDef,
-    InforNexusConnectorProfilePropertiesOutputTypeDef,
-    MarketoConnectorProfilePropertiesOutputTypeDef,
-    PardotConnectorProfilePropertiesOutputTypeDef,
-    RedshiftConnectorProfilePropertiesOutputTypeDef,
-    SalesforceConnectorProfilePropertiesOutputTypeDef,
-    ServiceNowConnectorProfilePropertiesOutputTypeDef,
-    SlackConnectorProfilePropertiesOutputTypeDef,
-    SnowflakeConnectorProfilePropertiesOutputTypeDef,
-    VeevaConnectorProfilePropertiesOutputTypeDef,
-    ZendeskConnectorProfilePropertiesOutputTypeDef,
     DatadogConnectorProfilePropertiesTypeDef,
     DynatraceConnectorProfilePropertiesTypeDef,
     InforNexusConnectorProfilePropertiesTypeDef,
     MarketoConnectorProfilePropertiesTypeDef,
     PardotConnectorProfilePropertiesTypeDef,
     RedshiftConnectorProfilePropertiesTypeDef,
     SalesforceConnectorProfilePropertiesTypeDef,
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
-    LambdaConnectorProvisioningConfigOutputTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
-    ErrorHandlingConfigOutputTypeDef,
     ErrorHandlingConfigTypeDef,
     OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
-    DataTransferApiTypeDef,
-    CustomerProfilesDestinationPropertiesOutputTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
-    DatadogSourcePropertiesOutputTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     DescribeConnectorsRequestRequestTypeDef,
     DescribeFlowExecutionRecordsRequestRequestTypeDef,
     DescribeFlowRequestRequestTypeDef,
     ExecutionDetailsTypeDef,
-    DynatraceSourcePropertiesOutputTypeDef,
     DynatraceSourcePropertiesTypeDef,
     ErrorInfoTypeDef,
     RangeTypeDef,
-    GlueDataCatalogConfigOutputTypeDef,
     GlueDataCatalogConfigTypeDef,
-    GoogleAnalyticsSourcePropertiesOutputTypeDef,
     GoogleAnalyticsSourcePropertiesTypeDef,
-    IncrementalPullConfigOutputTypeDef,
     IncrementalPullConfigTypeDef,
-    InforNexusSourcePropertiesOutputTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MarketoSourcePropertiesOutputTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
     OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
-    PardotSourcePropertiesOutputTypeDef,
     PardotSourcePropertiesTypeDef,
     PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
-    RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3InputFormatConfigOutputTypeDef,
     S3InputFormatConfigTypeDef,
-    SuccessResponseHandlingConfigOutputTypeDef,
     SuccessResponseHandlingConfigTypeDef,
-    SAPODataSourcePropertiesOutputTypeDef,
     SAPODataSourcePropertiesTypeDef,
-    SalesforceSourcePropertiesOutputTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesOutputTypeDef,
     ScheduledTriggerPropertiesTypeDef,
-    ServiceNowSourcePropertiesOutputTypeDef,
     ServiceNowSourcePropertiesTypeDef,
-    SingularSourcePropertiesOutputTypeDef,
     SingularSourcePropertiesTypeDef,
-    SlackSourcePropertiesOutputTypeDef,
     SlackSourcePropertiesTypeDef,
-    TrendmicroSourcePropertiesOutputTypeDef,
-    VeevaSourcePropertiesOutputTypeDef,
-    ZendeskSourcePropertiesOutputTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CustomAuthConfigTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterConnectorResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
-    CustomAuthConfigTypeDef,
     CustomConnectorSourcePropertiesOutputTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
     TaskOutputTypeDef,
     TaskTypeDef,
-    ConnectorProvisioningConfigOutputTypeDef,
     ConnectorProvisioningConfigTypeDef,
     CustomConnectorDestinationPropertiesOutputTypeDef,
-    EventBridgeDestinationPropertiesOutputTypeDef,
-    HoneycodeDestinationPropertiesOutputTypeDef,
-    MarketoDestinationPropertiesOutputTypeDef,
-    RedshiftDestinationPropertiesOutputTypeDef,
-    SalesforceDestinationPropertiesOutputTypeDef,
-    SnowflakeDestinationPropertiesOutputTypeDef,
-    ZendeskDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     ZendeskDestinationPropertiesTypeDef,
     CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
-    MetadataCatalogConfigOutputTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
     SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
     S3OutputFormatConfigOutputTypeDef,
     UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
-    S3SourcePropertiesOutputTypeDef,
     S3SourcePropertiesTypeDef,
     SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
     TriggerPropertiesOutputTypeDef,
     TriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
@@ -581,15 +536,15 @@
     UpdateConnectorProfileRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
     CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigOutputTypeDef:
+def get_structure() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/SOURCES.txt` & `mypy-boto3-appflow-1.28.15/mypy_boto3_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.12/setup.py` & `mypy-boto3-appflow-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appflow",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Appflow 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

